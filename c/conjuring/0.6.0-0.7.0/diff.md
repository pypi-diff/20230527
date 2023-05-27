# Comparing `tmp/conjuring-0.6.0.tar.gz` & `tmp/conjuring-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conjuring-0.6.0.tar", max compression
+gzip compressed data, was "conjuring-0.7.0.tar", max compression
```

## Comparing `conjuring-0.6.0.tar` & `conjuring-0.7.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1629 2023-05-24 21:03:33.289764 conjuring-0.6.0/docs/README.md
--rw-r--r--   0        0        0     3002 2023-05-24 21:03:33.289764 conjuring-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4393 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/__init__.py
--rw-r--r--   0        0        0      564 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/colors.py
--rw-r--r--   0        0        0      605 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/constants.py
--rw-r--r--   0        0        0    11407 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/grimoire.py
--rw-r--r--   0        0        0       50 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/__init__.py
--rw-r--r--   0        0        0     2392 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/aws.py
--rw-r--r--   0        0        0     2089 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/conjuring.py
--rw-r--r--   0        0        0     1319 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/direnv.py
--rw-r--r--   0        0        0     1366 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/docker.py
--rw-r--r--   0        0        0     1928 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/duplicity.py
--rw-r--r--   0        0        0     1126 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/fork.py
--rw-r--r--   0        0        0     3277 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/generic.py
--rw-r--r--   0        0        0    15370 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/git.py
--rw-r--r--   0        0        0     1288 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/jrnl.py
--rw-r--r--   0        0        0     3289 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/k8s.py
--rw-r--r--   0        0        0     7568 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/media.py
--rw-r--r--   0        0        0      949 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/mkdocs.py
--rw-r--r--   0        0        0     2807 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/mr.py
--rw-r--r--   0        0        0      966 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/onedrive.py
--rw-r--r--   0        0        0    12527 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/paperless.py
--rw-r--r--   0        0        0     2946 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/pre_commit.py
--rw-r--r--   0        0        0     9810 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/py.py
--rw-r--r--   0        0        0     1151 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/spells/shell.py
--rw-r--r--   0        0        0     2690 2023-05-24 21:03:33.289764 conjuring-0.6.0/src/conjuring/visibility.py
--rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 conjuring-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1629 2023-05-27 00:01:06.073684 conjuring-0.7.0/docs/README.md
+-rw-r--r--   0        0        0     3277 2023-05-27 00:01:06.073684 conjuring-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4407 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/__main__.py
+-rw-r--r--   0        0        0     5831 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/cli.py
+-rw-r--r--   0        0        0      564 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/colors.py
+-rw-r--r--   0        0        0      661 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/constants.py
+-rw-r--r--   0        0        0    11522 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/grimoire.py
+-rw-r--r--   0        0        0       50 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/__init__.py
+-rw-r--r--   0        0        0     2392 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/aws.py
+-rw-r--r--   0        0        0     1319 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/direnv.py
+-rw-r--r--   0        0        0     1366 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/docker.py
+-rw-r--r--   0        0        0     1928 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/duplicity.py
+-rw-r--r--   0        0        0     1126 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/fork.py
+-rw-r--r--   0        0        0     3277 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/generic.py
+-rw-r--r--   0        0        0    15590 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/git.py
+-rw-r--r--   0        0        0     1288 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/jrnl.py
+-rw-r--r--   0        0        0     3289 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/k8s.py
+-rw-r--r--   0        0        0     7568 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/media.py
+-rw-r--r--   0        0        0      949 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/mkdocs.py
+-rw-r--r--   0        0        0     2807 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/mr.py
+-rw-r--r--   0        0        0      966 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/onedrive.py
+-rw-r--r--   0        0        0    12527 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/paperless.py
+-rw-r--r--   0        0        0     2946 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/pre_commit.py
+-rw-r--r--   0        0        0    10199 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/py.py
+-rw-r--r--   0        0        0     1151 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/spells/shell.py
+-rw-r--r--   0        0        0     2690 2023-05-27 00:01:06.073684 conjuring-0.7.0/src/conjuring/visibility.py
+-rw-r--r--   0        0        0     2818 1970-01-01 00:00:00.000000 conjuring-0.7.0/PKG-INFO
```

### Comparing `conjuring-0.6.0/docs/README.md` & `conjuring-0.7.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/pyproject.toml` & `conjuring-0.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "conjuring"
-version = "0.6.0"
+version = "0.7.0"
 description = "🐍🤖 Reusable global Invoke tasks that can be merged with local project tasks"
 authors = ["W. Augusto Andreoli <andreoliwa@gmail.com>"]
 license = "MIT"
 readme = "docs/README.md"
 repository = "https://github.com/andreoliwa/conjuring"
 documentation = "https://andreoliwa.github.io/conjuring/"
 keywords = ["invoke", "tasks", "automation", "cli", "python"]
@@ -19,21 +19,29 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 invoke = "*"
 requests = "*"
 typer = "*"
+ruamel-yaml = "*"
+iterfzf = "*"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "*"
+pytest-cov = "*"
+pytest-datadir = "*"
+pytest-mock = "*"
+
+[tool.poetry.scripts]
+conjuring = "conjuring.cli:app"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.0"
+version = "0.7.0"
 
 # https://commitizen-tools.github.io/commitizen/bump/#configuration
 version_files = [
     "pyproject.toml:^version"
 ]
 tag_format = "v$version"
 update_changelog_on_bump = true
@@ -73,24 +81,27 @@
     "D107", # Missing docstring in ?
     "D203", # 1 blank line required before class docstring
     "D213", # Multi-line docstring summary should start at the second line
     "ERA", # https://beta.ruff.rs/docs/rules/#eradicate-era
     "FBT001", # Boolean positional arg in function definition
     "FBT002", # Boolean default value in function definition
     "FBT003", # Boolean positional value in function call
+    "TD001", # Invalid TO DO tag
     "TD002", # Missing author https://beta.ruff.rs/docs/rules/#flake8-todos-td
     "TD003", # Missing issue link on the line following this
 ]
 
 # https://beta.ruff.rs/docs/settings/#per-file-ignores
 [tool.ruff.per-file-ignores]
+# B008 Do not perform function call ? in argument defaults
 # D100 Missing docstring in public module
 # D103 Missing docstring in public function
 # D104 Missing docstring in public package
 # S101 Use of ? detected https://beta.ruff.rs/docs/rules/?q=S101
+"src/conjuring/cli.py" = ["B008"]
 "tests/**" = ["D100", "D103", "D104", "S101"]
 
 # https://beta.ruff.rs/docs/rules/#flake8-quotes-q
 [tool.ruff.flake8-quotes]
 inline-quotes = "double"
 
 # https://beta.ruff.rs/docs/rules/#mccabe-c90
```

### Comparing `conjuring-0.6.0/src/conjuring/__init__.py` & `conjuring-0.7.0/src/conjuring/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import importlib
 import sys
 from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING
 
+from conjuring.constants import CONJURING_SPELLS_DIR
 from conjuring.grimoire import collection_from_python_files, magically_add_tasks
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from invoke import Collection
 
@@ -35,15 +36,15 @@
     """A book with Invoke spells to cast."""
 
     def __init__(self) -> None:
         self.python_modules_to_import: dict[str, set[Path]] = defaultdict(set)
         self.sys_path_dirs: dict[Path, str] = {}
 
     def import_dirs(self, *spell_dir: str | Path) -> Spellbook:  # TODO: test
-        """Import all spells from the given glob pattern."""
+        """Import all Invoke tasks from the modules or packages that match the glob pattern."""
         for str_or_path in spell_dir:
             dir_ = Path(str_or_path).expanduser()
             if not dir_.is_dir():
                 msg = f"{dir_} is not a directory"
                 raise ValueError(msg)
 
             package = ""
@@ -81,19 +82,18 @@
             sys.modules[__name__],
             "tasks.py",
             "conjuring*.py",
             include=config.include,
             exclude=config.exclude,
         )
 
-        conjuring_spell_dir = (Path(__file__).parent / "spells").absolute()
         self._add_tasks(
             namespace,
-            sorted(conjuring_spell_dir.glob("*.py")),
-            ".".join(conjuring_spell_dir.parts[-2:]),
+            sorted(CONJURING_SPELLS_DIR.glob("*.py")),
+            ".".join(CONJURING_SPELLS_DIR.parts[-2:]),
             config,
         )
 
         # Add the package to PYTHONPATH so that we can import its modules
         package_count = 0
         for package_dir, package in self.sys_path_dirs.items():
             sys.path.insert(0, str(package_dir))
```

### Comparing `conjuring-0.6.0/src/conjuring/colors.py` & `conjuring-0.7.0/src/conjuring/colors.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/constants.py` & `conjuring-0.7.0/src/conjuring/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Paths, filenames and other constants."""
 from pathlib import Path
 
 # Paths
+CONJURING_SPELLS_DIR = Path(__file__).parent / "spells"
 DESKTOP_DIR = Path("~/Desktop").expanduser()
 DOCUMENTS_DIR = Path("~/Documents").expanduser()
 DOWNLOADS_DIR = Path("~/Downloads").expanduser()
 ONEDRIVE_DIR = Path("~/OneDrive").expanduser()
 ONEDRIVE_PICTURES_DIR = ONEDRIVE_DIR / "Pictures"
 
 # Filenames
```

### Comparing `conjuring-0.6.0/src/conjuring/grimoire.py` & `conjuring-0.7.0/src/conjuring/grimoire.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Helper functions used in other modules."""
 from __future__ import annotations
 
 import fnmatch
 import os
+import re
 import sys
 import time
 from collections import defaultdict
 from dataclasses import dataclass
 from importlib import import_module
 from pathlib import Path
 from shlex import quote
@@ -19,16 +20,19 @@
 from conjuring.colors import COLOR_BOLD_WHITE, COLOR_LIGHT_GREEN, COLOR_LIGHT_RED, COLOR_NONE, COLOR_YELLOW
 from conjuring.visibility import display_task
 
 if TYPE_CHECKING:
     import types
     from collections.abc import Sequence
 
+# TODO: document or remove this variable
 CONJURING_IGNORE_MODULES = os.environ.get("CONJURING_IGNORE_MODULES", "").split(",")
 
+REGEX_JIRA = re.compile(r"[A-Z]+-\d+")
+
 
 def join_pieces(*pieces: str) -> str:
     """Join pieces, ignoring empty strings."""
     return " ".join(str(piece) for piece in pieces if str(piece).strip())
 
 
 def run_command(c: Context, *pieces: str, dry: bool | None = None, **kwargs: str | bool) -> Result:
@@ -160,15 +164,15 @@
     NOTE: this is unstable and may break because Invoke has no public API to get the final task name.
     """
     formatted_task_name = slugify(name).replace("_", "-")
     return f"{prefix}.{formatted_task_name}" if prefix else formatted_task_name
 
 
 @dataclass
-class SpellBook:
+class PrefixedSpellbook:
     """A collection of Invoke tasks from a module, with a prefix."""
 
     prefix: str
     module: types.ModuleType
     display_all_tasks: bool
 
 
@@ -214,27 +218,27 @@
     1. If the task is a :py:class:`MagicTask`, then its ``should_display()`` method is used to check visibility.
     2. If the module has a ``should_display_tasks()`` function,
         it determines if the module is visible in the current directory.
     3. If the module has a ``SHOULD_PREFIX`` boolean variable defined,
         then the tasks will be added to the collection with a prefix.
     """
     resolved_module = resolve_module_str(from_module_or_str)
-    prefixed_spell_books: dict[str, list[SpellBook]] = defaultdict(list)
+    prefixed_spell_books: dict[str, list[PrefixedSpellbook]] = defaultdict(list)
 
     sub_collection = Collection.from_module(resolved_module)
     for t in sub_collection.tasks.values():
         task_module = import_module(t.__module__)
         should_display_tasks = getattr(task_module, "should_display_tasks", lambda: True)
         display_all_tasks = should_display_tasks()
 
         use_prefix: bool = getattr(task_module, "SHOULD_PREFIX", False)
         if use_prefix:
             # The module should have a prefix: add it later as a sub-collection of the main collection
             prefix = task_module.__name__.split(".")[-1]
-            prefixed_spell_books[prefix].append(SpellBook(prefix, task_module, display_all_tasks))
+            prefixed_spell_books[prefix].append(PrefixedSpellbook(prefix, task_module, display_all_tasks))
             continue
         if not display_task(t, display_all_tasks):
             continue
 
         if t.name in to_collection.tasks and resolved_module:
             # Task already exists with the same name: add a suffix
             clean_name = slugify(resolved_module.__name__)
```

### Comparing `conjuring-0.6.0/src/conjuring/spells/aws.py` & `conjuring-0.7.0/src/conjuring/spells/aws.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/direnv.py` & `conjuring-0.7.0/src/conjuring/spells/direnv.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/docker.py` & `conjuring-0.7.0/src/conjuring/spells/docker.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/duplicity.py` & `conjuring-0.7.0/src/conjuring/spells/duplicity.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/fork.py` & `conjuring-0.7.0/src/conjuring/spells/fork.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/generic.py` & `conjuring-0.7.0/src/conjuring/spells/generic.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/git.py` & `conjuring-0.7.0/src/conjuring/spells/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Git: update all, extract subtree, rewrite history, ..."""
-import re
 from configparser import ConfigParser
 from dataclasses import dataclass
 from functools import lru_cache
 from pathlib import Path
 
 import typer
 from invoke import Context, Exit, UnexpectedExit, task
 
 from conjuring.colors import COLOR_LIGHT_RED, COLOR_NONE
 from conjuring.grimoire import (
+    REGEX_JIRA,
     print_error,
     print_success,
     run_command,
     run_lines,
     run_multiple,
     run_stdout,
     run_with_fzf,
@@ -378,30 +378,36 @@
     if "no pull requests found for branch" in out:
         c.run("gh repo view --web")
 
 
 @task(
     help={
         "prefix": "Keep the Conventional Commits prefix",
-        "sort": "Sort bullets",
+        "original_order": "Don't sort bullets, keep them in original order",
     },
 )
-def body(c: Context, prefix: bool = True, sort: bool = True) -> None:
+def body(c: Context, prefix: bool = False, original_order: bool = False) -> None:
     """Prepare a commit body to be used on pull requests and squashed commits."""
     default_branch = set_default_branch(c)
     bullets = []
     for line in run_lines(c, f"git log {default_branch}..", "--format=%s%n%b"):
         clean = line.strip(" -")
-        if "Merge branch" in clean or "Revert " in clean or "This reverts" in clean or not clean:
+        if (
+            "Merge branch" in clean
+            or "Merge remote-tracking branch" in clean
+            or "Revert " in clean
+            or "This reverts" in clean
+            or not clean
+        ):
             continue
 
+        # Remove Jira ticket with regex
+        clean = REGEX_JIRA.sub("", clean).replace("()", "").replace("[]", "").strip(" -")
+
         # Split on the Conventional Commit prefix
         if not prefix and ":" in clean:
-            clean = clean.split(":", 1)[1]
-
-        # Remove Jira ticket with regex
-        clean = re.sub(r"\[?\D+-\d+[\]:]", "", clean).strip(" -")
+            clean = clean.split(":", 1)[1].strip()
 
         bullets.append(f"- {clean}")
 
-    results = sorted(set(bullets)) if sort else bullets
+    results = bullets if original_order else sorted(set(bullets))
     typer.echo("\n".join(results))
```

### Comparing `conjuring-0.6.0/src/conjuring/spells/jrnl.py` & `conjuring-0.7.0/src/conjuring/spells/jrnl.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/k8s.py` & `conjuring-0.7.0/src/conjuring/spells/k8s.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/media.py` & `conjuring-0.7.0/src/conjuring/spells/media.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/mkdocs.py` & `conjuring-0.7.0/src/conjuring/spells/mkdocs.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/mr.py` & `conjuring-0.7.0/src/conjuring/spells/mr.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/onedrive.py` & `conjuring-0.7.0/src/conjuring/spells/onedrive.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/paperless.py` & `conjuring-0.7.0/src/conjuring/spells/paperless.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/pre_commit.py` & `conjuring-0.7.0/src/conjuring/spells/pre_commit.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/spells/py.py` & `conjuring-0.7.0/src/conjuring/spells/py.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Python and Poetry: install venvs, run tests and coverage, install debug tools, generate Ruff config."""
 import re
 from collections import defaultdict
+from dataclasses import dataclass
 from pathlib import Path
 from textwrap import dedent
 from typing import Optional
 
 import typer
 from invoke import Context, Result, task
 
@@ -15,19 +16,19 @@
 SHOULD_PREFIX = True
 should_display_tasks: ShouldDisplayTasks = is_poetry_project
 
 REGEX_RUFF_LINE = re.compile(r"^(?P<filename>.*?):\d+:\d+: (?P<code>.*?)(?P<message> .*)$")
 REGEX_RUFF_MESSAGE = re.compile(r"`[^`]+`")
 
 
+@dataclass
 class PyEnv:
     """pyenv-related tasks."""
 
-    def __init__(self, context: Context) -> None:
-        self.context = context
+    context: Context
 
     def has_local(self) -> bool:
         """Check if a local Python version is set."""
         output = self.context.run("pyenv local", warn=True).stdout.strip()
         return output and "no local version" not in output
 
     def set_local(self, python_version: str) -> Result:
@@ -40,19 +41,19 @@
         all_versions = run_lines(self.context, "pyenv versions --bare")
         if not python_version:
             return all_versions
 
         return [version for version in all_versions if version.startswith(python_version)]
 
 
+@dataclass()
 class Poetry:
     """Poetry-related tasks."""
 
-    def __init__(self, context: Context) -> None:
-        self.context = context
+    context: Context
 
     def used_in_project(self, display_error: bool = True) -> bool:
         """Check if Poetry is being used."""
         used = int(
             run_command(
                 self.context,
                 f"grep tool.poetry {PYPROJECT_TOML} 2>/dev/null | wc -c",
@@ -92,14 +93,26 @@
         return list(versions)[0]
 
     def use_venv(self, python_version: str) -> Result:
         """Use a Poetry venv."""
         return self.context.run(f"poetry env use python{python_version}")
 
 
+class Pytest:
+    """Pytest-related tasks."""
+
+    @staticmethod
+    def command(s: bool) -> str:
+        """Build pytest command."""
+        command = "pytest -v"
+        if s:
+            command += " -s"
+        return command
+
+
 @task(help={"inject": "Pipx repo to inject this project into"})
 def editable(c: Context, inject: str = "") -> None:
     """Hack to install a Poetry package as editable until Poetry supports PEP660 hooks.
 
     It won't be needed anymore when https://github.com/python-poetry/poetry-core/pull/182 is merged.
     """
     if not Poetry(c).used_in_project():
@@ -148,36 +161,46 @@
     if force and not delete_all:
         poetry.remove_venv(version)
     poetry.use_venv(version)
 
     c.run("poetry lock --check && poetry install")
 
 
-@task(help={"watch": "Watch for changes and re-run affected tests. Install pytest-watch and pytest-testmon first."})
-def test(c: Context, watch: bool = False) -> None:
+@task(
+    help={
+        "watch": "Watch for changes and re-run affected tests. Install pytest-watch and pytest-testmon first.",
+        "s": "Don't capture output (same shortcut as pytest)",
+    },
+)
+def test(c: Context, watch: bool = False, s: bool = False) -> None:
     """Run tests with pytest."""
     if not Poetry(c).used_in_project():
         return
 
-    command = 'ptw --runner "pytest --testmon"' if watch else "pytest -v"
+    command = 'ptw --runner "pytest --testmon"' if watch else Pytest.command(s)
     run_command(c, "poetry run", command)
 
 
-@task(help={"show_all": "Show all lines, even if they are covered"})
-def coverage(c: Context, show_all: bool = False) -> None:
+@task(
+    help={
+        "show_all": "Show all lines, even if they are covered",
+        "s": "Don't capture output (same shortcut as pytest)",
+    },
+)
+def coverage(c: Context, show_all: bool = False, s: bool = False) -> None:
     """Run tests with pytest and coverage."""
     if not Poetry(c).used_in_project():
         return
 
     options = [f"--cov={source}" for source in ["src", Path.cwd().name, "app"] if Path(source).exists()]
 
     skip_option = "" if show_all else ":skip-covered"
     options.append(f"--cov-report=term-missing{skip_option}")
 
-    run_command(c, "poetry run pytest -v", *options)
+    run_command(c, "poetry run", Pytest.command(s), *options)
 
 
 @task(
     help={
         "all_": "Install all debug tools",
         "ipython": "Install https://pypi.org/project/ipython/",
         "ipdb": "Install https://pypi.org/project/ipdb/",
```

### Comparing `conjuring-0.6.0/src/conjuring/spells/shell.py` & `conjuring-0.7.0/src/conjuring/spells/shell.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/src/conjuring/visibility.py` & `conjuring-0.7.0/src/conjuring/visibility.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.6.0/PKG-INFO` & `conjuring-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conjuring
-Version: 0.6.0
+Version: 0.7.0
 Summary: 🐍🤖 Reusable global Invoke tasks that can be merged with local project tasks
 Home-page: https://github.com/andreoliwa/conjuring
 License: MIT
 Keywords: invoke,tasks,automation,cli,python
 Author: W. Augusto Andreoli
 Author-email: andreoliwa@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -17,15 +17,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Dist: invoke
+Requires-Dist: iterfzf
 Requires-Dist: requests
+Requires-Dist: ruamel-yaml
 Requires-Dist: typer
 Project-URL: Documentation, https://andreoliwa.github.io/conjuring/
 Project-URL: Repository, https://github.com/andreoliwa/conjuring
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable-file MD031 -->
```

