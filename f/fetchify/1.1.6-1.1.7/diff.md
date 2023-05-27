# Comparing `tmp/fetchify-1.1.6.tar.gz` & `tmp/fetchify-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetchify-1.1.6.tar", last modified: Sat May 27 15:21:05 2023, max compression
+gzip compressed data, was "fetchify-1.1.7.tar", last modified: Sat May 27 15:26:03 2023, max compression
```

## Comparing `fetchify-1.1.6.tar` & `fetchify-1.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 15:21:05.084965 fetchify-1.1.6/
--rw-rw-rw-   0        0        0      594 2023-05-27 15:21:05.083959 fetchify-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-05-19 11:17:31.000000 fetchify-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 15:21:05.080596 fetchify-1.1.6/fetchify.egg-info/
--rw-rw-rw-   0        0        0      594 2023-05-27 15:21:04.000000 fetchify-1.1.6/fetchify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-27 15:21:04.000000 fetchify-1.1.6/fetchify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 15:21:04.000000 fetchify-1.1.6/fetchify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 15:21:04.000000 fetchify-1.1.6/fetchify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 15:21:04.000000 fetchify-1.1.6/fetchify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      898 2023-05-27 15:20:35.000000 fetchify-1.1.6/fetchify.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 fetchify-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 15:21:05.085962 fetchify-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-05-27 15:20:45.000000 fetchify-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 15:26:03.226784 fetchify-1.1.7/
+-rw-rw-rw-   0        0        0      594 2023-05-27 15:26:03.106735 fetchify-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-05-19 11:17:31.000000 fetchify-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 15:26:03.104733 fetchify-1.1.7/fetchify.egg-info/
+-rw-rw-rw-   0        0        0      594 2023-05-27 15:26:02.000000 fetchify-1.1.7/fetchify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-27 15:26:02.000000 fetchify-1.1.7/fetchify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 15:26:02.000000 fetchify-1.1.7/fetchify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 15:26:02.000000 fetchify-1.1.7/fetchify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 15:26:02.000000 fetchify-1.1.7/fetchify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      899 2023-05-27 15:25:30.000000 fetchify-1.1.7/fetchify.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 fetchify-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 15:26:03.226784 fetchify-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-05-27 15:25:44.000000 fetchify-1.1.7/setup.py
```

### Comparing `fetchify-1.1.6/PKG-INFO` & `fetchify-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.1.6
+Version: 1.1.7
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.1.6/fetchify.egg-info/PKG-INFO` & `fetchify-1.1.7/fetchify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.1.6
+Version: 1.1.7
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.1.6/fetchify.py` & `fetchify-1.1.7/fetchify.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import requests
 url = {
     "py" : "https://raw.githubusercontent.com/Anupam1707/Python_Programmes/main/",
     "we" : "https://raw.githubusercontent.com/Anupam1707/weather-app-py/main/",
     "aiu" : "https://raw.githubusercontent.com/Anupam1707/ai/main/",
     "ds" : "https://raw.githubusercontent.com/Anupam1707/datasense/main/",
-    "spy" : "https://raw.githubusercontent.com/Anupam1707/SecuriPy/main/"
+    "spy" : "https://raw.githubusercontent.com/Anupam1707/SecuriPy/main/",
     "docs" : "https://raw.githubusercontent.com/Anupam1707/docs/main/"
 }
 
 def fetch(filename, code, image = False):
     page = requests.get(url[code] + filename)
     if image == False:
         return page.text
```

### Comparing `fetchify-1.1.6/setup.py` & `fetchify-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fetchify",
-    version="1.1.6",
+    version="1.1.7",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Library to access Code Files from Cloud",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://techinfoak.wixsite.com/tech-info",
     project_urls={
```

