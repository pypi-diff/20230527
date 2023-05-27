# Comparing `tmp/prfiesta-0.9.1b149.tar.gz` & `tmp/prfiesta-0.9.1b151.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.9.1b149.tar", max compression
+gzip compressed data, was "prfiesta-0.9.1b151.tar", max compression
```

## Comparing `prfiesta-0.9.1b149.tar` & `prfiesta-0.9.1b151.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-27 08:38:42.086292 prfiesta-0.9.1b149/LICENSE
--rw-r--r--   0        0        0     9095 2023-05-27 08:38:42.086292 prfiesta-0.9.1b149/README.md
--rw-r--r--   0        0        0      487 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/__init__.py
--rw-r--r--   0        0        0     3018 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-27 08:38:42.094292 prfiesta-0.9.1b149/prfiesta/spinner.py
--rw-r--r--   0        0        0     3179 2023-05-27 08:38:49.834370 prfiesta-0.9.1b149/pyproject.toml
--rw-r--r--   0        0        0    10456 1970-01-01 00:00:00.000000 prfiesta-0.9.1b149/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-27 09:04:53.084291 prfiesta-0.9.1b151/LICENSE
+-rw-r--r--   0        0        0     9095 2023-05-27 09:04:53.084291 prfiesta-0.9.1b151/README.md
+-rw-r--r--   0        0        0      487 2023-05-27 09:04:53.092291 prfiesta-0.9.1b151/prfiesta/__init__.py
+-rw-r--r--   0        0        0     3018 2023-05-27 09:04:53.092291 prfiesta-0.9.1b151/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-27 09:04:53.092291 prfiesta-0.9.1b151/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-27 09:04:53.092291 prfiesta-0.9.1b151/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-27 09:04:53.092291 prfiesta-0.9.1b151/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-27 09:04:53.092291 prfiesta-0.9.1b151/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-27 09:04:53.092291 prfiesta-0.9.1b151/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-27 09:04:53.092291 prfiesta-0.9.1b151/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-27 09:04:53.092291 prfiesta-0.9.1b151/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-27 09:04:53.092291 prfiesta-0.9.1b151/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3186 2023-05-27 09:05:05.260284 prfiesta-0.9.1b151/pyproject.toml
+-rw-r--r--   0        0        0    10463 1970-01-01 00:00:00.000000 prfiesta-0.9.1b151/PKG-INFO
```

### Comparing `prfiesta-0.9.1b149/LICENSE` & `prfiesta-0.9.1b151/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b149/README.md` & `prfiesta-0.9.1b151/README.md`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b149/prfiesta/__main__.py` & `prfiesta-0.9.1b151/prfiesta/__main__.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b149/prfiesta/analysis/plot.py` & `prfiesta-0.9.1b151/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b149/prfiesta/analysis/view.py` & `prfiesta-0.9.1b151/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b149/prfiesta/collectors/github.py` & `prfiesta-0.9.1b151/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b149/prfiesta/environment.py` & `prfiesta-0.9.1b151/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b149/prfiesta/output.py` & `prfiesta-0.9.1b151/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b149/pyproject.toml` & `prfiesta-0.9.1b151/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.9.1b149"
+version = "0.9.1b151"
 description = "Collect and Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
-homepage = "https://github.com/kiran94/prfiesta"
-repository = "https://github.com/kiran94/prfiesta"
+homepage = "https://pypi.org/project/prfiesta/"
+repository = "https://github.com/kiran94/prfiesta/pull/39"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
 keywords = [ "pull-request", "pull-request-review", "performance-review" ]
 classifiers = [
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
     "Topic :: Software Development",
```

### Comparing `prfiesta-0.9.1b149/PKG-INFO` & `prfiesta-0.9.1b151/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.9.1b149
+Version: 0.9.1b151
 Summary: Collect and Analyze Individual Contributor Pull Requests
-Home-page: https://github.com/kiran94/prfiesta
+Home-page: https://pypi.org/project/prfiesta/
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: pygithub (>=1.58.1,<2.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: urllib3 (<2)
 Project-URL: Documentation, https://github.com/kiran94/prfiesta/blob/main/README.md
-Project-URL: Repository, https://github.com/kiran94/prfiesta
+Project-URL: Repository, https://github.com/kiran94/prfiesta/pull/39
 Description-Content-Type: text/markdown
 
 # prfiesta 🦜🥳
 
 [![main](https://github.com/kiran94/prfiesta/actions/workflows/main.yml/badge.svg)](https://github.com/kiran94/prfiesta/actions/workflows/main.yml) ![GitHub](https://img.shields.io/github/license/kiran94/prfiesta) [![PyPI](https://img.shields.io/pypi/v/prfiesta)](https://pypi.org/project/prfiesta/)
 
 > Collect and Analyze Individual Contributor Pull Requests
```

