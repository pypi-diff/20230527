# Comparing `tmp/linkml_renderer-0.1.2.tar.gz` & `tmp/linkml_renderer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_renderer-0.1.2.tar", max compression
+gzip compressed data, was "linkml_renderer-0.2.0.tar", max compression
```

## Comparing `linkml_renderer-0.1.2.tar` & `linkml_renderer-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0    11358 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/LICENSE
--rw-r--r--   0        0        0     3061 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/README.md
--rw-r--r--   0        0        0     1329 2023-01-17 23:57:55.918002 linkml_renderer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      224 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/__init__.py
--rw-r--r--   0        0        0     2488 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/cli.py
--rw-r--r--   0        0        0        0 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/paths/__init__.py
--rw-r--r--   0        0        0     4952 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/paths/context.py
--rw-r--r--   0        0        0      373 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/paths/html_context.py
--rw-r--r--   0        0        0        0 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/renderers/__init__.py
--rw-r--r--   0        0        0    16264 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/renderers/html_renderer.py
--rw-r--r--   0        0        0    13975 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/renderers/markdown_renderer.py
--rw-r--r--   0        0        0     7308 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/renderers/mermaid_renderer.py
--rw-r--r--   0        0        0     3894 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/renderers/renderer.py
--rw-r--r--   0        0        0        0 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/style/__init__.py
--rw-r--r--   0        0        0     3140 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/style/model.py
--rw-r--r--   0        0        0     3211 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/style/model.yaml
--rw-r--r--   0        0        0     1976 2023-01-17 23:56:42.029312 linkml_renderer-0.1.2/src/linkml_renderer/style/style_engine.py
--rw-r--r--   0        0        0     4468 1970-01-01 00:00:00.000000 linkml_renderer-0.1.2/setup.py
--rw-r--r--   0        0        0     4143 1970-01-01 00:00:00.000000 linkml_renderer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-27 01:25:07.262133 linkml_renderer-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3061 2023-05-27 01:25:07.262133 linkml_renderer-0.2.0/README.md
+-rw-r--r--   0        0        0     1331 2023-05-27 01:25:42.358662 linkml_renderer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      224 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/__init__.py
+-rw-r--r--   0        0        0     3257 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/cli.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/paths/__init__.py
+-rw-r--r--   0        0        0     4952 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/paths/context.py
+-rw-r--r--   0        0        0      373 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/paths/html_context.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/renderers/__init__.py
+-rw-r--r--   0        0        0    16264 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/renderers/html_renderer.py
+-rw-r--r--   0        0        0    13975 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/renderers/markdown_renderer.py
+-rw-r--r--   0        0        0     7308 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/renderers/mermaid_renderer.py
+-rw-r--r--   0        0        0     3894 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/renderers/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/style/__init__.py
+-rw-r--r--   0        0        0     3140 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/style/model.py
+-rw-r--r--   0        0        0     3211 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/style/model.yaml
+-rw-r--r--   0        0        0     1976 2023-05-27 01:25:07.266133 linkml_renderer-0.2.0/src/linkml_renderer/style/style_engine.py
+-rw-r--r--   0        0        0     4097 1970-01-01 00:00:00.000000 linkml_renderer-0.2.0/PKG-INFO
```

### Comparing `linkml_renderer-0.1.2/LICENSE` & `linkml_renderer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.1.2/README.md` & `linkml_renderer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.1.2/pyproject.toml` & `linkml_renderer-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "linkml-renderer"
-version = "0.1.2"
+version = "0.2.0"
 description = "linkml-renderer"
 authors = ["Harshad Hegde <hhegde@lbl.gov>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 airium = "^0.2.5"
 click = "^8.1.3"
-linkml = "^1.4.1"
-linkml-runtime = "^1.4.1"
+linkml-runtime = ">=1.4.1"
 myst-parser = {version = "^0.18.1", extras = ["docs"]}
 sphinx = {version = "^5.3.0", extras = ["docs"]}
 sphinx-autodoc-typehints = {version = "^1.19.4", extras = ["docs"]}
 sphinx-click = {version = "^4.3.0", extras = ["docs"]}
 sphinx-rtd-theme = {version = "^1.0.0", extras = ["docs"]}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 poetry-dynamic-versioning = "^0.21.3"
 tox = "^3.25.1"
+linkml = ">=1.4.1"
 
 [tool.poetry.scripts]
 linkml-render = "linkml_renderer.cli:main"
 
 [tool.poetry.extras]
 docs = [
     "sphinx",
```

### Comparing `linkml_renderer-0.1.2/src/linkml_renderer/cli.py` & `linkml_renderer-0.2.0/src/linkml_renderer/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Command line interface for linkml-html."""
 import json
 import logging
+import os
 import sys
 
 import click
 import yaml
-from linkml.utils.datautils import _get_format
 from linkml_runtime import SchemaView
 
 from linkml_renderer import __version__
 from linkml_renderer.renderers.markdown_renderer import MarkdownRenderer
 
 __all__ = [
     "main",
@@ -24,14 +24,38 @@
 
 FORMAT_TO_RENDERER = {
     "html": HTMLRenderer,
     "markdown": MarkdownRenderer,
     "mermaid": MermaidRenderer,
 }
 
+aliases = {
+    "rdf": "ttl",
+    "jsonld": "json-ld",
+}
+
+
+def _get_format(path: str, specified_format: str = None, default=None):
+    if specified_format is None:
+        if path is None:
+            if default is None:
+                raise Exception("Must pass format option OR pass a filename with known file suffix")
+            else:
+                specified_format = default
+        else:
+            _, ext = os.path.splitext(path)
+            if ext is not None:
+                specified_format = ext.replace(".", "")
+            else:
+                raise Exception(f"Must pass format option OR use known file suffix: {path}")
+    specified_format = specified_format.lower()
+    if specified_format in aliases:
+        specified_format = aliases[specified_format]
+    return specified_format
+
 
 @click.command()
 @click.option("-v", "--verbose", count=True)
 @click.option("-q", "--quiet")
 @click.option("-s", "--schema", help="LinkML Schema file")
 @click.option("-c", "--config", help="Configuration file")
 @click.option("-o", "--output", type=click.File("w"), default=sys.stdin, help="Output file")
```

### Comparing `linkml_renderer-0.1.2/src/linkml_renderer/paths/context.py` & `linkml_renderer-0.2.0/src/linkml_renderer/paths/context.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.1.2/src/linkml_renderer/renderers/html_renderer.py` & `linkml_renderer-0.2.0/src/linkml_renderer/renderers/html_renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.1.2/src/linkml_renderer/renderers/markdown_renderer.py` & `linkml_renderer-0.2.0/src/linkml_renderer/renderers/markdown_renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.1.2/src/linkml_renderer/renderers/mermaid_renderer.py` & `linkml_renderer-0.2.0/src/linkml_renderer/renderers/mermaid_renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.1.2/src/linkml_renderer/renderers/renderer.py` & `linkml_renderer-0.2.0/src/linkml_renderer/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.1.2/src/linkml_renderer/style/model.py` & `linkml_renderer-0.2.0/src/linkml_renderer/style/model.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.1.2/src/linkml_renderer/style/model.yaml` & `linkml_renderer-0.2.0/src/linkml_renderer/style/model.yaml`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.1.2/src/linkml_renderer/style/style_engine.py` & `linkml_renderer-0.2.0/src/linkml_renderer/style/style_engine.py`

 * *Files identical despite different names*

### Comparing `linkml_renderer-0.1.2/setup.py` & `linkml_renderer-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: linkml-renderer
+Version: 0.2.0
+Summary: linkml-renderer
+License: Apache Software License 2.0
+Author: Harshad Hegde
+Author-email: hhegde@lbl.gov
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: docs
+Requires-Dist: airium (>=0.2.5,<0.3.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: linkml-runtime (>=1.4.1)
+Requires-Dist: myst-parser[docs] (>=0.18.1,<0.19.0) ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints[docs] (>=1.19.4,<2.0.0) ; extra == "docs"
+Requires-Dist: sphinx-click[docs] (>=4.3.0,<5.0.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme[docs] (>=1.0.0,<2.0.0) ; extra == "docs"
+Requires-Dist: sphinx[docs] (>=5.3.0,<6.0.0) ; extra == "docs"
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# linkml-renderer
 
-packages = \
-['linkml_renderer',
- 'linkml_renderer.paths',
- 'linkml_renderer.renderers',
- 'linkml_renderer.style']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['airium>=0.2.5,<0.3.0',
- 'click>=8.1.3,<9.0.0',
- 'linkml-runtime>=1.4.1,<2.0.0',
- 'linkml>=1.4.1,<2.0.0']
-
-extras_require = \
-{':extra == "docs"': ['myst-parser[docs]>=0.18.1,<0.19.0',
-                      'sphinx[docs]>=5.3.0,<6.0.0',
-                      'sphinx-autodoc-typehints[docs]>=1.19.4,<2.0.0',
-                      'sphinx-click[docs]>=4.3.0,<5.0.0',
-                      'sphinx-rtd-theme[docs]>=1.0.0,<2.0.0']}
-
-entry_points = \
-{'console_scripts': ['linkml-render = linkml_renderer.cli:main']}
-
-setup_kwargs = {
-    'name': 'linkml-renderer',
-    'version': '0.1.2',
-    'description': 'linkml-renderer',
-    'long_description': '# linkml-renderer\n\nGenerating HTML, Markdown, Mermaid, and other rendering artefacts from LinkML data.\n\nThis applies a configurable *generic* mapping between instance data and the target output file.\nThis is an example of a "no code" approach to generating visual representations of data.\n\nIn general, writing custom code (e.g. in Jinja) that is specific to your schema may produce\nmore user-friendly results. LinkML-renderer should only be used in cases where it is harder to\ncommit developer resources to writing custom code.\n\nStatus: experimental\n\n## Command Line Usage\n\nMinimally, you must pass in a schema (LinkML YAML) and a file of instance data conforming to the schema:\n\n`linkml-render -s my-schema.yaml my-data.yaml`\n\nor with a specific output file:\n\n`linkml-render -s my-schema.yaml my-data.yaml -o output.html`\n\nThe default output type is HTML.\n\nTo produce other formats:\n\n`linkml-render -s my-schema.yaml -f markdown my-data.yaml -o output.md`\n\nYou can pass in a configuration file using `--config` (`-c).\n\n`linkml-render -s my-schema.yaml  my-data.yaml -c my-config.yaml`\n\nThe YAML file should conform to the style datamodel Configuration object.\n(note: autodocumentation for this model will be produced later, for now\nconsult the LinkML file).\n\n## Python Usage\n\nWhen this library matures, the python documentation will be linked from the main LinkML docs.\n\nFor now, see the docstrings directly in the source, and the test folder for examples.\n\nSee minimal sphinx docs: https://linkml.github.io/linkml-renderer\n\n## Output types\n\n- HTML\n- Markdown\n- Mermaid\n\nNote that the mermaid can be optionally embedded inside the HTML or Markdown.\n\n## How it works\n\nThe input object is treated as a tree, and nodes in the tree are recursively visited, producing\noutput in the desired format.\n\nFor HTML and markdown generation, the following default rules are applied:\n\n- singular outer objects are translated to Description Lists\n- lists of objects are translated to tables \n\nThese rules are contextual:\n\n- Tables are not nested inside tables\n\nThe rules are also configurable. See the style schema and test cases for details.\n\nFor example, in the person infoschema, a Container contains a list of persons and a list of organizations.\nThe default rendering will create two tables, with each row representing an individual or organization.\n\nThis can lead to wide tables if there are a large number of slots.\n\nIf the `persons` or `organizations` slot is mapped to `RenderType.description_list`, then instead, each item\ngets its own description list, resulting in a longer narrower page.\n\n## Limitations and Future plans\n\nCurrently there are limits to customizability, both in terms of stylesheets and in terms of how schema\nelements map to output elements.\n\nThe HTML generation is currently hardwired to use Bootstrap.\n\nIt is likely that the functionality here may be subsumed into a future linkml.js library. At this time\nthe framework may be extended to include interactive form-based data entry.\n\nThe library has not yet been tested on a wide range of data.\n\n',
-    'author': 'Harshad Hegde',
-    'author_email': 'hhegde@lbl.gov',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+Generating HTML, Markdown, Mermaid, and other rendering artefacts from LinkML data.
+
+This applies a configurable *generic* mapping between instance data and the target output file.
+This is an example of a "no code" approach to generating visual representations of data.
+
+In general, writing custom code (e.g. in Jinja) that is specific to your schema may produce
+more user-friendly results. LinkML-renderer should only be used in cases where it is harder to
+commit developer resources to writing custom code.
+
+Status: experimental
+
+## Command Line Usage
+
+Minimally, you must pass in a schema (LinkML YAML) and a file of instance data conforming to the schema:
+
+`linkml-render -s my-schema.yaml my-data.yaml`
+
+or with a specific output file:
+
+`linkml-render -s my-schema.yaml my-data.yaml -o output.html`
+
+The default output type is HTML.
+
+To produce other formats:
+
+`linkml-render -s my-schema.yaml -f markdown my-data.yaml -o output.md`
+
+You can pass in a configuration file using `--config` (`-c).
+
+`linkml-render -s my-schema.yaml  my-data.yaml -c my-config.yaml`
+
+The YAML file should conform to the style datamodel Configuration object.
+(note: autodocumentation for this model will be produced later, for now
+consult the LinkML file).
+
+## Python Usage
+
+When this library matures, the python documentation will be linked from the main LinkML docs.
+
+For now, see the docstrings directly in the source, and the test folder for examples.
+
+See minimal sphinx docs: https://linkml.github.io/linkml-renderer
+
+## Output types
+
+- HTML
+- Markdown
+- Mermaid
+
+Note that the mermaid can be optionally embedded inside the HTML or Markdown.
+
+## How it works
+
+The input object is treated as a tree, and nodes in the tree are recursively visited, producing
+output in the desired format.
+
+For HTML and markdown generation, the following default rules are applied:
+
+- singular outer objects are translated to Description Lists
+- lists of objects are translated to tables 
+
+These rules are contextual:
+
+- Tables are not nested inside tables
+
+The rules are also configurable. See the style schema and test cases for details.
+
+For example, in the person infoschema, a Container contains a list of persons and a list of organizations.
+The default rendering will create two tables, with each row representing an individual or organization.
+
+This can lead to wide tables if there are a large number of slots.
+
+If the `persons` or `organizations` slot is mapped to `RenderType.description_list`, then instead, each item
+gets its own description list, resulting in a longer narrower page.
+
+## Limitations and Future plans
+
+Currently there are limits to customizability, both in terms of stylesheets and in terms of how schema
+elements map to output elements.
+
+The HTML generation is currently hardwired to use Bootstrap.
+
+It is likely that the functionality here may be subsumed into a future linkml.js library. At this time
+the framework may be extended to include interactive form-based data entry.
+
+The library has not yet been tested on a wide range of data.
 
 
-setup(**setup_kwargs)
```

