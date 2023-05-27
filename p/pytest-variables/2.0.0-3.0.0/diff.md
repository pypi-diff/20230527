# Comparing `tmp/pytest-variables-2.0.0.tar.gz` & `tmp/pytest_variables-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-variables-2.0.0.tar", max compression
+gzip compressed data, last modified: Sat May 27 19:24:26 2023, max compression
```

## Comparing `pytest-variables-2.0.0.tar` & `pytest_variables-3.0.0.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0      193 2022-03-27 00:53:54.743672 pytest-variables-2.0.0/LICENSE
--rw-r--r--   0        0        0     4728 2022-03-27 00:53:54.743672 pytest-variables-2.0.0/README.rst
--rw-r--r--   0        0        0     1534 2022-03-27 00:53:54.743672 pytest-variables-2.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-03-27 00:53:54.743672 pytest-variables-2.0.0/src/pytest_variables/__init__.py
--rw-r--r--   0        0        0      280 2022-03-27 00:53:54.743672 pytest-variables-2.0.0/src/pytest_variables/errors.py
--rw-r--r--   0        0        0     3248 2022-03-27 00:53:54.743672 pytest-variables-2.0.0/src/pytest_variables/plugin.py
--rw-r--r--   0        0        0     4700 2022-03-27 00:53:54.743672 pytest-variables-2.0.0/test_variables.py
--rw-r--r--   0        0        0     5907 2022-03-27 00:54:34.651013 pytest-variables-2.0.0/setup.py
--rw-r--r--   0        0        0     6071 2022-03-27 00:54:34.651491 pytest-variables-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      448 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1933 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/CHANGES.rst
+-rw-r--r--   0        0        0     1758 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/development.rst
+-rw-r--r--   0        0        0      738 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/tox.ini
+-rw-r--r--   0        0        0        0 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/src/pytest_variables/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/src/pytest_variables/__version.py
+-rw-r--r--   0        0        0      280 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/src/pytest_variables/errors.py
+-rw-r--r--   0        0        0     3319 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/src/pytest_variables/plugin.py
+-rw-r--r--   0        0        0     4700 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/tests/test_variables.py
+-rw-r--r--   0        0        0      102 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/.gitignore
+-rw-r--r--   0        0        0      193 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4728 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/README.rst
+-rw-r--r--   0        0        0     2017 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6616 2023-05-27 19:24:26.000000 pytest_variables-3.0.0/PKG-INFO
```

### Comparing `pytest-variables-2.0.0/README.rst` & `pytest_variables-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-variables-2.0.0/pyproject.toml` & `pytest_variables-3.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,83 @@
 [build-system]
- requires = ["poetry-core>=1.0.0"]
- build-backend = "poetry.core.masonry.api"
+build-backend = "hatchling.build"
+requires = [
+  "hatch-vcs>=0.3",
+  "hatchling>=1.13",
+]
 
-[tool.poetry]
+[project]
 name = "pytest-variables"
-version = "2.0.0"
 description = "pytest plugin for providing variables to tests/fixtures"
-license = "MPL-2.0"
-authors = [
-    "Dave Hunt <dhunt@mozilla.com>",
-    "Jim Brännlund <jimbrannlund@fastmail.com>"
-]
 readme = "README.rst"
-homepage = "https://github.com/pytest-dev/pytest-variables"
-repository = "https://github.com/pytest-dev/pytest-variables"
+license = "MPL-2.0"
+requires-python = ">=3.7"
 keywords = [
     "pytest",
     "json",
     "variables"
 ]
+authors = [
+  { name = "Dave Hunt", email =  "dhunt@mozilla.com" },
+  { name = "Jim Brannlund", email = "jimbrannlund@fastmail.com" },
+]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Framework :: Pytest",
-    "Intended Audience :: Developers",
-    "Operating System :: POSIX",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: MacOS :: MacOS X",
-    "Topic :: Software Development :: Quality Assurance",
-    "Topic :: Software Development :: Testing",
-    "Topic :: Utilities",
-]
-packages = [
-    { include = "pytest_variables", from = "src" },
-]
-include = [
-    "test_variables.py",
-]
-
-[tool.poetry.dependencies]
-python = "^3.7"
-pytest = ">=3.0.0,<8.0.0"
-
-hjson = { version = "*", optional = true }
-PyYAML = { version = "*", optional = true }
-toml = { version = "*", optional = true }
-
-[tool.poetry.extras]
-hjson = ["hjson"]
-yaml = ["PyYAML"]
-toml = ["toml"]
-
-[tool.poetry.dev-dependencies]
-black = "^22.1.0"
-flake8 = "^4.0.1"
-tox = "^3.24.5"
-pre-commit = "^2.17.0"
+  "Development Status :: 5 - Production/Stable",
+  "Framework :: Pytest",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Operating System :: POSIX",
+  "Operating System :: Microsoft :: Windows",
+  "Operating System :: MacOS :: MacOS X",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
+  "Topic :: Software Development :: Quality Assurance",
+  "Topic :: Software Development :: Testing",
+  "Topic :: Utilities",
+]
+dependencies = [
+  "pytest>=7.0.0",
+]
+dynamic = [
+  "version",
+]
+
+[project.optional-dependencies]
+hjson = [ "hjson" ]
+yaml = [ "PyYAML" ]
+toml = [ "toml" ]
+test = [
+  "black>=22.1.0",
+  "flake8>=4.0.1",
+  "pre-commit>=2.17.0",
+  "tox>=3.24.5",
+]
 
-[tool.poetry.plugins.pytest11]
+[project.urls]
+Homepage = "https://github.com/pytest-dev/pytest-variables"
+Tracker = "https://github.com/pytest-dev/pytest-variables/issues"
+Source = "https://github.com/pytest-dev/pytest-variables"
+
+[project.entry-points.pytest11]
 variables = 'pytest_variables.plugin'
 
-[tool.black]
-target-version = ['py37']
+[tool.hatch.envs.test]
+features = [
+  "test",
+]
+
+[tool.hatch.version]
+source = "vcs"
+
+[tool.hatch.build.targets.sdist]
+exclude = [
+  "/.github",
+]
+
+[tool.hatch.build.hooks.vcs]
+version-file = "src/pytest_variables/__version.py"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytest-variables-2.0.0/src/pytest_variables/plugin.py` & `pytest_variables-3.0.0/src/pytest_variables/plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     with io.open(path, "r", encoding="utf8") as f:
         try:
             return module.load(f, Loader=getattr(module, loader))
         except (AttributeError, TypeError):  # Module is not yaml or no loader
             return module.load(f)
 
 
+variables_key = pytest.StashKey[dict]()
+
 parser_table = {
     "json": ("json", default),
     "hjson": ("hjson", default),
     "yml": ("yaml", default),
     "yaml": ("yaml", default),
     "toml": ("toml", default),
 }
@@ -76,15 +78,15 @@
                 a[key] = b[key]
         else:
             a[key] = b[key]
     return a
 
 
 def pytest_configure(config):
-    config._variables = {}
+    config.stash[variables_key] = {}
     paths = config.getoption("variables")
     loader = config.getini("yaml_loader")
     for path in paths:
         ext = os.path.splitext(path)[1][1:].lower() or "json"
         try:
             import_type, parser_func = parser_table[ext]
             variables = import_parser(path, import_type, parser_func, loader)
@@ -100,14 +102,14 @@
             variables = import_parser(path, *parser_table["json"])
         except ValueError as e:
             raise errors.ValueError("Unable to parse {0}: {1}".format(path, e))
 
         if not isinstance(variables, dict):
             raise errors.ValueError("Unable to parse {0}".format(path))
 
-        reduce(_merge, [config._variables, variables])
+        reduce(_merge, [config.stash[variables_key], variables])
 
 
 @pytest.fixture(scope="session")
 def variables(pytestconfig):
     """Provide test variables from a specified file"""
-    return pytestconfig._variables
+    return pytestconfig.stash[variables_key]
```

### Comparing `pytest-variables-2.0.0/test_variables.py` & `pytest_variables-3.0.0/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `pytest-variables-2.0.0/PKG-INFO` & `pytest_variables-3.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 Metadata-Version: 2.1
 Name: pytest-variables
-Version: 2.0.0
+Version: 3.0.0
 Summary: pytest plugin for providing variables to tests/fixtures
-Home-page: https://github.com/pytest-dev/pytest-variables
-License: MPL-2.0
-Keywords: pytest,json,variables
-Author: Dave Hunt
-Author-email: dhunt@mozilla.com
-Requires-Python: >=3.7,<4.0
+Project-URL: Homepage, https://github.com/pytest-dev/pytest-variables
+Project-URL: Tracker, https://github.com/pytest-dev/pytest-variables/issues
+Project-URL: Source, https://github.com/pytest-dev/pytest-variables
+Author-email: Dave Hunt <dhunt@mozilla.com>, Jim Brannlund <jimbrannlund@fastmail.com>
+License-Expression: MPL-2.0
+License-File: LICENSE
+Keywords: json,pytest,variables
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Requires-Dist: pytest>=7.0.0
 Provides-Extra: hjson
+Requires-Dist: hjson; extra == 'hjson'
+Provides-Extra: test
+Requires-Dist: black>=22.1.0; extra == 'test'
+Requires-Dist: flake8>=4.0.1; extra == 'test'
+Requires-Dist: pre-commit>=2.17.0; extra == 'test'
+Requires-Dist: tox>=3.24.5; extra == 'test'
 Provides-Extra: toml
+Requires-Dist: toml; extra == 'toml'
 Provides-Extra: yaml
-Requires-Dist: PyYAML; extra == "yaml"
-Requires-Dist: hjson; extra == "hjson"
-Requires-Dist: pytest (>=3.0.0,<8.0.0)
-Requires-Dist: toml; extra == "toml"
-Project-URL: Repository, https://github.com/pytest-dev/pytest-variables
+Requires-Dist: pyyaml; extra == 'yaml'
 Description-Content-Type: text/x-rst
 
 pytest-variables
 ================
 
 pytest-variables is a plugin for pytest_ that provides variables to
 tests/fixtures as a dictionary via a file specified on the command line.
@@ -219,8 +228,7 @@
 .. _Human JSON: http://hjson.org
 .. _YAML: http://yaml.org
 .. _TOML: https://github.com/toml-lang/toml
 .. _dictionary: https://docs.python.org/tutorial/datastructures.html#dictionaries
 .. _Release Notes:  http://github.com/pytest-dev/pytest-variables/blob/master/CHANGES.rst
 .. _Issue Tracker: http://github.com/pytest-dev/pytest-variables/issues
 .. _Code: http://github.com/pytest-dev/pytest-variables
-
```

