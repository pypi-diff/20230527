# Comparing `tmp/python_lsp_pyre-0.1.2.tar.gz` & `tmp/python_lsp_pyre-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_lsp_pyre-0.1.2.tar", max compression
+gzip compressed data, was "python_lsp_pyre-0.1.3.tar", max compression
```

## Comparing `python_lsp_pyre-0.1.2.tar` & `python_lsp_pyre-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2800 2023-05-26 07:04:24.665541 python_lsp_pyre-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-26 07:04:24.665541 python_lsp_pyre-0.1.2/pylsp_pyre/__init__.py
--rw-r--r--   0        0        0     5701 2023-05-26 07:04:24.665541 python_lsp_pyre-0.1.2/pylsp_pyre/plugin.py
--rw-r--r--   0        0        0      730 2023-05-26 07:04:24.665541 python_lsp_pyre-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3390 1970-01-01 00:00:00.000000 python_lsp_pyre-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4147 2023-05-27 08:53:05.083700 python_lsp_pyre-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 08:53:05.087700 python_lsp_pyre-0.1.3/pylsp_pyre/__init__.py
+-rw-r--r--   0        0        0     6651 2023-05-27 08:53:05.087700 python_lsp_pyre-0.1.3/pylsp_pyre/plugin.py
+-rw-r--r--   0        0        0      730 2023-05-27 08:53:05.087700 python_lsp_pyre-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4737 1970-01-01 00:00:00.000000 python_lsp_pyre-0.1.3/PKG-INFO
```

### Comparing `python_lsp_pyre-0.1.2/pylsp_pyre/plugin.py` & `python_lsp_pyre-0.1.3/pylsp_pyre/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import dataclasses as dc
 import json
 import logging
 import subprocess
 from pathlib import Path
 from typing import Any, Dict, List
 
 import lsprotocol.converters as lsp_con
@@ -10,15 +11,27 @@
 import pylsp.lsp as pylsp_lsp
 import pylsp.workspace as pylsp_ws
 import pyre_check.client.language_server.protocol as pyre_proto
 from pylsp import hookimpl
 
 logger: logging.Logger = logging.getLogger(__name__)
 # A logging prefix.
-PLUGIN: str = "[python-lsp-pyre]"
+PLUGIN = "[python-lsp-pyre]"
+
+
+@dc.dataclass
+class Settings:
+    enabled: bool = dc.field(init=False)
+    create_pyre_config: bool = dc.field(init=False)
+
+    def from_pylsp(self, config: pylsp_conf.Config) -> "Settings":
+        settings = config.plugin_settings("pyre")
+        self.enabled = getattr(settings, "enabled", True)
+        self.create_pyre_config = getattr(settings, "create-pyre-config", False)
+        return self
 
 
 @hookimpl
 def pylsp_settings(config: pylsp_conf.Config) -> Dict[str, Dict[str, Dict[str, bool]]]:
     """
     Default configuration for the plugin. Ensures all keys are set.
     """
@@ -39,19 +52,21 @@
     document: pylsp_ws.Document,
     is_saved: bool,
 ) -> List[Dict[str, Any]]:
     """
     Lints files (saved, not in-progress) and returns found problems.
     """
     logger.debug(f"Working with {document.path}, {is_saved=}")
-    maybe_create_pyre_config(config=config, workspace=workspace)
     if is_saved:
+        plugin_settings = Settings().from_pylsp(config=config)
+        maybe_create_pyre_config(settings=plugin_settings, workspace=workspace)
         with workspace.report_progress("lint: pyre check", "running"):
-            settings = config.plugin_settings("pyre")
-            diagnostics = run_pyre(workspace=workspace, document=document, settings=settings)
+            diagnostics = run_pyre(
+                workspace=workspace, document=document, settings=plugin_settings
+            )
         workspace.show_message(message=f"Pyre reported {len(diagnostics)} issue(s).")
         # Deal with location stuff by using unstructure() for now.
         return lsp_con.get_converter().unstructure(diagnostics)
     else:
         return []
 
 
@@ -75,34 +90,40 @@
             start=pyre_proto.LspPosition(line=0, character=0),
             end=pyre_proto.LspPosition(line=0, character=1),
         ),
     }
 
 
 def run_pyre(
-    workspace: pylsp_ws.Workspace, document: pylsp_ws.Document, settings: Dict
+    workspace: pylsp_ws.Workspace, document: pylsp_ws.Document, settings: Settings
 ) -> List[Dict[str, Any]]:
     """
     Calls Pyre, converts output to internal structs
     """
     try:
-        data = really_run_pyre(root_path=workspace.root_path)
-        data = json.loads(data.decode("utf-8"))
+        pyre_out = really_run_pyre(root_path=workspace.root_path)
+        data = json.loads(pyre_out.decode("utf-8"))
+        # Pyre checks all files in the project, but at least with Kate, the LSP response is
+        # collected under the active file, making for misleading reading. Thus, filter on the
+        # path for now. This means that the Pyre output is less useful, because things like
+        # type changes on a commonly included attribute in one module will not show as
+        # problems in other modules unless the command line is used :(
         checks = [
             {
                 "source": "pyre",
                 "severity": lsp_types.DiagnosticSeverity.Error,
                 "code": x["code"],
                 "message": x["long_description"],
                 "range": pyre_proto.LspRange(
                     start=pyre_proto.LspPosition(line=(x["line"] - 1), character=x["column"]),
                     end=pyre_proto.LspPosition(
                         line=(x["stop_line"] - 1), character=x["stop_column"]
                     ),
                 ),
+                "path": x["path"]
             }
             for x in data
             if document.path == f"{workspace.root_path}/{x['path']}"
         ]
     except subprocess.CalledProcessError as e:
         msg = f"ABEND: Pyre failed: {str(e)}. {e.stderr.decode('utf-8')}"
         checks = [abend(message=msg, workspace=workspace)]
@@ -132,39 +153,38 @@
         # If there are typing errors, pyre exits with returncode 1
         # If there are configuration errors, pyre exits with returncode 6
         if e.returncode in (0, 1):
             return e.output
         raise
 
 
-def maybe_create_pyre_config(
-    config: pylsp_conf.Config, workspace: pylsp_ws.Workspace
-) -> None:
+def maybe_create_pyre_config(settings: Settings, workspace: pylsp_ws.Workspace) -> None:
     """
     Initializes a .pyre_configuration file if `create-pyre-config` setting is enabled.
 
     Only initializes if the file is missing.
     """
     default_config = json.loads(
         """
         {
       "site_package_search_strategy": "all",
       "source_directories": [
         "."
       ],
       "exclude": [
         "\/setup.py",
-        ".*\/build\/.*"
-      ]
+        ".*\/build\/.*",
+        ".*\/.pyre\/.*"
+      ],
+      "strict": true
     }
     """
     )
-    settings = config.plugin_settings("pyre")
     try:
-        if settings["create-pyre-config"]:
+        if settings.create_pyre_config:
             docroot = workspace.root_path
             path = Path(docroot).joinpath(".pyre_configuration")
             if not path.exists():
                 logger.info(f"Initializing {path}")
                 with path.open(mode="w") as f:
                     f.write(json.dumps(default_config, indent=4))
                     f.write("\n")
```

### Comparing `python_lsp_pyre-0.1.2/pyproject.toml` & `python_lsp_pyre-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-lsp-pyre"
-version = "0.1.2"
+version = "0.1.3"
 description = "Pyre linting plugin for pylsp"
 authors = ["Duncan Hill <python.projects@cricalix.net>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pylsp_pyre"}]
 
 [tool.poetry.dependencies]
```

