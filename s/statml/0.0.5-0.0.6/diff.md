# Comparing `tmp/statml-0.0.5.tar.gz` & `tmp/statml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statml-0.0.5.tar", last modified: Sun May 21 12:08:49 2023, max compression
+gzip compressed data, was "statml-0.0.6.tar", last modified: Sat May 27 02:36:59 2023, max compression
```

## Comparing `statml-0.0.5.tar` & `statml-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 12:08:49.744778 statml-0.0.5/
--rw-rw-rw-   0        0        0      381 2023-05-21 12:08:49.744778 statml-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-05-20 12:40:16.000000 statml-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 12:08:49.744778 statml-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      608 2023-05-21 11:58:06.000000 statml-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 12:08:49.729154 statml-0.0.5/statml/
--rw-rw-rw-   0        0        0       21 2023-05-21 11:57:52.000000 statml-0.0.5/statml/__init__.py
--rw-rw-rw-   0        0        0     3621 2023-05-21 11:57:23.000000 statml-0.0.5/statml/playchat.py
--rw-rw-rw-   0        0        0     5209 2023-05-21 11:26:39.000000 statml-0.0.5/statml/stepwise.py
-drwxrwxrwx   0        0        0        0 2023-05-21 12:08:49.744778 statml-0.0.5/statml.egg-info/
--rw-rw-rw-   0        0        0      381 2023-05-21 12:08:49.000000 statml-0.0.5/statml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-05-21 12:08:49.000000 statml-0.0.5/statml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 12:08:49.000000 statml-0.0.5/statml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-21 12:08:49.000000 statml-0.0.5/statml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 02:36:59.120626 statml-0.0.6/
+-rw-rw-rw-   0        0        0       24 2023-05-27 00:51:22.000000 statml-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      381 2023-05-27 02:36:59.120626 statml-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-05-20 12:40:16.000000 statml-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 02:36:59.120626 statml-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      608 2023-05-27 02:36:39.000000 statml-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:36:59.104999 statml-0.0.6/statml/
+-rw-rw-rw-   0        0        0       21 2023-05-27 02:36:49.000000 statml-0.0.6/statml/__init__.py
+-rw-rw-rw-   0        0        0     3621 2023-05-21 11:57:23.000000 statml-0.0.6/statml/playchat.py
+-rw-rw-rw-   0        0        0     5209 2023-05-21 11:26:39.000000 statml-0.0.6/statml/stepwise.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:36:59.120626 statml-0.0.6/statml.egg-info/
+-rw-rw-rw-   0        0        0      381 2023-05-27 02:36:58.000000 statml-0.0.6/statml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-27 02:36:59.000000 statml-0.0.6/statml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 02:36:58.000000 statml-0.0.6/statml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 02:36:58.000000 statml-0.0.6/statml.egg-info/top_level.txt
```

### Comparing `statml-0.0.5/setup.py` & `statml-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="statml",
-    version="0.0.5",
+    version="0.0.6",
     author="HaeWoon",
     author_email="likesea7@gmail.com",
     description="stat and ml example",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `statml-0.0.5/statml/playchat.py` & `statml-0.0.6/statml/playchat.py`

 * *Files identical despite different names*

### Comparing `statml-0.0.5/statml/stepwise.py` & `statml-0.0.6/statml/stepwise.py`

 * *Files identical despite different names*

