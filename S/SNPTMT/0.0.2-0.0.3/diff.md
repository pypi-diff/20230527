# Comparing `tmp/SNPTMT-0.0.2.tar.gz` & `tmp/SNPTMT-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SNPTMT-0.0.2.tar", last modified: Sat May 27 08:36:52 2023, max compression
+gzip compressed data, was "SNPTMT-0.0.3.tar", last modified: Sat May 27 08:38:23 2023, max compression
```

## Comparing `SNPTMT-0.0.2.tar` & `SNPTMT-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:36:52.406753 SNPTMT-0.0.2/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-26 21:11:36.000000 SNPTMT-0.0.2/LICENSE
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:36:52.406850 SNPTMT-0.0.2/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.2/README.md
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:36:52.406114 SNPTMT-0.0.2/SNPTMT.egg-info/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:36:52.000000 SNPTMT-0.0.2/SNPTMT.egg-info/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      314 2023-05-27 08:36:52.000000 SNPTMT-0.0.2/SNPTMT.egg-info/SOURCES.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-27 08:36:52.000000 SNPTMT-0.0.2/SNPTMT.egg-info/dependency_links.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-27 08:36:52.000000 SNPTMT-0.0.2/SNPTMT.egg-info/top_level.txt
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:36:52.406409 SNPTMT-0.0.2/package/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:27:58.000000 SNPTMT-0.0.2/package/__init__.py
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     8691 2023-05-26 21:11:38.000000 SNPTMT-0.0.2/package/snptmt.py
--rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-27 08:36:52.407162 SNPTMT-0.0.2/setup.cfg
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-27 08:36:20.000000 SNPTMT-0.0.2/setup.py
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:38:23.412735 SNPTMT-0.0.3/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-27 08:38:07.000000 SNPTMT-0.0.3/LICENSE
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:38:23.412808 SNPTMT-0.0.3/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.3/README.md
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:38:23.412079 SNPTMT-0.0.3/SNPTMT.egg-info/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:38:23.000000 SNPTMT-0.0.3/SNPTMT.egg-info/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      314 2023-05-27 08:38:23.000000 SNPTMT-0.0.3/SNPTMT.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-27 08:38:23.000000 SNPTMT-0.0.3/SNPTMT.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-27 08:38:23.000000 SNPTMT-0.0.3/SNPTMT.egg-info/top_level.txt
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:38:23.412402 SNPTMT-0.0.3/package/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      439 2023-05-27 08:38:04.000000 SNPTMT-0.0.3/package/__init__.py
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     8691 2023-05-27 08:38:05.000000 SNPTMT-0.0.3/package/snptmt.py
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-27 08:38:23.413071 SNPTMT-0.0.3/setup.cfg
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-27 08:37:59.000000 SNPTMT-0.0.3/setup.py
```

### Comparing `SNPTMT-0.0.2/LICENSE` & `SNPTMT-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SNPTMT-0.0.2/PKG-INFO` & `SNPTMT-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.2/SNPTMT.egg-info/PKG-INFO` & `SNPTMT-0.0.3/SNPTMT.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.2/package/snptmt.py` & `SNPTMT-0.0.3/package/snptmt.py`

 * *Files identical despite different names*

### Comparing `SNPTMT-0.0.2/setup.py` & `SNPTMT-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
-version = '0.0.2'
+version = '0.0.3'
 
 setup(
     name='SNPTMT',
     version=version,
 
     author='FIvER4IK',
     author_email='andrewshatalov3@gmail.com',
```

