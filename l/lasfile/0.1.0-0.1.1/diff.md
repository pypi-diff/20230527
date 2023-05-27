# Comparing `tmp/lasfile-0.1.0.tar.gz` & `tmp/lasfile-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasfile-0.1.0.tar", last modified: Sat May 27 01:39:27 2023, max compression
+gzip compressed data, was "lasfile-0.1.1.tar", last modified: Sat May 27 02:29:01 2023, max compression
```

## Comparing `lasfile-0.1.0.tar` & `lasfile-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 01:39:27.901308 lasfile-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-05-26 16:29:05.000000 lasfile-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       50 2023-05-26 18:15:21.000000 lasfile-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      612 2023-05-27 01:39:27.900308 lasfile-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-26 16:53:53.000000 lasfile-0.1.0/README.md
--rw-rw-rw-   0        0        0      501 2023-05-27 01:39:06.000000 lasfile-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 01:39:27.901308 lasfile-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 01:39:27.874308 lasfile-0.1.0/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 18:07:33.000000 lasfile-0.1.0/src/__init__.py
--rw-rw-rw-   0        0        0     3778 2023-02-14 02:36:37.000000 lasfile-0.1.0/src/known_sections.json
-drwxrwxrwx   0        0        0        0 2023-05-27 01:39:27.898306 lasfile-0.1.0/src/lasfile.egg-info/
--rw-rw-rw-   0        0        0      612 2023-05-27 01:39:27.000000 lasfile-0.1.0/src/lasfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-05-27 01:39:27.000000 lasfile-0.1.0/src/lasfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 01:39:27.000000 lasfile-0.1.0/src/lasfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-27 01:39:27.000000 lasfile-0.1.0/src/lasfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-05-27 01:39:27.000000 lasfile-0.1.0/src/lasfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-27 01:39:27.000000 lasfile-0.1.0/src/lasfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    51600 2023-05-26 16:47:33.000000 lasfile-0.1.0/src/lasfile.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:29:01.553236 lasfile-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-05-26 16:29:05.000000 lasfile-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-05-26 18:15:21.000000 lasfile-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      612 2023-05-27 02:29:01.552236 lasfile-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-26 16:53:53.000000 lasfile-0.1.1/README.md
+-rw-rw-rw-   0        0        0      501 2023-05-27 02:28:04.000000 lasfile-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 02:29:01.553236 lasfile-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 02:29:01.533233 lasfile-0.1.1/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 18:07:33.000000 lasfile-0.1.1/src/__init__.py
+-rw-rw-rw-   0        0        0     3778 2023-02-14 02:36:37.000000 lasfile-0.1.1/src/known_sections.json
+drwxrwxrwx   0        0        0        0 2023-05-27 02:29:01.551232 lasfile-0.1.1/src/lasfile.egg-info/
+-rw-rw-rw-   0        0        0      612 2023-05-27 02:29:01.000000 lasfile-0.1.1/src/lasfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-05-27 02:29:01.000000 lasfile-0.1.1/src/lasfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 02:29:01.000000 lasfile-0.1.1/src/lasfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-27 02:29:01.000000 lasfile-0.1.1/src/lasfile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-05-27 02:29:01.000000 lasfile-0.1.1/src/lasfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-27 02:29:01.000000 lasfile-0.1.1/src/lasfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    51748 2023-05-27 02:26:32.000000 lasfile-0.1.1/src/lasfile.py
```

### Comparing `lasfile-0.1.0/LICENSE` & `lasfile-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lasfile-0.1.0/PKG-INFO` & `lasfile-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasfile
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for reading LAS files.
 Project-URL: homepage, https://github.com/bzlmnop/lasfile
 Keywords: las,CWLS,las logs,petrophysical logs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lasfile-0.1.0/src/known_sections.json` & `lasfile-0.1.1/src/known_sections.json`

 * *Files identical despite different names*

### Comparing `lasfile-0.1.0/src/lasfile.egg-info/PKG-INFO` & `lasfile-0.1.1/src/lasfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasfile
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for reading LAS files.
 Project-URL: homepage, https://github.com/bzlmnop/lasfile
 Keywords: las,CWLS,las logs,petrophysical logs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lasfile-0.1.0/src/lasfile.py` & `lasfile-0.1.1/src/lasfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 
 import re
 import traceback
 from io import StringIO
 from numpy import genfromtxt
 from pandas import DataFrame
 import json
+from os import path
 
 # Set known versions
 known_versions = ['1.2','2.0','3.0']
+
+# Get the path to the known sections json file
+known_sections_path = path.join(path.dirname(__file__),"known_sections.json")
 # Load known sections from json file
-known_sections = json.load(open("known_sections.json",'r'))
+known_sections = json.load(open(known_sections_path,'r'))
 
 def get_version_num(data,handle_common_errors=True,accept_unknown_versions=False,allow_non_numeric=False):
     """
     Extracts and validates the version number from the given data.
 
     This function accepts either a string containing a version section, or a DataFrame containing a mnemonic column with a "VERS" value. It then tries to extract the version number and validate it. It handles several common errors, such as non-numeric versions, and allows the acceptance of unknown versions.
```

