# Comparing `tmp/d20-securityLayer-2.0.0a1.tar.gz` & `tmp/d20-securityLayer-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-0f4f7sg2\d20-securityLayer-2.0.0a1.tar", last modified: Fri May 19 00:34:42 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-yw1pxvlb\d20-securityLayer-2.0.0a2.tar", last modified: Fri May 26 23:56:24 2023, max compression
```

## Comparing `d20-securityLayer-2.0.0a1.tar` & `d20-securityLayer-2.0.0a2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 00:34:42.012267 d20-securityLayer-2.0.0a1/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-2.0.0a1/LICENSE
--rw-rw-rw-   0        0        0      677 2023-05-19 00:34:42.011299 d20-securityLayer-2.0.0a1/PKG-INFO
--rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-2.0.0a1/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-2.0.0a1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 00:34:42.012267 d20-securityLayer-2.0.0a1/setup.cfg
--rw-rw-rw-   0        0        0      964 2023-05-19 00:34:24.000000 d20-securityLayer-2.0.0a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 00:34:41.670903 d20-securityLayer-2.0.0a1/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 00:34:41.820267 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/
--rw-rw-rw-   0        0        0      677 2023-05-19 00:34:41.000000 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-05-19 00:34:41.000000 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 00:34:41.000000 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-19 00:34:41.000000 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-19 00:34:41.000000 d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 00:34:42.009262 d20-securityLayer-2.0.0a1/src/securityLayer/
--rw-rw-rw-   0        0        0    10081 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a1/src/securityLayer/AccessControl.py
--rw-rw-rw-   0        0        0      233 2023-05-16 00:25:53.000000 d20-securityLayer-2.0.0a1/src/securityLayer/AuthAnswer.py
--rw-rw-rw-   0        0        0     9697 2023-05-16 02:42:02.000000 d20-securityLayer-2.0.0a1/src/securityLayer/Error.py
--rw-rw-rw-   0        0        0    16923 2023-05-16 03:11:04.000000 d20-securityLayer-2.0.0a1/src/securityLayer/SSO.py
--rw-rw-rw-   0        0        0    15241 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a1/src/securityLayer/SecurityLayer.py
--rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-2.0.0a1/src/securityLayer/__init__.py
--rw-rw-rw-   0        0        0      156 2023-05-12 02:57:34.000000 d20-securityLayer-2.0.0a1/src/securityLayer/__version__.py
--rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-2.0.0a1/src/securityLayer/default.py
+drwxrwxrwx   0        0        0        0 2023-05-26 23:56:24.889098 d20-securityLayer-2.0.0a2/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-2.0.0a2/LICENSE
+-rw-rw-rw-   0        0        0      677 2023-05-26 23:56:24.886084 d20-securityLayer-2.0.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-2.0.0a2/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-2.0.0a2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 23:56:24.890108 d20-securityLayer-2.0.0a2/setup.cfg
+-rw-rw-rw-   0        0        0      964 2023-05-26 23:55:43.000000 d20-securityLayer-2.0.0a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 23:56:24.689836 d20-securityLayer-2.0.0a2/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 23:56:24.719309 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/
+-rw-rw-rw-   0        0        0      677 2023-05-26 23:56:24.000000 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-05-26 23:56:24.000000 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 23:56:24.000000 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-26 23:56:24.000000 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-26 23:56:24.000000 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 23:56:24.882087 d20-securityLayer-2.0.0a2/src/securityLayer/
+-rw-rw-rw-   0        0        0    10081 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a2/src/securityLayer/AccessControl.py
+-rw-rw-rw-   0        0        0      233 2023-05-16 00:25:53.000000 d20-securityLayer-2.0.0a2/src/securityLayer/AuthAnswer.py
+-rw-rw-rw-   0        0        0     9697 2023-05-16 02:42:02.000000 d20-securityLayer-2.0.0a2/src/securityLayer/Error.py
+-rw-rw-rw-   0        0        0    16923 2023-05-16 03:11:04.000000 d20-securityLayer-2.0.0a2/src/securityLayer/SSO.py
+-rw-rw-rw-   0        0        0    15241 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a2/src/securityLayer/SecurityLayer.py
+-rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-2.0.0a2/src/securityLayer/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-05-12 02:57:34.000000 d20-securityLayer-2.0.0a2/src/securityLayer/__version__.py
+-rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-2.0.0a2/src/securityLayer/default.py
```

### Comparing `d20-securityLayer-2.0.0a1/LICENSE` & `d20-securityLayer-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a1/PKG-INFO` & `d20-securityLayer-2.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-2.0.0a1/setup.py` & `d20-securityLayer-2.0.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-securityLayer",
-    version="2.0.0a1",
+    version="2.0.0a2",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A simple access manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/security_layer_python_arangodb",
     project_urls={
```

### Comparing `d20-securityLayer-2.0.0a1/src/d20_securityLayer.egg-info/PKG-INFO` & `d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-2.0.0a1/src/securityLayer/AccessControl.py` & `d20-securityLayer-2.0.0a2/src/securityLayer/AccessControl.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a1/src/securityLayer/Error.py` & `d20-securityLayer-2.0.0a2/src/securityLayer/Error.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a1/src/securityLayer/SSO.py` & `d20-securityLayer-2.0.0a2/src/securityLayer/SSO.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a1/src/securityLayer/SecurityLayer.py` & `d20-securityLayer-2.0.0a2/src/securityLayer/SecurityLayer.py`

 * *Files identical despite different names*

