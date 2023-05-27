# Comparing `tmp/renats-0.0.1.tar.gz` & `tmp/renats-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renats-0.0.1.tar", last modified: Fri May 26 11:54:20 2023, max compression
+gzip compressed data, was "renats-0.1.0.tar", last modified: Sat May 27 16:37:57 2023, max compression
```

## Comparing `renats-0.0.1.tar` & `renats-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 respirens  (1000) respirens  (1000)        0 2023-05-26 11:54:20.595347 renats-0.0.1/
--rw-rw-r--   0 respirens  (1000) respirens  (1000)      371 2023-05-26 11:54:20.595347 renats-0.0.1/PKG-INFO
--rw-rw-r--   0 respirens  (1000) respirens  (1000)        8 2023-05-26 11:43:56.000000 renats-0.0.1/README.md
-drwxrwxr-x   0 respirens  (1000) respirens  (1000)        0 2023-05-26 11:54:20.595347 renats-0.0.1/renats/
--rw-rw-r--   0 respirens  (1000) respirens  (1000)        0 2023-05-25 16:33:31.000000 renats-0.0.1/renats/__init__.py
-drwxrwxr-x   0 respirens  (1000) respirens  (1000)        0 2023-05-26 11:54:20.595347 renats-0.0.1/renats/client/
--rw-rw-r--   0 respirens  (1000) respirens  (1000)       27 2023-05-26 11:31:02.000000 renats-0.0.1/renats/client/__init__.py
--rw-rw-r--   0 respirens  (1000) respirens  (1000)     2557 2023-05-26 10:25:41.000000 renats-0.0.1/renats/client/renats.py
-drwxrwxr-x   0 respirens  (1000) respirens  (1000)        0 2023-05-26 11:54:20.595347 renats-0.0.1/renats/dispatcher/
--rw-rw-r--   0 respirens  (1000) respirens  (1000)       62 2023-05-26 11:30:51.000000 renats-0.0.1/renats/dispatcher/__init__.py
--rw-rw-r--   0 respirens  (1000) respirens  (1000)     1987 2023-05-26 10:38:12.000000 renats-0.0.1/renats/dispatcher/dispatcher.py
--rw-rw-r--   0 respirens  (1000) respirens  (1000)      884 2023-05-26 10:40:59.000000 renats-0.0.1/renats/dispatcher/router.py
--rw-rw-r--   0 respirens  (1000) respirens  (1000)      362 2023-05-26 10:20:00.000000 renats-0.0.1/renats/exceptions.py
--rw-rw-r--   0 respirens  (1000) respirens  (1000)      105 2023-05-25 19:12:50.000000 renats-0.0.1/renats/loggers.py
-drwxrwxr-x   0 respirens  (1000) respirens  (1000)        0 2023-05-26 11:54:20.595347 renats-0.0.1/renats.egg-info/
--rw-rw-r--   0 respirens  (1000) respirens  (1000)      371 2023-05-26 11:54:20.000000 renats-0.0.1/renats.egg-info/PKG-INFO
--rw-rw-r--   0 respirens  (1000) respirens  (1000)      365 2023-05-26 11:54:20.000000 renats-0.0.1/renats.egg-info/SOURCES.txt
--rw-rw-r--   0 respirens  (1000) respirens  (1000)        1 2023-05-26 11:54:20.000000 renats-0.0.1/renats.egg-info/dependency_links.txt
--rw-rw-r--   0 respirens  (1000) respirens  (1000)       30 2023-05-26 11:54:20.000000 renats-0.0.1/renats.egg-info/requires.txt
--rw-rw-r--   0 respirens  (1000) respirens  (1000)        7 2023-05-26 11:54:20.000000 renats-0.0.1/renats.egg-info/top_level.txt
--rw-rw-r--   0 respirens  (1000) respirens  (1000)       38 2023-05-26 11:54:20.595347 renats-0.0.1/setup.cfg
--rw-rw-r--   0 respirens  (1000) respirens  (1000)      685 2023-05-26 11:48:27.000000 renats-0.0.1/setup.py
+drwxrwxr-x   0 respirens  (1000) respirens  (1000)        0 2023-05-27 16:37:57.656145 renats-0.1.0/
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)      382 2023-05-27 16:37:57.656145 renats-0.1.0/PKG-INFO
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)        8 2023-05-26 11:43:56.000000 renats-0.1.0/README.md
+drwxrwxr-x   0 respirens  (1000) respirens  (1000)        0 2023-05-27 16:37:57.656145 renats-0.1.0/renats/
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)        0 2023-05-25 16:33:31.000000 renats-0.1.0/renats/__init__.py
+drwxrwxr-x   0 respirens  (1000) respirens  (1000)        0 2023-05-27 16:37:57.656145 renats-0.1.0/renats/client/
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)       60 2023-05-27 14:12:43.000000 renats-0.1.0/renats/client/__init__.py
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)     1862 2023-05-27 16:17:16.000000 renats-0.1.0/renats/client/client.py
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)      786 2023-05-27 14:16:56.000000 renats-0.1.0/renats/client/renats.py
+drwxrwxr-x   0 respirens  (1000) respirens  (1000)        0 2023-05-27 16:37:57.656145 renats-0.1.0/renats/dispatcher/
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)       62 2023-05-26 11:30:51.000000 renats-0.1.0/renats/dispatcher/__init__.py
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)     1670 2023-05-27 16:31:24.000000 renats-0.1.0/renats/dispatcher/dispatcher.py
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)      878 2023-05-27 16:13:08.000000 renats-0.1.0/renats/dispatcher/router.py
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)      452 2023-05-27 16:18:20.000000 renats-0.1.0/renats/exceptions.py
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)      162 2023-05-27 15:15:48.000000 renats-0.1.0/renats/loggers.py
+drwxrwxr-x   0 respirens  (1000) respirens  (1000)        0 2023-05-27 16:37:57.656145 renats-0.1.0/renats.egg-info/
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)      382 2023-05-27 16:37:57.000000 renats-0.1.0/renats.egg-info/PKG-INFO
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)      389 2023-05-27 16:37:57.000000 renats-0.1.0/renats.egg-info/SOURCES.txt
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)        1 2023-05-27 16:37:57.000000 renats-0.1.0/renats.egg-info/dependency_links.txt
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)       30 2023-05-27 16:37:57.000000 renats-0.1.0/renats.egg-info/requires.txt
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)        7 2023-05-27 16:37:57.000000 renats-0.1.0/renats.egg-info/top_level.txt
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)       38 2023-05-27 16:37:57.656145 renats-0.1.0/setup.cfg
+-rw-rw-r--   0 respirens  (1000) respirens  (1000)      696 2023-05-27 16:35:28.000000 renats-0.1.0/setup.py
```

### Comparing `renats-0.0.1/renats/dispatcher/router.py` & `renats-0.1.0/renats/dispatcher/router.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Any, Callable, Awaitable
+from typing import Callable, Awaitable, Any
 
-CallbackType = Callable[..., Awaitable[dict[str, Any]]]
+CallbackType = Callable[..., Awaitable[tuple[int, Any]]]
 
 
 class Router:
     def __init__(self):
         self._callbacks: dict[str, CallbackType] = {}
 
     def include_router(self, router: "Router"):
@@ -13,19 +13,18 @@
     def include_routers(self, *routers: "Router"):
         for router in routers:
             self.include_router(router)
 
     def route(self, subject: str) -> CallbackType | None:
         return self._callbacks.get(subject)
 
-    def register_callback(self, method: str, callback: CallbackType):
+    def register_method(self, method: str, callback: CallbackType):
         self._callbacks[method] = callback
 
-    def callback(self, method: str):
+    def method(self, method: str):
         def wrapper(callback: CallbackType):
-            self.register_callback(
+            self.register_method(
                 method=method,
                 callback=callback
             )
             return callback
         return wrapper
-
```

