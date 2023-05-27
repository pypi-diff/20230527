# Comparing `tmp/encapsia_api-0.4.1.tar.gz` & `tmp/encapsia_api-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsia_api-0.4.1.tar", max compression
+gzip compressed data, was "encapsia_api-0.4.2.tar", max compression
```

## Comparing `encapsia_api-0.4.1.tar` & `encapsia_api-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1078 2022-12-06 22:27:35.988855 encapsia_api-0.4.1/LICENSE
--rw-r--r--   0        0        0     2863 2023-05-27 11:09:29.802202 encapsia_api-0.4.1/README.md
--rw-r--r--   0        0        0      595 2023-05-27 13:43:16.249220 encapsia_api-0.4.1/encapsia_api/__init__.py
--rw-r--r--   0        0        0     1877 2023-05-27 11:09:29.802699 encapsia_api-0.4.1/encapsia_api/analytics.py
--rw-r--r--   0        0        0     2860 2023-05-27 11:09:29.802940 encapsia_api-0.4.1/encapsia_api/credentials.py
--rw-r--r--   0        0        0     3007 2023-05-27 11:09:29.803180 encapsia_api-0.4.1/encapsia_api/lib.py
--rw-r--r--   0        0        0     6284 2023-05-27 11:09:29.803506 encapsia_api-0.4.1/encapsia_api/package.py
--rw-r--r--   0        0        0     3406 2023-05-27 11:09:29.803788 encapsia_api-0.4.1/encapsia_api/plugin.py
--rw-r--r--   0        0        0     3987 2023-05-27 11:09:29.804083 encapsia_api-0.4.1/encapsia_api/resilient_request.py
--rw-r--r--   0        0        0    33035 2023-05-27 11:09:29.804668 encapsia_api-0.4.1/encapsia_api/rest.py
--rw-r--r--   0        0        0        0 2023-05-27 14:03:36.862191 encapsia_api-0.4.1/encapsia_api/tests/__init__.py
--rw-r--r--   0        0        0     3516 2023-05-27 11:09:29.805052 encapsia_api-0.4.1/encapsia_api/tests/test_credentials.py
--rw-r--r--   0        0        0     6371 2023-05-27 11:09:29.805336 encapsia_api-0.4.1/encapsia_api/tests/test_package.py
--rw-r--r--   0        0        0      536 2023-05-27 11:09:29.805873 encapsia_api-0.4.1/encapsia_api/tests/test_plugin.py
--rw-r--r--   0        0        0     9154 2023-05-27 11:09:29.806413 encapsia_api-0.4.1/encapsia_api/tests/test_resilient_request.py
--rw-r--r--   0        0        0     7006 2022-12-06 22:27:35.992544 encapsia_api-0.4.1/encapsia_api/tests/test_rest.py
--rw-r--r--   0        0        0      566 2023-05-27 11:09:29.806657 encapsia_api-0.4.1/encapsia_api/util.py
--rw-r--r--   0        0        0     3482 2023-05-27 13:59:46.354282 encapsia_api-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3712 1970-01-01 00:00:00.000000 encapsia_api-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-12-06 22:27:35.988855 encapsia_api-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2863 2023-05-27 11:09:29.802202 encapsia_api-0.4.2/README.md
+-rw-r--r--   0        0        0      595 2023-05-27 16:35:55.181103 encapsia_api-0.4.2/encapsia_api/__init__.py
+-rw-r--r--   0        0        0     1877 2023-05-27 11:09:29.802699 encapsia_api-0.4.2/encapsia_api/analytics.py
+-rw-r--r--   0        0        0     2860 2023-05-27 11:09:29.802940 encapsia_api-0.4.2/encapsia_api/credentials.py
+-rw-r--r--   0        0        0     3007 2023-05-27 11:09:29.803180 encapsia_api-0.4.2/encapsia_api/lib.py
+-rw-r--r--   0        0        0     6284 2023-05-27 11:09:29.803506 encapsia_api-0.4.2/encapsia_api/package.py
+-rw-r--r--   0        0        0     3406 2023-05-27 11:09:29.803788 encapsia_api-0.4.2/encapsia_api/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:32:32.459530 encapsia_api-0.4.2/encapsia_api/py.typed
+-rw-r--r--   0        0        0     3987 2023-05-27 11:09:29.804083 encapsia_api-0.4.2/encapsia_api/resilient_request.py
+-rw-r--r--   0        0        0    33035 2023-05-27 11:09:29.804668 encapsia_api-0.4.2/encapsia_api/rest.py
+-rw-r--r--   0        0        0        0 2023-05-27 14:03:36.862191 encapsia_api-0.4.2/encapsia_api/tests/__init__.py
+-rw-r--r--   0        0        0     3516 2023-05-27 11:09:29.805052 encapsia_api-0.4.2/encapsia_api/tests/test_credentials.py
+-rw-r--r--   0        0        0     6371 2023-05-27 11:09:29.805336 encapsia_api-0.4.2/encapsia_api/tests/test_package.py
+-rw-r--r--   0        0        0      536 2023-05-27 11:09:29.805873 encapsia_api-0.4.2/encapsia_api/tests/test_plugin.py
+-rw-r--r--   0        0        0     9154 2023-05-27 11:09:29.806413 encapsia_api-0.4.2/encapsia_api/tests/test_resilient_request.py
+-rw-r--r--   0        0        0     7006 2022-12-06 22:27:35.992544 encapsia_api-0.4.2/encapsia_api/tests/test_rest.py
+-rw-r--r--   0        0        0      566 2023-05-27 11:09:29.806657 encapsia_api-0.4.2/encapsia_api/util.py
+-rw-r--r--   0        0        0     3482 2023-05-27 16:34:02.179435 encapsia_api-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3712 1970-01-01 00:00:00.000000 encapsia_api-0.4.2/PKG-INFO
```

### Comparing `encapsia_api-0.4.1/LICENSE` & `encapsia_api-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/README.md` & `encapsia_api-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/__init__.py` & `encapsia_api-0.4.2/encapsia_api/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #: Keep in sync with git tag and package version in pyproject.toml.
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 
 class EncapsiaApiError(RuntimeError):
     def __init__(self, message, payload=None):
         super().__init__(message)
         self.message = message
         self.payload = payload
```

### Comparing `encapsia_api-0.4.1/encapsia_api/analytics.py` & `encapsia_api-0.4.2/encapsia_api/analytics.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/credentials.py` & `encapsia_api-0.4.2/encapsia_api/credentials.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/lib.py` & `encapsia_api-0.4.2/encapsia_api/lib.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/package.py` & `encapsia_api-0.4.2/encapsia_api/package.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/plugin.py` & `encapsia_api-0.4.2/encapsia_api/plugin.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/resilient_request.py` & `encapsia_api-0.4.2/encapsia_api/resilient_request.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/rest.py` & `encapsia_api-0.4.2/encapsia_api/rest.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/tests/test_credentials.py` & `encapsia_api-0.4.2/encapsia_api/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/tests/test_package.py` & `encapsia_api-0.4.2/encapsia_api/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/tests/test_plugin.py` & `encapsia_api-0.4.2/encapsia_api/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/tests/test_resilient_request.py` & `encapsia_api-0.4.2/encapsia_api/tests/test_resilient_request.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/tests/test_rest.py` & `encapsia_api-0.4.2/encapsia_api/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/encapsia_api/util.py` & `encapsia_api-0.4.2/encapsia_api/util.py`

 * *Files identical despite different names*

### Comparing `encapsia_api-0.4.1/pyproject.toml` & `encapsia_api-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "encapsia-api"
-version = "0.4.1"
+version = "0.4.2"
 description = "Client API for talking to an Encapsia system."
 readme = "README.md"
 authors = ["Timothy Corbett-Clark <timothy.corbettclark@gmail.com>"]
 maintainers = ["Petre Mierluțiu <pmierlutiu@cmedtechnology.com>"]
 license = "MIT"
 keywords = ["encapsia", "eSource", "EDC", "Clinical Trials"]
 homepage = "https://github.com/Encapsia/encapsia-api"
 
-
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = {version = ">=2.24",extras = ["security"]}
 toml = ">=0.10"
 arrow = ">=1.2.0"
 
 [tool.poetry.group.dev.dependencies]
@@ -21,14 +20,15 @@
 pytest = "^7.3.1"
 mypy = "^1.3.0"
 requests-mock = "^1.10.0"
 ruff = "^0.0.270"
 types-toml = "^0.10.8.6"
 types-requests = "^2.31.0.0"
 
+
 [build-system]
 requires = ["poetry>=1.0.5"]
 build-backend = "poetry.masonry.api"
 
 [tool.pytest.ini_options]
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
```

### Comparing `encapsia_api-0.4.1/PKG-INFO` & `encapsia_api-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsia-api
-Version: 0.4.1
+Version: 0.4.2
 Summary: Client API for talking to an Encapsia system.
 Home-page: https://github.com/Encapsia/encapsia-api
 License: MIT
 Keywords: encapsia,eSource,EDC,Clinical Trials
 Author: Timothy Corbett-Clark
 Author-email: timothy.corbettclark@gmail.com
 Maintainer: Petre Mierluțiu
```

