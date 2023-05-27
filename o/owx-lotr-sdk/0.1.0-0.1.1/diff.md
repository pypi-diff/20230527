# Comparing `tmp/owx_lotr_sdk-0.1.0.tar.gz` & `tmp/owx_lotr_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owx_lotr_sdk-0.1.0.tar", max compression
+gzip compressed data, was "owx_lotr_sdk-0.1.1.tar", max compression
```

## Comparing `owx_lotr_sdk-0.1.0.tar` & `owx_lotr_sdk-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     3585 2023-05-27 07:14:26.448238 owx_lotr_sdk-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-27 05:50:35.419694 owx_lotr_sdk-0.1.0/lotr_sdk/__init__.py
--rw-r--r--   0        0        0     8949 2023-05-27 06:13:02.909218 owx_lotr_sdk-0.1.0/lotr_sdk/client.py
--rw-r--r--   0        0        0     1539 2023-05-27 03:32:06.261258 owx_lotr_sdk-0.1.0/lotr_sdk/exceptions.py
--rw-r--r--   0        0        0     2335 2023-05-27 03:42:43.691200 owx_lotr_sdk-0.1.0/lotr_sdk/models.py
--rw-r--r--   0        0        0     2284 2023-05-27 01:18:14.752826 owx_lotr_sdk-0.1.0/lotr_sdk/options.py
--rw-r--r--   0        0        0    20325 2023-05-27 02:28:01.826043 owx_lotr_sdk-0.1.0/lotr_sdk/query.py
--rw-r--r--   0        0        0      454 2023-05-27 07:16:07.748100 owx_lotr_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4034 1970-01-01 00:00:00.000000 owx_lotr_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-05-27 07:28:59.136649 owx_lotr_sdk-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3710 2023-05-27 07:32:40.516393 owx_lotr_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 05:50:35.419694 owx_lotr_sdk-0.1.1/lotr_sdk/__init__.py
+-rw-r--r--   0        0        0     8949 2023-05-27 06:13:02.909218 owx_lotr_sdk-0.1.1/lotr_sdk/client.py
+-rw-r--r--   0        0        0     1539 2023-05-27 03:32:06.261258 owx_lotr_sdk-0.1.1/lotr_sdk/exceptions.py
+-rw-r--r--   0        0        0     2335 2023-05-27 03:42:43.691200 owx_lotr_sdk-0.1.1/lotr_sdk/models.py
+-rw-r--r--   0        0        0     2284 2023-05-27 01:18:14.752826 owx_lotr_sdk-0.1.1/lotr_sdk/options.py
+-rw-r--r--   0        0        0    20325 2023-05-27 02:28:01.826043 owx_lotr_sdk-0.1.1/lotr_sdk/query.py
+-rw-r--r--   0        0        0      454 2023-05-27 07:34:37.049605 owx_lotr_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4159 1970-01-01 00:00:00.000000 owx_lotr_sdk-0.1.1/PKG-INFO
```

### Comparing `owx_lotr_sdk-0.1.0/README.md` & `owx_lotr_sdk-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -74,23 +74,30 @@
 
 - `TestLotrClientUnit` runs through the client methods with mocked network requests.
 - `TestLotrClientIntegration` runs through the client methods making network requests. Beware of API
   rate limitations.
 - `TestLotrQueryBuilder` runs through the query builder methods to create query parameter
   dictionaries for all clauses.
 
+To install dependencies, run `poetry install`.
+
 To run a subset of tests, use the following syntax:
 `poetry run pytest tests/test_lotr_sdk.py::TestLotrClientUnit` to run only tests in that test class.
 
 `poetry run pytest tests/test_lotr_sdk.py::TestLotrClientUnit::test_get_books` to run only the
 `get_books` test in that test class.
 
-## Build
-To build `sdist` and `wheel`:
-`poetry build`
-
 ## Publish
+To install dependencies, run:
+`poetry install`
+
 To set your PyPI token:
 `poetry config pypi-token.pypi your-api-token`
 
+To build the project, run:
+`poetry build`
+
 To publish:
 `poetry publish`
+
+Alternatively:
+`poetry publish --build`
```

### Comparing `owx_lotr_sdk-0.1.0/lotr_sdk/client.py` & `owx_lotr_sdk-0.1.1/lotr_sdk/client.py`

 * *Files identical despite different names*

### Comparing `owx_lotr_sdk-0.1.0/lotr_sdk/exceptions.py` & `owx_lotr_sdk-0.1.1/lotr_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `owx_lotr_sdk-0.1.0/lotr_sdk/models.py` & `owx_lotr_sdk-0.1.1/lotr_sdk/models.py`

 * *Files identical despite different names*

### Comparing `owx_lotr_sdk-0.1.0/lotr_sdk/options.py` & `owx_lotr_sdk-0.1.1/lotr_sdk/options.py`

 * *Files identical despite different names*

### Comparing `owx_lotr_sdk-0.1.0/lotr_sdk/query.py` & `owx_lotr_sdk-0.1.1/lotr_sdk/query.py`

 * *Files identical despite different names*

### Comparing `owx_lotr_sdk-0.1.0/PKG-INFO` & `owx_lotr_sdk-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owx-lotr-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Owen Wiggins
 Author-email: o@owx.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
@@ -89,24 +89,31 @@
 
 - `TestLotrClientUnit` runs through the client methods with mocked network requests.
 - `TestLotrClientIntegration` runs through the client methods making network requests. Beware of API
   rate limitations.
 - `TestLotrQueryBuilder` runs through the query builder methods to create query parameter
   dictionaries for all clauses.
 
+To install dependencies, run `poetry install`.
+
 To run a subset of tests, use the following syntax:
 `poetry run pytest tests/test_lotr_sdk.py::TestLotrClientUnit` to run only tests in that test class.
 
 `poetry run pytest tests/test_lotr_sdk.py::TestLotrClientUnit::test_get_books` to run only the
 `get_books` test in that test class.
 
-## Build
-To build `sdist` and `wheel`:
-`poetry build`
-
 ## Publish
+To install dependencies, run:
+`poetry install`
+
 To set your PyPI token:
 `poetry config pypi-token.pypi your-api-token`
 
+To build the project, run:
+`poetry build`
+
 To publish:
 `poetry publish`
 
+Alternatively:
+`poetry publish --build`
+
```

