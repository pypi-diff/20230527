# Comparing `tmp/betterdataclass-3.0.tar.gz` & `tmp/betterdataclass-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterdataclass-3.0.tar", last modified: Fri May 26 05:29:40 2023, max compression
+gzip compressed data, was "betterdataclass-3.1.tar", last modified: Sat May 27 10:22:59 2023, max compression
```

## Comparing `betterdataclass-3.0.tar` & `betterdataclass-3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:40.711869 betterdataclass-3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 05:29:25.000000 betterdataclass-3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-26 05:29:40.711869 betterdataclass-3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-26 05:29:25.000000 betterdataclass-3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:40.711869 betterdataclass-3.0/betterdataclass/
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/StrictDictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/StrictList.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:40.711869 betterdataclass-3.0/betterdataclass/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/helper/initiate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/helper/to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/helper/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/strictEnum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:40.711869 betterdataclass-3.0/betterdataclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-26 05:29:40.000000 betterdataclass-3.0/betterdataclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-26 05:29:40.000000 betterdataclass-3.0/betterdataclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 05:29:40.000000 betterdataclass-3.0/betterdataclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 05:29:40.000000 betterdataclass-3.0/betterdataclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 05:29:40.711869 betterdataclass-3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-26 05:29:25.000000 betterdataclass-3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:22:59.991408 betterdataclass-3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-27 10:22:46.000000 betterdataclass-3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-27 10:22:59.991408 betterdataclass-3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-27 10:22:46.000000 betterdataclass-3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:22:59.991408 betterdataclass-3.1/betterdataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-27 10:22:46.000000 betterdataclass-3.1/betterdataclass/StrictDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-27 10:22:46.000000 betterdataclass-3.1/betterdataclass/StrictList.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 10:22:46.000000 betterdataclass-3.1/betterdataclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:22:59.991408 betterdataclass-3.1/betterdataclass/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 10:22:46.000000 betterdataclass-3.1/betterdataclass/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-27 10:22:46.000000 betterdataclass-3.1/betterdataclass/helper/initiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-27 10:22:46.000000 betterdataclass-3.1/betterdataclass/helper/to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-27 10:22:46.000000 betterdataclass-3.1/betterdataclass/helper/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-27 10:22:46.000000 betterdataclass-3.1/betterdataclass/strictEnum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:22:59.991408 betterdataclass-3.1/betterdataclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-27 10:22:59.000000 betterdataclass-3.1/betterdataclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-27 10:22:59.000000 betterdataclass-3.1/betterdataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:22:59.000000 betterdataclass-3.1/betterdataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 10:22:59.000000 betterdataclass-3.1/betterdataclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 10:22:59.991408 betterdataclass-3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-27 10:22:46.000000 betterdataclass-3.1/setup.py
```

### Comparing `betterdataclass-3.0/LICENSE` & `betterdataclass-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.0/PKG-INFO` & `betterdataclass-3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterdataclass
-Version: 3.0
+Version: 3.1
 Summary: A multipurpose dataclass libarary used for validation and data structuring.
 Home-page: https://github.com/dvnasutosh/betterdataclasses
 Author: Asutosh Rath
 Author-email: dvnasutosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `betterdataclass-3.0/README.rst` & `betterdataclass-3.1/README.rst`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.0/betterdataclass/StrictDictionary.py` & `betterdataclass-3.1/betterdataclass/StrictDictionary.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.0/betterdataclass/StrictList.py` & `betterdataclass-3.1/betterdataclass/StrictList.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.0/betterdataclass/helper/initiate.py` & `betterdataclass-3.1/betterdataclass/helper/initiate.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.0/betterdataclass/helper/to_dict.py` & `betterdataclass-3.1/betterdataclass/helper/to_dict.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,44 @@
+from ast import Str
 from enum import Enum
 
+from betterdataclass import StrictDictionary
+
 
 def to_raw_dict(obj: object, processed=None):
     if processed is None:
         processed = set()
     if id(obj) in processed:
         return "<circular reference>"
     processed.add(id(obj))
     if isinstance(obj, dict):
         out = {}
         for key, value in obj.items():
-            if isinstance(value, dict):
+            if value is None:
+                out[key] = value
+            elif isinstance(value, dict):
                 out[key] = to_raw_dict(value, processed)
             elif isinstance(value, Enum):
                 out[key] = [str(value), value.value]
             elif isinstance(value, (list, tuple, set)):
                 out[key] = to_raw_dict(value, processed)
             elif isinstance(value, (int, float, bool, complex, str)):
                 out[key] = value
+            elif isinstance(value,StrictDictionary.StrictDictionary):
+                out[key] = to_raw_dict(value.__data__, processed)
             elif isinstance(value, object):
                 out[key] = to_raw_dict(value.__dict__, processed)
             else:
                 out[key] = str(value)
         return out
     elif isinstance(obj, (list, tuple, set)):
         return [to_raw_dict(item, processed) for item in obj]
     elif isinstance(obj, (int, float, bool, complex, str)):
         return obj
     elif isinstance(obj, Enum):
         return [str(value), value.value]
+    elif isinstance(value,StrictDictionary.StrictDictionary):
+        out[key] = to_raw_dict(value.__data__, processed)
     elif isinstance(obj, object):
         return to_raw_dict(obj.__dict__, processed)
     else:
         return str(obj)
```

### Comparing `betterdataclass-3.0/betterdataclass/helper/validate.py` & `betterdataclass-3.1/betterdataclass/helper/validate.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.0/betterdataclass.egg-info/PKG-INFO` & `betterdataclass-3.1/betterdataclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterdataclass
-Version: 3.0
+Version: 3.1
 Summary: A multipurpose dataclass libarary used for validation and data structuring.
 Home-page: https://github.com/dvnasutosh/betterdataclasses
 Author: Asutosh Rath
 Author-email: dvnasutosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `betterdataclass-3.0/setup.py` & `betterdataclass-3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 import setuptools
 
 
 setup(
     name="betterdataclass",
-    version="3.0",
+    version="3.01",
     description="A multipurpose dataclass libarary used for validation and data structuring.",
     long_description=open('./README.rst').read(),
     url='https://github.com/dvnasutosh/betterdataclasses',
     
     author="Asutosh Rath",
     author_email="dvnasutosh@gmail.com",
     packages=find_packages(),
```

