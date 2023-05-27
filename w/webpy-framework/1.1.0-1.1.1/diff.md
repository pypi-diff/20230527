# Comparing `tmp/webpy-framework-1.1.0.tar.gz` & `tmp/webpy-framework-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpy-framework-1.1.0.tar", last modified: Sat May 27 15:46:25 2023, max compression
+gzip compressed data, was "webpy-framework-1.1.1.tar", last modified: Sat May 27 16:00:17 2023, max compression
```

## Comparing `webpy-framework-1.1.0.tar` & `webpy-framework-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 15:46:25.741187 webpy-framework-1.1.0/
--rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     6599 2023-05-27 15:46:25.739021 webpy-framework-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4651 2023-05-27 01:42:52.000000 webpy-framework-1.1.0/README.md
--rw-rw-rw-   0        0        0     1078 2023-05-27 15:35:35.000000 webpy-framework-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 15:46:25.741187 webpy-framework-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 15:46:25.709660 webpy-framework-1.1.0/webpy/
--rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.1.0/webpy/__init__.py
--rw-rw-rw-   0        0        0    10520 2023-05-27 15:34:19.000000 webpy-framework-1.1.0/webpy/__main__.py
--rw-rw-rw-   0        0        0     1809 2023-05-27 15:07:10.000000 webpy-framework-1.1.0/webpy/fs_routes.py
--rw-rw-rw-   0        0        0     1492 2023-05-27 15:28:10.000000 webpy-framework-1.1.0/webpy/pysite_semantic_tags.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:46:25.736492 webpy-framework-1.1.0/webpy_framework.egg-info/
--rw-rw-rw-   0        0        0     6599 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      158 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-27 15:46:25.000000 webpy-framework-1.1.0/webpy_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 16:00:17.140449 webpy-framework-1.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6599 2023-05-27 16:00:17.139450 webpy-framework-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4651 2023-05-27 01:42:52.000000 webpy-framework-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1075 2023-05-27 15:59:55.000000 webpy-framework-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 16:00:17.140449 webpy-framework-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 16:00:17.116834 webpy-framework-1.1.1/webpy/
+-rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.1.1/webpy/__init__.py
+-rw-rw-rw-   0        0        0    10520 2023-05-27 15:34:19.000000 webpy-framework-1.1.1/webpy/__main__.py
+-rw-rw-rw-   0        0        0     1809 2023-05-27 15:07:10.000000 webpy-framework-1.1.1/webpy/fs_routes.py
+-rw-rw-rw-   0        0        0     1492 2023-05-27 15:28:10.000000 webpy-framework-1.1.1/webpy/pysite_semantic_tags.py
+drwxrwxrwx   0        0        0        0 2023-05-27 16:00:17.137073 webpy-framework-1.1.1/webpy_framework.egg-info/
+-rw-rw-rw-   0        0        0     6599 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      155 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-27 16:00:17.000000 webpy-framework-1.1.1/webpy_framework.egg-info/top_level.txt
```

### Comparing `webpy-framework-1.1.0/LICENSE` & `webpy-framework-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.1.0/PKG-INFO` & `webpy-framework-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.1.0
+Version: 1.1.1
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `webpy-framework-1.1.0/README.md` & `webpy-framework-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.1.0/pyproject.toml` & `webpy-framework-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webpy-framework"
-version = "1.1.0"
+version = "1.1.1"
 description = "Easy-to-use Python web framework built on top of Flask"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
@@ -22,15 +22,15 @@
 	"dill >= 0.3.5.1",
 	"python-minifier >= 2.8.0",
 	"dill >= 0.3.6",
 	"flask-session >= 0.5.0",
 	"flask-sqlalchemy >= 3.0.0",
 	"py-domapi >= 1.0.0",
 	"pyx-pysite >= 1.0.1",
-	"markdown >= 3.4.0"
+	"marko >= 1.3.0"
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://github.com/User0332/webpy"
 Documentation = "https://webpy-framework.readthedocs.io/"
```

### Comparing `webpy-framework-1.1.0/webpy/__init__.py` & `webpy-framework-1.1.1/webpy/__init__.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.1.0/webpy/__main__.py` & `webpy-framework-1.1.1/webpy/__main__.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.1.0/webpy/fs_routes.py` & `webpy-framework-1.1.1/webpy/fs_routes.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.1.0/webpy/pysite_semantic_tags.py` & `webpy-framework-1.1.1/webpy/pysite_semantic_tags.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.1.0/webpy_framework.egg-info/PKG-INFO` & `webpy-framework-1.1.1/webpy_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.1.0
+Version: 1.1.1
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

