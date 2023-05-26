# Comparing `tmp/wtisdk-1.3.tar.gz` & `tmp/wtisdk-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtisdk-1.3.tar", last modified: Fri May 26 21:31:24 2023, max compression
+gzip compressed data, was "wtisdk-1.4.tar", last modified: Fri May 26 22:50:11 2023, max compression
```

## Comparing `wtisdk-1.3.tar` & `wtisdk-1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:31:24.577357 wtisdk-1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 21:31:15.000000 wtisdk-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-26 21:31:24.577357 wtisdk-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-26 21:31:15.000000 wtisdk-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:31:24.581357 wtisdk-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-26 21:31:15.000000 wtisdk-1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:31:24.577357 wtisdk-1.3/wtisdk/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 21:31:15.000000 wtisdk-1.3/wtisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:31:24.577357 wtisdk-1.3/wtisdk/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:31:15.000000 wtisdk-1.3/wtisdk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 21:31:15.000000 wtisdk-1.3/wtisdk/tests/test_wtisdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    37138 2023-05-26 21:31:15.000000 wtisdk-1.3/wtisdk/wtisdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:31:24.577357 wtisdk-1.3/wtisdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-26 21:31:24.000000 wtisdk-1.3/wtisdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 21:31:24.000000 wtisdk-1.3/wtisdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:31:24.000000 wtisdk-1.3/wtisdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 21:31:24.000000 wtisdk-1.3/wtisdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 21:31:24.000000 wtisdk-1.3/wtisdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:50:10.997582 wtisdk-1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 22:50:00.000000 wtisdk-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-26 22:50:10.997582 wtisdk-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-05-26 22:50:00.000000 wtisdk-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 22:50:10.997582 wtisdk-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-26 22:50:00.000000 wtisdk-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:50:10.993581 wtisdk-1.4/wtisdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 22:50:00.000000 wtisdk-1.4/wtisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:50:10.993581 wtisdk-1.4/wtisdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 22:50:00.000000 wtisdk-1.4/wtisdk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 22:50:00.000000 wtisdk-1.4/wtisdk/tests/test_wtisdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37138 2023-05-26 22:50:00.000000 wtisdk-1.4/wtisdk/wtisdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:50:10.993581 wtisdk-1.4/wtisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-26 22:50:10.000000 wtisdk-1.4/wtisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 22:50:10.000000 wtisdk-1.4/wtisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 22:50:10.000000 wtisdk-1.4/wtisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 22:50:10.000000 wtisdk-1.4/wtisdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 22:50:10.000000 wtisdk-1.4/wtisdk.egg-info/top_level.txt
```

### Comparing `wtisdk-1.3/LICENSE` & `wtisdk-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wtisdk-1.3/PKG-INFO` & `wtisdk-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.3
+Version: 1.4
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wtisdk-1.3/setup.py` & `wtisdk-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wtisdk',
-    version='1.3',
+    version='1.4',
     author='Melih Teke',
     author_email='me@mteke.com',
     description='WTI SDK for interacting with WTI devices',
     long_description='''
                         WTI SDK: Python SDK for interacting with WTI devices
 
                         The WTI SDK is a powerful Python library that enables developers to easily interact with WTI devices, providing a comprehensive set of functions for managing and controlling operational and configuration aspects.
```

### Comparing `wtisdk-1.3/wtisdk/tests/test_wtisdk.py` & `wtisdk-1.4/wtisdk/tests/test_wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.3/wtisdk/wtisdk.py` & `wtisdk-1.4/wtisdk/wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.3/wtisdk.egg-info/PKG-INFO` & `wtisdk-1.4/wtisdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.3
+Version: 1.4
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

