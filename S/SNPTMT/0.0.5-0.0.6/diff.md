# Comparing `tmp/SNPTMT-0.0.5.tar.gz` & `tmp/SNPTMT-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SNPTMT-0.0.5.tar", last modified: Sat May 27 08:55:46 2023, max compression
+gzip compressed data, was "SNPTMT-0.0.6.tar", last modified: Sat May 27 08:59:38 2023, max compression
```

## Comparing `SNPTMT-0.0.5.tar` & `SNPTMT-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:55:46.366066 SNPTMT-0.0.5/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-27 08:38:07.000000 SNPTMT-0.0.5/LICENSE
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:55:46.366139 SNPTMT-0.0.5/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.5/README.md
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:55:46.365051 SNPTMT-0.0.5/SNPTMT/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      518 2023-05-27 08:55:13.000000 SNPTMT-0.0.5/SNPTMT/__init__.py
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     8692 2023-05-27 08:55:15.000000 SNPTMT-0.0.5/SNPTMT/snptmt.py
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:55:46.365719 SNPTMT-0.0.5/SNPTMT.egg-info/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:55:46.000000 SNPTMT-0.0.5/SNPTMT.egg-info/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      312 2023-05-27 08:55:46.000000 SNPTMT-0.0.5/SNPTMT.egg-info/SOURCES.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-27 08:55:46.000000 SNPTMT-0.0.5/SNPTMT.egg-info/dependency_links.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        7 2023-05-27 08:55:46.000000 SNPTMT-0.0.5/SNPTMT.egg-info/top_level.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-27 08:55:46.366407 SNPTMT-0.0.5/setup.cfg
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-27 08:55:23.000000 SNPTMT-0.0.5/setup.py
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:59:38.683927 SNPTMT-0.0.6/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-27 08:38:07.000000 SNPTMT-0.0.6/LICENSE
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:59:38.684007 SNPTMT-0.0.6/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.6/README.md
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:59:38.682875 SNPTMT-0.0.6/SNPTMT/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      332 2023-05-27 08:58:59.000000 SNPTMT-0.0.6/SNPTMT/__init__.py
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     8692 2023-05-27 08:55:15.000000 SNPTMT-0.0.6/SNPTMT/snptmt.py
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:59:38.683567 SNPTMT-0.0.6/SNPTMT.egg-info/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:59:38.000000 SNPTMT-0.0.6/SNPTMT.egg-info/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      312 2023-05-27 08:59:38.000000 SNPTMT-0.0.6/SNPTMT.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-27 08:59:38.000000 SNPTMT-0.0.6/SNPTMT.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        7 2023-05-27 08:59:38.000000 SNPTMT-0.0.6/SNPTMT.egg-info/top_level.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-27 08:59:38.684279 SNPTMT-0.0.6/setup.cfg
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-27 08:59:26.000000 SNPTMT-0.0.6/setup.py
```

### Comparing `SNPTMT-0.0.5/LICENSE` & `SNPTMT-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SNPTMT-0.0.5/PKG-INFO` & `SNPTMT-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.5/SNPTMT/snptmt.py` & `SNPTMT-0.0.6/SNPTMT/snptmt.py`

 * *Files identical despite different names*

### Comparing `SNPTMT-0.0.5/SNPTMT.egg-info/PKG-INFO` & `SNPTMT-0.0.6/SNPTMT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.5/setup.py` & `SNPTMT-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
-version = '0.0.5'
+version = '0.0.6'
 
 setup(
     name='SNPTMT',
     version=version,
 
     author='FIvER4IK',
     author_email='andrewshatalov3@gmail.com',
```

