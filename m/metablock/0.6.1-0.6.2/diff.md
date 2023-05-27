# Comparing `tmp/metablock-0.6.1.tar.gz` & `tmp/metablock-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metablock-0.6.1.tar", max compression
+gzip compressed data, was "metablock-0.6.2.tar", max compression
```

## Comparing `metablock-0.6.1.tar` & `metablock-0.6.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1482 2023-05-23 09:21:08.497285 metablock-0.6.1/LICENSE
--rw-r--r--   0        0        0      502 2023-05-23 09:21:08.497285 metablock-0.6.1/metablock/__init__.py
--rw-r--r--   0        0        0     4004 2023-05-23 09:21:08.497285 metablock-0.6.1/metablock/client.py
--rw-r--r--   0        0        0     7955 2023-05-23 09:21:08.497285 metablock-0.6.1/metablock/components.py
--rw-r--r--   0        0        0      564 2023-05-23 09:21:08.497285 metablock-0.6.1/metablock/extensions.py
--rw-r--r--   0        0        0     1850 2023-05-23 09:21:08.497285 metablock-0.6.1/metablock/orgs.py
--rw-r--r--   0        0        0        0 2023-05-23 09:21:08.497285 metablock-0.6.1/metablock/py.typed
--rw-r--r--   0        0        0     3029 2023-05-23 09:21:08.497285 metablock-0.6.1/metablock/spaces.py
--rw-r--r--   0        0        0     1482 2023-05-23 09:21:08.497285 metablock-0.6.1/metablock/user.py
--rw-r--r--   0        0        0      531 2023-05-23 09:21:08.497285 metablock-0.6.1/metablock/utils.py
--rw-r--r--   0        0        0      564 2023-05-23 09:21:08.497285 metablock-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1010 2023-05-23 09:21:08.497285 metablock-0.6.1/readme.md
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 metablock-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1482 2023-05-26 18:29:27.902507 metablock-0.6.2/LICENSE
+-rw-r--r--   0        0        0      502 2023-05-26 18:29:27.902507 metablock-0.6.2/metablock/__init__.py
+-rw-r--r--   0        0        0     1971 2023-05-26 18:29:27.902507 metablock-0.6.2/metablock/cli.py
+-rw-r--r--   0        0        0     4004 2023-05-26 18:29:27.902507 metablock-0.6.2/metablock/client.py
+-rw-r--r--   0        0        0     7955 2023-05-26 18:29:27.902507 metablock-0.6.2/metablock/components.py
+-rw-r--r--   0        0        0      564 2023-05-26 18:29:27.902507 metablock-0.6.2/metablock/extensions.py
+-rw-r--r--   0        0        0     1850 2023-05-26 18:29:27.902507 metablock-0.6.2/metablock/orgs.py
+-rw-r--r--   0        0        0        0 2023-05-26 18:29:27.902507 metablock-0.6.2/metablock/py.typed
+-rw-r--r--   0        0        0     3029 2023-05-26 18:29:27.902507 metablock-0.6.2/metablock/spaces.py
+-rw-r--r--   0        0        0     1482 2023-05-26 18:29:27.902507 metablock-0.6.2/metablock/user.py
+-rw-r--r--   0        0        0      531 2023-05-26 18:29:27.902507 metablock-0.6.2/metablock/utils.py
+-rw-r--r--   0        0        0      681 2023-05-26 18:29:27.906507 metablock-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1120 2023-05-26 18:29:27.906507 metablock-0.6.2/readme.md
+-rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 metablock-0.6.2/PKG-INFO
```

### Comparing `metablock-0.6.1/LICENSE` & `metablock-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metablock-0.6.1/metablock/client.py` & `metablock-0.6.2/metablock/client.py`

 * *Files identical despite different names*

### Comparing `metablock-0.6.1/metablock/components.py` & `metablock-0.6.2/metablock/components.py`

 * *Files identical despite different names*

### Comparing `metablock-0.6.1/metablock/extensions.py` & `metablock-0.6.2/metablock/extensions.py`

 * *Files identical despite different names*

### Comparing `metablock-0.6.1/metablock/orgs.py` & `metablock-0.6.2/metablock/orgs.py`

 * *Files identical despite different names*

### Comparing `metablock-0.6.1/metablock/spaces.py` & `metablock-0.6.2/metablock/spaces.py`

 * *Files identical despite different names*

### Comparing `metablock-0.6.1/metablock/user.py` & `metablock-0.6.2/metablock/user.py`

 * *Files identical despite different names*

### Comparing `metablock-0.6.1/metablock/utils.py` & `metablock-0.6.2/metablock/utils.py`

 * *Files identical despite different names*

### Comparing `metablock-0.6.1/pyproject.toml` & `metablock-0.6.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 [tool.poetry]
 name = "metablock"
-version = "0.6.1"
+version = "0.6.2"
 description = "Metablock cloud python client"
 authors = ["Luca <luca@quantmind.com>"]
 license = "BSD"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 aiohttp = "^3.8.3"
+click = "^8.1.3"
+pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.21.0"
 pytest = "^7.0.1"
 pytest-cov = "^4.0.0"
 mypy = "^1.3.0"
 black = "^23.3.0"
 isort = "^5.11.3"
 flake8 = "^6.0.0"
 flake8-builtins = "^2.0.1"
 python-dotenv = "^1.0.0"
+types-pyyaml = "^6.0.12.10"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+metablock = "metablock.cli:main"
```

### Comparing `metablock-0.6.1/readme.md` & `metablock-0.6.2/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,8 +24,13 @@
 
 cli = Metablock()
 
 # get the user associated with the API token
 user = await cli.get_user()
 ```
 
-For the authentication token you can create the `METABLOCK_API_TOKEN` environment variable.
+For the authentication token, you can use the `METABLOCK_API_TOKEN` environment variable,
+alternatively, you can pass it to the client constructor:
+
+```python
+cli = Metablock(auth_key="your-token")
+```
```

### Comparing `metablock-0.6.1/PKG-INFO` & `metablock-0.6.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: metablock
-Version: 0.6.1
+Version: 0.6.2
 Summary: Metablock cloud python client
 License: BSD
 Author: Luca
 Author-email: luca@quantmind.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 # A Python Client for Metablock API
 
 [![PyPI version](https://badge.fury.io/py/metablock.svg)](https://badge.fury.io/py/metablock)
 [![Python versions](https://img.shields.io/pypi/pyversions/metablock.svg)](https://pypi.org/project/metablock)
 [![Build](https://github.com/quantmind/metablock-py/workflows/build/badge.svg)](https://github.com/quantmind/metablock-py/actions?query=workflow%3Abuild)
@@ -39,9 +41,14 @@
 
 cli = Metablock()
 
 # get the user associated with the API token
 user = await cli.get_user()
 ```
 
-For the authentication token you can create the `METABLOCK_API_TOKEN` environment variable.
+For the authentication token, you can use the `METABLOCK_API_TOKEN` environment variable,
+alternatively, you can pass it to the client constructor:
+
+```python
+cli = Metablock(auth_key="your-token")
+```
```

