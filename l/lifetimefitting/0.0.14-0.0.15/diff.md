# Comparing `tmp/lifetimefitting-0.0.14.tar.gz` & `tmp/lifetimefitting-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.14.tar", last modified: Sat May 27 02:04:58 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.15.tar", last modified: Sat May 27 02:11:02 2023, max compression
```

## Comparing `lifetimefitting-0.0.14.tar` & `lifetimefitting-0.0.15.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:04:58.220316 lifetimefitting-0.0.14/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 02:04:58.216316 lifetimefitting-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:04:58.216316 lifetimefitting-0.0.14/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:04:58.216316 lifetimefitting-0.0.14/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/app/lifetimefitting/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/app/lifetimefitting/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/app/lifetimefitting/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/app/lifetimefitting/phd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:04:58.216316 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 02:04:58.000000 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-27 02:04:58.000000 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:04:58.000000 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 02:04:58.000000 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 02:04:58.000000 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:04:58.220316 lifetimefitting-0.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:11:02.434800 lifetimefitting-0.0.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 02:11:02.434800 lifetimefitting-0.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:11:02.430800 lifetimefitting-0.0.15/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:11:02.434800 lifetimefitting-0.0.15/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/app/lifetimefitting/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/app/lifetimefitting/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/app/lifetimefitting/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/app/lifetimefitting/phd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:11:02.434800 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 02:11:02.000000 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-27 02:11:02.000000 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:11:02.000000 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 02:11:02.000000 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 02:11:02.000000 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:11:02.434800 lifetimefitting-0.0.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/setup.py
```

### Comparing `lifetimefitting-0.0.14/LICENSE.md` & `lifetimefitting-0.0.15/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.14/PKG-INFO` & `lifetimefitting-0.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.14
+Version: 0.0.15
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.14/README.md` & `lifetimefitting-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.14/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.15/app/lifetimefitting/__main__.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.14/app/lifetimefitting/funcs.py` & `lifetimefitting-0.0.15/app/lifetimefitting/funcs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.14/app/lifetimefitting/gui.py` & `lifetimefitting-0.0.15/app/lifetimefitting/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         self.maxIter_widg.setMaximum(100000000)
         self.maxIter_widg.setSingleStep(1000)
         self.maxIter_widg.setProperty("value", 5000)
         self.maxIter_widg.setObjectName("maxIter_widg")
         self.verticalLayout.addWidget(self.maxIter_widg)
         self.startOffset_widg = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
         self.startOffset_widg.setObjectName("startOffset_widg")
+        self.startOffset_widg.setMaximum(10000)
         self.verticalLayout.addWidget(self.startOffset_widg)
         self.maxTime_widg = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
         self.maxTime_widg.setMaximum(9999999)
         self.maxTime_widg.setProperty("value", 1000)
         self.maxTime_widg.setObjectName("maxTime_widg")
         self.verticalLayout.addWidget(self.maxTime_widg)
         self.expCount_widg = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
```

### Comparing `lifetimefitting-0.0.14/app/lifetimefitting/phd.py` & `lifetimefitting-0.0.15/app/lifetimefitting/phd.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.14/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.15/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.14
+Version: 0.0.15
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.14/setup.py` & `lifetimefitting-0.0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.14",
+    version = "0.0.15",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
```

