# Comparing `tmp/lifetimefitting-0.0.12.tar.gz` & `tmp/lifetimefitting-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.12.tar", last modified: Fri May 26 05:00:50 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.13.tar", last modified: Sat May 27 01:46:13 2023, max compression
```

## Comparing `lifetimefitting-0.0.12.tar` & `lifetimefitting-0.0.13.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/app/lifetimefitting/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/app/lifetimefitting/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/app/lifetimefitting/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/app/lifetimefitting/phd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-26 05:00:50.000000 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 05:00:50.000000 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 05:00:50.000000 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 05:00:50.000000 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 05:00:50.000000 lifetimefitting-0.0.12/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 05:00:50.536514 lifetimefitting-0.0.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-26 05:00:39.000000 lifetimefitting-0.0.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:46:13.778628 lifetimefitting-0.0.13/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 01:46:13.778628 lifetimefitting-0.0.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:46:13.774628 lifetimefitting-0.0.13/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:46:13.774628 lifetimefitting-0.0.13/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/app/lifetimefitting/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/app/lifetimefitting/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/app/lifetimefitting/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/app/lifetimefitting/phd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:46:13.778628 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 01:46:13.000000 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-27 01:46:13.000000 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 01:46:13.000000 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 01:46:13.000000 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 01:46:13.000000 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 01:46:13.778628 lifetimefitting-0.0.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/setup.py
```

### Comparing `lifetimefitting-0.0.12/LICENSE.md` & `lifetimefitting-0.0.13/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.12/PKG-INFO` & `lifetimefitting-0.0.13/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.12
+Version: 0.0.13
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,27 +31,27 @@
 ```
 
 ### Manually
 
 * Python (I'm not sure how old you could go, but I know it runs on >3.9)
 * Matplotlib
 * Numpy
-* PyQt5
+* PyQt6
 * Scipy
 
 These can be installed pretty easily via pip
 
 ```bash
-pip install matplotlib numpy scipy pyqt5
+pip install matplotlib numpy scipy pyqt6
 ```
 
 or conda
 
 ```bash
-conda install matplotlib numpy scipy pyqt5
+conda install matplotlib numpy scipy pyqt6
 ```
 
 Then you can clone the module down and install it manually
 
 ```bash
 git clone https://github.com/adreasnow/LifetimeFittingTool.git
 cd LifetimeFittingTool
```

### Comparing `lifetimefitting-0.0.12/README.md` & `lifetimefitting-0.0.13/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 ```
 
 ### Manually
 
 * Python (I'm not sure how old you could go, but I know it runs on >3.9)
 * Matplotlib
 * Numpy
-* PyQt5
+* PyQt6
 * Scipy
 
 These can be installed pretty easily via pip
 
 ```bash
-pip install matplotlib numpy scipy pyqt5
+pip install matplotlib numpy scipy pyqt6
 ```
 
 or conda
 
 ```bash
-conda install matplotlib numpy scipy pyqt5
+conda install matplotlib numpy scipy pyqt6
 ```
 
 Then you can clone the module down and install it manually
 
 ```bash
 git clone https://github.com/adreasnow/LifetimeFittingTool.git
 cd LifetimeFittingTool
@@ -82,8 +82,8 @@
 * $C_i =$ Linear coefficient for each decay
 
 $\chi^2$ is calculated as per [fluortools](http://www.fluortools.com/software/decayfit/documentation/fit)
 
 $$
 \chi^2 = \sum_{j=1}^{n} (c_j-\hat{c_j})^2/\hat{c_j}\\
 \chi^2_{red}=\frac{\chi^2}{n}
-$$
+$$
```

### Comparing `lifetimefitting-0.0.12/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.13/app/lifetimefitting/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import struct
 from scipy.optimize import curve_fit
-from PyQt5 import QtCore, QtGui, QtWidgets
-from PyQt5.QtWidgets import QFileDialog, QMessageBox
+from PyQt6 import QtCore, QtGui, QtWidgets
+from PyQt6.QtWidgets import QFileDialog, QMessageBox
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 
 import os
 from .phd import TRF
 from .funcs import expFunc, expFuncWC, expFuncx2, expFuncx3, expFuncx4
 from .funcs import linFunc, linFuncWC, linFuncx2, linFuncx3, linFuncx4
 from .gui import Ui_Form
```

### Comparing `lifetimefitting-0.0.12/app/lifetimefitting/funcs.py` & `lifetimefitting-0.0.13/app/lifetimefitting/funcs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.12/app/lifetimefitting/gui.py` & `lifetimefitting-0.0.13/app/lifetimefitting/gui.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.12/app/lifetimefitting/phd.py` & `lifetimefitting-0.0.13/app/lifetimefitting/phd.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.12/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.13/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.12
+Version: 0.0.13
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,27 +31,27 @@
 ```
 
 ### Manually
 
 * Python (I'm not sure how old you could go, but I know it runs on >3.9)
 * Matplotlib
 * Numpy
-* PyQt5
+* PyQt6
 * Scipy
 
 These can be installed pretty easily via pip
 
 ```bash
-pip install matplotlib numpy scipy pyqt5
+pip install matplotlib numpy scipy pyqt6
 ```
 
 or conda
 
 ```bash
-conda install matplotlib numpy scipy pyqt5
+conda install matplotlib numpy scipy pyqt6
 ```
 
 Then you can clone the module down and install it manually
 
 ```bash
 git clone https://github.com/adreasnow/LifetimeFittingTool.git
 cd LifetimeFittingTool
```

### Comparing `lifetimefitting-0.0.12/setup.py` & `lifetimefitting-0.0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.12",
+    version = "0.0.13",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir = {"": "app"},
     packages = find_packages(where="app"),
     extras_require = {"dev": ["twine>=4.0.2"]},
-    install_requires=['matplotlib', 'numpy', 'scipy', 'pyqt5'],
+    install_requires=['matplotlib', 'numpy', 'scipy', 'pyqt6'],
     python_requires = ">=3.8",
 )
```

