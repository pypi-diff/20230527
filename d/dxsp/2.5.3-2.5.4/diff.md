# Comparing `tmp/dxsp-2.5.3.tar.gz` & `tmp/dxsp-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.5.3.tar", max compression
+gzip compressed data, was "dxsp-2.5.4.tar", max compression
```

## Comparing `dxsp-2.5.3.tar` & `dxsp-2.5.4.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-27 11:34:12.088821 dxsp-2.5.3/LICENSE
--rw-r--r--   0        0        0     2439 2023-05-27 11:34:12.088821 dxsp-2.5.3/README.md
--rw-r--r--   0        0        0       86 2023-05-27 11:34:12.948825 dxsp-2.5.3/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-27 11:34:12.088821 dxsp-2.5.3/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-27 11:34:12.088821 dxsp-2.5.3/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      386 2023-05-27 11:34:12.088821 dxsp-2.5.3/dxsp/config.py
--rw-r--r--   0        0        0     3548 2023-05-27 11:34:12.088821 dxsp-2.5.3/dxsp/default_settings.toml
--rw-r--r--   0        0        0    20785 2023-05-27 11:34:12.088821 dxsp-2.5.3/dxsp/main.py
--rw-r--r--   0        0        0     1973 2023-05-27 11:34:12.948825 dxsp-2.5.3/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-27 13:33:45.995262 dxsp-2.5.4/LICENSE
+-rw-r--r--   0        0        0     2439 2023-05-27 13:33:45.995262 dxsp-2.5.4/README.md
+-rw-r--r--   0        0        0       86 2023-05-27 13:33:46.783326 dxsp-2.5.4/dxsp/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-27 13:33:45.995262 dxsp-2.5.4/dxsp/config.py
+-rw-r--r--   0        0        0     3548 2023-05-27 13:33:45.995262 dxsp-2.5.4/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    20785 2023-05-27 13:33:45.995262 dxsp-2.5.4/dxsp/main.py
+-rw-r--r--   0        0        0     1996 2023-05-27 13:33:46.783326 dxsp-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.5.4/PKG-INFO
```

### Comparing `dxsp-2.5.3/LICENSE` & `dxsp-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.3/README.md` & `dxsp-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.3/dxsp/default_settings.toml` & `dxsp-2.5.4/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.3/dxsp/main.py` & `dxsp-2.5.4/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.3/pyproject.toml` & `dxsp-2.5.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.5.3"
+version = "2.5.4"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -40,15 +40,16 @@
   "*Test"
 ]
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 pythonpath = [
   "."
 ]
-addopts = "--capture=no --ignore-glob=example_*"
+addopts = "--capture=no --ignore-glob=example*"
+ignore="tests examples"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
```

### Comparing `dxsp-2.5.3/PKG-INFO` & `dxsp-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.5.3
+Version: 2.5.4
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

