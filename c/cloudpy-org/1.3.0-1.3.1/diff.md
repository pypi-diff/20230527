# Comparing `tmp/cloudpy_org-1.3.0.tar.gz` & `tmp/cloudpy_org-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.3.0.tar", last modified: Sat May 27 04:25:08 2023, max compression
+gzip compressed data, was "dist\cloudpy_org-1.3.1.tar", last modified: Sat May 27 04:39:23 2023, max compression
```

## Comparing `cloudpy_org-1.3.0.tar` & `cloudpy_org-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 04:25:08.670574 cloudpy_org-1.3.0/
--rw-rw-rw-   0        0        0      935 2023-05-27 04:25:08.669765 cloudpy_org-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 04:25:08.526534 cloudpy_org-1.3.0/cloudpy_org/
--rw-rw-rw-   0        0        0       62 2023-05-27 04:09:21.000000 cloudpy_org-1.3.0/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    71190 2023-05-27 04:21:16.000000 cloudpy_org-1.3.0/cloudpy_org/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-27 04:25:08.649296 cloudpy_org-1.3.0/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2023-05-27 04:25:07.000000 cloudpy_org-1.3.0/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-27 04:25:08.000000 cloudpy_org-1.3.0/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 04:25:07.000000 cloudpy_org-1.3.0/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-27 04:25:07.000000 cloudpy_org-1.3.0/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-27 04:25:07.000000 cloudpy_org-1.3.0/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 04:25:08.670574 cloudpy_org-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1324 2023-05-27 04:17:36.000000 cloudpy_org-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 04:39:23.679280 cloudpy_org-1.3.1/
+-rw-rw-rw-   0        0        0      935 2023-05-27 04:39:23.678740 cloudpy_org-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 04:39:23.549549 cloudpy_org-1.3.1/cloudpy_org/
+-rw-rw-rw-   0        0        0       82 2023-05-27 04:35:22.000000 cloudpy_org-1.3.1/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    71190 2023-05-27 04:21:16.000000 cloudpy_org-1.3.1/cloudpy_org/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-27 04:39:23.657084 cloudpy_org-1.3.1/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-05-27 04:39:23.000000 cloudpy_org-1.3.1/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-27 04:39:23.000000 cloudpy_org-1.3.1/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 04:39:23.000000 cloudpy_org-1.3.1/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-27 04:39:23.000000 cloudpy_org-1.3.1/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-27 04:39:23.000000 cloudpy_org-1.3.1/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 04:39:23.679504 cloudpy_org-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2023-05-27 04:37:53.000000 cloudpy_org-1.3.1/setup.py
```

### Comparing `cloudpy_org-1.3.0/PKG-INFO` & `cloudpy_org-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.3.0
+Version: 1.3.1
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.3.0/cloudpy_org/tools.py` & `cloudpy_org-1.3.1/cloudpy_org/tools.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.3.0/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.3.1/cloudpy_org.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.3.0
+Version: 1.3.1
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.3.0/setup.py` & `cloudpy_org-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.3.0",
+    version="1.3.1",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

