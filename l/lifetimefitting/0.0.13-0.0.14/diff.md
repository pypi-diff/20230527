# Comparing `tmp/lifetimefitting-0.0.13.tar.gz` & `tmp/lifetimefitting-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifetimefitting-0.0.13.tar", last modified: Sat May 27 01:46:13 2023, max compression
+gzip compressed data, was "lifetimefitting-0.0.14.tar", last modified: Sat May 27 02:04:58 2023, max compression
```

## Comparing `lifetimefitting-0.0.13.tar` & `lifetimefitting-0.0.14.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:46:13.778628 lifetimefitting-0.0.13/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 01:46:13.778628 lifetimefitting-0.0.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:46:13.774628 lifetimefitting-0.0.13/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:46:13.774628 lifetimefitting-0.0.13/app/lifetimefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/app/lifetimefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/app/lifetimefitting/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/app/lifetimefitting/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/app/lifetimefitting/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/app/lifetimefitting/phd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:46:13.778628 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 01:46:13.000000 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-27 01:46:13.000000 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 01:46:13.000000 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 01:46:13.000000 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 01:46:13.000000 lifetimefitting-0.0.13/app/lifetimefitting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 01:46:13.778628 lifetimefitting-0.0.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-27 01:46:01.000000 lifetimefitting-0.0.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:04:58.220316 lifetimefitting-0.0.14/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 02:04:58.216316 lifetimefitting-0.0.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:04:58.216316 lifetimefitting-0.0.14/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:04:58.216316 lifetimefitting-0.0.14/app/lifetimefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/app/lifetimefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/app/lifetimefitting/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/app/lifetimefitting/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/app/lifetimefitting/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/app/lifetimefitting/phd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:04:58.216316 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 02:04:58.000000 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-27 02:04:58.000000 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:04:58.000000 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 02:04:58.000000 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 02:04:58.000000 lifetimefitting-0.0.14/app/lifetimefitting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:04:58.220316 lifetimefitting-0.0.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-27 02:04:45.000000 lifetimefitting-0.0.14/setup.py
```

### Comparing `lifetimefitting-0.0.13/LICENSE.md` & `lifetimefitting-0.0.14/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.13/PKG-INFO` & `lifetimefitting-0.0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.13
+Version: 0.0.14
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.13/README.md` & `lifetimefitting-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.13/app/lifetimefitting/__main__.py` & `lifetimefitting-0.0.14/app/lifetimefitting/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,17 +109,17 @@
     x = x[:index]
     y = y[:index]
 
     if plot:
         if ui.plotIRF_widg.isChecked() and plot:
             ui.axList += ui.ax3.plot([i*binSize*1e-3 for i in range(len(irf))], irf, c='g')
 
-        x_func = np.arange(-2, ui.max_x_widg.value(), 0.01)
+        x_func = np.arange(-2, ui.max_x.value(), 0.01)
         # Log Plot
-        ui.ax1.set_xlim(-2, ui.max_x_widg.value())
+        ui.ax1.set_xlim(-2, ui.max_x.value())
         ui.axList += [ui.ax1.axvline(cutoff, c='r', lw=0.5)]
         ui.axList += [ui.ax1.scatter(x_raw, y_raw, s=0.1, c='b')]
         # Linear plot
         ui.ax3.set_ylim(-300, max(y_raw)+300, auto=False)
         ui.axList += [ui.ax3.axvline(cutoff, c='r', lw=0.5)]
         ui.axList += [ui.ax3.scatter(x_raw, y_raw, s=0.1, c='b')]
 
@@ -252,24 +252,24 @@
     ui.ax4.set_xlabel('Time (ns)')
     ui.ax4.set_ylabel('Residuals\n(lin)')
     ui.ax4.axvline(0, c='k', lw=0.5)
     ui.ax4.axhline(0, c='k', lw=0.5)
 
 def savePlot():
     save_plot_dialog = QFileDialog()
-    save_plot_dialog.setFileMode(QFileDialog.AnyFile)
+    # save_plot_dialog.setFileMode(QFileDialog.AnyFile)
     name = save_plot_dialog.getSaveFileName(filter="PNG Image (*.png);;SVG Image (*.svg);;PDF Document (*.pdf)")[0]
     if name != '':
-        plt.savefig(name)
+        plt.savefig(name, dpi=900)
 
 def saveCSV():
     global csv
     if 'csv' in globals():
         save_csv_dialog = QFileDialog()
-        save_csv_dialog.setFileMode(QFileDialog.AnyFile)
+        # save_csv_dialog.setFileMode(QFileDialog.AnyFile)
         name = save_csv_dialog.getSaveFileName(filter="CSV Sheet (*.csv)")[0]
         if name != '':
             with open(name, 'w+') as f:
                 f.writelines(csv)
 
 if __name__ == "__main__":
     import sys
@@ -277,17 +277,17 @@
     Form = QtWidgets.QWidget()
     ui = Ui_Form()
     ui.setupUi(Form)
     setupPlot()
 
     # file loading
     file_dialog = QFileDialog()
-    file_dialog.setFileMode(QFileDialog.ExistingFile)
+    # file_dialog.setFileMode(QFileDialog.AnyFile)
     ui.trf_browse.clicked.connect(trf_browse)
     ui.irf_browse.clicked.connect(irf_browse)
     ui.plot_browse.clicked.connect(savePlot)
     ui.csv_browse.clicked.connect(saveCSV)
 
     ui.fit_button.clicked.connect(plotFL)
 
     Form.show()
-    sys.exit(app.exec_())
+    sys.exit(app.exec())
```

### Comparing `lifetimefitting-0.0.13/app/lifetimefitting/funcs.py` & `lifetimefitting-0.0.14/app/lifetimefitting/funcs.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.13/app/lifetimefitting/gui.py` & `lifetimefitting-0.0.14/app/lifetimefitting/gui.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
+
 
 class Ui_Form(object):
     def setupUi(self, Form):
         Form.setObjectName("Form")
         Form.setEnabled(True)
         Form.resize(1024, 900)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Maximum)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Maximum)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(Form.sizePolicy().hasHeightForWidth())
         Form.setSizePolicy(sizePolicy)
         Form.setMinimumSize(QtCore.QSize(700, 665))
         self.verticalLayout_11 = QtWidgets.QVBoxLayout(Form)
         self.verticalLayout_11.setObjectName("verticalLayout_11")
-        self.groupBox_4 = QtWidgets.QGroupBox(Form)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Maximum)
+        self.groupBox_4 = QtWidgets.QGroupBox(parent=Form)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Maximum)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.groupBox_4.sizePolicy().hasHeightForWidth())
         self.groupBox_4.setSizePolicy(sizePolicy)
         self.groupBox_4.setObjectName("groupBox_4")
         self.horizontalLayout_5 = QtWidgets.QHBoxLayout(self.groupBox_4)
         self.horizontalLayout_5.setObjectName("horizontalLayout_5")
         self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_2.setObjectName("horizontalLayout_2")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout()
         self.verticalLayout_4.setObjectName("verticalLayout_4")
-        self.trf_file = QtWidgets.QLineEdit(self.groupBox_4)
+        self.trf_file = QtWidgets.QLineEdit(parent=self.groupBox_4)
         self.trf_file.setReadOnly(True)
         self.trf_file.setObjectName("trf_file")
         self.verticalLayout_4.addWidget(self.trf_file)
-        self.irf_file = QtWidgets.QLineEdit(self.groupBox_4)
+        self.irf_file = QtWidgets.QLineEdit(parent=self.groupBox_4)
         self.irf_file.setReadOnly(True)
         self.irf_file.setObjectName("irf_file")
         self.verticalLayout_4.addWidget(self.irf_file)
         self.horizontalLayout_2.addLayout(self.verticalLayout_4)
         self.verticalLayout_7 = QtWidgets.QVBoxLayout()
         self.verticalLayout_7.setObjectName("verticalLayout_7")
-        self.trf_browse = QtWidgets.QPushButton(self.groupBox_4)
+        self.trf_browse = QtWidgets.QPushButton(parent=self.groupBox_4)
         self.trf_browse.setAcceptDrops(True)
         self.trf_browse.setObjectName("trf_browse")
         self.verticalLayout_7.addWidget(self.trf_browse)
-        self.irf_browse = QtWidgets.QPushButton(self.groupBox_4)
+        self.irf_browse = QtWidgets.QPushButton(parent=self.groupBox_4)
         self.irf_browse.setAcceptDrops(True)
         self.irf_browse.setObjectName("irf_browse")
         self.verticalLayout_7.addWidget(self.irf_browse)
         self.horizontalLayout_2.addLayout(self.verticalLayout_7)
         self.horizontalLayout_5.addLayout(self.horizontalLayout_2)
         self.verticalLayout_11.addWidget(self.groupBox_4)
-        self.groupBox = QtWidgets.QGroupBox(Form)
+        self.groupBox = QtWidgets.QGroupBox(parent=Form)
         self.groupBox.setObjectName("groupBox")
         self.horizontalLayout_4 = QtWidgets.QHBoxLayout(self.groupBox)
         self.horizontalLayout_4.setObjectName("horizontalLayout_4")
-        self.verticalGroupBox = QtWidgets.QGroupBox(self.groupBox)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Preferred)
+        self.verticalGroupBox = QtWidgets.QGroupBox(parent=self.groupBox)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Maximum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.verticalGroupBox.sizePolicy().hasHeightForWidth())
         self.verticalGroupBox.setSizePolicy(sizePolicy)
         self.verticalGroupBox.setObjectName("verticalGroupBox")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.verticalGroupBox)
-        self.verticalLayout_5.setSizeConstraint(QtWidgets.QLayout.SetDefaultConstraint)
+        self.verticalLayout_5.setSizeConstraint(QtWidgets.QLayout.SizeConstraint.SetDefaultConstraint)
         self.verticalLayout_5.setContentsMargins(-1, 10, -1, -1)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.horizontalLayout = QtWidgets.QHBoxLayout()
         self.horizontalLayout.setObjectName("horizontalLayout")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout()
         self.verticalLayout_2.setObjectName("verticalLayout_2")
-        self.label = QtWidgets.QLabel(self.verticalGroupBox)
+        self.label = QtWidgets.QLabel(parent=self.verticalGroupBox)
         self.label.setObjectName("label")
         self.verticalLayout_2.addWidget(self.label)
-        self.label_2 = QtWidgets.QLabel(self.verticalGroupBox)
+        self.label_2 = QtWidgets.QLabel(parent=self.verticalGroupBox)
         self.label_2.setObjectName("label_2")
         self.verticalLayout_2.addWidget(self.label_2)
-        self.label_5 = QtWidgets.QLabel(self.verticalGroupBox)
+        self.label_5 = QtWidgets.QLabel(parent=self.verticalGroupBox)
         self.label_5.setObjectName("label_5")
         self.verticalLayout_2.addWidget(self.label_5)
-        self.label_6 = QtWidgets.QLabel(self.verticalGroupBox)
+        self.label_6 = QtWidgets.QLabel(parent=self.verticalGroupBox)
         self.label_6.setObjectName("label_6")
         self.verticalLayout_2.addWidget(self.label_6)
-        self.label_24 = QtWidgets.QLabel(self.verticalGroupBox)
+        self.label_24 = QtWidgets.QLabel(parent=self.verticalGroupBox)
         self.label_24.setObjectName("label_24")
         self.verticalLayout_2.addWidget(self.label_24)
         self.horizontalLayout.addLayout(self.verticalLayout_2)
         self.verticalLayout = QtWidgets.QVBoxLayout()
         self.verticalLayout.setObjectName("verticalLayout")
-        self.binSize_widg = QtWidgets.QDoubleSpinBox(self.verticalGroupBox)
+        self.binSize_widg = QtWidgets.QDoubleSpinBox(parent=self.verticalGroupBox)
         self.binSize_widg.setMaximum(9999999.0)
         self.binSize_widg.setObjectName("binSize_widg")
         self.verticalLayout.addWidget(self.binSize_widg)
-        self.maxIter_widg = QtWidgets.QSpinBox(self.verticalGroupBox)
+        self.maxIter_widg = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
         self.maxIter_widg.setMinimum(1000)
         self.maxIter_widg.setMaximum(100000000)
         self.maxIter_widg.setSingleStep(1000)
         self.maxIter_widg.setProperty("value", 5000)
         self.maxIter_widg.setObjectName("maxIter_widg")
         self.verticalLayout.addWidget(self.maxIter_widg)
-        self.startOffset_widg = QtWidgets.QSpinBox(self.verticalGroupBox)
-        self.startOffset_widg.setMaximum(9999999)
+        self.startOffset_widg = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
         self.startOffset_widg.setObjectName("startOffset_widg")
         self.verticalLayout.addWidget(self.startOffset_widg)
-        self.maxTime_widg = QtWidgets.QSpinBox(self.verticalGroupBox)
+        self.maxTime_widg = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
         self.maxTime_widg.setMaximum(9999999)
         self.maxTime_widg.setProperty("value", 1000)
         self.maxTime_widg.setObjectName("maxTime_widg")
         self.verticalLayout.addWidget(self.maxTime_widg)
-        self.expCount_widg = QtWidgets.QSpinBox(self.verticalGroupBox)
+        self.expCount_widg = QtWidgets.QSpinBox(parent=self.verticalGroupBox)
         self.expCount_widg.setWrapping(False)
         self.expCount_widg.setMinimum(1)
         self.expCount_widg.setMaximum(4)
         self.expCount_widg.setProperty("value", 1)
         self.expCount_widg.setObjectName("expCount_widg")
         self.verticalLayout.addWidget(self.expCount_widg)
         self.horizontalLayout.addLayout(self.verticalLayout)
         self.verticalLayout_5.addLayout(self.horizontalLayout)
-        self.label_3 = QtWidgets.QLabel(self.verticalGroupBox)
+        self.label_3 = QtWidgets.QLabel(parent=self.verticalGroupBox)
         self.label_3.setObjectName("label_3")
         self.verticalLayout_5.addWidget(self.label_3)
-        self.max_x_widg = QtWidgets.QSlider(self.verticalGroupBox)
-        self.max_x_widg.setMaximum(300)
-        self.max_x_widg.setProperty("value", 20)
-        self.max_x_widg.setSliderPosition(20)
-        self.max_x_widg.setOrientation(QtCore.Qt.Horizontal)
-        self.max_x_widg.setInvertedAppearance(False)
-        self.max_x_widg.setInvertedControls(False)
-        self.max_x_widg.setObjectName("max_x_widg")
-        self.verticalLayout_5.addWidget(self.max_x_widg)
-        self.logFit_widg = QtWidgets.QCheckBox(self.verticalGroupBox)
+        self.max_x = QtWidgets.QSlider(parent=self.verticalGroupBox)
+        self.max_x.setMaximum(300)
+        self.max_x.setProperty("value", 20)
+        self.max_x.setSliderPosition(20)
+        self.max_x.setOrientation(QtCore.Qt.Orientation.Horizontal)
+        self.max_x.setInvertedAppearance(False)
+        self.max_x.setInvertedControls(False)
+        self.max_x.setObjectName("max_x")
+        self.verticalLayout_5.addWidget(self.max_x)
+        self.logFit_widg = QtWidgets.QCheckBox(parent=self.verticalGroupBox)
         self.logFit_widg.setEnabled(True)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.logFit_widg.sizePolicy().hasHeightForWidth())
         self.logFit_widg.setSizePolicy(sizePolicy)
         self.logFit_widg.setCheckable(True)
         self.logFit_widg.setChecked(False)
         self.logFit_widg.setObjectName("logFit_widg")
         self.verticalLayout_5.addWidget(self.logFit_widg)
-        self.plotIRF_widg = QtWidgets.QCheckBox(self.verticalGroupBox)
+        self.plotIRF_widg = QtWidgets.QCheckBox(parent=self.verticalGroupBox)
         self.plotIRF_widg.setCheckable(True)
         self.plotIRF_widg.setChecked(False)
         self.plotIRF_widg.setObjectName("plotIRF_widg")
         self.verticalLayout_5.addWidget(self.plotIRF_widg)
-        self.scaled_widg = QtWidgets.QCheckBox(self.verticalGroupBox)
+        self.scaled_widg = QtWidgets.QCheckBox(parent=self.verticalGroupBox)
         self.scaled_widg.setCheckable(True)
         self.scaled_widg.setChecked(True)
         self.scaled_widg.setObjectName("scaled_widg")
         self.verticalLayout_5.addWidget(self.scaled_widg)
-        self.fit_button = QtWidgets.QPushButton(self.verticalGroupBox)
+        self.fit_button = QtWidgets.QPushButton(parent=self.verticalGroupBox)
         self.fit_button.setObjectName("fit_button")
         self.verticalLayout_5.addWidget(self.fit_button)
-        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.verticalLayout_5.addItem(spacerItem)
-        self.label_4 = QtWidgets.QLabel(self.verticalGroupBox)
+        self.label_4 = QtWidgets.QLabel(parent=self.verticalGroupBox)
         self.label_4.setObjectName("label_4")
         self.verticalLayout_5.addWidget(self.label_4)
-        self.text_output = QtWidgets.QTextEdit(self.verticalGroupBox)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+        self.text_output = QtWidgets.QTextEdit(parent=self.verticalGroupBox)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.text_output.sizePolicy().hasHeightForWidth())
         self.text_output.setSizePolicy(sizePolicy)
         self.text_output.setObjectName("text_output")
         self.verticalLayout_5.addWidget(self.text_output)
         self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_3.setObjectName("horizontalLayout_3")
-        self.plot_browse = QtWidgets.QPushButton(self.verticalGroupBox)
+        self.plot_browse = QtWidgets.QPushButton(parent=self.verticalGroupBox)
         self.plot_browse.setAcceptDrops(True)
         self.plot_browse.setObjectName("plot_browse")
         self.horizontalLayout_3.addWidget(self.plot_browse)
-        self.csv_browse = QtWidgets.QPushButton(self.verticalGroupBox)
+        self.csv_browse = QtWidgets.QPushButton(parent=self.verticalGroupBox)
         self.csv_browse.setAcceptDrops(True)
         self.csv_browse.setObjectName("csv_browse")
         self.horizontalLayout_3.addWidget(self.csv_browse)
         self.verticalLayout_5.addLayout(self.horizontalLayout_3)
         self.horizontalLayout_4.addWidget(self.verticalGroupBox)
-        self.frame = QtWidgets.QFrame(self.groupBox)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.frame = QtWidgets.QFrame(parent=self.groupBox)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.frame.sizePolicy().hasHeightForWidth())
         self.frame.setSizePolicy(sizePolicy)
-        self.frame.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.frame.setFrameShadow(QtWidgets.QFrame.Raised)
+        self.frame.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.frame.setFrameShadow(QtWidgets.QFrame.Shadow.Raised)
         self.frame.setObjectName("frame")
         self.horizontalLayout_4.addWidget(self.frame)
         self.verticalLayout_11.addWidget(self.groupBox)
 
         self.retranslateUi(Form)
         QtCore.QMetaObject.connectSlotsByName(Form)
 
@@ -196,18 +196,17 @@
         self.groupBox_4.setTitle(_translate("Form", "Input"))
         self.trf_browse.setText(_translate("Form", "Browse for TRF"))
         self.irf_browse.setText(_translate("Form", "Browse for IRF"))
         self.groupBox.setTitle(_translate("Form", "Fitting"))
         self.label.setText(_translate("Form", "Bin Width (ps)"))
         self.label_2.setText(_translate("Form", "Maximum Fitting Iterations"))
         self.label_5.setText(_translate("Form", "Offset for the Starting Bin"))
-        self.label_6.setText(_translate("Form", "Maximum Time to fit (ns)"))
+        self.label_6.setText(_translate("Form", "Minimum Time (ns)"))
         self.label_24.setText(_translate("Form", "Number of Decays to fit"))
         self.label_3.setText(_translate("Form", "Maximum Time to Plot (ns)"))
         self.logFit_widg.setText(_translate("Form", "Fit in Log Space"))
-        self.plotIRF_widg.setText(_translate("Form", "Plot the IRF (This will not be aligned to anything)"))
+        self.plotIRF_widg.setText(_translate("Form", "Plot the IRF"))
         self.scaled_widg.setText(_translate("Form", "Plot the Decays scaled by Their Coefficients"))
         self.fit_button.setText(_translate("Form", "Fit"))
         self.label_4.setText(_translate("Form", "Output"))
         self.plot_browse.setText(_translate("Form", "Save Image"))
         self.csv_browse.setText(_translate("Form", "Save CSV"))
-
```

### Comparing `lifetimefitting-0.0.13/app/lifetimefitting/phd.py` & `lifetimefitting-0.0.14/app/lifetimefitting/phd.py`

 * *Files identical despite different names*

### Comparing `lifetimefitting-0.0.13/app/lifetimefitting.egg-info/PKG-INFO` & `lifetimefitting-0.0.14/app/lifetimefitting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifetimefitting
-Version: 0.0.13
+Version: 0.0.14
 Summary: PicoHarp TCSPC lifetime fitting tool
 Home-page: https://github.com/adreasnow/LifetimeFittingTool
 Author: Adrea Snow
 Author-email: adrea.snow@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lifetimefitting-0.0.13/setup.py` & `lifetimefitting-0.0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "lifetimefitting",
-    version = "0.0.13",
+    version = "0.0.14",
     author = "Adrea Snow",
     author_email = "adrea.snow@gmail.com",
     description = "PicoHarp TCSPC lifetime fitting tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adreasnow/LifetimeFittingTool",
     classifiers = [
```

