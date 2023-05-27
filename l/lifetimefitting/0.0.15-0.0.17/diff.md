# Comparing `tmp/lifetimefitting-0.0.15.tar.gz` & `tmp/lifetimefitting-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.15.tar", last modified: Sat May 27 02:11:02 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.17.tar", last modified: Sat May 27 03:32:10 2023, max compression
```

## Comparing `lifetimefitting-0.0.15.tar` & `lifetimefitting-0.0.17.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:11:02.434800 lifetimefitting-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 02:11:02.434800 lifetimefitting-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:11:02.430800 lifetimefitting-0.0.15/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:11:02.434800 lifetimefitting-0.0.15/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/app/lifetimefitting/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/app/lifetimefitting/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/app/lifetimefitting/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/app/lifetimefitting/phd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:11:02.434800 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 02:11:02.000000 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-27 02:11:02.000000 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:11:02.000000 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 02:11:02.000000 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 02:11:02.000000 lifetimefitting-0.0.15/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:11:02.434800 lifetimefitting-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-27 02:10:47.000000 lifetimefitting-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:32:10.716631 lifetimefitting-0.0.17/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/app/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/funcs/expFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/funcs/fittingFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/funcs/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/app/lifetimefitting/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 03:32:10.000000 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-27 03:32:10.000000 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 03:32:10.000000 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-27 03:32:10.000000 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 03:32:10.000000 lifetimefitting-0.0.17/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 03:32:10.720631 lifetimefitting-0.0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 03:31:53.000000 lifetimefitting-0.0.17/setup.py
```

### Comparing `lifetimefitting-0.0.15/LICENSE.md` & `lifetimefitting-0.0.17/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.15/PKG-INFO` & `lifetimefitting-0.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.15
+Version: 0.0.17
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.15/README.md` & `lifetimefitting-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.15/app/lifetimefitting/funcs.py` & `lifetimefitting-0.0.17/app/funcs/expFuncs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import numpy as np
+import numpy as np 
 def expFunc(t, I0, τ) -> float:
     return np.multiply(np.exp(np.negative(np.divide(t, τ))), I0)
 
 def expFuncWC(t, I0, τ, c) -> float:
     return np.multiply(expFunc(t, I0, τ), c)
 
 def expFuncx2(t, I0, τ_1, c_1, τ_2, c_2):
@@ -36,8 +36,8 @@
                                 np.multiply(linFunc(t, I0, τ_2), c_2)),
                          np.multiply(linFunc(t, I0, τ_3), c_3)))
 
 def linFuncx4(t, I0, τ_1, c_1, τ_2, c_2, τ_3, c_3, τ_4, c_4):
     return np.log(np.add(np.add(np.add(np.multiply(linFunc(t, I0, τ_1), c_1), 
                                        np.multiply(linFunc(t, I0, τ_2), c_2)), 
                                 np.multiply(linFunc(t, I0, τ_3), c_3)), 
-                         np.multiply(linFunc(t, I0, τ_4), c_4)))
+                         np.multiply(linFunc(t, I0, τ_4), c_4)))
```

### Comparing `lifetimefitting-0.0.15/app/lifetimefitting/gui.py` & `lifetimefitting-0.0.17/app/funcs/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt6 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtWidgets
 
 
 class Ui_Form(object):
     def setupUi(self, Form):
         Form.setObjectName("Form")
         Form.setEnabled(True)
         Form.resize(1024, 900)
@@ -94,16 +94,16 @@
         self.maxIter_widg.setMinimum(1000)
         self.maxIter_widg.setMaximum(100000000)
         self.maxIter_widg.setSingleStep(1000)
         self.maxIter_widg.setProperty("value", 5000)
         self.maxIter_widg.setObjectName("maxIter_widg")
         self.verticalLayout.addWidget(self.maxIter_widg)
         self.startOffset_widg = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
+        self.startOffset_widg.setMaximum(999999)
         self.startOffset_widg.setObjectName("startOffset_widg")
-        self.startOffset_widg.setMaximum(10000)
         self.verticalLayout.addWidget(self.startOffset_widg)
         self.maxTime_widg = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
         self.maxTime_widg.setMaximum(9999999)
         self.maxTime_widg.setProperty("value", 1000)
         self.maxTime_widg.setObjectName("maxTime_widg")
         self.verticalLayout.addWidget(self.maxTime_widg)
         self.expCount_widg = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
@@ -114,23 +114,34 @@
         self.expCount_widg.setObjectName("expCount_widg")
         self.verticalLayout.addWidget(self.expCount_widg)
         self.horizontalLayout.addLayout(self.verticalLayout)
         self.verticalLayout_5.addLayout(self.horizontalLayout)
         self.label_3 = QtWidgets.QLabel(parent=self.verticalGroupBox)
         self.label_3.setObjectName("label_3")
         self.verticalLayout_5.addWidget(self.label_3)
+        self.horizontalLayout_6 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_6.setObjectName("horizontalLayout_6")
         self.max_x = QtWidgets.QSlider(parent=self.verticalGroupBox)
-        self.max_x.setMaximum(300)
+        self.max_x.setMaximum(500)
         self.max_x.setProperty("value", 20)
         self.max_x.setSliderPosition(20)
         self.max_x.setOrientation(QtCore.Qt.Orientation.Horizontal)
         self.max_x.setInvertedAppearance(False)
         self.max_x.setInvertedControls(False)
+        self.max_x.setTickPosition(QtWidgets.QSlider.TickPosition.TicksBelow)
+        self.max_x.setTickInterval(100)
         self.max_x.setObjectName("max_x")
-        self.verticalLayout_5.addWidget(self.max_x)
+        self.horizontalLayout_6.addWidget(self.max_x)
+        self.max_x_out = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
+        self.max_x_out.setButtonSymbols(QtWidgets.QAbstractSpinBox.ButtonSymbols.NoButtons)
+        self.max_x_out.setMaximum(500)
+        self.max_x_out.setValue(20)
+        self.max_x_out.setObjectName("max_x_out")
+        self.horizontalLayout_6.addWidget(self.max_x_out)
+        self.verticalLayout_5.addLayout(self.horizontalLayout_6)
         self.logFit_widg = QtWidgets.QCheckBox(parent=self.verticalGroupBox)
         self.logFit_widg.setEnabled(True)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.logFit_widg.sizePolicy().hasHeightForWidth())
         self.logFit_widg.setSizePolicy(sizePolicy)
@@ -147,16 +158,14 @@
         self.scaled_widg.setCheckable(True)
         self.scaled_widg.setChecked(True)
         self.scaled_widg.setObjectName("scaled_widg")
         self.verticalLayout_5.addWidget(self.scaled_widg)
         self.fit_button = QtWidgets.QPushButton(parent=self.verticalGroupBox)
         self.fit_button.setObjectName("fit_button")
         self.verticalLayout_5.addWidget(self.fit_button)
-        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.verticalLayout_5.addItem(spacerItem)
         self.label_4 = QtWidgets.QLabel(parent=self.verticalGroupBox)
         self.label_4.setObjectName("label_4")
         self.verticalLayout_5.addWidget(self.label_4)
         self.text_output = QtWidgets.QTextEdit(parent=self.verticalGroupBox)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
@@ -197,17 +206,17 @@
         self.groupBox_4.setTitle(_translate("Form", "Input"))
         self.trf_browse.setText(_translate("Form", "Browse for TRF"))
         self.irf_browse.setText(_translate("Form", "Browse for IRF"))
         self.groupBox.setTitle(_translate("Form", "Fitting"))
         self.label.setText(_translate("Form", "Bin Width (ps)"))
         self.label_2.setText(_translate("Form", "Maximum Fitting Iterations"))
         self.label_5.setText(_translate("Form", "Offset for the Starting Bin"))
-        self.label_6.setText(_translate("Form", "Minimum Time (ns)"))
+        self.label_6.setText(_translate("Form", "Maximum Time to Fit (ns)"))
         self.label_24.setText(_translate("Form", "Number of Decays to fit"))
         self.label_3.setText(_translate("Form", "Maximum Time to Plot (ns)"))
         self.logFit_widg.setText(_translate("Form", "Fit in Log Space"))
         self.plotIRF_widg.setText(_translate("Form", "Plot the IRF"))
         self.scaled_widg.setText(_translate("Form", "Plot the Decays scaled by Their Coefficients"))
         self.fit_button.setText(_translate("Form", "Fit"))
         self.label_4.setText(_translate("Form", "Output"))
         self.plot_browse.setText(_translate("Form", "Save Image"))
-        self.csv_browse.setText(_translate("Form", "Save CSV"))
+        self.csv_browse.setText(_translate("Form", "Save CSV"))
```

### Comparing `lifetimefitting-0.0.15/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.17/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.15
+Version: 0.0.17
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.15/setup.py` & `lifetimefitting-0.0.17/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.15",
+    version = "0.0.17",
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
-    install_requires=['matplotlib', 'numpy', 'scipy', 'pyqt6'],
+    install_requires=['matplotlib', 'numpy', 'scipy', 'pyqt6', 'phdimporter'],
     python_requires = ">=3.8",
-)
+)
```

