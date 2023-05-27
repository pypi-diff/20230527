# Comparing `tmp/pyuserside-0.1.0.tar.gz` & `tmp/pyuserside-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuserside-0.1.0.tar", last modified: Sat Mar 25 00:45:16 2023, max compression
+gzip compressed data, was "pyuserside-0.1.1.tar", last modified: Sat May 27 08:08:23 2023, max compression
```

## Comparing `pyuserside-0.1.0.tar` & `pyuserside-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 00:45:16.370038 pyuserside-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-25 00:45:05.000000 pyuserside-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-25 00:45:16.370038 pyuserside-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-25 00:45:05.000000 pyuserside-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-25 00:45:05.000000 pyuserside-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 00:45:16.370038 pyuserside-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-25 00:45:05.000000 pyuserside-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 00:45:16.362038 pyuserside-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 00:45:16.366038 pyuserside-0.1.0/src/pyuserside/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 00:45:05.000000 pyuserside-0.1.0/src/pyuserside/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 00:45:16.370038 pyuserside-0.1.0/src/pyuserside/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 00:45:05.000000 pyuserside-0.1.0/src/pyuserside/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-25 00:45:05.000000 pyuserside-0.1.0/src/pyuserside/api/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-25 00:45:05.000000 pyuserside-0.1.0/src/pyuserside/api/synchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-25 00:45:05.000000 pyuserside-0.1.0/src/pyuserside/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 00:45:16.366038 pyuserside-0.1.0/src/pyuserside.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-25 00:45:16.000000 pyuserside-0.1.0/src/pyuserside.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-25 00:45:16.000000 pyuserside-0.1.0/src/pyuserside.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 00:45:16.000000 pyuserside-0.1.0/src/pyuserside.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-25 00:45:16.000000 pyuserside-0.1.0/src/pyuserside.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-25 00:45:16.000000 pyuserside-0.1.0/src/pyuserside.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:08:23.643986 pyuserside-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 08:08:11.000000 pyuserside-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-27 08:08:23.643986 pyuserside-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 08:08:11.000000 pyuserside-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-27 08:08:11.000000 pyuserside-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:08:23.643986 pyuserside-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:08:23.643986 pyuserside-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:08:23.643986 pyuserside-0.1.1/src/pyuserside/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-27 08:08:11.000000 pyuserside-0.1.1/src/pyuserside/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-27 08:08:11.000000 pyuserside-0.1.1/src/pyuserside/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:08:23.643986 pyuserside-0.1.1/src/pyuserside.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-27 08:08:23.000000 pyuserside-0.1.1/src/pyuserside.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-27 08:08:23.000000 pyuserside-0.1.1/src/pyuserside.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:08:23.000000 pyuserside-0.1.1/src/pyuserside.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 08:08:23.000000 pyuserside-0.1.1/src/pyuserside.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 08:08:23.000000 pyuserside-0.1.1/src/pyuserside.egg-info/top_level.txt
```

### Comparing `pyuserside-0.1.0/LICENSE` & `pyuserside-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuserside-0.1.0/src/pyuserside/api/asynchronous.py` & `pyuserside-0.1.1/src/pyuserside/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-import aiohttp
-
-from ..parser import parse_response
+import json.decoder
+import httpx
 
 
 class UsersideCategory:
     def __init__(self, category: str, api: 'UsersideAPI'):
         self._api = api
         self._cat = category
 
     def __getattr__(self, action: str):
-        async def method(**kwargs):
-            return await self._api._request(cat=self._cat,
-                                            action=action,
-                                            **kwargs)
+        def method(**kwargs):
+            return self._api._request(cat=self._cat,
+                                      action=action,
+                                      **kwargs)
         return method
 
 
 class UsersideAPI:
-    def __init__(self, url: str, key: str):
+    def __init__(self,
+                 url: str,
+                 key: str, ):
         self._url = url
         self._key = key
         self._in_use = 0
-        self._session: aiohttp.ClientSession | None = None
+        self._session = httpx.Client(params={'key': self._key})
 
-    async def _request(self, cat: str, action: str, **kwargs):
-        params = {'key': self._key, 'cat': cat, 'action': action}
+    def _request(self, cat: str, action: str, **kwargs):
+        params = {'cat': cat, 'action': action}
         params.update(kwargs)
-        async with self._session.get(url=self._url, params=params) as response:
-            content = await response.json()
-            if not response.ok:
-                raise RuntimeError(content.get('error', 'No error from Userside'))
-            elif not response.content:
-                raise RuntimeError('Empty response')
-        return parse_response(content)
+        response = self._session.get(url=self._url, params=params)
+        try:
+            content = response.json()
+        except json.decoder.JSONDecodeError:
+            raise RuntimeError('Non-JSON response')
+        if not response.status_code == 200:
+            raise RuntimeError(content.get('error', 'No error from Userside'))
+        elif not response.text:
+            raise RuntimeError('Empty response')
+        return self._parse_response(content)
+
+    @staticmethod
+    def _parse_response(response: dict):
+        if (id_ := response.get('id')) is not None:
+            return id_
+        if (data := response.get('data')) is not None:
+            return data
+        if (list_ := response.get('list')) is not None:
+            return list_.split(',')
+        return response
 
     def __getattr__(self, item):
         return UsersideCategory(item, self)
-
-    async def __aenter__(self):
-        if (self._in_use == 0) and (not self._session):
-            self._session = aiohttp.ClientSession()
-        self._in_use += 1
-        return self
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        self._in_use -= 1
-        if (self._in_use == 0) and self._session:
-            await self._session.close()
-            self._session = None
```

