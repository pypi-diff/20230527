# Comparing `tmp/NaturalAPI-0.0.8.tar.gz` & `tmp/NaturalAPI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NaturalAPI-0.0.8.tar", last modified: Sat May 27 11:26:58 2023, max compression
+gzip compressed data, was "NaturalAPI-0.0.9.tar", last modified: Sat May 27 12:10:20 2023, max compression
```

## Comparing `NaturalAPI-0.0.8.tar` & `NaturalAPI-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 11:26:58.769889 NaturalAPI-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-05-27 08:51:54.000000 NaturalAPI-0.0.8/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-27 11:26:58.769889 NaturalAPI-0.0.8/NaturalAPI.egg-info/
--rw-rw-rw-   0        0        0     2862 2023-05-27 11:26:58.000000 NaturalAPI-0.0.8/NaturalAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-05-27 11:26:58.000000 NaturalAPI-0.0.8/NaturalAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:26:58.000000 NaturalAPI-0.0.8/NaturalAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:26:58.000000 NaturalAPI-0.0.8/NaturalAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2862 2023-05-27 11:26:58.769889 NaturalAPI-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2443 2023-05-27 11:23:24.000000 NaturalAPI-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 11:26:58.769889 NaturalAPI-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-05-27 11:26:53.000000 NaturalAPI-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:20.895583 NaturalAPI-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-05-27 08:51:54.000000 NaturalAPI-0.0.9/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-27 12:10:20.386132 NaturalAPI-0.0.9/NaturalAPI.egg-info/
+-rw-rw-rw-   0        0        0     2862 2023-05-27 12:10:16.000000 NaturalAPI-0.0.9/NaturalAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-05-27 12:10:17.000000 NaturalAPI-0.0.9/NaturalAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 12:10:16.000000 NaturalAPI-0.0.9/NaturalAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 12:10:17.000000 NaturalAPI-0.0.9/NaturalAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2862 2023-05-27 12:10:20.755991 NaturalAPI-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2443 2023-05-27 11:23:24.000000 NaturalAPI-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 12:10:20.895583 NaturalAPI-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-05-27 12:10:08.000000 NaturalAPI-0.0.9/setup.py
```

### Comparing `NaturalAPI-0.0.8/LICENSE` & `NaturalAPI-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `NaturalAPI-0.0.8/NaturalAPI.egg-info/PKG-INFO` & `NaturalAPI-0.0.9/NaturalAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NaturalAPI
-Version: 0.0.8
+Version: 0.0.9
 Summary: API for a small studio
 Home-page: https://github.com/Buelie/Natural
 Author: yydshmcl@outlook.com
 Author-email: yydshmcl@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NaturalAPI-0.0.8/PKG-INFO` & `NaturalAPI-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NaturalAPI
-Version: 0.0.8
+Version: 0.0.9
 Summary: API for a small studio
 Home-page: https://github.com/Buelie/Natural
 Author: yydshmcl@outlook.com
 Author-email: yydshmcl@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NaturalAPI-0.0.8/README.md` & `NaturalAPI-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `NaturalAPI-0.0.8/setup.py` & `NaturalAPI-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name="NaturalAPI",
-  version="0.0.8",
+  version="0.0.9",
   author="yydshmcl@outlook.com",
   author_email="yydshmcl@outlook.com",
   description="API for a small studio",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Buelie/Natural",
   packages=setuptools.find_packages(),
```

