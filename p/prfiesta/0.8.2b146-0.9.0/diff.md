# Comparing `tmp/prfiesta-0.8.2b146.tar.gz` & `tmp/prfiesta-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.8.2b146.tar", max compression
+gzip compressed data, was "prfiesta-0.9.0.tar", max compression
```

## Comparing `prfiesta-0.8.2b146.tar` & `prfiesta-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-27 08:00:23.120097 prfiesta-0.8.2b146/LICENSE
--rw-r--r--   0        0        0     9115 2023-05-27 08:00:23.120097 prfiesta-0.8.2b146/README.md
--rw-r--r--   0        0        0      487 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/__init__.py
--rw-r--r--   0        0        0     3018 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-27 08:00:23.128097 prfiesta-0.8.2b146/prfiesta/spinner.py
--rw-r--r--   0        0        0     3179 2023-05-27 08:00:31.912191 prfiesta-0.8.2b146/pyproject.toml
--rw-r--r--   0        0        0    10476 1970-01-01 00:00:00.000000 prfiesta-0.8.2b146/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-27 08:10:57.151480 prfiesta-0.9.0/LICENSE
+-rw-r--r--   0        0        0     9115 2023-05-27 08:10:57.151480 prfiesta-0.9.0/README.md
+-rw-r--r--   0        0        0      487 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/__init__.py
+-rw-r--r--   0        0        0     3018 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-27 08:10:57.159480 prfiesta-0.9.0/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3175 2023-05-27 08:11:15.324779 prfiesta-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10472 1970-01-01 00:00:00.000000 prfiesta-0.9.0/PKG-INFO
```

### Comparing `prfiesta-0.8.2b146/LICENSE` & `prfiesta-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b146/README.md` & `prfiesta-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b146/prfiesta/__main__.py` & `prfiesta-0.9.0/prfiesta/__main__.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b146/prfiesta/analysis/plot.py` & `prfiesta-0.9.0/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b146/prfiesta/analysis/view.py` & `prfiesta-0.9.0/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b146/prfiesta/collectors/github.py` & `prfiesta-0.9.0/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b146/prfiesta/environment.py` & `prfiesta-0.9.0/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b146/prfiesta/output.py` & `prfiesta-0.9.0/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.2b146/pyproject.toml` & `prfiesta-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.8.2b146"
+version = "0.9.0"
 description = "Collect and Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kiran94/prfiesta"
 repository = "https://github.com/kiran94/prfiesta"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
```

### Comparing `prfiesta-0.8.2b146/PKG-INFO` & `prfiesta-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.8.2b146
+Version: 0.9.0
 Summary: Collect and Analyze Individual Contributor Pull Requests
 Home-page: https://github.com/kiran94/prfiesta
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

