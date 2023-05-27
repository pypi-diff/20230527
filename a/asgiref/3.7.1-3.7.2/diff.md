# Comparing `tmp/asgiref-3.7.1.tar.gz` & `tmp/asgiref-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgiref-3.7.1.tar", last modified: Wed May 24 05:24:25 2023, max compression
+gzip compressed data, was "asgiref-3.7.2.tar", last modified: Sat May 27 17:21:19 2023, max compression
```

## Comparing `asgiref-3.7.1.tar` & `asgiref-3.7.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-24 05:24:25.658527 asgiref-3.7.1/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1552 2023-05-23 16:35:51.000000 asgiref-3.7.1/LICENSE
--rw-r--r--   0 andrew    (1000) andrew    (1000)       70 2023-05-23 16:35:51.000000 asgiref-3.7.1/MANIFEST.in
--rw-r--r--   0 andrew    (1000) andrew    (1000)     9006 2023-05-24 05:24:25.658527 asgiref-3.7.1/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)     7756 2023-05-23 16:35:51.000000 asgiref-3.7.1/README.rst
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-24 05:24:25.658527 asgiref-3.7.1/asgiref/
--rw-r--r--   0 andrew    (1000) andrew    (1000)       22 2023-05-24 05:23:39.000000 asgiref-3.7.1/asgiref/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1606 2023-05-23 16:35:51.000000 asgiref-3.7.1/asgiref/compatibility.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3985 2023-05-23 16:35:51.000000 asgiref-3.7.1/asgiref/current_thread_executor.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4854 2023-05-23 16:35:51.000000 asgiref-3.7.1/asgiref/local.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)        0 2023-05-23 16:35:51.000000 asgiref-3.7.1/asgiref/py.typed
--rw-r--r--   0 andrew    (1000) andrew    (1000)     6005 2023-05-23 16:35:51.000000 asgiref-3.7.1/asgiref/server.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)    21906 2023-05-23 16:35:51.000000 asgiref-3.7.1/asgiref/sync.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3119 2023-05-23 16:35:51.000000 asgiref-3.7.1/asgiref/testing.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3627 2023-05-23 16:35:51.000000 asgiref-3.7.1/asgiref/timeout.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     6238 2023-05-23 16:35:51.000000 asgiref-3.7.1/asgiref/typing.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     6575 2023-05-23 16:35:51.000000 asgiref-3.7.1/asgiref/wsgi.py
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-24 05:24:25.658527 asgiref-3.7.1/asgiref.egg-info/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     9006 2023-05-24 05:24:25.000000 asgiref-3.7.1/asgiref.egg-info/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)      613 2023-05-24 05:24:25.000000 asgiref-3.7.1/asgiref.egg-info/SOURCES.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2023-05-24 05:24:25.000000 asgiref-3.7.1/asgiref.egg-info/dependency_links.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2023-05-24 05:24:25.000000 asgiref-3.7.1/asgiref.egg-info/not-zip-safe
--rw-r--r--   0 andrew    (1000) andrew    (1000)       92 2023-05-24 05:24:25.000000 asgiref-3.7.1/asgiref.egg-info/requires.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        8 2023-05-24 05:24:25.000000 asgiref-3.7.1/asgiref.egg-info/top_level.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2741 2023-05-24 05:24:25.658527 asgiref-3.7.1/setup.cfg
--rw-r--r--   0 andrew    (1000) andrew    (1000)       62 2023-05-23 16:35:51.000000 asgiref-3.7.1/setup.py
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-24 05:24:25.658527 asgiref-3.7.1/tests/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2329 2023-05-23 16:35:51.000000 asgiref-3.7.1/tests/test_compatibility.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8031 2023-05-23 16:35:51.000000 asgiref-3.7.1/tests/test_local.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4837 2023-05-23 16:35:51.000000 asgiref-3.7.1/tests/test_server.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)    20811 2023-05-23 16:35:51.000000 asgiref-3.7.1/tests/test_sync.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2121 2023-05-23 16:35:51.000000 asgiref-3.7.1/tests/test_sync_contextvars.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1396 2023-05-23 16:35:51.000000 asgiref-3.7.1/tests/test_testing.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8718 2023-05-23 16:35:51.000000 asgiref-3.7.1/tests/test_wsgi.py
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-27 17:21:19.747680 asgiref-3.7.2/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1552 2023-05-23 16:35:51.000000 asgiref-3.7.2/LICENSE
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       70 2023-05-23 16:35:51.000000 asgiref-3.7.2/MANIFEST.in
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     9006 2023-05-27 17:21:19.747680 asgiref-3.7.2/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     7756 2023-05-23 16:35:51.000000 asgiref-3.7.2/README.rst
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-27 17:21:19.737680 asgiref-3.7.2/asgiref/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       22 2023-05-27 17:20:44.000000 asgiref-3.7.2/asgiref/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1606 2023-05-23 16:35:51.000000 asgiref-3.7.2/asgiref/compatibility.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3985 2023-05-23 16:35:51.000000 asgiref-3.7.2/asgiref/current_thread_executor.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     4854 2023-05-23 16:35:51.000000 asgiref-3.7.2/asgiref/local.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        0 2023-05-23 16:35:51.000000 asgiref-3.7.2/asgiref/py.typed
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     6005 2023-05-23 16:35:51.000000 asgiref-3.7.2/asgiref/server.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)    22941 2023-05-27 17:19:57.000000 asgiref-3.7.2/asgiref/sync.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3119 2023-05-23 16:35:51.000000 asgiref-3.7.2/asgiref/testing.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3627 2023-05-23 16:35:51.000000 asgiref-3.7.2/asgiref/timeout.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     6238 2023-05-23 16:35:51.000000 asgiref-3.7.2/asgiref/typing.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     6575 2023-05-23 16:35:51.000000 asgiref-3.7.2/asgiref/wsgi.py
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-27 17:21:19.747680 asgiref-3.7.2/asgiref.egg-info/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     9006 2023-05-27 17:21:19.000000 asgiref-3.7.2/asgiref.egg-info/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      613 2023-05-27 17:21:19.000000 asgiref-3.7.2/asgiref.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2023-05-27 17:21:19.000000 asgiref-3.7.2/asgiref.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2023-05-27 17:21:19.000000 asgiref-3.7.2/asgiref.egg-info/not-zip-safe
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       92 2023-05-27 17:21:19.000000 asgiref-3.7.2/asgiref.egg-info/requires.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        8 2023-05-27 17:21:19.000000 asgiref-3.7.2/asgiref.egg-info/top_level.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2741 2023-05-27 17:21:19.747680 asgiref-3.7.2/setup.cfg
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       62 2023-05-23 16:35:51.000000 asgiref-3.7.2/setup.py
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-27 17:21:19.747680 asgiref-3.7.2/tests/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2329 2023-05-23 16:35:51.000000 asgiref-3.7.2/tests/test_compatibility.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     8031 2023-05-23 16:35:51.000000 asgiref-3.7.2/tests/test_local.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     4837 2023-05-23 16:35:51.000000 asgiref-3.7.2/tests/test_server.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)    20811 2023-05-23 16:35:51.000000 asgiref-3.7.2/tests/test_sync.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2121 2023-05-23 16:35:51.000000 asgiref-3.7.2/tests/test_sync_contextvars.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1396 2023-05-23 16:35:51.000000 asgiref-3.7.2/tests/test_testing.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     8718 2023-05-23 16:35:51.000000 asgiref-3.7.2/tests/test_wsgi.py
```

### Comparing `asgiref-3.7.1/LICENSE` & `asgiref-3.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/PKG-INFO` & `asgiref-3.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgiref
-Version: 3.7.1
+Version: 3.7.2
 Summary: ASGI specs, helper code, and adapters
 Home-page: https://github.com/django/asgiref/
 Author: Django Software Foundation
 Author-email: foundation@djangoproject.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://asgi.readthedocs.io/
 Project-URL: Further Documentation, https://docs.djangoproject.com/en/stable/topics/async/#async-adapter-functions
```

### Comparing `asgiref-3.7.1/README.rst` & `asgiref-3.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/asgiref/compatibility.py` & `asgiref-3.7.2/asgiref/compatibility.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/asgiref/current_thread_executor.py` & `asgiref-3.7.2/asgiref/current_thread_executor.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/asgiref/local.py` & `asgiref-3.7.2/asgiref/local.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/asgiref/server.py` & `asgiref-3.7.2/asgiref/server.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/asgiref/sync.py` & `asgiref-3.7.2/asgiref/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -550,42 +550,92 @@
         """
         try:
             return asyncio.current_task()
         except RuntimeError:
             return None
 
 
-# Lowercase aliases (and decorator friendliness)
-async_to_sync = AsyncToSync
+@overload
+def async_to_sync(
+    *,
+    force_new_loop: bool = False,
+) -> Callable[
+    [Union[Callable[_P, Coroutine[Any, Any, _R]], Callable[_P, Awaitable[_R]]]],
+    Callable[_P, _R],
+]:
+    ...
+
+
+@overload
+def async_to_sync(
+    awaitable: Union[
+        Callable[_P, Coroutine[Any, Any, _R]],
+        Callable[_P, Awaitable[_R]],
+    ],
+    *,
+    force_new_loop: bool = False,
+) -> Callable[_P, _R]:
+    ...
+
+
+def async_to_sync(
+    awaitable: Optional[
+        Union[
+            Callable[_P, Coroutine[Any, Any, _R]],
+            Callable[_P, Awaitable[_R]],
+        ]
+    ] = None,
+    *,
+    force_new_loop: bool = False,
+) -> Union[
+    Callable[
+        [Union[Callable[_P, Coroutine[Any, Any, _R]], Callable[_P, Awaitable[_R]]]],
+        Callable[_P, _R],
+    ],
+    Callable[_P, _R],
+]:
+    if awaitable is None:
+        return lambda f: AsyncToSync(
+            f,
+            force_new_loop=force_new_loop,
+        )
+    return AsyncToSync(
+        awaitable,
+        force_new_loop=force_new_loop,
+    )
 
 
 @overload
 def sync_to_async(
     *,
     thread_sensitive: bool = True,
     executor: Optional["ThreadPoolExecutor"] = None,
-) -> Callable[[Callable[_P, _R]], SyncToAsync[_P, _R]]:
+) -> Callable[[Callable[_P, _R]], Callable[_P, Coroutine[Any, Any, _R]]]:
     ...
 
 
 @overload
 def sync_to_async(
     func: Callable[_P, _R],
     *,
     thread_sensitive: bool = True,
     executor: Optional["ThreadPoolExecutor"] = None,
-) -> SyncToAsync[_P, _R]:
+) -> Callable[_P, Coroutine[Any, Any, _R]]:
     ...
 
 
 def sync_to_async(
     func: Optional[Callable[_P, _R]] = None,
+    *,
     thread_sensitive: bool = True,
     executor: Optional["ThreadPoolExecutor"] = None,
-) -> Union[Callable[[Callable[_P, _R]], SyncToAsync[_P, _R]], SyncToAsync[_P, _R]]:
+) -> Union[
+    Callable[[Callable[_P, _R]], Callable[_P, Coroutine[Any, Any, _R]]],
+    Callable[_P, Coroutine[Any, Any, _R]],
+]:
     if func is None:
         return lambda f: SyncToAsync(
             f,
             thread_sensitive=thread_sensitive,
             executor=executor,
         )
     return SyncToAsync(
```

### Comparing `asgiref-3.7.1/asgiref/testing.py` & `asgiref-3.7.2/asgiref/testing.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/asgiref/timeout.py` & `asgiref-3.7.2/asgiref/timeout.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/asgiref/typing.py` & `asgiref-3.7.2/asgiref/typing.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/asgiref/wsgi.py` & `asgiref-3.7.2/asgiref/wsgi.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/asgiref.egg-info/PKG-INFO` & `asgiref-3.7.2/asgiref.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgiref
-Version: 3.7.1
+Version: 3.7.2
 Summary: ASGI specs, helper code, and adapters
 Home-page: https://github.com/django/asgiref/
 Author: Django Software Foundation
 Author-email: foundation@djangoproject.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://asgi.readthedocs.io/
 Project-URL: Further Documentation, https://docs.djangoproject.com/en/stable/topics/async/#async-adapter-functions
```

### Comparing `asgiref-3.7.1/asgiref.egg-info/SOURCES.txt` & `asgiref-3.7.2/asgiref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/setup.cfg` & `asgiref-3.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/tests/test_compatibility.py` & `asgiref-3.7.2/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/tests/test_local.py` & `asgiref-3.7.2/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/tests/test_server.py` & `asgiref-3.7.2/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/tests/test_sync.py` & `asgiref-3.7.2/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/tests/test_sync_contextvars.py` & `asgiref-3.7.2/tests/test_sync_contextvars.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/tests/test_testing.py` & `asgiref-3.7.2/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `asgiref-3.7.1/tests/test_wsgi.py` & `asgiref-3.7.2/tests/test_wsgi.py`

 * *Files identical despite different names*

