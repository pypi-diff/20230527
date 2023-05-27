# Comparing `tmp/NaturalAPI-0.0.2.tar.gz` & `tmp/NaturalAPI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NaturalAPI-0.0.2.tar", last modified: Sat May 27 09:21:55 2023, max compression
+gzip compressed data, was "NaturalAPI-0.0.3.tar", last modified: Sat May 27 10:30:18 2023, max compression
```

## Comparing `NaturalAPI-0.0.2.tar` & `NaturalAPI-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 09:21:55.769575 NaturalAPI-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-05-27 08:51:54.000000 NaturalAPI-0.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-27 09:21:55.749695 NaturalAPI-0.0.2/NaturalAPI.egg-info/
--rw-rw-rw-   0        0        0     1521 2023-05-27 09:21:55.000000 NaturalAPI-0.0.2/NaturalAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-05-27 09:21:55.000000 NaturalAPI-0.0.2/NaturalAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:21:55.000000 NaturalAPI-0.0.2/NaturalAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:21:55.000000 NaturalAPI-0.0.2/NaturalAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1521 2023-05-27 09:21:55.769575 NaturalAPI-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1102 2023-05-27 09:20:22.000000 NaturalAPI-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 09:21:55.769575 NaturalAPI-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-05-27 09:20:12.000000 NaturalAPI-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:30:18.421726 NaturalAPI-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-27 08:51:54.000000 NaturalAPI-0.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-27 10:30:18.421726 NaturalAPI-0.0.3/NaturalAPI.egg-info/
+-rw-rw-rw-   0        0        0     2862 2023-05-27 10:30:18.000000 NaturalAPI-0.0.3/NaturalAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-05-27 10:30:18.000000 NaturalAPI-0.0.3/NaturalAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 10:30:18.000000 NaturalAPI-0.0.3/NaturalAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 10:30:18.000000 NaturalAPI-0.0.3/NaturalAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2862 2023-05-27 10:30:18.421726 NaturalAPI-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2443 2023-05-27 10:22:02.000000 NaturalAPI-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 10:30:18.421726 NaturalAPI-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-05-27 10:29:17.000000 NaturalAPI-0.0.3/setup.py
```

### Comparing `NaturalAPI-0.0.2/LICENSE` & `NaturalAPI-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NaturalAPI-0.0.2/setup.py` & `NaturalAPI-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name="NaturalAPI",
-  version="0.0.2",
+  version="0.0.3",
   author="yydshmcl@outlook.com",
   author_email="yydshmcl@outlook.com",
   description="API for a small studio",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Buelie/Natural",
   packages=setuptools.find_packages(),
```

