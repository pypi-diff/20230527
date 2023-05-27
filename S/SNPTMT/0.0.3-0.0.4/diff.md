# Comparing `tmp/SNPTMT-0.0.3.tar.gz` & `tmp/SNPTMT-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SNPTMT-0.0.3.tar", last modified: Sat May 27 08:38:23 2023, max compression
+gzip compressed data, was "SNPTMT-0.0.4.tar", last modified: Sat May 27 08:50:09 2023, max compression
```

## Comparing `SNPTMT-0.0.3.tar` & `SNPTMT-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:38:23.412735 SNPTMT-0.0.3/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-27 08:38:07.000000 SNPTMT-0.0.3/LICENSE
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:38:23.412808 SNPTMT-0.0.3/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.3/README.md
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:38:23.412079 SNPTMT-0.0.3/SNPTMT.egg-info/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:38:23.000000 SNPTMT-0.0.3/SNPTMT.egg-info/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      314 2023-05-27 08:38:23.000000 SNPTMT-0.0.3/SNPTMT.egg-info/SOURCES.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-27 08:38:23.000000 SNPTMT-0.0.3/SNPTMT.egg-info/dependency_links.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-27 08:38:23.000000 SNPTMT-0.0.3/SNPTMT.egg-info/top_level.txt
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:38:23.412402 SNPTMT-0.0.3/package/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      439 2023-05-27 08:38:04.000000 SNPTMT-0.0.3/package/__init__.py
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     8691 2023-05-27 08:38:05.000000 SNPTMT-0.0.3/package/snptmt.py
--rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-27 08:38:23.413071 SNPTMT-0.0.3/setup.cfg
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-27 08:37:59.000000 SNPTMT-0.0.3/setup.py
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:50:09.474051 SNPTMT-0.0.4/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-27 08:38:07.000000 SNPTMT-0.0.4/LICENSE
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:50:09.474127 SNPTMT-0.0.4/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.4/README.md
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:50:09.473059 SNPTMT-0.0.4/SNPTMT/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      439 2023-05-27 08:38:04.000000 SNPTMT-0.0.4/SNPTMT/__init__.py
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     8692 2023-05-27 08:47:59.000000 SNPTMT-0.0.4/SNPTMT/snptmt.py
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:50:09.473727 SNPTMT-0.0.4/SNPTMT.egg-info/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:50:09.000000 SNPTMT-0.0.4/SNPTMT.egg-info/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      312 2023-05-27 08:50:09.000000 SNPTMT-0.0.4/SNPTMT.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-27 08:50:09.000000 SNPTMT-0.0.4/SNPTMT.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        7 2023-05-27 08:50:09.000000 SNPTMT-0.0.4/SNPTMT.egg-info/top_level.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-27 08:50:09.474391 SNPTMT-0.0.4/setup.cfg
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-27 08:46:39.000000 SNPTMT-0.0.4/setup.py
```

### Comparing `SNPTMT-0.0.3/LICENSE` & `SNPTMT-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SNPTMT-0.0.3/PKG-INFO` & `SNPTMT-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.3/SNPTMT.egg-info/PKG-INFO` & `SNPTMT-0.0.4/SNPTMT.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.3/package/snptmt.py` & `SNPTMT-0.0.4/SNPTMT/snptmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,7 +251,8 @@
     return cluster_dict, updated_cluster_counters
 
 
 
 def initialize_cluster_counters(cluster_dict):
     cluster_counters = {cluster_id: 1 for cluster_id in cluster_dict}
     return cluster_counters
+
```

### Comparing `SNPTMT-0.0.3/setup.py` & `SNPTMT-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
-version = '0.0.3'
+version = '0.0.4'
 
 setup(
     name='SNPTMT',
     version=version,
 
     author='FIvER4IK',
     author_email='andrewshatalov3@gmail.com',
```

