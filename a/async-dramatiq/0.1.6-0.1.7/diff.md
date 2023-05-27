# Comparing `tmp/async_dramatiq-0.1.6.tar.gz` & `tmp/async_dramatiq-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_dramatiq-0.1.6.tar", max compression
+gzip compressed data, was "async_dramatiq-0.1.7.tar", max compression
```

## Comparing `async_dramatiq-0.1.6.tar` & `async_dramatiq-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1065 2023-05-26 08:26:10.164949 async_dramatiq-0.1.6/LICENSE
--rw-r--r--   0        0        0     2936 2023-05-26 23:57:12.060719 async_dramatiq-0.1.6/README.md
--rw-r--r--   0        0        0     3506 2023-05-27 00:23:13.868376 async_dramatiq-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      254 2023-05-26 11:00:24.176230 async_dramatiq-0.1.6/src/async_dramatiq/__init__.py
--rw-r--r--   0        0        0     3182 2023-05-26 23:41:05.167085 async_dramatiq-0.1.6/src/async_dramatiq/actors.py
--rw-r--r--   0        0        0      491 2023-05-26 07:37:33.566566 async_dramatiq-0.1.6/src/async_dramatiq/backends/__init__.py
--rw-r--r--   0        0        0     1700 2023-05-27 00:15:20.555394 async_dramatiq-0.1.6/src/async_dramatiq/backends/async_redis.py
--rw-r--r--   0        0        0     1758 2023-05-26 07:37:33.566814 async_dramatiq-0.1.6/src/async_dramatiq/backends/async_stub.py
--rw-r--r--   0        0        0      112 2023-05-26 07:37:33.566965 async_dramatiq-0.1.6/src/async_dramatiq/middleware/__init__.py
--rw-r--r--   0        0        0      934 2023-05-27 00:22:09.609050 async_dramatiq-0.1.6/src/async_dramatiq/middleware/async_base.py
--rw-r--r--   0        0        0     1159 2023-05-26 18:57:12.390516 async_dramatiq-0.1.6/src/async_dramatiq/middleware/async_stub.py
--rw-r--r--   0        0        0     1416 2023-05-26 18:47:19.511369 async_dramatiq-0.1.6/src/async_dramatiq/scheduler.py
--rw-r--r--   0        0        0      485 2023-05-27 00:22:09.606670 async_dramatiq-0.1.6/src/async_dramatiq/types.py
--rw-r--r--   0        0        0     1232 2023-05-26 18:42:58.013316 async_dramatiq-0.1.6/src/async_dramatiq/worker.py
--rw-r--r--   0        0        0        0 2023-05-26 08:26:10.167650 async_dramatiq-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     1471 2023-05-26 08:26:10.167926 async_dramatiq-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0     3812 2023-05-26 09:10:55.772756 async_dramatiq-0.1.6/tests/test_actors.py
--rw-r--r--   0        0        0     2563 2023-05-26 08:26:10.168282 async_dramatiq-0.1.6/tests/test_backends.py
--rw-r--r--   0        0        0     1024 2023-05-26 08:26:10.168435 async_dramatiq-0.1.6/tests/test_scheduler.py
--rw-r--r--   0        0        0      595 2023-05-26 08:26:10.168609 async_dramatiq-0.1.6/tests/test_workers.py
--rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 async_dramatiq-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-26 08:26:10.164949 async_dramatiq-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2936 2023-05-27 01:25:25.985962 async_dramatiq-0.1.7/README.md
+-rw-r--r--   0        0        0     3506 2023-05-27 01:27:35.394466 async_dramatiq-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      254 2023-05-27 01:25:25.990049 async_dramatiq-0.1.7/src/async_dramatiq/__init__.py
+-rw-r--r--   0        0        0     3182 2023-05-27 01:25:25.990257 async_dramatiq-0.1.7/src/async_dramatiq/actors.py
+-rw-r--r--   0        0        0      491 2023-05-26 07:37:33.566566 async_dramatiq-0.1.7/src/async_dramatiq/backends/__init__.py
+-rw-r--r--   0        0        0     1700 2023-05-27 01:25:25.990467 async_dramatiq-0.1.7/src/async_dramatiq/backends/async_redis.py
+-rw-r--r--   0        0        0     1758 2023-05-26 07:37:33.566814 async_dramatiq-0.1.7/src/async_dramatiq/backends/async_stub.py
+-rw-r--r--   0        0        0      112 2023-05-26 07:37:33.566965 async_dramatiq-0.1.7/src/async_dramatiq/middleware/__init__.py
+-rw-r--r--   0        0        0      934 2023-05-27 01:25:25.990649 async_dramatiq-0.1.7/src/async_dramatiq/middleware/async_base.py
+-rw-r--r--   0        0        0     1159 2023-05-27 01:25:25.990830 async_dramatiq-0.1.7/src/async_dramatiq/middleware/async_stub.py
+-rw-r--r--   0        0        0     1416 2023-05-27 01:25:25.991007 async_dramatiq-0.1.7/src/async_dramatiq/scheduler.py
+-rw-r--r--   0        0        0      485 2023-05-27 01:25:25.991283 async_dramatiq-0.1.7/src/async_dramatiq/types.py
+-rw-r--r--   0        0        0     1232 2023-05-27 01:25:25.991465 async_dramatiq-0.1.7/src/async_dramatiq/worker.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:26:10.167650 async_dramatiq-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     1471 2023-05-26 08:26:10.167926 async_dramatiq-0.1.7/tests/conftest.py
+-rw-r--r--   0        0        0     3812 2023-05-26 09:10:55.772756 async_dramatiq-0.1.7/tests/test_actors.py
+-rw-r--r--   0        0        0     2563 2023-05-26 08:26:10.168282 async_dramatiq-0.1.7/tests/test_backends.py
+-rw-r--r--   0        0        0     1024 2023-05-26 08:26:10.168435 async_dramatiq-0.1.7/tests/test_scheduler.py
+-rw-r--r--   0        0        0      595 2023-05-26 08:26:10.168609 async_dramatiq-0.1.7/tests/test_workers.py
+-rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 async_dramatiq-0.1.7/PKG-INFO
```

### Comparing `async_dramatiq-0.1.6/LICENSE` & `async_dramatiq-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/README.md` & `async_dramatiq-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/pyproject.toml` & `async_dramatiq-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async_dramatiq"
-version = "0.1.6"
+version = "0.1.7"
 description = "Dramatiq with Asyncio support and some other goodies"
 authors = ["Ryan Houlihan <ryan@rhoulihan.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{ include = "async_dramatiq", from = "src" }]
 include = [{ path = "tests", format = "sdist" }]
 homepage = "https://github.com/motherofcoconuts/async-dramatiq"
```

### Comparing `async_dramatiq-0.1.6/src/async_dramatiq/actors.py` & `async_dramatiq-0.1.7/src/async_dramatiq/actors.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/src/async_dramatiq/backends/async_redis.py` & `async_dramatiq-0.1.7/src/async_dramatiq/backends/async_redis.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/src/async_dramatiq/backends/async_stub.py` & `async_dramatiq-0.1.7/src/async_dramatiq/backends/async_stub.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/src/async_dramatiq/middleware/async_base.py` & `async_dramatiq-0.1.7/src/async_dramatiq/middleware/async_base.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/src/async_dramatiq/middleware/async_stub.py` & `async_dramatiq-0.1.7/src/async_dramatiq/middleware/async_stub.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/src/async_dramatiq/scheduler.py` & `async_dramatiq-0.1.7/src/async_dramatiq/scheduler.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/src/async_dramatiq/worker.py` & `async_dramatiq-0.1.7/src/async_dramatiq/worker.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/tests/conftest.py` & `async_dramatiq-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/tests/test_actors.py` & `async_dramatiq-0.1.7/tests/test_actors.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/tests/test_backends.py` & `async_dramatiq-0.1.7/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/tests/test_scheduler.py` & `async_dramatiq-0.1.7/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/tests/test_workers.py` & `async_dramatiq-0.1.7/tests/test_workers.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.6/PKG-INFO` & `async_dramatiq-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-dramatiq
-Version: 0.1.6
+Version: 0.1.7
 Summary: Dramatiq with Asyncio support and some other goodies
 Home-page: https://github.com/motherofcoconuts/async-dramatiq
 License: MIT
 Author: Ryan Houlihan
 Author-email: ryan@rhoulihan.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

