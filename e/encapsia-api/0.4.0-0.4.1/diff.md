# Comparing `tmp/encapsia_api-0.4.0.tar.gz` & `tmp/encapsia_api-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsia_api-0.4.0.tar", max compression
+gzip compressed data, was "encapsia_api-0.4.1.tar", max compression
```

## Comparing `encapsia_api-0.4.0.tar` & `encapsia_api-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1078 2022-01-07 06:44:29.651749 encapsia_api-0.4.0/LICENSE
--rw-r--r--   0        0        0     2863 2023-05-05 07:11:44.945138 encapsia_api-0.4.0/README.md
--rw-r--r--   0        0        0      595 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/__init__.py
--rw-r--r--   0        0        0     1877 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/analytics.py
--rw-r--r--   0        0        0     2860 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/credentials.py
--rw-r--r--   0        0        0     3007 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/lib.py
--rw-r--r--   0        0        0     6284 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/package.py
--rw-r--r--   0        0        0     3406 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/plugin.py
--rw-r--r--   0        0        0     3987 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/resilient_request.py
--rw-r--r--   0        0        0    33035 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/rest.py
--rw-r--r--   0        0        0     3516 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/tests/test_credentials.py
--rw-r--r--   0        0        0     6371 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/tests/test_package.py
--rw-r--r--   0        0        0      536 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/tests/test_plugin.py
--rw-r--r--   0        0        0     9154 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/tests/test_resilient_request.py
--rw-r--r--   0        0        0     7006 2023-05-02 17:09:35.347096 encapsia_api-0.4.0/encapsia_api/tests/test_rest.py
--rw-r--r--   0        0        0      566 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/encapsia_api/util.py
--rw-r--r--   0        0        0     3479 2023-05-05 07:11:44.949138 encapsia_api-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 encapsia_api-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-12-06 22:27:35.988855 encapsia_api-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2863 2023-05-27 11:09:29.802202 encapsia_api-0.4.1/README.md
+-rw-r--r--   0        0        0      595 2023-05-27 13:43:16.249220 encapsia_api-0.4.1/encapsia_api/__init__.py
+-rw-r--r--   0        0        0     1877 2023-05-27 11:09:29.802699 encapsia_api-0.4.1/encapsia_api/analytics.py
+-rw-r--r--   0        0        0     2860 2023-05-27 11:09:29.802940 encapsia_api-0.4.1/encapsia_api/credentials.py
+-rw-r--r--   0        0        0     3007 2023-05-27 11:09:29.803180 encapsia_api-0.4.1/encapsia_api/lib.py
+-rw-r--r--   0        0        0     6284 2023-05-27 11:09:29.803506 encapsia_api-0.4.1/encapsia_api/package.py
+-rw-r--r--   0        0        0     3406 2023-05-27 11:09:29.803788 encapsia_api-0.4.1/encapsia_api/plugin.py
+-rw-r--r--   0        0        0     3987 2023-05-27 11:09:29.804083 encapsia_api-0.4.1/encapsia_api/resilient_request.py
+-rw-r--r--   0        0        0    33035 2023-05-27 11:09:29.804668 encapsia_api-0.4.1/encapsia_api/rest.py
+-rw-r--r--   0        0        0        0 2023-05-27 14:03:36.862191 encapsia_api-0.4.1/encapsia_api/tests/__init__.py
+-rw-r--r--   0        0        0     3516 2023-05-27 11:09:29.805052 encapsia_api-0.4.1/encapsia_api/tests/test_credentials.py
+-rw-r--r--   0        0        0     6371 2023-05-27 11:09:29.805336 encapsia_api-0.4.1/encapsia_api/tests/test_package.py
+-rw-r--r--   0        0        0      536 2023-05-27 11:09:29.805873 encapsia_api-0.4.1/encapsia_api/tests/test_plugin.py
+-rw-r--r--   0        0        0     9154 2023-05-27 11:09:29.806413 encapsia_api-0.4.1/encapsia_api/tests/test_resilient_request.py
+-rw-r--r--   0        0        0     7006 2022-12-06 22:27:35.992544 encapsia_api-0.4.1/encapsia_api/tests/test_rest.py
+-rw-r--r--   0        0        0      566 2023-05-27 11:09:29.806657 encapsia_api-0.4.1/encapsia_api/util.py
+-rw-r--r--   0        0        0     3482 2023-05-27 13:59:46.354282 encapsia_api-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3712 1970-01-01 00:00:00.000000 encapsia_api-0.4.1/PKG-INFO
```

### Comparing `encapsia_api-0.4.0/LICENSE` & `encapsia_api-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/README.md` & `encapsia_api-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/__init__.py` & `encapsia_api-0.4.1/encapsia_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #: Keep in sync with git tag and package version in pyproject.toml.
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 
 class EncapsiaApiError(RuntimeError):
     def __init__(self, message, payload=None):
         super().__init__(message)
         self.message = message
         self.payload = payload
```

### Comparing `encapsia_api-0.4.0/encapsia_api/analytics.py` & `encapsia_api-0.4.1/encapsia_api/analytics.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/credentials.py` & `encapsia_api-0.4.1/encapsia_api/credentials.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/lib.py` & `encapsia_api-0.4.1/encapsia_api/lib.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/package.py` & `encapsia_api-0.4.1/encapsia_api/package.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/plugin.py` & `encapsia_api-0.4.1/encapsia_api/plugin.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/resilient_request.py` & `encapsia_api-0.4.1/encapsia_api/resilient_request.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/rest.py` & `encapsia_api-0.4.1/encapsia_api/rest.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/tests/test_credentials.py` & `encapsia_api-0.4.1/encapsia_api/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/tests/test_package.py` & `encapsia_api-0.4.1/encapsia_api/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/tests/test_plugin.py` & `encapsia_api-0.4.1/encapsia_api/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/tests/test_resilient_request.py` & `encapsia_api-0.4.1/encapsia_api/tests/test_resilient_request.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/tests/test_rest.py` & `encapsia_api-0.4.1/encapsia_api/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/encapsia_api/util.py` & `encapsia_api-0.4.1/encapsia_api/util.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.0/pyproject.toml` & `encapsia_api-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "encapsia-api"
-version = "0.4.0"
+version = "0.4.1"
 description = "Client API for talking to an Encapsia system."
 readme = "README.md"
 authors = ["Timothy Corbett-Clark <timothy.corbettclark@gmail.com>"]
 maintainers = ["Petre Mierluțiu <pmierlutiu@cmedtechnology.com>"]
 license = "MIT"
 keywords = ["encapsia", "eSource", "EDC", "Clinical Trials"]
 homepage = "https://github.com/Encapsia/encapsia-api"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = {version = "^2.24",extras = ["security"]}
-toml = "^0.10"
-arrow = "^0.16"
+requests = {version = ">=2.24",extras = ["security"]}
+toml = ">=0.10"
+arrow = ">=1.2.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10.0"
-pytest = "^7.2.0"
-mypy = "^0.990"
+black = "^23.3.0"
+pytest = "^7.3.1"
+mypy = "^1.3.0"
 requests-mock = "^1.10.0"
-ruff = "^0.0.264"
+ruff = "^0.0.270"
 types-toml = "^0.10.8.6"
-types-requests = "^2.29.0.0"
+types-requests = "^2.31.0.0"
 
 [build-system]
 requires = ["poetry>=1.0.5"]
 build-backend = "poetry.masonry.api"
 
 [tool.pytest.ini_options]
 markers = [
```

### Comparing `encapsia_api-0.4.0/PKG-INFO` & `encapsia_api-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsia-api
-Version: 0.4.0
+Version: 0.4.1
 Summary: Client API for talking to an Encapsia system.
 Home-page: https://github.com/Encapsia/encapsia-api
 License: MIT
 Keywords: encapsia,eSource,EDC,Clinical Trials
 Author: Timothy Corbett-Clark
 Author-email: timothy.corbettclark@gmail.com
 Maintainer: Petre Mierluțiu
@@ -12,17 +12,17 @@
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: arrow (>=0.16,<0.17)
-Requires-Dist: requests[security] (>=2.24,<3.0)
-Requires-Dist: toml (>=0.10,<0.11)
+Requires-Dist: arrow (>=1.2.0)
+Requires-Dist: requests[security] (>=2.24)
+Requires-Dist: toml (>=0.10)
 Description-Content-Type: text/markdown
 
 # Encapsia API Library
 
 ![Workflows](https://github.com/encapsia/encapsia-api/actions/workflows/main.yml/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/encapsia-api?style=flat)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
```

