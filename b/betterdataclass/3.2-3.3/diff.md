# Comparing `tmp/betterdataclass-3.2.tar.gz` & `tmp/betterdataclass-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterdataclass-3.2.tar", last modified: Sat May 27 10:44:09 2023, max compression
+gzip compressed data, was "betterdataclass-3.3.tar", last modified: Sat May 27 12:48:23 2023, max compression
```

## Comparing `betterdataclass-3.2.tar` & `betterdataclass-3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:44:09.657407 betterdataclass-3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-27 10:43:54.000000 betterdataclass-3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-27 10:44:09.657407 betterdataclass-3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-27 10:43:54.000000 betterdataclass-3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:44:09.657407 betterdataclass-3.2/betterdataclass/
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-27 10:43:54.000000 betterdataclass-3.2/betterdataclass/StrictDictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-27 10:43:54.000000 betterdataclass-3.2/betterdataclass/StrictList.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 10:43:54.000000 betterdataclass-3.2/betterdataclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:44:09.657407 betterdataclass-3.2/betterdataclass/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 10:43:54.000000 betterdataclass-3.2/betterdataclass/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-27 10:43:54.000000 betterdataclass-3.2/betterdataclass/helper/initiate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-27 10:43:54.000000 betterdataclass-3.2/betterdataclass/helper/to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-27 10:43:54.000000 betterdataclass-3.2/betterdataclass/helper/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-27 10:43:54.000000 betterdataclass-3.2/betterdataclass/strictEnum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:44:09.657407 betterdataclass-3.2/betterdataclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-27 10:44:09.000000 betterdataclass-3.2/betterdataclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-27 10:44:09.000000 betterdataclass-3.2/betterdataclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:44:09.000000 betterdataclass-3.2/betterdataclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 10:44:09.000000 betterdataclass-3.2/betterdataclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 10:44:09.657407 betterdataclass-3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-27 10:43:54.000000 betterdataclass-3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:23.268362 betterdataclass-3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-27 12:48:10.000000 betterdataclass-3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-27 12:48:23.268362 betterdataclass-3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-27 12:48:10.000000 betterdataclass-3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:23.268362 betterdataclass-3.3/betterdataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/StrictDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/StrictList.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:23.268362 betterdataclass-3.3/betterdataclass/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/helper/initiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/helper/to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/helper/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-27 12:48:10.000000 betterdataclass-3.3/betterdataclass/strictEnum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:48:23.268362 betterdataclass-3.3/betterdataclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-27 12:48:23.000000 betterdataclass-3.3/betterdataclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-27 12:48:23.000000 betterdataclass-3.3/betterdataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:48:23.000000 betterdataclass-3.3/betterdataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 12:48:23.000000 betterdataclass-3.3/betterdataclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 12:48:23.268362 betterdataclass-3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-27 12:48:10.000000 betterdataclass-3.3/setup.py
```

### Comparing `betterdataclass-3.2/LICENSE` & `betterdataclass-3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.2/PKG-INFO` & `betterdataclass-3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterdataclass
-Version: 3.2
+Version: 3.3
 Summary: A multipurpose dataclass libarary used for validation and data structuring.
 Home-page: https://github.com/dvnasutosh/betterdataclasses
 Author: Asutosh Rath
 Author-email: dvnasutosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `betterdataclass-3.2/README.rst` & `betterdataclass-3.3/README.rst`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.2/betterdataclass/StrictDictionary.py` & `betterdataclass-3.3/betterdataclass/StrictDictionary.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.2/betterdataclass/StrictList.py` & `betterdataclass-3.3/betterdataclass/StrictList.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.2/betterdataclass/helper/initiate.py` & `betterdataclass-3.3/betterdataclass/helper/initiate.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.2/betterdataclass/helper/to_dict.py` & `betterdataclass-3.3/betterdataclass/helper/to_dict.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,19 +26,21 @@
             elif isinstance(value,StrictDictionary):
                 out[key] = to_raw_dict(value.__data__, processed)
             elif isinstance(value, object):
                 out[key] = to_raw_dict(value.__dict__, processed)
             else:
                 out[key] = str(value)
         return out
+    elif obj is None:
+        return obj
     elif isinstance(obj, (list, tuple, set)):
         return [to_raw_dict(item, processed) for item in obj]
     elif isinstance(obj, (int, float, bool, complex, str)):
         return obj
     elif isinstance(obj, Enum):
-        return [str(value), value.value]
-    elif isinstance(value,StrictDictionary.StrictDictionary):
-        out[key] = to_raw_dict(value.__data__, processed)
+        return [str(obj), obj.value]
+    elif isinstance(obj,StrictDictionary.StrictDictionary):
+        return to_raw_dict(obj.__data__, processed)
     elif isinstance(obj, object):
         return to_raw_dict(obj.__dict__, processed)
     else:
         return str(obj)
```

### Comparing `betterdataclass-3.2/betterdataclass/helper/validate.py` & `betterdataclass-3.3/betterdataclass/helper/validate.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-3.2/betterdataclass.egg-info/PKG-INFO` & `betterdataclass-3.3/betterdataclass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterdataclass
-Version: 3.2
+Version: 3.3
 Summary: A multipurpose dataclass libarary used for validation and data structuring.
 Home-page: https://github.com/dvnasutosh/betterdataclasses
 Author: Asutosh Rath
 Author-email: dvnasutosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `betterdataclass-3.2/setup.py` & `betterdataclass-3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 import setuptools
 
 
 setup(
     name="betterdataclass",
-    version="3.02",
+    version="3.03",
     description="A multipurpose dataclass libarary used for validation and data structuring.",
     long_description=open('./README.rst').read(),
     url='https://github.com/dvnasutosh/betterdataclasses',
     
     author="Asutosh Rath",
     author_email="dvnasutosh@gmail.com",
     packages=find_packages(),
```

