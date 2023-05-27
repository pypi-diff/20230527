# Comparing `tmp/hstsparser-1.1.6.tar.gz` & `tmp/hstsparser-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstsparser-1.1.6.tar", max compression
+gzip compressed data, was "hstsparser-1.1.8.tar", max compression
```

## Comparing `hstsparser-1.1.6.tar` & `hstsparser-1.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-05-21 01:24:40.839179 hstsparser-1.1.6/LICENSE
--rw-r--r--   0        0        0     2727 2023-05-21 01:24:40.839179 hstsparser-1.1.6/README.md
--rwxr-xr-x   0        0        0     6281 2023-05-21 01:24:40.839179 hstsparser-1.1.6/hstsparser.py
--rw-r--r--   0        0        0     1356 2023-05-21 01:25:07.231100 hstsparser-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 hstsparser-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-27 00:18:43.203215 hstsparser-1.1.8/LICENSE
+-rw-r--r--   0        0        0     2949 2023-05-27 00:18:43.203215 hstsparser-1.1.8/README.md
+-rwxr-xr-x   0        0        0     6552 2023-05-27 00:18:43.203215 hstsparser-1.1.8/hstsparser.py
+-rw-r--r--   0        0        0     1368 2023-05-27 00:19:12.719627 hstsparser-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3866 1970-01-01 00:00:00.000000 hstsparser-1.1.8/PKG-INFO
```

### Comparing `hstsparser-1.1.6/LICENSE` & `hstsparser-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hstsparser-1.1.6/README.md` & `hstsparser-1.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HSTS Parser
 
-[![Lint Codebase](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml) [![Build Releases](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml) [![Licence](https://img.shields.io/github/license/thebeanogamer/hstsparser)](./LICENSE) ![Python 3.11.x](https://img.shields.io/badge/python-3.11.x-yellow.svg) [![PyPI](https://img.shields.io/pypi/v/hstsparser)](https://pypi.org/project/hstsparser) [![Downloads](https://pepy.tech/badge/hstsparser)](https://pepy.tech/project/hstsparser)
+[![Lint Codebase](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml) [![Build Releases](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml) [![Licence](https://img.shields.io/github/license/thebeanogamer/hstsparser)](./LICENSE) ![Python 3.11.x](https://img.shields.io/badge/python-3.11.x-yellow.svg) [![PyPI](https://img.shields.io/pypi/v/hstsparser)](https://pypi.org/project/hstsparser) [![Downloads](https://pepy.tech/badge/hstsparser)](https://pepy.tech/project/hstsparser) [![Copr build status](https://copr.fedorainfracloud.org/coprs/thebeanogamer/hstsparser/package/hstsparser/status_image/last_build.png)](https://copr.fedorainfracloud.org/coprs/thebeanogamer/hstsparser/package/hstsparser/)
 
 HSTS Parser is a simple tool to parse Firefox and Chrome's HSTS databases into actually helpful forensic artifacts! You can read more about the research behind this tool and potential uses for it over on [my blog](https://blog.daniel-milnes.uk/hsts-for-forensics-you-can-run-but-you-cant)!
 
 ## Installation
 
 HSTS Parser can be installed via pip, or with [Poetry](https://python-poetry.org/).
```

### Comparing `hstsparser-1.1.6/hstsparser.py` & `hstsparser-1.1.8/hstsparser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 import csv
 import datetime
+import importlib.metadata
 import json
 import os
 import re
 import typing
 from argparse import ArgumentParser, Namespace
 from base64 import b64encode
 from hashlib import sha256
@@ -80,15 +81,15 @@
 def date_round(date: datetime.datetime) -> datetime.datetime:
     """Round `datetime` object"""
     return date - datetime.timedelta(
         minutes=date.minute % 10, seconds=date.second, microseconds=date.microsecond
     )
 
 
-parser = ArgumentParser(description="Process HSTS databases")
+parser = ArgumentParser(prog="hstsparser", description="Process HSTS databases")
 parser.add_argument(
     dest="database_file",
     help="The path to the database to be processed",
     metavar="FILE",
     type=lambda x: is_valid_file(parser, x),
 )
 parser.add_argument(
@@ -105,14 +106,21 @@
     metavar="CSV",
     type=lambda x: file_already_exists(parser, x),
 )
 group = parser.add_mutually_exclusive_group(required=True)
 group.add_argument("--firefox", action="store_true", help="Process a Firefox database")
 group.add_argument("--chrome", action="store_true", help="Process a Chrome database")
 
+try:
+    __version__ = importlib.metadata.version("hstsparser")
+except importlib.metadata.PackageNotFoundError:
+    __version__ = "0.0.1"
+
+parser.add_argument('--version', action='version', version=f'%(prog)s {__version__}')
+
 
 def main() -> None:
     """Entry point for command line alias."""
     args = parser.parse_args()
 
     dirtydb = args.database_file.read()
     database = []
```

### Comparing `hstsparser-1.1.6/pyproject.toml` & `hstsparser-1.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstsparser"
-version = "1.1.6"
+version = "1.1.8"
 description = "A tool to parse Firefox and Chrome HSTS databases into forensic artifacts."
 authors = ["Daniel Milnes <daniel@daniel-milnes.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thebeanogamer/hstsparser"
 repository = "https://github.com/thebeanogamer/hstsparser"
 documentation = "https://github.com/thebeanogamer/hstsparser"
@@ -17,32 +17,32 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Security",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-prettytable = "^3.7.0"
+prettytable = ">=0.7.2,<3.8"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.scripts]
+hstsparser = "hstsparser:main"
+
+[tool.poetry.group.windows.dependencies]
+pyinstaller = "^5.11.0"
+pywin32-ctypes = "^0.2.0"
+pefile = "^2023.2.7"
+
+[tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 flake8-bandit = "^4.1.1"
 flake8-bugbear = "^23.5.9"
 flake8-import-order = "^0.18.2"
 flake8-string-format = "^0.3.0"
 flake8-tidy-imports = "^4.8.0"
 flake8-todo = "^0.7"
 safety = "^2.3.5"
 flake8-formatter-junit-xml = "^0.0.6"
 
-[tool.poetry.scripts]
-hstsparser = "hstsparser:main"
-
-[tool.poetry.group.windows.dependencies]
-pyinstaller = "^5.11.0"
-pywin32-ctypes = "^0.2.0"
-pefile = "^2023.2.7"
-
 [build-system]
 requires = ["poetry>=1.3"]
 build-backend = "poetry.masonry.api"
```

### Comparing `hstsparser-1.1.6/PKG-INFO` & `hstsparser-1.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstsparser
-Version: 1.1.6
+Version: 1.1.8
 Summary: A tool to parse Firefox and Chrome HSTS databases into forensic artifacts.
 Home-page: https://github.com/thebeanogamer/hstsparser
 License: MIT
 Keywords: chrome,firefox,dfir,forensics,hsts
 Author: Daniel Milnes
 Author-email: daniel@daniel-milnes.uk
 Requires-Python: >=3.9,<3.12
@@ -12,22 +12,22 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Requires-Dist: prettytable (>=3.7.0,<4.0.0)
+Requires-Dist: prettytable (>=0.7.2,<3.8)
 Project-URL: Documentation, https://github.com/thebeanogamer/hstsparser
 Project-URL: Repository, https://github.com/thebeanogamer/hstsparser
 Description-Content-Type: text/markdown
 
 # HSTS Parser
 
-[![Lint Codebase](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml) [![Build Releases](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml) [![Licence](https://img.shields.io/github/license/thebeanogamer/hstsparser)](./LICENSE) ![Python 3.11.x](https://img.shields.io/badge/python-3.11.x-yellow.svg) [![PyPI](https://img.shields.io/pypi/v/hstsparser)](https://pypi.org/project/hstsparser) [![Downloads](https://pepy.tech/badge/hstsparser)](https://pepy.tech/project/hstsparser)
+[![Lint Codebase](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/lint.yaml) [![Build Releases](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml/badge.svg)](https://github.com/thebeanogamer/hstsparser/actions/workflows/build.yaml) [![Licence](https://img.shields.io/github/license/thebeanogamer/hstsparser)](./LICENSE) ![Python 3.11.x](https://img.shields.io/badge/python-3.11.x-yellow.svg) [![PyPI](https://img.shields.io/pypi/v/hstsparser)](https://pypi.org/project/hstsparser) [![Downloads](https://pepy.tech/badge/hstsparser)](https://pepy.tech/project/hstsparser) [![Copr build status](https://copr.fedorainfracloud.org/coprs/thebeanogamer/hstsparser/package/hstsparser/status_image/last_build.png)](https://copr.fedorainfracloud.org/coprs/thebeanogamer/hstsparser/package/hstsparser/)
 
 HSTS Parser is a simple tool to parse Firefox and Chrome's HSTS databases into actually helpful forensic artifacts! You can read more about the research behind this tool and potential uses for it over on [my blog](https://blog.daniel-milnes.uk/hsts-for-forensics-you-can-run-but-you-cant)!
 
 ## Installation
 
 HSTS Parser can be installed via pip, or with [Poetry](https://python-poetry.org/).
```

