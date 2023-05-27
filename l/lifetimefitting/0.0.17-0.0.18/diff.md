# Comparing `tmp/lifetimefitting-0.0.17.tar.gz` & `tmp/lifetimefitting-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.17.tar", last modified: Sat May 27 03:32:10 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.18.tar", last modified: Sat May 27 03:40:25 2023, max compression
```

## Comparing `lifetimefitting-0.0.17.tar` & `lifetimefitting-0.0.18.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:32:10.716631 lifetimefitting-0.0.17/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/app/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/funcs/expFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/funcs/fittingFuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/funcs/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/lifetimefitting/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 03:32:10.000000 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-27 03:32:10.000000 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 03:32:10.000000 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-27 03:32:10.000000 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 03:32:10.000000 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:25.186601 lifetimefitting-0.0.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 03:40:25.186601 lifetimefitting-0.0.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:25.178601 lifetimefitting-0.0.18/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:25.182601 lifetimefitting-0.0.18/app/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/funcs/expFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/funcs/fittingFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/funcs/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:25.182601 lifetimefitting-0.0.18/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/app/lifetimefitting/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:40:25.182601 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 03:40:25.000000 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-27 03:40:25.000000 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 03:40:25.000000 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-27 03:40:25.000000 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 03:40:25.000000 lifetimefitting-0.0.18/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 03:40:25.186601 lifetimefitting-0.0.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 03:40:14.000000 lifetimefitting-0.0.18/setup.py
```

### Comparing `lifetimefitting-0.0.17/LICENSE.md` & `lifetimefitting-0.0.18/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.17/PKG-INFO` & `lifetimefitting-0.0.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.17
+Version: 0.0.18
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.17/README.md` & `lifetimefitting-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.17/app/funcs/expFuncs.py` & `lifetimefitting-0.0.18/app/funcs/expFuncs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.17/app/funcs/fittingFuncs.py` & `lifetimefitting-0.0.18/app/funcs/fittingFuncs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.17/app/funcs/gui.py` & `lifetimefitting-0.0.18/app/funcs/gui.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.17/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.18/app/lifetimefitting/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 
 def irf_browse():
     ui.irf_file.setText(file_dialog.getOpenFileName(directory="/Users/adrea/gdrive/Monash/PhD/Fluorophore/data/tr/AAQ", filter="PicoHarp binary of text file (*.phd *.txt)")[0])
 
 def update_max_x():
     ui.max_x_out.setValue(ui.max_x.value())
 
+def update_max_x_from_out():
+    ui.max_x.setValue(ui.max_x_out.value())
+
 def setupPlot():
     ui.horizontalLayout_plot = QtWidgets.QHBoxLayout(ui.frame)
     ui.horizontalLayout_plot.setObjectName("horizontalLayout_plot")
     ui.figure, (ui.ax1, ui.ax3, ui.ax2, ui.ax4) = plt.subplots(4, 1, figsize=(8, 10), sharex=True, height_ratios=[3, 3, 1, 1])
     ui.canvas = FigureCanvas(ui.figure)
     ui.horizontalLayout_plot.addWidget(ui.canvas)
     ui.axList = []
@@ -79,12 +82,13 @@
     # file loading
     file_dialog = QFileDialog()
     ui.trf_browse.clicked.connect(trf_browse)
     ui.irf_browse.clicked.connect(irf_browse)
     ui.plot_browse.clicked.connect(savePlot)
     ui.csv_browse.clicked.connect(saveCSV)
     ui.max_x.sliderMoved.connect(update_max_x)
+    ui.max_x_out.valueChanged.connect(update_max_x_from_out)
 
     ui.fit_button.clicked.connect(plotFL)
 
     Form.show()
     sys.exit(app.exec())
```

### Comparing `lifetimefitting-0.0.17/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.18/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.17
+Version: 0.0.18
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.17/setup.py` & `lifetimefitting-0.0.18/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.17",
+    version = "0.0.18",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
```

