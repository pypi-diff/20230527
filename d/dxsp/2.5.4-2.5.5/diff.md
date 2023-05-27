# Comparing `tmp/dxsp-2.5.4.tar.gz` & `tmp/dxsp-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.5.4.tar", max compression
+gzip compressed data, was "dxsp-2.5.5.tar", max compression
```

## Comparing `dxsp-2.5.4.tar` & `dxsp-2.5.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-27 13:33:45.995262 dxsp-2.5.4/LICENSE
--rw-r--r--   0        0        0     2439 2023-05-27 13:33:45.995262 dxsp-2.5.4/README.md
--rw-r--r--   0        0        0       86 2023-05-27 13:33:46.783326 dxsp-2.5.4/dxsp/__init__.py
--rw-r--r--   0        0        0      386 2023-05-27 13:33:45.995262 dxsp-2.5.4/dxsp/config.py
--rw-r--r--   0        0        0     3548 2023-05-27 13:33:45.995262 dxsp-2.5.4/dxsp/default_settings.toml
--rw-r--r--   0        0        0    20785 2023-05-27 13:33:45.995262 dxsp-2.5.4/dxsp/main.py
--rw-r--r--   0        0        0     1996 2023-05-27 13:33:46.783326 dxsp-2.5.4/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-27 13:48:18.044194 dxsp-2.5.5/LICENSE
+-rw-r--r--   0        0        0     2439 2023-05-27 13:48:18.044194 dxsp-2.5.5/README.md
+-rw-r--r--   0        0        0       86 2023-05-27 13:48:18.676208 dxsp-2.5.5/dxsp/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-27 13:48:18.044194 dxsp-2.5.5/dxsp/config.py
+-rw-r--r--   0        0        0     3548 2023-05-27 13:48:18.044194 dxsp-2.5.5/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    20785 2023-05-27 13:48:18.044194 dxsp-2.5.5/dxsp/main.py
+-rw-r--r--   0        0        0     1994 2023-05-27 13:48:18.676208 dxsp-2.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.5.5/PKG-INFO
```

### Comparing `dxsp-2.5.4/LICENSE` & `dxsp-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.4/README.md` & `dxsp-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.4/dxsp/default_settings.toml` & `dxsp-2.5.5/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.4/dxsp/main.py` & `dxsp-2.5.5/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.4/pyproject.toml` & `dxsp-2.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.5.4"
+version = "2.5.5"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -41,15 +41,15 @@
 ]
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 pythonpath = [
   "."
 ]
 addopts = "--capture=no --ignore-glob=example*"
-ignore="tests examples"
+ignore="test example"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
```

### Comparing `dxsp-2.5.4/PKG-INFO` & `dxsp-2.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.5.4
+Version: 2.5.5
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

