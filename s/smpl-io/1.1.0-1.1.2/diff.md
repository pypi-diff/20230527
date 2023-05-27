# Comparing `tmp/smpl_io-1.1.0.tar.gz` & `tmp/smpl_io-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpl_io-1.1.0.tar", max compression
+gzip compressed data, was "smpl_io-1.1.2.tar", max compression
```

## Comparing `smpl_io-1.1.0.tar` & `smpl_io-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-04-02 09:08:17.487420 smpl_io-1.1.0/LICENSE
--rw-r--r--   0        0        0     2814 2023-04-02 09:08:17.487420 smpl_io-1.1.0/README.md
--rw-r--r--   0        0        0     1559 2023-04-02 09:08:19.875433 smpl_io-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    16384 2023-04-02 09:08:17.491420 smpl_io-1.1.0/smpl_io/.io.py.swp
--rw-r--r--   0        0        0      137 2023-04-02 09:08:17.491420 smpl_io-1.1.0/smpl_io/__init__.py
--rw-r--r--   0        0        0     1100 2023-04-02 09:08:17.491420 smpl_io-1.1.0/smpl_io/grep.py
--rw-r--r--   0        0        0     1024 2023-04-02 09:08:17.491420 smpl_io-1.1.0/smpl_io/head.py
--rw-r--r--   0        0        0     7798 2023-04-02 09:08:17.491420 smpl_io-1.1.0/smpl_io/io.py
--rw-r--r--   0        0        0      540 2023-04-02 09:08:17.491420 smpl_io-1.1.0/smpl_io/read_buffer.py
--rw-r--r--   0        0        0      538 2023-04-02 09:08:17.491420 smpl_io-1.1.0/smpl_io/sed.py
--rw-r--r--   0        0        0     1008 2023-04-02 09:08:17.491420 smpl_io-1.1.0/smpl_io/tail.py
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 smpl_io-1.1.0/setup.py
--rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 smpl_io-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-27 17:23:26.869935 smpl_io-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2814 2023-05-27 17:23:26.869935 smpl_io-1.1.2/README.md
+-rw-r--r--   0        0        0     1670 2023-05-27 17:23:28.677974 smpl_io-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      137 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/__init__.py
+-rw-r--r--   0        0        0     1100 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/grep.py
+-rw-r--r--   0        0        0     1024 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/head.py
+-rw-r--r--   0        0        0     8396 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/io.py
+-rw-r--r--   0        0        0      540 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/read_buffer.py
+-rw-r--r--   0        0        0      538 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/sed.py
+-rw-r--r--   0        0        0     1008 2023-05-27 17:23:26.869935 smpl_io-1.1.2/smpl_io/tail.py
+-rw-r--r--   0        0        0     3563 1970-01-01 00:00:00.000000 smpl_io-1.1.2/setup.py
+-rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 smpl_io-1.1.2/PKG-INFO
```

### Comparing `smpl_io-1.1.0/LICENSE` & `smpl_io-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.0/README.md` & `smpl_io-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.0/pyproject.toml` & `smpl_io-1.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 [tool.poetry]
 name = "smpl_io"
-version = "1.1.0"
+version = "1.1.2"
 description = "simple input and output for python"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/smpl_io"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-smpl_doc = "*"
+smpl_doc =  "^1.0.5"
+requests = "*"
+
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
+pytest = "*"
+pytest-cov =  "*"
+pytest-profiling =  "*"
+#pytest-line-profiler-apn = {path="/home/apn/git/pytest-line-profiler", develop = true}
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "*"
 sphinx-rtd-theme = "*"
@@ -28,22 +38,18 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pandas = ">=1.0.0"
 pre-commit = "^2.20.0"
-pytest = "*"
-pytest-cov =  "*"
-pytest-profiling =  "*"
-#pytest-line-profiler-apn = {path="/home/apn/git/pytest-line-profiler", develop = true}
+poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21.1,<0.23.0"}
 #ipython =  "*"
 #jupyterlab =  "*"
 #jupyter = "*"
-poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.21.1"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `smpl_io-1.1.0/smpl_io/grep.py` & `smpl_io-1.1.2/smpl_io/grep.py`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.0/smpl_io/head.py` & `smpl_io-1.1.2/smpl_io/head.py`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.0/smpl_io/io.py` & `smpl_io-1.1.2/smpl_io/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,55 @@
 """Simplified input and output."""
+import contextlib
 import os
 import pathlib
+import re
+import shutil
 import sys
 from io import StringIO
 from pathlib import Path
-import re
-import shutil
-import contextlib
 
+import requests
 
 from .grep import *
-from .tail import *
 from .head import *
 from .sed import *
+from .tail import *
 
 
+def read(to_be_read: str):
+    """
+    Open either a file or URI and return the content.
+    Reads the file ``to_be_read``.
+
+    Parameters
+    ----------
+    fname : str
+        file name.
+
+    Returns
+    -------
+    str
+        content of the file.
+
+    Examples
+    --------
+    >>> read("nonexistent.txt")
+    ''
+    >>> write("test.out","hi")
+    >>> read("test.out")
+    'hi'
+    """
+    if to_be_read.startswith("http"):
+        return requests.get(to_be_read).text
+    else:
+        if not os.path.exists(to_be_read):
+            return ""
+        with open(to_be_read, "r") as f:
+            return f.read()
 
 
 @contextlib.contextmanager
 def pushd(new_dir, tmp=False, cd=True):
     """
     Move to a new directory and return to the previous one after context.
 
@@ -85,41 +116,14 @@
     ...     write("tmptest/test.txt","hi\\nho1\\n2\\n3\\n4\\n")
     ...     glob_re(".*[xt][xt][xt]", "tmptest")
     ['test.txt']
 
     """
     return list(filter(re.compile(pattern).match, os.listdir(path)))
 
-def read(fname):
-    """
-    Reads the file ``fname``.
-
-    Parameters
-    ----------
-    fname : str
-        file name.
-
-    Returns
-    -------
-    str
-        content of the file.
-
-    Examples
-    --------
-    >>> read("nonexistent.txt")
-    ''
-    >>> write("test.out","hi")
-    >>> read("test.out")
-    'hi'
-    """
-    if not os.path.exists(fname):
-        return ""
-    with open(fname, "r") as f:
-        return f.read()
-
 
 def write(destination, content, mode="w+", create_dir=True):
     """
     Write to file by string or writable :obj:`destiantion`.
 
     Parameters
     ----------
@@ -375,17 +379,17 @@
         unchanged ``a``.
     """
     gl = globals()
     for key in gl:
         if gl[key] == a:
             print(key)
     if nnl:
-        print("%s=%s" % (a.__name__, a), end="")
+        print(f"{a.__name__}={a}", end="")
     else:
-        print("%s=%s" % (a.__name__, a))
+        print(f"{a.__name__}={a}")
     return a
 
 
 def remove(file):
     """
     Removes ``file``.
 
@@ -396,7 +400,24 @@
 
     Examples
     --------
     >>> remove("test.out")
     """
     if os.path.exists(file):
         os.remove(file)
+
+
+alias_open = open
+
+
+def open(to_be_read: str, mode="r"):
+    """
+    Return opened buffer of either file or URI
+    """
+    if mode != "r":
+        return alias_open(to_be_read, mode)
+    if to_be_read.startswith("http"):
+        return StringIO(requests.get(to_be_read).text)
+    else:
+        if not os.path.exists(to_be_read):
+            return StringIO("")
+        return alias_open(to_be_read, "r")
```

### Comparing `smpl_io-1.1.0/smpl_io/read_buffer.py` & `smpl_io-1.1.2/smpl_io/read_buffer.py`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.0/smpl_io/sed.py` & `smpl_io-1.1.2/smpl_io/sed.py`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.0/smpl_io/tail.py` & `smpl_io-1.1.2/smpl_io/tail.py`

 * *Files identical despite different names*

### Comparing `smpl_io-1.1.0/setup.py` & `smpl_io-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['smpl_io']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['smpl_doc']
+['requests', 'smpl_doc>=1.0.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'smpl-io',
-    'version': '1.1.0',
+    'version': '1.1.2',
     'description': 'simple input and output for python',
     'long_description': '# smpl_io\nSimplified plotting and fitting in python.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/smpl_io.svg)\n\n[![test][a t image]][a t link]     [![Coverage Status][c t i]][c t l] \n\n## Documentation\n\n-   <https://apn-pucky.github.io/smpl_io/index.html>\n\n## Versions\n\n### Stable\n\n```sh\npip install smpl_io\n```\n\nOptional: --user or --upgrade\n\n### Dev\n\n```sh\npip install --index-url https://test.pypi.org/simple/ smpl_io\n```\n\n[doc stable]: https://apn-pucky.github.io/smpl_io/index.html\n[doc test]: https://apn-pucky.github.io/smpl_io/test/index.html\n\n[pypi image]: https://badge.fury.io/py/smpl_io.svg\n[pypi link]: https://pypi.org/project/smpl_io/\n[pypi versions]: https://img.shields.io/pypi/pyversions/smpl_io.svg\n\n[a s image]: https://github.com/APN-Pucky/smpl_io/actions/workflows/stable.yml/badge.svg\n[a s link]: https://github.com/APN-Pucky/smpl_io/actions/workflows/stable.yml\n[a t link]: https://github.com/APN-Pucky/smpl_io/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/smpl_io/actions/workflows/test.yml/badge.svg\n\n[cc s q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s q l]: https://www.codacy.com/gh/APN-Pucky/smpl_io/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl_io&amp;utm_campaign=Badge_Grade?branch=stable\n[cc s c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s c l]: https://www.codacy.com/gh/APN-Pucky/smpl_io/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl_io&utm_campaign=Badge_Coverage?branch=stable\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/smpl_io/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl_io&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/smpl_io/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl_io&utm_campaign=Badge_Coverage\n\n[c s i]: https://coveralls.io/repos/github/APN-Pucky/smpl_io/badge.svg?branch=stable\n[c s l]: https://coveralls.io/github/APN-Pucky/smpl_io?branch=stable\n[c t l]: https://coveralls.io/github/APN-Pucky/smpl_io?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/smpl_io/badge.svg?branch=master\n\n[rtd s i]: https://readthedocs.org/projects/smpl_io/badge/?version=stable\n[rtd s l]: https://smpl_io.readthedocs.io/en/stable/?badge=stable\n[rtd t i]: https://readthedocs.org/projects/smpl_io/badge/?version=latest\n[rtd t l]: https://smpl_io.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/smpl_io',
```

### Comparing `smpl_io-1.1.0/PKG-INFO` & `smpl_io-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: smpl-io
-Version: 1.1.0
+Version: 1.1.2
 Summary: simple input and output for python
 Home-page: https://github.com/APN-Pucky/smpl_io
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: smpl_doc
+Requires-Dist: requests
+Requires-Dist: smpl_doc (>=1.0.5,<2.0.0)
 Project-URL: Repository, https://github.com/APN-Pucky/smpl_io
 Description-Content-Type: text/markdown
 
 # smpl_io
 Simplified plotting and fitting in python.
 
 [![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/smpl_io.svg)
```

