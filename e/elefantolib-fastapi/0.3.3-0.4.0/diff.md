# Comparing `tmp/elefantolib_fastapi-0.3.3.tar.gz` & `tmp/elefantolib_fastapi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib_fastapi-0.3.3.tar", max compression
+gzip compressed data, was "elefantolib_fastapi-0.4.0.tar", max compression
```

## Comparing `elefantolib_fastapi-0.3.3.tar` & `elefantolib_fastapi-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      878 2023-05-25 14:55:37.926114 elefantolib_fastapi-0.3.3/README.md
--rw-r--r--   0        0        0       22 2023-05-25 14:55:37.926114 elefantolib_fastapi-0.3.3/elefantolib_fastapi/__init__.py
--rw-r--r--   0        0        0      736 2023-05-25 14:55:37.926114 elefantolib_fastapi-0.3.3/elefantolib_fastapi/depends.py
--rw-r--r--   0        0        0      354 2023-05-25 14:55:37.926114 elefantolib_fastapi-0.3.3/elefantolib_fastapi/exceptions.py
--rw-r--r--   0        0        0      374 2023-05-25 14:55:37.926114 elefantolib_fastapi-0.3.3/elefantolib_fastapi/requests.py
--rw-r--r--   0        0        0      898 2023-05-25 14:55:37.926114 elefantolib_fastapi-0.3.3/elefantolib_fastapi/routes.py
--rw-r--r--   0        0        0      890 2023-05-25 14:55:52.150523 elefantolib_fastapi-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.3.3/setup.py
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/__init__.py
+-rw-r--r--   0        0        0     1018 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/connection.py
+-rw-r--r--   0        0        0      736 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/depends.py
+-rw-r--r--   0        0        0      934 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/exceptions.py
+-rw-r--r--   0        0        0      209 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/requests.py
+-rw-r--r--   0        0        0      721 2023-05-27 13:32:46.411285 elefantolib_fastapi-0.4.0/elefantolib_fastapi/routes.py
+-rw-r--r--   0        0        0      890 2023-05-27 13:33:00.147497 elefantolib_fastapi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.4.0/setup.py
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 elefantolib_fastapi-0.4.0/PKG-INFO
```

### Comparing `elefantolib_fastapi-0.3.3/README.md` & `elefantolib_fastapi-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.3.3/elefantolib_fastapi/depends.py` & `elefantolib_fastapi-0.4.0/elefantolib_fastapi/depends.py`

 * *Files identical despite different names*

### Comparing `elefantolib_fastapi-0.3.3/elefantolib_fastapi/routes.py` & `elefantolib_fastapi-0.4.0/elefantolib_fastapi/routes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-import os
 from typing import Callable
 
 from elefantolib import context
 from elefantolib.provider import fastapi_provider
 
 import fastapi
 from fastapi import routing
 
-from redis import asyncio as aioredis
-
 from .requests import Request
 
 
 class APIRoute(routing.APIRoute):
 
     def get_route_handler(self) -> Callable:
         original_route_handler = super().get_route_handler()
 
         async def custom_route_handler(request: fastapi.Request) -> fastapi.Response:
             pvr = fastapi_provider.FastAPIProvider(request=request)
             request.scope['pfm'] = context.AsyncPlatformContext(pvr=pvr)
-
-            if redis_url := os.environ.get('REDIS_URL'):
-                request.scope['redis'] = aioredis.from_url(redis_url)
-
             new_request = Request(request.scope, request.receive)
             return await original_route_handler(new_request)
+
         return custom_route_handler
```

### Comparing `elefantolib_fastapi-0.3.3/pyproject.toml` & `elefantolib_fastapi-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elefantolib-fastapi"
-version = "0.3.3"
+version = "0.4.0"
 description = ""
 authors = ["gglassota <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "elefantolib_fastapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `elefantolib_fastapi-0.3.3/setup.py` & `elefantolib_fastapi-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['elefantolib>=0.12.1,<0.13.0',
  'fastapi>=0.95.2,<0.96.0',
  'redis>=4.5.5,<5.0.0']
 
 setup_kwargs = {
     'name': 'elefantolib-fastapi',
-    'version': '0.3.3',
+    'version': '0.4.0',
     'description': '',
     'long_description': '## Elefantolib for FastAPI\n\n> **_NOTE:_**  Only for this library developers. After clone this repository you should run command:\n> \n\n ```console \ngit config core.hooksPath .githooks\n```\n\n\n## Installation\n\n<div class="termy">\n\n```console\npoetry add elefantolib-fastapi\n```\n</div>\n\n## Example\n\n### Prepare\n\n* Add environmental variables\n\n```\nSECRET=\nALGORITHM=\nISSUER=\n```\n* Defaults:\n    \n    - SECRET - not set, this is required\n    - ALGORITHM=HS256\n    - ISSUER=Consumer\n\n### Create it\n\n* Create a file `main.py` with:\n\n```Python\nfrom elefantolib_fastapi.requests import Request\nfrom elefantolib_fastapi.routes import APIRoute\n\nfrom fastapi import FastAPI\n\napp = FastAPI()\n\napp.router.route_class = APIRoute\n\n\n@app.get(\'/\')\ndef index(request: Request):\n    # TODO something\n    response = request.pfm.services.some_service_name.get(\'path-to-endpoint\')\n    return response\n\n```',
     'author': 'gglassota',
     'author_email': 'gglassota2@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `elefantolib_fastapi-0.3.3/PKG-INFO` & `elefantolib_fastapi-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefantolib-fastapi
-Version: 0.3.3
+Version: 0.4.0
 Summary: 
 Author: gglassota
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

