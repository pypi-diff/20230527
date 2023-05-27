# Comparing `tmp/makeprediction-4.1.0.tar.gz` & `tmp/makeprediction-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makeprediction-4.1.0.tar", last modified: Mon May  1 22:37:42 2023, max compression
+gzip compressed data, was "makeprediction-4.1.1.tar", last modified: Sat May 27 11:42:44 2023, max compression
```

## Comparing `makeprediction-4.1.0.tar` & `makeprediction-4.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 tolba      (501) staff       (20)        0 2023-05-01 22:37:42.001843 makeprediction-4.1.0/
--rw-r--r--   0 tolba      (501) staff       (20)     7651 2023-04-30 09:45:48.000000 makeprediction-4.1.0/LICENSE
--rw-r--r--   0 tolba      (501) staff       (20)      216 2023-04-30 09:45:48.000000 makeprediction-4.1.0/MANIFEST.in
--rw-r--r--   0 tolba      (501) staff       (20)     7357 2023-05-01 22:37:41.997803 makeprediction-4.1.0/PKG-INFO
--rw-r--r--   0 tolba      (501) staff       (20)     6388 2023-04-30 09:45:48.000000 makeprediction-4.1.0/README.md
-drwxr-xr-x   0 tolba      (501) staff       (20)        0 2023-05-01 22:37:41.712529 makeprediction-4.1.0/Unit_test/
--rw-r--r--   0 tolba      (501) staff       (20)        0 2023-04-30 09:45:48.000000 makeprediction-4.1.0/Unit_test/__init__.py
--rw-r--r--   0 tolba      (501) staff       (20)     3589 2023-04-30 09:45:48.000000 makeprediction-4.1.0/Unit_test/test_gpr.py
--rw-r--r--   0 tolba      (501) staff       (20)      851 2023-04-30 09:45:48.000000 makeprediction-4.1.0/Unit_test/test_inv.py
--rw-r--r--   0 tolba      (501) staff       (20)     5357 2023-04-30 09:45:48.000000 makeprediction-4.1.0/Unit_test/test_kernel.py
-drwxr-xr-x   0 tolba      (501) staff       (20)        0 2023-05-01 22:37:41.806882 makeprediction-4.1.0/makeprediction/
--rw-r--r--   0 tolba      (501) staff       (20)      936 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction/__init__.py
--rw-r--r--   0 tolba      (501) staff       (20)     4684 2023-05-01 21:59:37.000000 makeprediction-4.1.0/makeprediction/api.py
--rw-r--r--   0 tolba      (501) staff       (20)      618 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction/exceptions.py
--rw-r--r--   0 tolba      (501) staff       (20)    24866 2023-05-01 12:30:22.000000 makeprediction-4.1.0/makeprediction/gaussianprocess.py
--rw-r--r--   0 tolba      (501) staff       (20)    17867 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction/gpts.py
--rw-r--r--   0 tolba      (501) staff       (20)     4490 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction/invtools.py
--rw-r--r--   0 tolba      (501) staff       (20)    13860 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction/kernels.py
--rw-r--r--   0 tolba      (501) staff       (20)     1107 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction/metrics.py
--rw-r--r--   0 tolba      (501) staff       (20)     2103 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction/scores.py
--rw-r--r--   0 tolba      (501) staff       (20)     3505 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction/store.py
--rw-r--r--   0 tolba      (501) staff       (20)     2013 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction/stream.py
--rw-r--r--   0 tolba      (501) staff       (20)     3095 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction/tools.py
--rw-r--r--   0 tolba      (501) staff       (20)      332 2023-05-01 22:36:48.000000 makeprediction-4.1.0/makeprediction/version.py
--rw-r--r--   0 tolba      (501) staff       (20)    12024 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction/visualization.py
-drwxr-xr-x   0 tolba      (501) staff       (20)        0 2023-05-01 22:37:41.836802 makeprediction-4.1.0/makeprediction.egg-info/
--rw-r--r--   0 tolba      (501) staff       (20)     7357 2023-05-01 22:37:41.000000 makeprediction-4.1.0/makeprediction.egg-info/PKG-INFO
--rw-r--r--   0 tolba      (501) staff       (20)     1100 2023-05-01 22:37:41.000000 makeprediction-4.1.0/makeprediction.egg-info/SOURCES.txt
--rw-r--r--   0 tolba      (501) staff       (20)        1 2023-05-01 22:37:41.000000 makeprediction-4.1.0/makeprediction.egg-info/dependency_links.txt
--rw-r--r--   0 tolba      (501) staff       (20)       76 2023-05-01 22:37:41.000000 makeprediction-4.1.0/makeprediction.egg-info/requires.txt
--rw-r--r--   0 tolba      (501) staff       (20)       43 2023-05-01 22:37:41.000000 makeprediction-4.1.0/makeprediction.egg-info/top_level.txt
-drwxr-xr-x   0 tolba      (501) staff       (20)        0 2023-05-01 22:37:41.992984 makeprediction-4.1.0/makeprediction_v0/
--rw-r--r--   0 tolba      (501) staff       (20)      940 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/__init__.py
--rw-r--r--   0 tolba      (501) staff       (20)     4479 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/api.py
--rw-r--r--   0 tolba      (501) staff       (20)      618 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/exceptions.py
--rw-r--r--   0 tolba      (501) staff       (20)    24789 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/gaussianprocess.py
--rw-r--r--   0 tolba      (501) staff       (20)    17384 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/gpts.py
--rw-r--r--   0 tolba      (501) staff       (20)     4417 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/invtools.py
--rw-r--r--   0 tolba      (501) staff       (20)    13860 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/kernels.py
--rw-r--r--   0 tolba      (501) staff       (20)     1107 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/metrics.py
--rw-r--r--   0 tolba      (501) staff       (20)     2103 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/scores.py
--rw-r--r--   0 tolba      (501) staff       (20)     2605 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/store.py
--rw-r--r--   0 tolba      (501) staff       (20)     2034 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/stream.py
--rw-r--r--   0 tolba      (501) staff       (20)     3095 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/tools.py
--rw-r--r--   0 tolba      (501) staff       (20)      328 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/version.py
--rw-r--r--   0 tolba      (501) staff       (20)    11914 2023-04-30 09:45:48.000000 makeprediction-4.1.0/makeprediction_v0/visualization.py
--rw-r--r--   0 tolba      (501) staff       (20)       38 2023-05-01 22:37:42.003239 makeprediction-4.1.0/setup.cfg
--rw-r--r--   0 tolba      (501) staff       (20)     3742 2023-04-30 09:45:48.000000 makeprediction-4.1.0/setup.py
+drwxr-xr-x   0 tolba      (501) staff       (20)        0 2023-05-27 11:42:44.208878 makeprediction-4.1.1/
+-rw-r--r--   0 tolba      (501) staff       (20)     7651 2023-04-30 09:45:48.000000 makeprediction-4.1.1/LICENSE
+-rw-r--r--   0 tolba      (501) staff       (20)      216 2023-04-30 09:45:48.000000 makeprediction-4.1.1/MANIFEST.in
+-rw-r--r--   0 tolba      (501) staff       (20)     7357 2023-05-27 11:42:44.208286 makeprediction-4.1.1/PKG-INFO
+-rw-r--r--   0 tolba      (501) staff       (20)     6388 2023-04-30 09:45:48.000000 makeprediction-4.1.1/README.md
+drwxr-xr-x   0 tolba      (501) staff       (20)        0 2023-05-27 11:42:44.136827 makeprediction-4.1.1/Unit_test/
+-rw-r--r--   0 tolba      (501) staff       (20)        0 2023-04-30 09:45:48.000000 makeprediction-4.1.1/Unit_test/__init__.py
+-rw-r--r--   0 tolba      (501) staff       (20)     3589 2023-04-30 09:45:48.000000 makeprediction-4.1.1/Unit_test/test_gpr.py
+-rw-r--r--   0 tolba      (501) staff       (20)      851 2023-04-30 09:45:48.000000 makeprediction-4.1.1/Unit_test/test_inv.py
+-rw-r--r--   0 tolba      (501) staff       (20)     5357 2023-04-30 09:45:48.000000 makeprediction-4.1.1/Unit_test/test_kernel.py
+drwxr-xr-x   0 tolba      (501) staff       (20)        0 2023-05-27 11:42:44.157165 makeprediction-4.1.1/makeprediction/
+-rw-r--r--   0 tolba      (501) staff       (20)      936 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction/__init__.py
+-rw-r--r--   0 tolba      (501) staff       (20)     5141 2023-05-27 11:25:26.000000 makeprediction-4.1.1/makeprediction/api.py
+-rw-r--r--   0 tolba      (501) staff       (20)      618 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction/exceptions.py
+-rw-r--r--   0 tolba      (501) staff       (20)    24866 2023-05-01 12:30:22.000000 makeprediction-4.1.1/makeprediction/gaussianprocess.py
+-rw-r--r--   0 tolba      (501) staff       (20)    17867 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction/gpts.py
+-rw-r--r--   0 tolba      (501) staff       (20)     4490 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction/invtools.py
+-rw-r--r--   0 tolba      (501) staff       (20)    13860 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction/kernels.py
+-rw-r--r--   0 tolba      (501) staff       (20)     1107 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction/metrics.py
+-rw-r--r--   0 tolba      (501) staff       (20)     2103 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction/scores.py
+-rw-r--r--   0 tolba      (501) staff       (20)     3505 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction/store.py
+-rw-r--r--   0 tolba      (501) staff       (20)     2013 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction/stream.py
+-rw-r--r--   0 tolba      (501) staff       (20)     3095 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction/tools.py
+-rw-r--r--   0 tolba      (501) staff       (20)      334 2023-05-27 11:28:26.000000 makeprediction-4.1.1/makeprediction/version.py
+-rw-r--r--   0 tolba      (501) staff       (20)    12024 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction/visualization.py
+drwxr-xr-x   0 tolba      (501) staff       (20)        0 2023-05-27 11:42:44.165371 makeprediction-4.1.1/makeprediction.egg-info/
+-rw-r--r--   0 tolba      (501) staff       (20)     7357 2023-05-27 11:42:43.000000 makeprediction-4.1.1/makeprediction.egg-info/PKG-INFO
+-rw-r--r--   0 tolba      (501) staff       (20)     1100 2023-05-27 11:42:44.000000 makeprediction-4.1.1/makeprediction.egg-info/SOURCES.txt
+-rw-r--r--   0 tolba      (501) staff       (20)        1 2023-05-27 11:42:43.000000 makeprediction-4.1.1/makeprediction.egg-info/dependency_links.txt
+-rw-r--r--   0 tolba      (501) staff       (20)       76 2023-05-27 11:42:43.000000 makeprediction-4.1.1/makeprediction.egg-info/requires.txt
+-rw-r--r--   0 tolba      (501) staff       (20)       43 2023-05-27 11:42:43.000000 makeprediction-4.1.1/makeprediction.egg-info/top_level.txt
+drwxr-xr-x   0 tolba      (501) staff       (20)        0 2023-05-27 11:42:44.206585 makeprediction-4.1.1/makeprediction_v0/
+-rw-r--r--   0 tolba      (501) staff       (20)      940 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/__init__.py
+-rw-r--r--   0 tolba      (501) staff       (20)     4479 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/api.py
+-rw-r--r--   0 tolba      (501) staff       (20)      618 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/exceptions.py
+-rw-r--r--   0 tolba      (501) staff       (20)    24789 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/gaussianprocess.py
+-rw-r--r--   0 tolba      (501) staff       (20)    17384 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/gpts.py
+-rw-r--r--   0 tolba      (501) staff       (20)     4417 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/invtools.py
+-rw-r--r--   0 tolba      (501) staff       (20)    13860 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/kernels.py
+-rw-r--r--   0 tolba      (501) staff       (20)     1107 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/metrics.py
+-rw-r--r--   0 tolba      (501) staff       (20)     2103 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/scores.py
+-rw-r--r--   0 tolba      (501) staff       (20)     2605 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/store.py
+-rw-r--r--   0 tolba      (501) staff       (20)     2034 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/stream.py
+-rw-r--r--   0 tolba      (501) staff       (20)     3095 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/tools.py
+-rw-r--r--   0 tolba      (501) staff       (20)      328 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/version.py
+-rw-r--r--   0 tolba      (501) staff       (20)    11914 2023-04-30 09:45:48.000000 makeprediction-4.1.1/makeprediction_v0/visualization.py
+-rw-r--r--   0 tolba      (501) staff       (20)       38 2023-05-27 11:42:44.209014 makeprediction-4.1.1/setup.cfg
+-rw-r--r--   0 tolba      (501) staff       (20)     3742 2023-05-27 11:41:16.000000 makeprediction-4.1.1/setup.py
```

### Comparing `makeprediction-4.1.0/LICENSE` & `makeprediction-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/PKG-INFO` & `makeprediction-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makeprediction
-Version: 4.1.0
+Version: 4.1.1
 Summary: Automatic and fast Gaussian process for time serie prediction.
 Home-page: https://github.com/HananyTolba/MakePrediction.git
 Download-URL: https://github.com/HananyTolba/MakePrediction.git
 Author: Hanany Tolba
 Author-email: hananytolba@yahoo.com
 License: GPLv3
 Keywords: Gaussian Process Regression,Time series prediction,Machine Learning
```

### Comparing `makeprediction-4.1.0/README.md` & `makeprediction-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/Unit_test/test_gpr.py` & `makeprediction-4.1.1/Unit_test/test_gpr.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/Unit_test/test_inv.py` & `makeprediction-4.1.1/Unit_test/test_inv.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/Unit_test/test_kernel.py` & `makeprediction-4.1.1/Unit_test/test_kernel.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/__init__.py` & `makeprediction-4.1.1/makeprediction/__init__.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/api.py` & `makeprediction-4.1.1/makeprediction_v0/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 # from .tools import LargeKernelNames, SmallKernelNames
 from urllib.parse import urljoin
 import re
 
 
 
 class Instance(enum.Enum):
-    # SIMPLE = os.environ.get("BASE_URL", 'https://simple.makeprediction.com/')
-    # PERIODIC = os.environ.get("BASE_URL", 'https://periodic.makeprediction.com/')
-    SIMPLE = os.environ.get("BASE_URL", 'http://api.gprts.info/')
-    PERIODIC = os.environ.get("BASE_URL", 'http://api.gprts.info/')
+    SIMPLE = os.environ.get("BASE_URL", 'https://simple.makeprediction.com/')
+    PERIODIC = os.environ.get("BASE_URL", 'https://periodic.makeprediction.com/')
 
 class ContainerName(enum.Enum):
     pass
 
 class PeriodicContainerName(ContainerName):
 
-    Periodic = "tf_PeriodicPlusMatern"
+    Periodic = "periodic_model"
     PeriodicPlusMatern = "tf_PeriodicPlusMatern"
     PeriodicPlusRBF = "tf_PeriodicPlusRBF"
     PeriodicModel = "periodic_model"
     which_stationarity = "stationary_kernel_predict"
-
     @classmethod
     def attrmatch(cls,value):
         return hasattr(cls,value)
     @classmethod
     def get(cls,value):
         if cls.attrmatch(value):  
             return getattr(cls,value)
@@ -111,16 +108,15 @@
         return urljoin(Instance.SIMPLE.value, url)
 
     
     @classmethod
     def get_url(cls,name):
         if SimpleContainerName.attrmatch(name):
             value = SimpleContainerName.get(name).value
-            # path = f"/{value.replace('_1d','')}/v1/models/{value}:predict"
-            path = f"/{value}/v1/models/{value}:predict"
+            path = f"/{value.replace('_1d','')}/v1/models/{value}:predict"
             return urljoin(Instance.SIMPLE.value, path)
         elif PeriodicContainerName.attrmatch(name):
             value = PeriodicContainerName.get(name).value
             LS = PeriodicLengthScaleIID.LS.value
             IID = PeriodicLengthScaleIID.IID.value
             path1 = f"/{value}/v1/models/{value}:predict"
             path2 = f"/{LS}/v1/models/{LS}:predict"
```

### Comparing `makeprediction-4.1.0/makeprediction/exceptions.py` & `makeprediction-4.1.1/makeprediction/exceptions.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/gaussianprocess.py` & `makeprediction-4.1.1/makeprediction/gaussianprocess.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/gpts.py` & `makeprediction-4.1.1/makeprediction/gpts.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/invtools.py` & `makeprediction-4.1.1/makeprediction/invtools.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/kernels.py` & `makeprediction-4.1.1/makeprediction/kernels.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/metrics.py` & `makeprediction-4.1.1/makeprediction/metrics.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/scores.py` & `makeprediction-4.1.1/makeprediction/scores.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/store.py` & `makeprediction-4.1.1/makeprediction/store.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/stream.py` & `makeprediction-4.1.1/makeprediction/stream.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/tools.py` & `makeprediction-4.1.1/makeprediction/tools.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction/visualization.py` & `makeprediction-4.1.1/makeprediction/visualization.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction.egg-info/PKG-INFO` & `makeprediction-4.1.1/makeprediction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makeprediction
-Version: 4.1.0
+Version: 4.1.1
 Summary: Automatic and fast Gaussian process for time serie prediction.
 Home-page: https://github.com/HananyTolba/MakePrediction.git
 Download-URL: https://github.com/HananyTolba/MakePrediction.git
 Author: Hanany Tolba
 Author-email: hananytolba@yahoo.com
 License: GPLv3
 Keywords: Gaussian Process Regression,Time series prediction,Machine Learning
```

### Comparing `makeprediction-4.1.0/makeprediction.egg-info/SOURCES.txt` & `makeprediction-4.1.1/makeprediction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/__init__.py` & `makeprediction-4.1.1/makeprediction_v0/__init__.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/api.py` & `makeprediction-4.1.1/makeprediction/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,33 @@
 # from .tools import LargeKernelNames, SmallKernelNames
 from urllib.parse import urljoin
 import re
 
 
 
 class Instance(enum.Enum):
-    SIMPLE = os.environ.get("BASE_URL", 'https://simple.makeprediction.com/')
-    PERIODIC = os.environ.get("BASE_URL", 'https://periodic.makeprediction.com/')
+    # SIMPLE = os.environ.get("BASE_URL", 'https://simple.makeprediction.com/')
+    # PERIODIC = os.environ.get("BASE_URL", 'https://periodic.makeprediction.com/')
+    # SIMPLE = os.environ.get("BASE_URL", 'http://api.gprts.info/')
+    # SIMPLE = os.environ.get("BASE_URL", 'http://localhost/')
+    # PERIODIC = os.environ.get("BASE_URL", 'http://localhost/')
+    SIMPLE = os.environ.get("BASE_URL", 'http://api.gprts.info/')
+    PERIODIC = os.environ.get("BASE_URL", 'http://api.gprts.info/')
 
 class ContainerName(enum.Enum):
     pass
 
 class PeriodicContainerName(ContainerName):
 
-    Periodic = "periodic_model"
+    Periodic = "tf_PeriodicPlusMatern"
     PeriodicPlusMatern = "tf_PeriodicPlusMatern"
     PeriodicPlusRBF = "tf_PeriodicPlusRBF"
     PeriodicModel = "periodic_model"
     which_stationarity = "stationary_kernel_predict"
+
     @classmethod
     def attrmatch(cls,value):
         return hasattr(cls,value)
     @classmethod
     def get(cls,value):
         if cls.attrmatch(value):  
             return getattr(cls,value)
@@ -71,14 +77,15 @@
 
 class API:
     @classmethod
     def simple_url(cls,name):
         if SimpleContainerName.attrmatch(name):
             value = SimpleContainerName.get(name).value
             path = f"/{value.replace('_1d','')}/v1/models/{value}:predict"
+            path = f"/{name}_1d"
             return urljoin(Instance.SIMPLE.value, path)
         
     @classmethod
     def periodic_url(cls,name):
         if PeriodicContainerName.attrmatch(name):
             value = PeriodicContainerName.get(name).value
             LS = PeriodicLengthScaleIID.LS.value
@@ -89,39 +96,48 @@
             urls = [urljoin(Instance.PERIODIC.value, path) for path in (path1,path2,path3)]
             return urls
 
     @classmethod
     def url_which_stationarity(cls):
         which_stationarity = PeriodicContainerName.which_stationarity.value
         url = f"{which_stationarity}/v1/models/{which_stationarity}:predict"
+        url = f"{which_stationarity}"
         return urljoin(Instance.PERIODIC.value, url)
 
     @classmethod
     def url_is_periodic(cls):
         is_periodic = SimpleContainerName.is_periodic.value
         url = f"/{is_periodic}/v1/models/{is_periodic}:predict"
+        url = f"/{is_periodic}"
         return urljoin(Instance.SIMPLE.value, url)
 
     @classmethod
     def url_is_linear(cls):
         is_linear = SimpleContainerName.is_linear.value
         url = f"/{is_linear}/v1/models/{is_linear}:predict"
+        url = f"/{is_linear}"
         return urljoin(Instance.SIMPLE.value, url)
 
     
     @classmethod
     def get_url(cls,name):
         if SimpleContainerName.attrmatch(name):
             value = SimpleContainerName.get(name).value
-            path = f"/{value.replace('_1d','')}/v1/models/{value}:predict"
+            # path = f"/{value.replace('_1d','')}/v1/models/{value}:predict"
+            # path = f"/{value}/v1/models/{value}:predict"
+            path = f"/{value}"
             return urljoin(Instance.SIMPLE.value, path)
         elif PeriodicContainerName.attrmatch(name):
             value = PeriodicContainerName.get(name).value
             LS = PeriodicLengthScaleIID.LS.value
             IID = PeriodicLengthScaleIID.IID.value
-            path1 = f"/{value}/v1/models/{value}:predict"
-            path2 = f"/{LS}/v1/models/{LS}:predict"
-            path3 = f"/{IID}/v1/models/{IID}:predict"
+            # path1 = f"/{value}/v1/models/{value}:predict"
+            # path2 = f"/{LS}/v1/models/{LS}:predict"
+            # path3 = f"/{IID}/v1/models/{IID}:predict"
+            path1 = f"{value}"
+            path2 = f"{LS}"
+            path3 = f"{IID}"
+
             urls = [urljoin(Instance.PERIODIC.value, path) for path in (path1,path2,path3)]
             return tuple(urls)
         return cls.url_which_stationarity()
```

### Comparing `makeprediction-4.1.0/makeprediction_v0/exceptions.py` & `makeprediction-4.1.1/makeprediction_v0/exceptions.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/gaussianprocess.py` & `makeprediction-4.1.1/makeprediction_v0/gaussianprocess.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/gpts.py` & `makeprediction-4.1.1/makeprediction_v0/gpts.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/invtools.py` & `makeprediction-4.1.1/makeprediction_v0/invtools.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/kernels.py` & `makeprediction-4.1.1/makeprediction_v0/kernels.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/metrics.py` & `makeprediction-4.1.1/makeprediction_v0/metrics.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/scores.py` & `makeprediction-4.1.1/makeprediction_v0/scores.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/store.py` & `makeprediction-4.1.1/makeprediction_v0/store.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/stream.py` & `makeprediction-4.1.1/makeprediction_v0/stream.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/tools.py` & `makeprediction-4.1.1/makeprediction_v0/tools.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/makeprediction_v0/visualization.py` & `makeprediction-4.1.1/makeprediction_v0/visualization.py`

 * *Files identical despite different names*

### Comparing `makeprediction-4.1.0/setup.py` & `makeprediction-4.1.1/setup.py`

 * *Files identical despite different names*

