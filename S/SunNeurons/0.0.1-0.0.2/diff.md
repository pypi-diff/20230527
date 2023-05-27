# Comparing `tmp/SunNeurons-0.0.1.tar.gz` & `tmp/SunNeurons-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SunNeurons-0.0.1.tar", last modified: Sat May 27 09:43:43 2023, max compression
+gzip compressed data, was "SunNeurons-0.0.2.tar", last modified: Sat May 27 10:02:43 2023, max compression
```

## Comparing `SunNeurons-0.0.1.tar` & `SunNeurons-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 09:43:43.465345 SunNeurons-0.0.1/
--rw-rw-rw-   0        0        0      613 2023-05-27 09:43:43.465345 SunNeurons-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-27 09:43:43.369325 SunNeurons-0.0.1/SunNeurons/
--rw-rw-rw-   0        0        0    23117 2023-05-27 09:39:47.000000 SunNeurons-0.0.1/SunNeurons/Fill.py
--rw-rw-rw-   0        0        0    18647 2023-05-27 09:12:33.000000 SunNeurons-0.0.1/SunNeurons/SunNeurons.py
--rw-rw-rw-   0        0        0      100 2023-05-27 09:12:33.000000 SunNeurons-0.0.1/SunNeurons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 09:43:43.457345 SunNeurons-0.0.1/SunNeurons.egg-info/
--rw-rw-rw-   0        0        0      613 2023-05-27 09:43:43.000000 SunNeurons-0.0.1/SunNeurons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-27 09:43:43.000000 SunNeurons-0.0.1/SunNeurons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:43:43.000000 SunNeurons-0.0.1/SunNeurons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-27 09:43:43.000000 SunNeurons-0.0.1/SunNeurons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-27 09:43:43.000000 SunNeurons-0.0.1/SunNeurons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 09:43:43.465345 SunNeurons-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      799 2023-05-27 09:43:09.000000 SunNeurons-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:02:43.642348 SunNeurons-0.0.2/
+-rw-rw-rw-   0        0        0      613 2023-05-27 10:02:43.640348 SunNeurons-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-27 10:02:43.614344 SunNeurons-0.0.2/SunNeurons/
+-rw-rw-rw-   0        0        0    23117 2023-05-27 09:39:47.000000 SunNeurons-0.0.2/SunNeurons/Fill.py
+-rw-rw-rw-   0        0        0    18647 2023-05-27 09:12:33.000000 SunNeurons-0.0.2/SunNeurons/SunNeurons.py
+-rw-rw-rw-   0        0        0       70 2023-05-27 10:02:15.000000 SunNeurons-0.0.2/SunNeurons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:02:43.638347 SunNeurons-0.0.2/SunNeurons.egg-info/
+-rw-rw-rw-   0        0        0      613 2023-05-27 10:02:43.000000 SunNeurons-0.0.2/SunNeurons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-27 10:02:43.000000 SunNeurons-0.0.2/SunNeurons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 10:02:43.000000 SunNeurons-0.0.2/SunNeurons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-27 10:02:43.000000 SunNeurons-0.0.2/SunNeurons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-27 10:02:43.000000 SunNeurons-0.0.2/SunNeurons.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 10:02:43.643349 SunNeurons-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      799 2023-05-27 10:02:12.000000 SunNeurons-0.0.2/setup.py
```

### Comparing `SunNeurons-0.0.1/PKG-INFO` & `SunNeurons-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SunNeurons
-Version: 0.0.1
+Version: 0.0.2
 Summary: SunNeurons
 Home-page: UNKNOWN
 Author: Sunny Kumar
 Author-email: <1709krsunny@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,neural networks,ann,mcculloh-pitt,ART neural network
```

### Comparing `SunNeurons-0.0.1/SunNeurons/Fill.py` & `SunNeurons-0.0.2/SunNeurons/Fill.py`

 * *Files identical despite different names*

### Comparing `SunNeurons-0.0.1/SunNeurons/SunNeurons.py` & `SunNeurons-0.0.2/SunNeurons/SunNeurons.py`

 * *Files identical despite different names*

### Comparing `SunNeurons-0.0.1/SunNeurons.egg-info/PKG-INFO` & `SunNeurons-0.0.2/SunNeurons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SunNeurons
-Version: 0.0.1
+Version: 0.0.2
 Summary: SunNeurons
 Home-page: UNKNOWN
 Author: Sunny Kumar
 Author-email: <1709krsunny@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,neural networks,ann,mcculloh-pitt,ART neural network
```

### Comparing `SunNeurons-0.0.1/setup.py` & `SunNeurons-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'SunNeurons'
  
 # Setting up
 setup(
     name="SunNeurons",
     version=VERSION,
     author="Sunny Kumar",
```

