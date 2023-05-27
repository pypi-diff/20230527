# Comparing `tmp/NaturalAPI-0.0.6.tar.gz` & `tmp/NaturalAPI-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NaturalAPI-0.0.6.tar", last modified: Sat May 27 11:23:29 2023, max compression
+gzip compressed data, was "NaturalAPI-0.0.7.tar", last modified: Sat May 27 11:25:14 2023, max compression
```

## Comparing `NaturalAPI-0.0.6.tar` & `NaturalAPI-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 11:23:29.089323 NaturalAPI-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-05-27 08:51:54.000000 NaturalAPI-0.0.6/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-27 11:23:29.089323 NaturalAPI-0.0.6/NaturalAPI.egg-info/
--rw-rw-rw-   0        0        0      415 2023-05-27 11:23:28.000000 NaturalAPI-0.0.6/NaturalAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-05-27 11:23:29.000000 NaturalAPI-0.0.6/NaturalAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:23:28.000000 NaturalAPI-0.0.6/NaturalAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:23:28.000000 NaturalAPI-0.0.6/NaturalAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      415 2023-05-27 11:23:29.089323 NaturalAPI-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2443 2023-05-27 11:23:24.000000 NaturalAPI-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 11:23:29.089323 NaturalAPI-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      688 2023-05-27 11:23:15.000000 NaturalAPI-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:25:14.525827 NaturalAPI-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-05-27 08:51:54.000000 NaturalAPI-0.0.7/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-27 11:25:14.510206 NaturalAPI-0.0.7/NaturalAPI.egg-info/
+-rw-rw-rw-   0        0        0      415 2023-05-27 11:25:14.000000 NaturalAPI-0.0.7/NaturalAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-05-27 11:25:14.000000 NaturalAPI-0.0.7/NaturalAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:25:14.000000 NaturalAPI-0.0.7/NaturalAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:25:14.000000 NaturalAPI-0.0.7/NaturalAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      415 2023-05-27 11:25:14.525827 NaturalAPI-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2443 2023-05-27 11:23:24.000000 NaturalAPI-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 11:25:14.525827 NaturalAPI-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      688 2023-05-27 11:25:09.000000 NaturalAPI-0.0.7/setup.py
```

### Comparing `NaturalAPI-0.0.6/LICENSE` & `NaturalAPI-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `NaturalAPI-0.0.6/README.md` & `NaturalAPI-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `NaturalAPI-0.0.6/setup.py` & `NaturalAPI-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name="NaturalAPI",
-  version="0.0.6",
+  version="0.0.7",
   author="yydshmcl@outlook.com",
   author_email="yydshmcl@outlook.com",
   description="API for a small studio",
   #long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Buelie/Natural",
   packages=setuptools.find_packages(),
```

