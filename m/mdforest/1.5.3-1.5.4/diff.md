# Comparing `tmp/mdforest-1.5.3.tar.gz` & `tmp/mdforest-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdforest-1.5.3.tar", last modified: Thu May 25 23:02:47 2023, max compression
+gzip compressed data, was "mdforest-1.5.4.tar", last modified: Fri May 26 02:57:14 2023, max compression
```

## Comparing `mdforest-1.5.3.tar` & `mdforest-1.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 23:02:47.014836 mdforest-1.5.3/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 02:15:26.000000 mdforest-1.5.3/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-25 23:02:47.014836 mdforest-1.5.3/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2592 2023-05-20 13:55:14.000000 mdforest-1.5.3/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 23:02:47.013836 mdforest-1.5.3/mdforest/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1292 2023-05-25 23:02:18.000000 mdforest-1.5.3/mdforest/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3255 2023-05-25 04:00:23.000000 mdforest-1.5.3/mdforest/mdforest.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 23:02:47.014836 mdforest-1.5.3/mdforest/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-19 02:13:23.000000 mdforest-1.5.3/mdforest/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3378 2023-05-25 03:54:31.000000 mdforest-1.5.3/mdforest/tree/types.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-19 02:13:23.000000 mdforest-1.5.3/mdforest/treebuild.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 23:02:47.013836 mdforest-1.5.3/mdforest.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-25 23:02:46.000000 mdforest-1.5.3/mdforest.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      335 2023-05-25 23:02:46.000000 mdforest-1.5.3/mdforest.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-25 23:02:46.000000 mdforest-1.5.3/mdforest.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-25 23:02:46.000000 mdforest-1.5.3/mdforest.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-25 23:02:46.000000 mdforest-1.5.3/mdforest.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 02:27:02.000000 mdforest-1.5.3/pyproject.toml
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-25 23:02:47.014836 mdforest-1.5.3/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      918 2023-05-25 23:02:45.000000 mdforest-1.5.3/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 23:02:47.014836 mdforest-1.5.3/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-05-19 02:13:23.000000 mdforest-1.5.3/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-26 02:57:14.184498 mdforest-1.5.4/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 02:15:26.000000 mdforest-1.5.4/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2996 2023-05-26 02:57:14.183498 mdforest-1.5.4/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2592 2023-05-20 13:55:14.000000 mdforest-1.5.4/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-26 02:57:14.180498 mdforest-1.5.4/mdforest/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1530 2023-05-26 02:30:49.000000 mdforest-1.5.4/mdforest/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3255 2023-05-25 04:00:23.000000 mdforest-1.5.4/mdforest/mdforest.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-26 02:57:14.182498 mdforest-1.5.4/mdforest/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-19 02:13:23.000000 mdforest-1.5.4/mdforest/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3378 2023-05-25 03:54:31.000000 mdforest-1.5.4/mdforest/tree/types.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-19 02:13:23.000000 mdforest-1.5.4/mdforest/treebuild.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-26 02:57:14.182498 mdforest-1.5.4/mdforest.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2996 2023-05-26 02:57:14.000000 mdforest-1.5.4/mdforest.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      335 2023-05-26 02:57:14.000000 mdforest-1.5.4/mdforest.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-26 02:57:14.000000 mdforest-1.5.4/mdforest.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-26 02:57:14.000000 mdforest-1.5.4/mdforest.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-26 02:57:14.000000 mdforest-1.5.4/mdforest.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 02:27:02.000000 mdforest-1.5.4/pyproject.toml
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-26 02:57:14.184498 mdforest-1.5.4/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      918 2023-05-26 02:29:21.000000 mdforest-1.5.4/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-26 02:57:14.183498 mdforest-1.5.4/tests/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-05-19 02:13:23.000000 mdforest-1.5.4/tests/test_mdtree.py
```

### Comparing `mdforest-1.5.3/LICENSE` & `mdforest-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.3/PKG-INFO` & `mdforest-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.5.3
+Version: 1.5.4
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/mdforest
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.4.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.3.zip
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 mdforest - Markdown Forest
 ==========================
 
 A library to convert Markdown documents into tree data structures and
@@ -109,9 +108,7 @@
 
 License
 -------
 
 The `original project <https://github.com/alvinwan/md2py>`__ was
 licensed under the Apache 2.0 License and a copy is provided in this
 repo as well. All the files changed are listed in the CHANGELOG.
-
-
```

### Comparing `mdforest-1.5.3/README.rst` & `mdforest-1.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.3/mdforest/__init__.py` & `mdforest-1.5.4/mdforest/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from bs4 import BeautifulSoup
 from .mdforest import *
 from .tree.types import *
 
 def treeify(name:str="[document]", md:str="", *args, **kwargs) -> MarkdownForest:
     """
     Converts markdown file to a Python object (MarkdownForest).
     """
@@ -15,18 +16,24 @@
     
     return mdtextify(tree, *args, **kwargs)
 
 def clean_markdown(md:str) -> str:
     """
     Cleans markdown file of bold and italics formatting.
     """
-    
+        
     # Remove the metadata
     _, markdown_text = find_metadata(md)
     
+     # Create a BeautifulSoup object with the input markdown text
+    soup = BeautifulSoup(markdown_text, 'html.parser')
+
+    # Remove HTML tags from the document
+    markdown_text = soup.get_text()
+    
     # Remove links
     markdown_text = re.sub(r'!\[(.*?)\]\((.*?)\)', '', markdown_text)
     markdown_text = re.sub(r'\[(.*?)\]\((.*?)\)', '', markdown_text)
     markdown_text = markdown_text.replace('>', '')
     
     # Remove bold and italics formatting
     markdown_text = re.sub(r'\*\*(.*?)\*\*', r'\1', markdown_text)
```

### Comparing `mdforest-1.5.3/mdforest/mdforest.py` & `mdforest-1.5.4/mdforest/mdforest.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.3/mdforest/tree/types.py` & `mdforest-1.5.4/mdforest/tree/types.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.3/mdforest/treebuild.py` & `mdforest-1.5.4/mdforest/treebuild.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.3/mdforest.egg-info/PKG-INFO` & `mdforest-1.5.4/mdforest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.5.3
+Version: 1.5.4
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/mdforest
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.4.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.3.zip
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 mdforest - Markdown Forest
 ==========================
 
 A library to convert Markdown documents into tree data structures and
@@ -109,9 +108,7 @@
 
 License
 -------
 
 The `original project <https://github.com/alvinwan/md2py>`__ was
 licensed under the Apache 2.0 License and a copy is provided in this
 repo as well. All the files changed are listed in the CHANGELOG.
-
-
```

### Comparing `mdforest-1.5.3/setup.py` & `mdforest-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '1.5.3'
+VERSION = '1.5.4'
 DESCRIPTION = 'A package to convert between Markdown and a forest data structure for efficient processing.'
 
 setup(
     name = "mdforest",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
```

### Comparing `mdforest-1.5.3/tests/test_mdtree.py` & `mdforest-1.5.4/tests/test_mdtree.py`

 * *Files identical despite different names*

