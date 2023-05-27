# Comparing `tmp/smpl_doc-1.1.1.tar.gz` & `tmp/smpl_doc-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpl_doc-1.1.1.tar", max compression
+gzip compressed data, was "smpl_doc-1.1.3.tar", max compression
```

## Comparing `smpl_doc-1.1.1.tar` & `smpl_doc-1.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-01-04 21:09:21.134541 smpl_doc-1.1.1/LICENSE
--rw-r--r--   0        0        0     2865 2023-01-04 21:09:21.134541 smpl_doc-1.1.1/README.md
--rw-r--r--   0        0        0     1538 2023-01-04 21:09:22.590541 smpl_doc-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      138 2023-01-04 21:09:21.138541 smpl_doc-1.1.1/smpl_doc/__init__.py
--rw-r--r--   0        0        0     9032 2023-01-04 21:09:21.138541 smpl_doc-1.1.1/smpl_doc/doc.py
--rw-r--r--   0        0        0     3587 1970-01-01 00:00:00.000000 smpl_doc-1.1.1/setup.py
--rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 smpl_doc-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-27 16:20:19.499276 smpl_doc-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2827 2023-05-27 16:20:19.499276 smpl_doc-1.1.3/README.md
+-rw-r--r--   0        0        0     1629 2023-05-27 16:20:20.951311 smpl_doc-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      138 2023-05-27 16:20:19.499276 smpl_doc-1.1.3/smpl_doc/__init__.py
+-rw-r--r--   0        0        0     9091 2023-05-27 16:20:19.499276 smpl_doc-1.1.3/smpl_doc/doc.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 smpl_doc-1.1.3/setup.py
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 smpl_doc-1.1.3/PKG-INFO
```

### Comparing `smpl_doc-1.1.1/LICENSE` & `smpl_doc-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smpl_doc-1.1.1/README.md` & `smpl_doc-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # smpl_doc
 Simplified plotting and fitting in python.
 
 [![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/smpl_doc.svg)
 
- [![test][a t image]][a t link]    [![Coverage Status][c t i]][c t l]  [![Documentation][rtd t i]][rtd t l]
+ [![test][a t image]][a t link]    [![Coverage Status][c t i]][c t l]
 
 ## Documentation
 
 -   <https://apn-pucky.github.io/smpl_doc/index.html>
 
 ## Versions
```

### Comparing `smpl_doc-1.1.1/pyproject.toml` & `smpl_doc-1.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smpl_doc"
-version = "1.1.1"
+version = "1.1.3"
 description = "SiMPLe plotting and fitting"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/smpl_doc"
 
 [tool.poetry.dependencies]
 python = "^3.7"
@@ -22,27 +22,33 @@
 sphinx-autoapi = "*"
 sphinx_autobuild = "*"
 pandoc = "*"
 numpydoc = "*"
 myst-parser  = "*"
 toml = "*"
 
-[tool.poetry.group.dev]
+
+[tool.poetry.group.test]
 optional = true
 
-[tool.poetry.group.dev.dependencies]
-pre-commit = "^2.20.0"
+[tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-cov =  "*"
 pytest-profiling =  "*"
 #pytest-line-profiler-apn = {path="/home/apn/git/pytest-line-profiler", develop = true}
+
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^2.20.0"
 #ipython =  "*"
 #jupyterlab =  "*"
 #jupyter = "*"
-poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.21.1"}
+poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21.1,<0.23.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `smpl_doc-1.1.1/smpl_doc/doc.py` & `smpl_doc-1.1.3/smpl_doc/doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Simplified python code documentation."""
 import warnings
+
 from deprecation import deprecated as _deprecated
 
 
 def append(txt):
     """
     Append ``txt`` in the ``target`` function docstring.
 
@@ -76,15 +77,15 @@
     ... def hi():
     ...     '''Hi'''
     ...     print(hi.__doc__)
     >>> hi()
     HiHo
 
     """
-    return append_str(original.__doc__)
+    return append_str(original.__doc__ if original.__doc__ is not None else "")
 
 
 def insert(txt):
     """
     Insert ``txt`` in the ``target`` function docstring.
 
     Examples
@@ -183,15 +184,15 @@
     reason : ``str``
         Reason for deprecation.
     details : ``str``
         Details about the deprecation.
 
     Examples
     --------
-    >>> @deprecated('0.0.0',"Old")
+    >>> @deprecated('0.0.0',removed_in='0.2.0')
     ... def ho():
     ...     '''Ho'''
     ...     print(ho.__doc__)
     >>> ho()
     Ho
     <BLANKLINE>
     .. deprecated:: 0.0.0
@@ -205,18 +206,18 @@
         details = reason + " " + details
 
     # merge deprecated_in and version
     if version is None:
         version = deprecated_in
 
     # increment minor version
-    if removed_in is None:
-        removed_in = ".".join(
-            [version.split(".")[0]] + [str(int(version.split(".")[1]) + 2)] + ["0"]
-        )
+    # if removed_in is None:
+    #    removed_in = ".".join(
+    #        [version.split(".")[0]] + [str(int(version.split(".")[1]) + 2)] + ["0"]
+    #    )
 
     return _deprecated(
         deprecated_in=version,
         removed_in=removed_in,
         # current_version=_version("pyfeyn2"),
         details=details,
     )
```

### Comparing `smpl_doc-1.1.1/setup.py` & `smpl_doc-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['deprecation']
 
 setup_kwargs = {
     'name': 'smpl-doc',
-    'version': '1.1.1',
+    'version': '1.1.3',
     'description': 'SiMPLe plotting and fitting',
-    'long_description': '# smpl_doc\nSimplified plotting and fitting in python.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/smpl_doc.svg)\n\n [![test][a t image]][a t link]    [![Coverage Status][c t i]][c t l]  [![Documentation][rtd t i]][rtd t l]\n\n## Documentation\n\n-   <https://apn-pucky.github.io/smpl_doc/index.html>\n\n## Versions\n\n### Stable\n\n```sh\npip install smpl_doc\n```\n\nOptional: --user or --upgrade\n\n### Dev\n\n```sh\npip install --index-url https://test.pypi.org/simple/ smpl_doc\n```\n\n[doc stable]: https://apn-pucky.github.io/smpl_doc/index.html\n[doc test]: https://apn-pucky.github.io/smpl_doc/test/index.html\n\n[pypi image]: https://badge.fury.io/py/smpl_doc.svg\n[pypi link]: https://pypi.org/project/smpl_doc/\n[pypi versions]: https://img.shields.io/pypi/pyversions/smpl_doc.svg\n\n[a s image]: https://github.com/APN-Pucky/smpl_doc/actions/workflows/stable.yml/badge.svg\n[a s link]: https://github.com/APN-Pucky/smpl_doc/actions/workflows/stable.yml\n[a t link]: https://github.com/APN-Pucky/smpl_doc/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/smpl_doc/actions/workflows/test.yml/badge.svg\n\n[cc s q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s q l]: https://www.codacy.com/gh/APN-Pucky/smpl_doc/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl&amp;utm_campaign=Badge_Grade?branch=stable\n[cc s c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s c l]: https://www.codacy.com/gh/APN-Pucky/smpl_doc/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl&utm_campaign=Badge_Coverage?branch=stable\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/smpl_doc/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/smpl_doc/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl&utm_campaign=Badge_Coverage\n\n[c s i]: https://coveralls.io/repos/github/APN-Pucky/smpl_doc/badge.svg?branch=stable\n[c s l]: https://coveralls.io/github/APN-Pucky/smpl_doc?branch=stable\n[c t l]: https://coveralls.io/github/APN-Pucky/smpl_doc?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/smpl_doc/badge.svg?branch=master\n\n[rtd s i]: https://readthedocs.org/projects/smpl_doc/badge/?version=stable\n[rtd s l]: https://smpl_doc.readthedocs.io/en/stable/?badge=stable\n[rtd t i]: https://readthedocs.org/projects/smpl_doc/badge/?version=latest\n[rtd t l]: https://smpl_doc.readthedocs.io/en/latest/?badge=latest\n',
+    'long_description': '# smpl_doc\nSimplified plotting and fitting in python.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/smpl_doc.svg)\n\n [![test][a t image]][a t link]    [![Coverage Status][c t i]][c t l]\n\n## Documentation\n\n-   <https://apn-pucky.github.io/smpl_doc/index.html>\n\n## Versions\n\n### Stable\n\n```sh\npip install smpl_doc\n```\n\nOptional: --user or --upgrade\n\n### Dev\n\n```sh\npip install --index-url https://test.pypi.org/simple/ smpl_doc\n```\n\n[doc stable]: https://apn-pucky.github.io/smpl_doc/index.html\n[doc test]: https://apn-pucky.github.io/smpl_doc/test/index.html\n\n[pypi image]: https://badge.fury.io/py/smpl_doc.svg\n[pypi link]: https://pypi.org/project/smpl_doc/\n[pypi versions]: https://img.shields.io/pypi/pyversions/smpl_doc.svg\n\n[a s image]: https://github.com/APN-Pucky/smpl_doc/actions/workflows/stable.yml/badge.svg\n[a s link]: https://github.com/APN-Pucky/smpl_doc/actions/workflows/stable.yml\n[a t link]: https://github.com/APN-Pucky/smpl_doc/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/smpl_doc/actions/workflows/test.yml/badge.svg\n\n[cc s q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s q l]: https://www.codacy.com/gh/APN-Pucky/smpl_doc/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl&amp;utm_campaign=Badge_Grade?branch=stable\n[cc s c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s c l]: https://www.codacy.com/gh/APN-Pucky/smpl_doc/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl&utm_campaign=Badge_Coverage?branch=stable\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/smpl_doc/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/smpl_doc/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl&utm_campaign=Badge_Coverage\n\n[c s i]: https://coveralls.io/repos/github/APN-Pucky/smpl_doc/badge.svg?branch=stable\n[c s l]: https://coveralls.io/github/APN-Pucky/smpl_doc?branch=stable\n[c t l]: https://coveralls.io/github/APN-Pucky/smpl_doc?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/smpl_doc/badge.svg?branch=master\n\n[rtd s i]: https://readthedocs.org/projects/smpl_doc/badge/?version=stable\n[rtd s l]: https://smpl_doc.readthedocs.io/en/stable/?badge=stable\n[rtd t i]: https://readthedocs.org/projects/smpl_doc/badge/?version=latest\n[rtd t l]: https://smpl_doc.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/smpl_doc',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `smpl_doc-1.1.1/PKG-INFO` & `smpl_doc-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smpl-doc
-Version: 1.1.1
+Version: 1.1.3
 Summary: SiMPLe plotting and fitting
 Home-page: https://github.com/APN-Pucky/smpl_doc
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 
 # smpl_doc
 Simplified plotting and fitting in python.
 
 [![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/smpl_doc.svg)
 
- [![test][a t image]][a t link]    [![Coverage Status][c t i]][c t l]  [![Documentation][rtd t i]][rtd t l]
+ [![test][a t image]][a t link]    [![Coverage Status][c t i]][c t l]
 
 ## Documentation
 
 -   <https://apn-pucky.github.io/smpl_doc/index.html>
 
 ## Versions
```

