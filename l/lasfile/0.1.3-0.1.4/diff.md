# Comparing `tmp/lasfile-0.1.3.tar.gz` & `tmp/lasfile-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasfile-0.1.3.tar", last modified: Sat May 27 02:48:22 2023, max compression
+gzip compressed data, was "lasfile-0.1.4.tar", last modified: Sat May 27 02:53:37 2023, max compression
```

## Comparing `lasfile-0.1.3.tar` & `lasfile-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 02:48:22.250716 lasfile-0.1.3/
--rw-rw-rw-   0        0        0     1084 2023-05-26 16:29:05.000000 lasfile-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       50 2023-05-26 18:15:21.000000 lasfile-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      612 2023-05-27 02:48:22.249712 lasfile-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-26 16:53:53.000000 lasfile-0.1.3/README.md
--rw-rw-rw-   0        0        0      501 2023-05-27 02:47:45.000000 lasfile-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 02:48:22.251712 lasfile-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 02:48:22.230712 lasfile-0.1.3/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 18:07:33.000000 lasfile-0.1.3/src/__init__.py
--rw-rw-rw-   0        0        0     3778 2023-02-14 02:36:37.000000 lasfile-0.1.3/src/known_sections.json
-drwxrwxrwx   0        0        0        0 2023-05-27 02:48:22.247716 lasfile-0.1.3/src/lasfile.egg-info/
--rw-rw-rw-   0        0        0      612 2023-05-27 02:48:22.000000 lasfile-0.1.3/src/lasfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-05-27 02:48:22.000000 lasfile-0.1.3/src/lasfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 02:48:22.000000 lasfile-0.1.3/src/lasfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-27 02:48:22.000000 lasfile-0.1.3/src/lasfile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-05-27 02:48:22.000000 lasfile-0.1.3/src/lasfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-27 02:48:22.000000 lasfile-0.1.3/src/lasfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    51784 2023-05-27 02:46:59.000000 lasfile-0.1.3/src/lasfile.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:53:37.892836 lasfile-0.1.4/
+-rw-rw-rw-   0        0        0     1084 2023-05-26 16:29:05.000000 lasfile-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-05-26 18:15:21.000000 lasfile-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      612 2023-05-27 02:53:37.891837 lasfile-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-26 16:53:53.000000 lasfile-0.1.4/README.md
+-rw-rw-rw-   0        0        0      501 2023-05-27 02:52:53.000000 lasfile-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 02:53:37.892836 lasfile-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 02:53:37.871836 lasfile-0.1.4/src/
+-rw-rw-rw-   0        0        0        0 2023-05-26 18:07:33.000000 lasfile-0.1.4/src/__init__.py
+-rw-rw-rw-   0        0        0     3778 2023-02-14 02:36:37.000000 lasfile-0.1.4/src/known_sections.json
+drwxrwxrwx   0        0        0        0 2023-05-27 02:53:37.890836 lasfile-0.1.4/src/lasfile.egg-info/
+-rw-rw-rw-   0        0        0      612 2023-05-27 02:53:37.000000 lasfile-0.1.4/src/lasfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-05-27 02:53:37.000000 lasfile-0.1.4/src/lasfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 02:53:37.000000 lasfile-0.1.4/src/lasfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-27 02:53:37.000000 lasfile-0.1.4/src/lasfile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-05-27 02:53:37.000000 lasfile-0.1.4/src/lasfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-27 02:53:37.000000 lasfile-0.1.4/src/lasfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    51764 2023-05-27 02:52:11.000000 lasfile-0.1.4/src/lasfile.py
```

### Comparing `lasfile-0.1.3/LICENSE` & `lasfile-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lasfile-0.1.3/PKG-INFO` & `lasfile-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasfile
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for reading LAS files.
 Project-URL: homepage, https://github.com/bzlmnop/lasfile
 Keywords: las,CWLS,las logs,petrophysical logs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lasfile-0.1.3/src/known_sections.json` & `lasfile-0.1.4/src/known_sections.json`

 * *Files identical despite different names*

### Comparing `lasfile-0.1.3/src/lasfile.egg-info/PKG-INFO` & `lasfile-0.1.4/src/lasfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasfile
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for reading LAS files.
 Project-URL: homepage, https://github.com/bzlmnop/lasfile
 Keywords: las,CWLS,las logs,petrophysical logs
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lasfile-0.1.3/src/lasfile.py` & `lasfile-0.1.4/src/lasfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import re
 import traceback
 from io import StringIO
 from numpy import genfromtxt
 from pandas import DataFrame
 import json
 from os import path
-import importlib.resources
+from pkgutil import get_data
 
 # Set known versions
 known_versions = ['1.2','2.0','3.0']
 
 # Get the path to the known sections json file
-known_sections_path = importlib.resources.open_text("lasfile", "known_sections.json")
+known_sections_path = get_data('lasfile','known_sections.json')
 # Load known sections from json file
 known_sections = json.load(open(known_sections_path,'r'))
 
 def get_version_num(data,handle_common_errors=True,accept_unknown_versions=False,allow_non_numeric=False):
     """
     Extracts and validates the version number from the given data.
```

