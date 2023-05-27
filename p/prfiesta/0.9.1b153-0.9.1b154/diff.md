# Comparing `tmp/prfiesta-0.9.1b153.tar.gz` & `tmp/prfiesta-0.9.1b154.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.9.1b153.tar", max compression
+gzip compressed data, was "prfiesta-0.9.1b154.tar", max compression
```

## Comparing `prfiesta-0.9.1b153.tar` & `prfiesta-0.9.1b154.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-27 13:54:57.882139 prfiesta-0.9.1b153/LICENSE
--rw-r--r--   0        0        0     9095 2023-05-27 13:54:57.882139 prfiesta-0.9.1b153/README.md
--rw-r--r--   0        0        0      487 2023-05-27 13:54:57.890140 prfiesta-0.9.1b153/prfiesta/__init__.py
--rw-r--r--   0        0        0     3800 2023-05-27 13:54:57.890140 prfiesta-0.9.1b153/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-27 13:54:57.890140 prfiesta-0.9.1b153/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-27 13:54:57.890140 prfiesta-0.9.1b153/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-27 13:54:57.890140 prfiesta-0.9.1b153/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-27 13:54:57.890140 prfiesta-0.9.1b153/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     5929 2023-05-27 13:54:57.890140 prfiesta-0.9.1b153/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-27 13:54:57.890140 prfiesta-0.9.1b153/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-27 13:54:57.890140 prfiesta-0.9.1b153/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-27 13:54:57.890140 prfiesta-0.9.1b153/prfiesta/spinner.py
--rw-r--r--   0        0        0     3203 2023-05-27 13:55:06.198639 prfiesta-0.9.1b153/pyproject.toml
--rw-r--r--   0        0        0    10501 1970-01-01 00:00:00.000000 prfiesta-0.9.1b153/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-27 13:57:11.028542 prfiesta-0.9.1b154/LICENSE
+-rw-r--r--   0        0        0     9095 2023-05-27 13:57:11.028542 prfiesta-0.9.1b154/README.md
+-rw-r--r--   0        0        0      487 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/__init__.py
+-rw-r--r--   0        0        0     3799 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     5929 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-27 13:57:11.036542 prfiesta-0.9.1b154/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3203 2023-05-27 13:57:25.512561 prfiesta-0.9.1b154/pyproject.toml
+-rw-r--r--   0        0        0    10501 1970-01-01 00:00:00.000000 prfiesta-0.9.1b154/PKG-INFO
```

### Comparing `prfiesta-0.9.1b153/LICENSE` & `prfiesta-0.9.1b154/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b153/README.md` & `prfiesta-0.9.1b154/README.md`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b153/prfiesta/__main__.py` & `prfiesta-0.9.1b154/prfiesta/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     output: str = kwargs.get('output')
     output_type: str = kwargs.get('output_type')
     before: datetime = kwargs.get('before')
     after: datetime = kwargs.get('after')
     drop_columns: list[str] = list(kwargs.get('drop_columns'))
     use_updated: bool = kwargs.get('use_updated')
     use_involves: bool = kwargs.get('use_involves')
-
     use_reviewed_by: bool = kwargs.get('use_reviewed_by')
     use_review_requested: bool = kwargs.get('use_review_requested')
 
     logger.info('[bold green]PR Fiesta 🦜🥳')
 
     spinner = Spinner('dots', text=Text('Loading', style=SPINNER_STYLE))
```

### Comparing `prfiesta-0.9.1b153/prfiesta/analysis/plot.py` & `prfiesta-0.9.1b154/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b153/prfiesta/analysis/view.py` & `prfiesta-0.9.1b154/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b153/prfiesta/collectors/github.py` & `prfiesta-0.9.1b154/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b153/prfiesta/environment.py` & `prfiesta-0.9.1b154/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b153/prfiesta/output.py` & `prfiesta-0.9.1b154/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.9.1b153/pyproject.toml` & `prfiesta-0.9.1b154/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.9.1b153"
+version = "0.9.1b154"
 description = "Collect and Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/prfiesta/"
 repository = "https://github.com/kiran94/prfiesta/pull/40"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
```

### Comparing `prfiesta-0.9.1b153/PKG-INFO` & `prfiesta-0.9.1b154/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.9.1b153
+Version: 0.9.1b154
 Summary: Collect and Analyze Individual Contributor Pull Requests
 Home-page: https://pypi.org/project/prfiesta/
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

