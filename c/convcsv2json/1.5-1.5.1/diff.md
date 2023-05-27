# Comparing `tmp/convcsv2json-1.5.tar.gz` & `tmp/convcsv2json-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convcsv2json-1.5.tar", last modified: Sat May 27 10:30:17 2023, max compression
+gzip compressed data, was "convcsv2json-1.5.1.tar", last modified: Sat May 27 10:35:38 2023, max compression
```

## Comparing `convcsv2json-1.5.tar` & `convcsv2json-1.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 kewl      (1000) kewl      (1000)        0 2023-05-27 10:30:17.051752 convcsv2json-1.5/
--rw-rw-r--   0 kewl      (1000) kewl      (1000)    35149 2023-05-27 10:20:35.000000 convcsv2json-1.5/LICENSE
--rw-rw-r--   0 kewl      (1000) kewl      (1000)     1442 2023-05-27 10:30:17.051752 convcsv2json-1.5/PKG-INFO
--rw-rw-r--   0 kewl      (1000) kewl      (1000)      857 2023-05-27 10:20:35.000000 convcsv2json-1.5/README.md
-drwxrwxr-x   0 kewl      (1000) kewl      (1000)        0 2023-05-27 10:30:17.051752 convcsv2json-1.5/convcsv2json/
--rw-rw-r--   0 kewl      (1000) kewl      (1000)     1160 2023-05-27 10:20:35.000000 convcsv2json-1.5/convcsv2json/__init__.py
-drwxrwxr-x   0 kewl      (1000) kewl      (1000)        0 2023-05-27 10:30:17.051752 convcsv2json-1.5/convcsv2json.egg-info/
--rw-rw-r--   0 kewl      (1000) kewl      (1000)     1442 2023-05-27 10:30:17.000000 convcsv2json-1.5/convcsv2json.egg-info/PKG-INFO
--rw-rw-r--   0 kewl      (1000) kewl      (1000)      195 2023-05-27 10:30:17.000000 convcsv2json-1.5/convcsv2json.egg-info/SOURCES.txt
--rw-rw-r--   0 kewl      (1000) kewl      (1000)        1 2023-05-27 10:30:17.000000 convcsv2json-1.5/convcsv2json.egg-info/dependency_links.txt
--rw-rw-r--   0 kewl      (1000) kewl      (1000)       13 2023-05-27 10:30:17.000000 convcsv2json-1.5/convcsv2json.egg-info/top_level.txt
--rw-rw-r--   0 kewl      (1000) kewl      (1000)       38 2023-05-27 10:30:17.051752 convcsv2json-1.5/setup.cfg
--rw-rw-r--   0 kewl      (1000) kewl      (1000)      740 2023-05-27 10:23:24.000000 convcsv2json-1.5/setup.py
+drwxrwxr-x   0 kewl      (1000) kewl      (1000)        0 2023-05-27 10:35:38.566383 convcsv2json-1.5.1/
+-rw-rw-r--   0 kewl      (1000) kewl      (1000)    35149 2023-05-27 10:20:35.000000 convcsv2json-1.5.1/LICENSE
+-rw-rw-r--   0 kewl      (1000) kewl      (1000)     1447 2023-05-27 10:35:38.566383 convcsv2json-1.5.1/PKG-INFO
+-rw-rw-r--   0 kewl      (1000) kewl      (1000)      860 2023-05-27 10:34:31.000000 convcsv2json-1.5.1/README.md
+drwxrwxr-x   0 kewl      (1000) kewl      (1000)        0 2023-05-27 10:35:38.566383 convcsv2json-1.5.1/convcsv2json/
+-rw-rw-r--   0 kewl      (1000) kewl      (1000)     1160 2023-05-27 10:20:35.000000 convcsv2json-1.5.1/convcsv2json/__init__.py
+drwxrwxr-x   0 kewl      (1000) kewl      (1000)        0 2023-05-27 10:35:38.566383 convcsv2json-1.5.1/convcsv2json.egg-info/
+-rw-rw-r--   0 kewl      (1000) kewl      (1000)     1447 2023-05-27 10:35:38.000000 convcsv2json-1.5.1/convcsv2json.egg-info/PKG-INFO
+-rw-rw-r--   0 kewl      (1000) kewl      (1000)      195 2023-05-27 10:35:38.000000 convcsv2json-1.5.1/convcsv2json.egg-info/SOURCES.txt
+-rw-rw-r--   0 kewl      (1000) kewl      (1000)        1 2023-05-27 10:35:38.000000 convcsv2json-1.5.1/convcsv2json.egg-info/dependency_links.txt
+-rw-rw-r--   0 kewl      (1000) kewl      (1000)       13 2023-05-27 10:35:38.000000 convcsv2json-1.5.1/convcsv2json.egg-info/top_level.txt
+-rw-rw-r--   0 kewl      (1000) kewl      (1000)       38 2023-05-27 10:35:38.566383 convcsv2json-1.5.1/setup.cfg
+-rw-rw-r--   0 kewl      (1000) kewl      (1000)      742 2023-05-27 10:35:29.000000 convcsv2json-1.5.1/setup.py
```

### Comparing `convcsv2json-1.5/LICENSE` & `convcsv2json-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `convcsv2json-1.5/PKG-INFO` & `convcsv2json-1.5.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convcsv2json
-Version: 1.5
+Version: 1.5.1
 Summary: Convert a CSV file into JSON format based on CSV headers
 Home-page: https://github.com/1337kid/convcsv2json
 Author: 1337kid
 Author-email: 1337kid@proton.me
 License: UNKNOWN
 Project-URL: Source, https://github.com/1337kid/convcsv2json
 Platform: UNKNOWN
@@ -43,18 +43,18 @@
 kewldog,12
 kewlcat,23
 ```
 ### Generated JSON
 ```json
 [
     {
-        "name": "kewl",
-        "age": "344"
+        "name": "kewldog",
+        "age": "12"
     },
     {
-        "name": "noice",
-        "age": "456"
+        "name": "kewlcat",
+        "age": "23"
     }
 ]
 ```
```

### Comparing `convcsv2json-1.5/README.md` & `convcsv2json-1.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 kewldog,12
 kewlcat,23
 ```
 ### Generated JSON
 ```json
 [
     {
-        "name": "kewl",
-        "age": "344"
+        "name": "kewldog",
+        "age": "12"
     },
     {
-        "name": "noice",
-        "age": "456"
+        "name": "kewlcat",
+        "age": "23"
     }
 ]
 ```
```

### Comparing `convcsv2json-1.5/convcsv2json/__init__.py` & `convcsv2json-1.5.1/convcsv2json/__init__.py`

 * *Files identical despite different names*

### Comparing `convcsv2json-1.5/convcsv2json.egg-info/PKG-INFO` & `convcsv2json-1.5.1/convcsv2json.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convcsv2json
-Version: 1.5
+Version: 1.5.1
 Summary: Convert a CSV file into JSON format based on CSV headers
 Home-page: https://github.com/1337kid/convcsv2json
 Author: 1337kid
 Author-email: 1337kid@proton.me
 License: UNKNOWN
 Project-URL: Source, https://github.com/1337kid/convcsv2json
 Platform: UNKNOWN
@@ -43,18 +43,18 @@
 kewldog,12
 kewlcat,23
 ```
 ### Generated JSON
 ```json
 [
     {
-        "name": "kewl",
-        "age": "344"
+        "name": "kewldog",
+        "age": "12"
     },
     {
-        "name": "noice",
-        "age": "456"
+        "name": "kewlcat",
+        "age": "23"
     }
 ]
 ```
```

### Comparing `convcsv2json-1.5/setup.py` & `convcsv2json-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name = "convcsv2json",
-    version = "1.5",
+    version = "1.5.1",
     author = "1337kid",
     author_email = "1337kid@proton.me",
     description = "Convert a CSV file into JSON format based on CSV headers",
     long_description = open('README.md').read()  ,
     long_description_content_type = "text/markdown",
     url = "https://github.com/1337kid/convcsv2json",
     project_urls = {'Source': 'https://github.com/1337kid/convcsv2json',},
```

