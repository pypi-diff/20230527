# Comparing `tmp/vision6D-0.0.7.tar.gz` & `tmp/vision6D-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.0.7.tar", last modified: Mon May 15 22:54:36 2023, max compression
+gzip compressed data, was "dist\vision6D-0.0.8.tar", last modified: Sat May 27 00:10:38 2023, max compression
```

## Comparing `vision6D-0.0.7.tar` & `vision6D-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 22:54:36.166899 vision6D-0.0.7/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1603 2023-05-15 22:54:36.166899 vision6D-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-15 22:13:50.000000 vision6D-0.0.7/README.md
--rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0     1918 2023-05-15 22:54:36.172901 vision6D-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      132 2023-05-15 22:38:05.000000 vision6D-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:54:36.097901 vision6D-0.0.7/test/
--rw-rw-rw-   0        0        0    21974 2023-05-14 22:36:01.000000 vision6D-0.0.7/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.0.7/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:54:36.122895 vision6D-0.0.7/vision6D/
--rw-rw-rw-   0        0        0    41677 2023-05-15 22:14:12.000000 vision6D-0.0.7/vision6D/GUI.py
--rw-rw-rw-   0        0        0      939 2023-05-15 22:21:02.000000 vision6D-0.0.7/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.0.7/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-14 22:36:01.000000 vision6D-0.0.7/vision6D/config.py
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.0.7/vision6D/interface.py
--rw-rw-rw-   0        0        0    28470 2023-05-15 22:13:50.000000 vision6D-0.0.7/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.0.7/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14100 2023-05-15 22:51:44.000000 vision6D-0.0.7/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.0.7/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.0.7/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:54:36.164896 vision6D-0.0.7/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-05-15 22:54:35.000000 vision6D-0.0.7/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-05-15 22:54:35.000000 vision6D-0.0.7/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 22:54:35.000000 vision6D-0.0.7/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-05-15 22:54:35.000000 vision6D-0.0.7/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 22:54:35.000000 vision6D-0.0.7/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 00:10:38.613222 vision6D-0.0.8/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1603 2023-05-27 00:10:38.614312 vision6D-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-27 00:06:55.000000 vision6D-0.0.8/README.md
+-rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1918 2023-05-27 00:10:38.619226 vision6D-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      366 2023-05-27 00:07:57.000000 vision6D-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:10:38.422145 vision6D-0.0.8/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.0.8/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.0.8/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:10:38.467145 vision6D-0.0.8/vision6D/
+-rw-rw-rw-   0        0        0    45165 2023-05-27 00:06:55.000000 vision6D-0.0.8/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      939 2023-05-27 00:06:55.000000 vision6D-0.0.8/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.0.8/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-27 00:06:55.000000 vision6D-0.0.8/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:10:38.600224 vision6D-0.0.8/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.0.8/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.0.8/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.0.8/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.0.8/vision6D/interface.py
+-rw-rw-rw-   0        0        0    27855 2023-05-27 00:06:55.000000 vision6D-0.0.8/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.0.8/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.0.8/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.0.8/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.0.8/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:10:38.538156 vision6D-0.0.8/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-05-27 00:10:37.000000 vision6D-0.0.8/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-27 00:10:37.000000 vision6D-0.0.8/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 00:10:37.000000 vision6D-0.0.8/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      248 2023-05-27 00:10:37.000000 vision6D-0.0.8/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 00:10:37.000000 vision6D-0.0.8/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.0.7/LICENSE` & `vision6D-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.7/PKG-INFO` & `vision6D-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.0.7
+Version: 0.0.8
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.0.7/README.md` & `vision6D-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.7/setup.cfg` & `vision6D-0.0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e37 0d0a 7572  sion = 0.0.7..ur
+00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 7572  sion = 0.0.8..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.0.7/test/test_create_dataset.py` & `vision6D-0.0.8/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.7/test/test_projection.py` & `vision6D-0.0.8/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.7/vision6D/GUI.py` & `vision6D-0.0.8/vision6D/GUI.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import pyvista as pv
 import functools
 import trimesh
 import pathlib
 import PIL
 import ast
 import json
+import math
 
 # Qt5 import
 from PyQt5 import QtWidgets, QtGui
 from pyvistaqt import QtInteractor, MainWindow
-from PyQt5.QtWidgets import QLabel, QMessageBox, QInputDialog, QFileDialog, QLineEdit, QDialogButtonBox, QFormLayout, QDialog
 from PyQt5.QtCore import Qt, QPoint
 
 # self defined package import
 import vision6D as vis
 
 np.set_printoptions(suppress=True)
 
-class YesNoBox(QMessageBox):
+class YesNoBox(QtWidgets.QMessageBox):
     def __init__(self, *args, **kwargs):
         super(YesNoBox, self).__init__(*args, **kwargs)
         self.canceled = False
 
     def closeEvent(self, event: QtGui.QCloseEvent):
         self.canceled = True
         super(YesNoBox, self).closeEvent(event)
@@ -49,34 +49,34 @@
                 button = QtWidgets.QPushButton(name)
                 button.clicked.connect(lambda _, idx=name: on_button_click(str(idx)))
                 button_grid.addWidget(button, j, i)
                 button_count += 1
 
         self.setLayout(button_grid)
 
-class CameraPropsInputDialog(QDialog):
+class CameraPropsInputDialog(QtWidgets.QDialog):
     def __init__(self, parent=None, 
                     line1=(None, None), 
                     line2=(None, None), 
                     line3=(None, None), 
                     line4=(None, None), 
                     line5=(None, None),
                     line6=(None, None)):
         super().__init__(parent)
 
-        self.args1 = QLineEdit(self, text=str(line1[1]))
-        self.args2 = QLineEdit(self, text=str(line2[1]))
-        self.args3 = QLineEdit(self, text=str(line3[1]))
-        self.args4 = QLineEdit(self, text=str(line4[1]))
-        self.args5 = QLineEdit(self, text=str(line5[1]))
-        self.args6 = QLineEdit(self, text=str(line6[1]))
+        self.args1 = QtWidgets.QLineEdit(self, text=str(line1[1]))
+        self.args2 = QtWidgets.QLineEdit(self, text=str(line2[1]))
+        self.args3 = QtWidgets.QLineEdit(self, text=str(line3[1]))
+        self.args4 = QtWidgets.QLineEdit(self, text=str(line4[1]))
+        self.args5 = QtWidgets.QLineEdit(self, text=str(line5[1]))
+        self.args6 = QtWidgets.QLineEdit(self, text=str(line6[1]))
 
-        buttonBox = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel, self)
+        buttonBox = QtWidgets.QDialogButtonBox(QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel, self)
 
-        layout = QFormLayout(self)
+        layout = QtWidgets.QFormLayout(self)
         layout.addRow(f"{line1[0]}", self.args1)
         layout.addRow(f"{line2[0]}", self.args2)
         layout.addRow(f"{line3[0]}", self.args3)
         layout.addRow(f"{line4[0]}", self.args4)
         layout.addRow(f"{line5[0]}", self.args5)
         layout.addRow(f"{line6[0]}", self.args6)
         layout.addWidget(buttonBox)
@@ -87,47 +87,79 @@
     def getInputs(self):
         return (self.args1.text(), 
                 self.args2.text(), 
                 self.args3.text(),
                 self.args4.text(),
                 self.args5.text(),
                 self.args6.text())
+    
+class GetTextDialog(QtWidgets.QDialog):
+    def __init__(self, parent=None):
+        super(GetTextDialog, self).__init__(parent)
+        
+        self.setWindowTitle("Vision6D")
+        self.introLabel = QtWidgets.QLabel("Input the Ground Truth Pose:")
+        self.textEdit = QtWidgets.QTextEdit(self)
+        self.textEdit.setPlainText(f"[[1, 0, 0, 0], \n[0, 1, 0, 0], \n[0, 0, 1, 0], \n[0, 0, 0, 1]]")
+        self.btnSubmit = QtWidgets.QPushButton("Submit", self)
+        self.btnSubmit.clicked.connect(self.submit_text)
+
+        layout = QtWidgets.QVBoxLayout(self)
+        layout.addWidget(self.introLabel)
+        layout.addWidget(self.textEdit)
+        layout.addWidget(self.btnSubmit)
+
+    def submit_text(self):
+        self.user_text = self.textEdit.toPlainText()
+        self.accept()
+
+    def get_text(self):
+        return self.user_text
 
 class MyMainWindow(MainWindow):
     def __init__(self, parent=None):
         QtWidgets.QMainWindow.__init__(self, parent)
 
         # Set up the main window layout
         self.setWindowTitle("Vision6D")
         self.window_size = (1920, 1080)
         self.main_widget = QtWidgets.QWidget()
         self.setCentralWidget(self.main_widget)
         self.setAcceptDrops(True)
 
         self.track_actors_names = []
-        self.button_group_track_actors_names = QtWidgets.QButtonGroup(self)
+        self.button_group_actors_names = QtWidgets.QButtonGroup(self)
 
         # Set panel bar
         self.set_panel_bar()
         
         # Set menu bar
         self.set_menu_bars()
 
         # Create the plotter
         self.create_plotter()
+        
+        # Set the camera
+        self.fx = 50000
+        self.fy = 50000
+        self.cx = 960
+        self.cy = 540
+        self.cam_viewup = (0, -1, 0)
+        self.cam_position = -500
+        self.set_camera_props()
 
         # Set up the main layout with the left panel and the render window using QSplitter
         self.main_layout = QtWidgets.QHBoxLayout(self.main_widget)
         self.splitter = QtWidgets.QSplitter()
         self.splitter.addWidget(self.panel_widget)
         self.splitter.addWidget(self.plotter)
         self.main_layout.addWidget(self.splitter)
 
         # Add a QLabel as an overlay hint label
-        self.hintLabel = QLabel(self.plotter)
+        self.hintLabel = QtWidgets.QLabel(self.plotter)
         self.hintLabel.setText("Drag and drop a file here...")
         self.hintLabel.setStyleSheet("""
                                     color: white; 
                                     background-color: rgba(0, 0, 0, 127); 
                                     padding: 10px;
                                     border: 2px dashed gray;
                                     """)
@@ -147,46 +179,47 @@
         for url in e.mimeData().urls():
             file_path = url.toLocalFile()
             if file_path.endswith(('.mesh', '.ply', '.stl', '.obj', '.off', '.dae', '.fbx', '.3ds', '.x3d')):  # add mesh
                 self.mesh_path = file_path
                 self.add_mesh_file(prompt=False)
             elif file_path.endswith(('.png', '.jpg')):  # add image/mask
                 yes_no_box = YesNoBox()
-                yes_no_box.setIcon(QMessageBox.Question)
+                yes_no_box.setIcon(QtWidgets.QMessageBox.Question)
                 yes_no_box.setWindowTitle("Vision6D")
                 yes_no_box.setText("Do you want to load the image as mask?")
-                yes_no_box.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
+                yes_no_box.setStandardButtons(QtWidgets.QMessageBox.Yes | QtWidgets.QMessageBox.No)
                 button_clicked = yes_no_box.exec_()
                 if not yes_no_box.canceled:
-                    if button_clicked == QMessageBox.Yes:
+                    if button_clicked == QtWidgets.QMessageBox.Yes:
                         self.mask_path = file_path
                         self.add_mask_file(prompt=False)
-                    elif button_clicked == QMessageBox.No:
+                    elif button_clicked == QtWidgets.QMessageBox.No:
                         self.image_path = file_path
                         self.add_image_file(prompt=False)
             elif file_path.endswith('.npy'):
                 self.pose_path = file_path
                 self.add_pose_file(prompt=False)
             else:
-                QMessageBox.warning(self, 'vision6D', "File format is not supported!", QMessageBox.Ok, QMessageBox.Ok)
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "File format is not supported!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                 return 0
 
     def resizeEvent(self, e):
         x = (self.plotter.size().width() - self.hintLabel.width()) // 2
         y = (self.plotter.size().height() - self.hintLabel.height()) // 2
         self.initialHintLabelPosition = self.hintLabel.pos()
         self.hintLabel.move(x, y)
         super().resizeEvent(e)
 
     # ^Main Menu
     def set_menu_bars(self):
         mainMenu = self.menuBar()
         # simple dialog to record users input info
-        self.input_dialog = QInputDialog()
-        self.file_dialog = QFileDialog()
+        self.input_dialog = QtWidgets.QInputDialog()
+        self.file_dialog = QtWidgets.QFileDialog()
+        self.get_text_dialog = GetTextDialog()
         
         self.image_path = None
         self.mask_path = None
         self.mesh_path = None
         self.pose_path = None
         self.meshdict = {}
             
@@ -232,57 +265,87 @@
         PnPMenu = mainMenu.addMenu('Run')
         PnPMenu.addAction('EPnP with mesh', self.epnp_mesh)
         epnp_nocs_mask = functools.partial(self.epnp_mask, True)
         PnPMenu.addAction('EPnP with nocs mask', epnp_nocs_mask)
         epnp_latlon_mask = functools.partial(self.epnp_mask, False)
         PnPMenu.addAction('EPnP with latlon mask', epnp_latlon_mask)
 
+    def set_camera_extrinsics(self):
+        self.camera.SetPosition((0,0,self.cam_position))
+        self.camera.SetFocalPoint((*self.camera.GetWindowCenter(),0)) # Get the camera window center
+        self.camera.SetViewUp(self.cam_viewup)
+    
+    def set_camera_intrinsics(self):
+        
+        # Set camera intrinsic attribute
+        self.camera_intrinsics = np.array([
+            [self.fx, 0, self.cx],
+            [0, self.fy, self.cy],
+            [0, 0, 1]
+        ])
+                
+        # convert the principal point to window center (normalized coordinate system) and set it
+        wcx = -2*(self.cx - float(self.window_size[0])/2) / self.window_size[0]
+        wcy =  2*(self.cy - float(self.window_size[1])/2) / self.window_size[1]
+        self.camera.SetWindowCenter(wcx, wcy) # (0,0)
+        
+        # Setting the view angle in degrees
+        view_angle = (180 / math.pi) * (2.0 * math.atan2(self.window_size[1]/2.0, self.fx)) # or view_angle = np.degrees(2.0 * math.atan2(height/2.0, f)) # focal_length = (1080 / 2.0) / math.tan(math.radians(self.plotter.camera.view_angle / 2))
+        self.camera.SetViewAngle(view_angle) # view angle should be in degrees
+ 
+    def set_camera_props(self):
+        # Set up the camera
+        self.camera = pv.Camera()
+        self.set_camera_intrinsics()
+        self.set_camera_extrinsics()
+        self.plotter.camera = self.camera.copy()
+
     def set_camera(self):
         dialog = CameraPropsInputDialog(
             line1=("Fx", self.fx), 
             line2=("Fy", self.fy), 
             line3=("Cx", self.cx), 
             line4=("Cy", self.cy), 
             line5=("View Up", self.cam_viewup), 
             line6=("Cam Position", self.cam_position))
         if dialog.exec():
             fx, fy, cx, cy, cam_viewup, cam_position = dialog.getInputs()
             pre_fx, pre_fy, pre_cx, pre_cy, pre_cam_viewup, pre_cam_position = self.fx, self.fy, self.cx, self.cy, self.cam_viewup, self.cam_position
             if not (fx == '' or fy == '' or cx == '' or cy == '' or cam_viewup == '' or cam_position == ''):
                 try:
                     self.fx, self.fy, self.cx, self.cy, self.cam_viewup, self.cam_position = ast.literal_eval(fx), ast.literal_eval(fy), ast.literal_eval(cx), ast.literal_eval(cy), ast.literal_eval(cam_viewup), ast.literal_eval(cam_position)
-                    self.set_camera_props(self.fx, self.fy, self.cx, self.cy, self.cam_viewup, self.cam_position)
+                    self.set_camera_props()
                 except:
                     self.fx, self.fy, self.cx, self.cy, self.cam_viewup, self.cam_position = pre_fx, pre_fy, pre_cx, pre_cy, pre_cam_viewup, pre_cam_position
-                    QMessageBox.warning(self, 'vision6D', "Error occured, check the format of the input values", QMessageBox.Ok, QMessageBox.Ok)
+                    QtWidgets.QMessageBox.warning(self, 'vision6D', "Error occured, check the format of the input values", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def set_spacing(self):
-        checked_button = self.button_group_track_actors_names.checkedButton()
+        checked_button = self.button_group_actors_names.checkedButton()
         if checked_button is not None:
             if checked_button.text() == 'image':
                 spacing, ok = self.input_dialog.getText(self, 'Input', "Set Spacing", text=str(self.image_spacing))
                 if ok:
                     try: self.image_spacing = ast.literal_eval(spacing)
-                    except: QMessageBox.warning(self, 'vision6D', "Format is not correct", QMessageBox.Ok, QMessageBox.Ok)
+                    except: QtWidgets.QMessageBox.warning(self, 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                     self.add_image(self.image_path)
             elif checked_button.text() == 'mask':
                 spacing, ok = self.input_dialog.getText(self, 'Input', "Set Spacing", text=str(self.mask_spacing))
                 if ok:
                     try: self.mask_spacing = ast.literal_eval(spacing)
-                    except: QMessageBox.warning(self, 'vision6D', "Format is not correct", QMessageBox.Ok, QMessageBox.Ok)
+                    except: QtWidgets.QMessageBox.warning(self, 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                     self.add_mask(self.mask_path)
             else:
                 spacing, ok = self.input_dialog.getText(self, 'Input', "Set Spacing", text=str(self.mesh_spacing))
                 if ok:
                     actor_name = checked_button.text()
                     try: self.mesh_spacing = ast.literal_eval(spacing)
-                    except: QMessageBox.warning(self, 'vision6D', "Format is not correct", QMessageBox.Ok, QMessageBox.Ok)
+                    except: QtWidgets.QMessageBox.warning(self, 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                     self.add_mesh(actor_name, self.meshdict[actor_name])
         else:
-            QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def add_workspace(self):
         workspace_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.json)")
         if workspace_path != '':
             self.hintLabel.hide()
             with open(str(workspace_path), 'r') as f: 
                 workspace = json.load(f)
@@ -383,15 +446,15 @@
                 self.mirror_x = False
                 self.mirror_y = True
             elif (curr_image_data == original_image_data[:, ::-1, :][::-1, :, :]).all():
                 self.mirror_x = True
                 self.mirror_y = True
             self.add_image(original_image_data)
         else:
-            QMessageBox.warning(self, 'vision6D', "Need to load an image first!", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
         if self.mask_actor is not None:
             #^ mirror the mask actor
             original_mask_data = np.array(PIL.Image.open(self.mask_path), dtype='uint8')
             if len(original_mask_data.shape) == 2: original_mask_data = original_mask_data[..., None]
             self.add_mask(original_mask_data)
@@ -424,34 +487,34 @@
             self.color_button.setText("Color")
             self.mesh_spacing = [1, 1, 1]
 
         self.plotter.remove_actor(actor)
         self.track_actors_names.remove(name)
         self.output_text.clear(); self.output_text.append(f"Remove actor: <span style='background-color:yellow; color:black;'>{name}</span>")
         # remove the button from the button group
-        self.button_group_track_actors_names.removeButton(button)
+        self.button_group_actors_names.removeButton(button)
         # remove the button from the self.button_layout widget
         self.button_layout.removeWidget(button)
         # offically delete the button
         button.deleteLater()
 
         # clear out the plot if there is no actor
         if self.image_actor is None and self.mask_actor is None and len(self.mesh_actors) == 0: self.clear_plot()
    
     def clear_plot(self):
         
         # Clear out everything in the remove menu
-        for button in self.button_group_track_actors_names.buttons():
+        for button in self.button_group_actors_names.buttons():
             name = button.text()
             if name == 'image': actor = self.image_actor
             elif name == 'mask': actor = self.mask_actor
             else: actor = self.mesh_actors[name]
             self.plotter.remove_actor(actor)
             # remove the button from the button group
-            self.button_group_track_actors_names.removeButton(button)
+            self.button_group_actors_names.removeButton(button)
             # remove the button from the self.button_layout widget
             self.button_layout.removeWidget(button)
             # offically delete the button
             button.deleteLater()
 
         self.hintLabel.show()
 
@@ -487,80 +550,80 @@
         self.ignore_slider_value_change = True
         self.opacity_slider.setValue(100)
         self.ignore_slider_value_change = False
 
     def export_image_plot(self):
 
         if self.image_actor is None:
-            QMessageBox.warning(self, 'vision6D', "Need to load an image first!", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         
-        reply = QMessageBox.question(self,"vision6D", "Reset Camera?", QMessageBox.Yes, QMessageBox.No)
-        if reply == QMessageBox.Yes: camera = self.camera.copy()
+        reply = QtWidgets.QMessageBox.question(self,"vision6D", "Reset Camera?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
+        if reply == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
         else: camera = self.plotter.camera.copy()
 
         self.render.clear()
         image_actor = self.image_actor.copy(deep=True)
         image_actor.GetProperty().opacity = 1
         self.render.add_actor(image_actor, pickable=False, name="image")
         self.render.camera = camera
         self.render.disable()
         self.render.show(auto_close=False)
 
         # obtain the rendered image
         image = self.render.last_image
-        output_path, _ = QFileDialog.getSaveFileName(self, "Save File", "", "Image Files (*.png)")
+        output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Image Files (*.png)")
         if output_path: 
             rendered_image = PIL.Image.fromarray(image)
             rendered_image.save(output_path)
             self.output_text.clear()
             self.output_text.append(f"Export image render to:\n {str(output_path)}")
 
     def export_mask_plot(self):
         if self.mask_actor is None:
-            QMessageBox.warning(self, 'vision6D', "Need to load a mask first!", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a mask first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         
-        reply = QMessageBox.question(self,"vision6D", "Reset Camera?", QMessageBox.Yes, QMessageBox.No)
-        if reply == QMessageBox.Yes: camera = self.camera.copy()
+        reply = QtWidgets.QMessageBox.question(self,"vision6D", "Reset Camera?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
+        if reply == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
         else: camera = self.plotter.camera.copy()
 
         self.render.clear()
         mask_actor = self.mask_actor.copy(deep=True)
         mask_actor.GetProperty().opacity = 1
         self.render.add_actor(mask_actor, pickable=False, name="mask")
         self.render.camera = camera
         self.render.disable()
         self.render.show(auto_close=False)
 
         # obtain the rendered image
         image = self.render.last_image
-        output_path, _ = QFileDialog.getSaveFileName(self, "Save File", "", "Mask Files (*.png)")
+        output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Mask Files (*.png)")
         if output_path:
             rendered_image = PIL.Image.fromarray(image)
             rendered_image.save(output_path)
             self.output_text.clear()
             self.output_text.append(f"Export mask render to:\n {str(output_path)}")
 
     def export_mesh_plot(self, reply_reset_camera=None, reply_render_mesh=None, reply_export_surface=None, save_render=True):
 
         if self.reference is None:
-            QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
         if reply_reset_camera is None and reply_render_mesh is None and reply_export_surface is None:
-            reply_reset_camera = QMessageBox.question(self,"vision6D", "Reset Camera?", QMessageBox.Yes, QMessageBox.No)
-            reply_render_mesh = QMessageBox.question(self,"vision6D", "Only render the reference mesh?", QMessageBox.Yes, QMessageBox.No)
-            reply_export_surface = QMessageBox.question(self,"vision6D", "Export the mesh as surface?", QMessageBox.Yes, QMessageBox.No)
+            reply_reset_camera = QtWidgets.QMessageBox.question(self,"vision6D", "Reset Camera?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
+            reply_render_mesh = QtWidgets.QMessageBox.question(self,"vision6D", "Only render the reference mesh?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
+            reply_export_surface = QtWidgets.QMessageBox.question(self,"vision6D", "Export the mesh as surface?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
             
-        if reply_reset_camera == QMessageBox.Yes: camera = self.camera.copy()
+        if reply_reset_camera == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
         else: camera = self.plotter.camera.copy()
-        if reply_render_mesh == QMessageBox.No: render_all_meshes = True
+        if reply_render_mesh == QtWidgets.QMessageBox.No: render_all_meshes = True
         else: render_all_meshes = False
-        if reply_export_surface == QMessageBox.No: point_clouds = True
+        if reply_export_surface == QtWidgets.QMessageBox.No: point_clouds = True
         else: point_clouds = False
         
         # Clear out the render
         self.render.clear()
 
         for mesh_name, mesh_actor in self.mesh_actors.items():
             if not render_all_meshes:
@@ -578,39 +641,39 @@
         self.render.camera = camera
         self.render.disable(); self.render.show(auto_close=False)
 
         # obtain the rendered image
         image = self.render.last_image
 
         if save_render:
-            output_path, _ = QFileDialog.getSaveFileName(self, "Save File", "", "Mesh Files (*.png)")
+            output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Mesh Files (*.png)")
             if output_path:
                 rendered_image = PIL.Image.fromarray(image)
                 rendered_image.save(output_path)
                 self.output_text.clear()
                 self.output_text.append(f"Export reference mesh render to:\n {str(output_path)}")
 
         return image
 
     def export_segmesh_plot(self):
 
         if self.reference is None:
-            QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         
         if self.mask_actor is None: 
-            QMessageBox.warning(self, 'vision6D', "Need to load a segmentation mask first", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a segmentation mask first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
-        reply_reset_camera = QMessageBox.question(self,"vision6D", "Reset Camera?", QMessageBox.Yes, QMessageBox.No)
-        reply_export_surface = QMessageBox.question(self,"vision6D", "Export the mesh as surface?", QMessageBox.Yes, QMessageBox.No)
+        reply_reset_camera = QtWidgets.QMessageBox.question(self,"vision6D", "Reset Camera?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
+        reply_export_surface = QtWidgets.QMessageBox.question(self,"vision6D", "Export the mesh as surface?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
 
-        if reply_reset_camera == QMessageBox.Yes: camera = self.camera.copy()
+        if reply_reset_camera == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
         else: camera = self.plotter.camera.copy()
-        if reply_export_surface == QMessageBox.No: point_clouds = True
+        if reply_export_surface == QtWidgets.QMessageBox.No: point_clouds = True
         else: point_clouds = False
 
         self.render.clear()
         mask_actor = self.mask_actor.copy(deep=True)
         mask_actor.GetProperty().opacity = 1
         self.render.add_actor(mask_actor, pickable=False, name="mask")
         self.render.camera = camera
@@ -635,29 +698,29 @@
 
         self.render.camera = camera
         self.render.disable(); self.render.show(auto_close=False)
 
         # obtain the rendered image
         image = self.render.last_image
         image = (image * segmask).astype(np.uint8)
-        output_path, _ = QFileDialog.getSaveFileName(self, "Save File", "", "SegMesh Files (*.png)")
+        output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "SegMesh Files (*.png)")
         if output_path:
             rendered_image = PIL.Image.fromarray(image)
             rendered_image.save(output_path)
             self.output_text.clear()
             self.output_text.append(f"Export segmask render:\n to {str(output_path)}")
             
         # return image
 
     def export_pose(self):
         if self.reference is None: 
-            QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         self.update_gt_pose()
-        output_path, _ = QFileDialog.getSaveFileName(self, "Save File", "", "Pose Files (*.npy)")
+        output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Pose Files (*.npy)")
         if output_path:
             np.save(output_path, self.transformation_matrix)
             self.output_text.clear()
             self.output_text.append(f"\nSaved:\n{self.transformation_matrix}\nExport to:\n {str(output_path)}")
 
     # ^Panel
     def set_panel_bar(self):
@@ -694,69 +757,71 @@
             y = (self.plotter.size().height() - self.hintLabel.height()) // 2
             self.hintLabel.move(x, y)
 
     def add_button_actor_name(self, actor_name):
         button = QtWidgets.QPushButton(actor_name)
         button.setCheckable(True)  # Set the button to be checkable
         button.clicked.connect(lambda _, text=actor_name: self.button_actor_name_clicked(text))
+        button.setChecked(True)
         button.setFixedSize(self.display.size().width(), 50)
         self.button_layout.insertWidget(0, button) # insert from the top # self.button_layout.addWidget(button)
-        self.button_group_track_actors_names.addButton(button)
+        self.button_group_actors_names.addButton(button)
+        self.button_actor_name_clicked(actor_name)
 
     def update_color_button_text(self, text, popup):
         self.color_button.setText(text)
         popup.close() # automatically close the popup window
 
     def show_color_popup(self):
 
-        checked_button = self.button_group_track_actors_names.checkedButton()
+        checked_button = self.button_group_actors_names.checkedButton()
         if checked_button is None:
-            QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
         actor_name = checked_button.text()
 
         if actor_name not in self.mesh_actors:
-            QMessageBox.warning(self, 'vision6D', "Only be able to color mesh actors", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Only be able to color mesh actors", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
         popup = PopUpDialog(self, on_button_click=lambda text: self.update_color_button_text(text, popup))
         button_position = self.color_button.mapToGlobal(QPoint(0, 0))
         popup.move(button_position + QPoint(self.color_button.width(), 0))
         popup.exec_()
 
         text = self.color_button.text()
         self.mesh_colors[actor_name] = text
         if text == 'nocs': self.set_scalar(True, actor_name)
         elif text == 'latlon': self.set_scalar(False, actor_name)
         else: self.set_color(text, actor_name)
 
     def remove_actors_button(self):
-        checked_button = self.button_group_track_actors_names.checkedButton()
+        checked_button = self.button_group_actors_names.checkedButton()
         if checked_button is None: 
-            QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
         else: self.remove_actor(checked_button)
 
     def opacity_value_change(self, value):
         if self.ignore_slider_value_change: return 0
-        checked_button = self.button_group_track_actors_names.checkedButton()
+        checked_button = self.button_group_actors_names.checkedButton()
         if checked_button is not None:
             actor_name = checked_button.text()
             if actor_name == 'image': self.set_image_opacity(value / 100)
             elif actor_name == 'mask': self.set_mask_opacity(value / 100)
             else: 
                 self.mesh_opacity[actor_name] = value / 100
                 self.set_mesh_opacity(actor_name, self.mesh_opacity[actor_name])
             self.output_text.clear()
             self.output_text.append(f"Current actor <span style='background-color:yellow; color:black;'>{actor_name}</span>'s opacity is {value / 100}")
         else:
             self.ignore_slider_value_change = True
             self.opacity_slider.setValue(100)
             self.ignore_slider_value_change = False
-            QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         
     def panel_display(self):
         self.display = QtWidgets.QGroupBox("Console")
         display_layout = QtWidgets.QVBoxLayout()
         display_layout.setContentsMargins(10, 20, 10, 10)
```

### Comparing `vision6D-0.0.7/vision6D/__init__.py` & `vision6D-0.0.8/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.7/vision6D/app.py` & `vision6D-0.0.8/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.7/vision6D/config.py` & `vision6D-0.0.8/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.7/vision6D/interface.py` & `vision6D-0.0.8/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.7/vision6D/interface_gui.py` & `vision6D-0.0.8/vision6D/interface_gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import pathlib
 import logging
 import numpy as np
-import math
 import trimesh
 import numpy as np
 import matplotlib.pyplot as plt
 import json
 import PIL
 import vtk
+import ast
 
 # Setting the Qt bindings for QtPy
 import os
 os.environ["QT_API"] = "pyqt5"
 
-from PyQt5.QtWidgets import QMessageBox
+from PyQt5 import QtWidgets
 import pyvista as pv
 from pyvistaqt import QtInteractor, MainWindow
 import vision6D as vis
 from .GUI import MyMainWindow
 
 np.set_printoptions(suppress=True)
 
@@ -48,16 +48,15 @@
         # default opacity for image and surface
         self.image_opacity = 0.99
         self.mask_opacity = 0.5
         self.surface_opacity = 0.8
         self.image_spacing = [0.01, 0.01, 1]
         self.mask_spacing = [0.01, 0.01, 1]
         self.mesh_spacing = [1, 1, 1]
-        self.set_camera_props(fx=50000, fy=50000, cx=960, cy=540, cam_viewup=(0, -1, 0), cam_position=-500)
-
+        
     def button_actor_name_clicked(self, text):
         if text in self.mesh_actors:
             # set the current mesh color
             self.color_button.setText(self.mesh_colors[text])
             # set mesh reference
             self.reference = text
             curr_opacity = self.mesh_actors[self.reference].GetProperty().opacity
@@ -88,54 +87,14 @@
     def set_mesh_opacity(self, name: str, surface_opacity: float):
         assert surface_opacity>=0 and surface_opacity<=1, "mesh opacity should range from 0 to 1!"
         self.mesh_opacity[name] = surface_opacity
         self.mesh_actors[name].user_matrix = pv.array_from_vtkmatrix(self.mesh_actors[name].GetMatrix())
         self.mesh_actors[name].GetProperty().opacity = surface_opacity
         self.plotter.add_actor(self.mesh_actors[name], pickable=True, name=name)
 
-    def set_camera_extrinsics(self, cam_position, cam_viewup):
-        self.camera.SetPosition((0,0,cam_position))
-        self.camera.SetFocalPoint((0,0,0))
-        self.camera.SetViewUp(cam_viewup)
-    
-    def set_camera_intrinsics(self, width, height, fx, fy, cx, cy):
-        
-        # Set camera intrinsic attribute
-        self.camera_intrinsics = np.array([
-            [fx, 0, cx],
-            [0, fy, cy],
-            [0, 0, 1]
-        ])
-        
-        cx = self.camera_intrinsics[0,2]
-        cy = self.camera_intrinsics[1,2]
-        f = self.camera_intrinsics[0,0]
-        
-        # convert the principal point to window center (normalized coordinate system) and set it
-        wcx = -2*(cx - float(width)/2) / width
-        wcy =  2*(cy - float(height)/2) / height
-        self.camera.SetWindowCenter(wcx, wcy) # (0,0)
-        
-        # Setting the view angle in degrees
-        view_angle = (180 / math.pi) * (2.0 * math.atan2(height/2.0, f)) # or view_angle = np.degrees(2.0 * math.atan2(height/2.0, f)) # focal_length = (1080 / 2.0) / math.tan(math.radians(self.plotter.camera.view_angle / 2))
-        self.camera.SetViewAngle(view_angle) # view angle should be in degrees
- 
-    def set_camera_props(self, fx, fy, cx, cy, cam_viewup, cam_position):
-        # Set up the camera
-        self.camera = pv.Camera()
-        self.fx = fx
-        self.fy = fy
-        self.cx = cx
-        self.cy = cy
-        self.cam_viewup = cam_viewup
-        self.cam_position = cam_position
-        self.set_camera_intrinsics(self.window_size[0], self.window_size[1], self.fx, self.fy, self.cx, self.cy)
-        self.set_camera_extrinsics(self.cam_position, self.cam_viewup)
-        self.plotter.camera = self.camera.copy()
-
     def add_image(self, image_source):
 
         if isinstance(image_source, pathlib.WindowsPath) or isinstance(image_source, str):
             image_source = np.array(PIL.Image.open(image_source), dtype='uint8')
         if len(image_source.shape) == 2: 
             image_source = image_source[..., None]
 
@@ -160,14 +119,16 @@
         assert (image_data == image_source).all() or (image_data*255 == image_source).all(), "image_data and image_source should be equal"
 
         # add remove current image to removeMenu
         if 'image' not in self.track_actors_names:
             self.track_actors_names.append('image')
             self.add_button_actor_name('image')
 
+        self.check_button('image')
+
         # reset the camera
         self.reset_camera()
 
     def add_mask(self, mask_source):
 
         if isinstance(mask_source, pathlib.WindowsPath) or isinstance(mask_source, str):
             mask_source = np.array(PIL.Image.open(mask_source), dtype='uint8')
@@ -195,14 +156,16 @@
         assert (mask_data == mask_source).all() or (mask_data*255 == mask_source).all(), "mask_data and mask_source should be equal"
 
         # add remove current image to removeMenu
         if 'mask' not in self.track_actors_names:
             self.track_actors_names.append('mask')
             self.add_button_actor_name('mask')
 
+        self.check_button('mask')
+
         # reset the camera
         self.reset_camera()
   
     def add_pose(self, matrix:np.ndarray=None, rot:np.ndarray=None, trans:np.ndarray=None):
         if matrix is None: matrix = np.vstack((np.hstack((rot, trans)), [0, 0, 0, 1])) #if (rot is not None and trans is not None) else None
         self.initial_pose = matrix #if matrix is not None else self.transformation_matrix
         self.reset_gt_pose()
@@ -229,15 +192,15 @@
         if isinstance(mesh_source, pv.PolyData):
             mesh_data = mesh_source
             source_verts = mesh_source.points * self.mesh_spacing
             source_faces = mesh_source.faces.reshape((-1, 4))[:, 1:]
             flag = True
 
         if not flag:
-            QMessageBox.warning(self, 'vision6D', "The mesh format is not supported!", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "The mesh format is not supported!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
         # consider the mesh verts spacing
         mesh_data.points = mesh_data.points * self.mesh_spacing
 
         # assign a color to every mesh
         if len(self.colors) != 0: mesh_color = self.colors.pop(0)
@@ -267,44 +230,45 @@
         self.reset_camera()
 
         # add remove current mesh to removeMenu
         if mesh_name not in self.track_actors_names:
             self.track_actors_names.append(mesh_name)
             self.add_button_actor_name(mesh_name)
 
+        self.check_button(mesh_name)
+
     def reset_camera(self, *args):
         self.plotter.camera = self.camera.copy()
 
     def zoom_in(self, *args):
         self.plotter.camera.zoom(2)
 
     def zoom_out(self, *args):
         self.plotter.camera.zoom(0.5)
 
-    def pick_callback(self, obj, event):
+    def check_button(self, actor_name):
+        for button in self.button_group_actors_names.buttons():
+            if button.text() == actor_name: 
+                button.setChecked(True)
+                self.button_actor_name_clicked(actor_name)
+                break
+
+    def pick_callback(self, obj, *args):
         x, y = obj.GetEventPosition()
         picker = vtk.vtkCellPicker()
         picker.Pick(x, y, 0, self.plotter.renderer)
         picked_actor = picker.GetActor()
         if picked_actor is not None:
             actor_name = picked_actor.name
             if actor_name in self.mesh_actors:        
                 if actor_name not in self.undo_poses: self.undo_poses[actor_name] = []
                 self.undo_poses[actor_name].append(self.mesh_actors[actor_name].user_matrix)
                 if len(self.undo_poses[actor_name]) > 20: self.undo_poses[actor_name].pop(0)
-                checked_button = self.button_group_track_actors_names.checkedButton()
-                # uncheck the current button if it is not None
-                if checked_button is not None:
-                    if checked_button.text() != actor_name: checked_button.setChecked(False)
                 # check the picked button
-                for button in self.button_group_track_actors_names.buttons():
-                    if button.text() == actor_name: 
-                        button.setChecked(True)
-                        self.button_actor_name_clicked(actor_name)
-                        break
+                self.check_button(actor_name)
 
     def reset_gt_pose(self, *args):
         self.output_text.clear(); self.output_text.append(f"\nReset the GT pose to: \n{self.initial_pose}\n")
         for actor_name, actor in self.mesh_actors.items():
             actor.user_matrix = self.initial_pose
             self.plotter.add_actor(actor, pickable=True, name=actor_name)
 
@@ -325,18 +289,18 @@
             self.output_text.append(f"Current reference mesh is: <span style='background-color:yellow; color:black;'>{self.reference}</span>")
             self.output_text.append(f"\nCurrent pose is: \n{transformation_matrix}\n")
             for actor_name, actor in self.mesh_actors.items():
                 actor.user_matrix = transformation_matrix
                 self.plotter.add_actor(actor, pickable=True, name=actor_name)
 
     def undo_pose(self, *args):
-        if self.button_group_track_actors_names.checkedButton() is not None:
-            actor_name = self.button_group_track_actors_names.checkedButton().text()
+        if self.button_group_actors_names.checkedButton() is not None:
+            actor_name = self.button_group_actors_names.checkedButton().text()
         else:
-            QMessageBox.warning(self, 'vision6D', "Choose a mesh actor first", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Choose a mesh actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         if len(self.undo_poses[actor_name]) != 0: 
             transformation_matrix = self.undo_poses[actor_name].pop()
             if (transformation_matrix == self.mesh_actors[actor_name].user_matrix).all():
                 if len(self.undo_poses[actor_name]) != 0: 
                     transformation_matrix = self.undo_poses[actor_name].pop()
 
@@ -351,15 +315,15 @@
         vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[actor_name])
         vertices_color = vertices
         if self.mirror_x: vertices_color = vis.utils.transform_vertices(vertices_color, np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]))
         if self.mirror_y: vertices_color = vis.utils.transform_vertices(vertices_color, np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]))
         # get the corresponding color
         colors = vis.utils.color_mesh(vertices_color, nocs=nocs)
         if colors.shape != vertices.shape: 
-            QMessageBox.warning(self, 'vision6D', "Cannot set the selected color", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Cannot set the selected color", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         assert colors.shape == vertices.shape, "colors shape should be the same as vertices shape"
         # color the mesh and actor
         mesh_data = pv.wrap(trimesh.Trimesh(vertices, faces, process=False))
         mesh = self.plotter.add_mesh(mesh_data, scalars=colors, rgb=True, opacity=self.mesh_opacity[actor_name], name=actor_name)
         transformation_matrix = pv.array_from_vtkmatrix(self.mesh_actors[actor_name].GetMatrix())
         mesh.user_matrix = transformation_matrix
@@ -420,88 +384,108 @@
 
         return predicted_pose
 
     def epnp_mesh(self):
         if self.reference is not None:
             colors = vis.utils.get_mesh_actor_scalars(self.mesh_actors[self.reference])
             if colors is None or (np.all(colors == colors[0])):
-                QMessageBox.warning(self, 'vision6D', "The mesh need to be colored with nocs or latlon with gradient color", QMessageBox.Ok, QMessageBox.Ok)
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "The mesh need to be colored with nocs or latlon with gradient color", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                 return 0
-            color_mask = self.export_mesh_plot(QMessageBox.Yes, QMessageBox.Yes, QMessageBox.Yes, save_render=False)
+            color_mask = self.export_mesh_plot(QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.Yes, save_render=False)
             gt_pose = self.mesh_actors[self.reference].user_matrix
             if self.mirror_x: gt_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
             if self.mirror_y: gt_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
 
             if np.sum(color_mask) == 0:
-                QMessageBox.warning(self, 'vision6D', "The color mask is blank (maybe set the reference mesh wrong)", QMessageBox.Ok, QMessageBox.Ok)
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "The color mask is blank (maybe set the reference mesh wrong)", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                 return 0
                 
             if self.mesh_colors[self.reference] == 'nocs':
                 vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[self.reference])
                 mesh = trimesh.Trimesh(vertices, faces, process=False)
                 predicted_pose = self.nocs_epnp(color_mask, mesh)
                 if self.mirror_x: predicted_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
                 if self.mirror_y: predicted_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
                 error = np.sum(np.abs(predicted_pose - gt_pose))
                 self.output_text.clear()
                 self.output_text.append(f"PREDICTED POSE WITH <span style='background-color:yellow; color:black;'>NOCS COLOR</span>: ")
                 self.output_text.append(f"\n{predicted_pose}\n\nGT POSE: \n\n{gt_pose}\n\nERROR: \n\n{error}")
 
             else:
-                QMessageBox.warning(self, 'vision6D', "Only works using EPnP with latlon mask", QMessageBox.Ok, QMessageBox.Ok)
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "Only works using EPnP with latlon mask", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
         else:
-            QMessageBox.warning(self, 'vision6D', "A mesh need to be loaded/mesh reference need to be set", QMessageBox.Ok, QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "A mesh need to be loaded/mesh reference need to be set", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
     def epnp_mask(self, nocs_method):
         if self.mask_actor is not None:
             mask_data = vis.utils.get_image_mask_actor_scalars(self.mask_actor)
             if np.max(mask_data) > 1: mask_data = mask_data / 255
 
             # binary mask
             if np.all(np.logical_or(mask_data == 0, mask_data == 1)):
                 if self.reference is not None:
                     colors = vis.utils.get_mesh_actor_scalars(self.mesh_actors[self.reference])
                     if colors is None or (np.all(colors == colors[0])):
-                        QMessageBox.warning(self, 'vision6D', "The mesh need to be colored with nocs or latlon with gradient color", QMessageBox.Ok, QMessageBox.Ok)
+                        QtWidgets.QMessageBox.warning(self, 'vision6D', "The mesh need to be colored with nocs or latlon with gradient color", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                         return 0
-                    color_mask = self.export_mesh_plot(QMessageBox.Yes, QMessageBox.Yes, QMessageBox.Yes, save_render=False)
+                    color_mask = self.export_mesh_plot(QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.Yes, save_render=False)
                     # nocs_color = False if np.sum(color_mask[..., 2]) == 0 else True
                     nocs_color = (self.mesh_colors[self.reference] == 'nocs')
                     gt_pose = self.mesh_actors[self.reference].user_matrix
                     if self.mirror_x: gt_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
                     if self.mirror_y: gt_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
                     vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[self.reference])
                     mesh = trimesh.Trimesh(vertices, faces, process=False)
                 else: 
-                    QMessageBox.warning(self, 'vision6D', "A mesh need to be loaded/mesh reference need to be set", QMessageBox.Ok, QMessageBox.Ok)
+                    QtWidgets.QMessageBox.warning(self, 'vision6D', "A mesh need to be loaded/mesh reference need to be set", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                     return 0
                 color_mask = (color_mask * mask_data).astype(np.uint8)
             # color mask
             else:
                 color_mask = mask_data
                 if np.sum(color_mask) != 0:
                     unique, counts = np.unique(color_mask, return_counts=True)
                     digit_counts = dict(zip(unique, counts))
                     if digit_counts[0] == np.max(counts): 
                         nocs_color = False if np.sum(color_mask[..., 2]) == 0 else True
-                        gt_pose_dir = pathlib.Path(self.mask_path).parent.parent.parent/ 'labels' / 'info.json'
-                        with open(gt_pose_dir) as f: data = json.load(f)
-                        gt_pose = np.array(data[pathlib.Path(self.mask_path).stem]['gt_pose'])
-                        id = pathlib.Path(self.mask_path).stem.split('_')[0].split('.')[1]
-                        #TODO: hard coded, and needed to be updated in the future
-                        mesh_path = pathlib.Path(self.mask_path).stem.split('_')[0] + '_video_trim' 
-                        mesh = vis.utils.load_trimesh(pathlib.Path(self.mesh_dir / mesh_path / "mesh" / "processed_meshes" / f"{id}_right_ossicles_processed.mesh"))
+
+                        # get the gt pose
+                        res = self.get_text_dialog.exec_()
+
+                        if res == QtWidgets.QDialog.Accepted:
+                            try:
+                                gt_pose = ast.literal_eval(self.get_text_dialog.user_text)
+                                gt_pose = np.array(gt_pose)
+                                if gt_pose.shape != (4, 4): 
+                                    QtWidgets.QMessageBox.warning(self, 'vision6D', "It needs to be a 4 by 4 matrix", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok) 
+                                    return 0
+                            except: 
+                                QtWidgets.QMessageBox.warning(self, 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+                                return 0
+                        else: 
+                            return 0
+
+                        self.output_text.clear()
+                        self.output_text.append(f"The input ground truth pose is:\n[{gt_pose[0]}, \n{gt_pose[1]}, \n{gt_pose[2]}, \n{gt_pose[3]}]")
+                        QtWidgets.QMessageBox.information(self, "Information", "Please load the corresponding mesh")
+
+                        # add the mesh object file
+                        self.transformation_matrix = gt_pose
+                        self.add_mesh_file(prompt=True)
+                        checked_button = self.button_group_actors_names.checkedButton()
+                        vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[checked_button.text()])
+                        mesh = trimesh.Trimesh(vertices, faces, process=False)
                     else:
-                        QMessageBox.warning(self, 'vision6D', "A color mask need to be loaded", QMessageBox.Ok, QMessageBox.Ok)
+                        QtWidgets.QMessageBox.warning(self, 'vision6D', "A color mask need to be loaded", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                         return 0
         
             if np.sum(color_mask) == 0:
-                QMessageBox.warning(self, 'vision6D', "The color mask is blank (maybe set the reference mesh wrong)", QMessageBox.Ok, QMessageBox.Ok)
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "The color mask is blank (maybe set the reference mesh wrong)", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                 return 0
                 
             if nocs_method == nocs_color:
                 if nocs_method: 
                     predicted_pose = self.nocs_epnp(color_mask, mesh)
                     if self.mirror_x: predicted_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
                     if self.mirror_y: predicted_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
@@ -517,10 +501,10 @@
                     color_theme = 'LATLON'
                 error = np.sum(np.abs(predicted_pose - gt_pose))
                 self.output_text.clear()
                 self.output_text.append(f"PREDICTED POSE WITH <span style='background-color:yellow; color:black;'>{color_theme} COLOR (MASKED)</span>: ")
                 self.output_text.append(f"\n{predicted_pose}\n\nGT POSE: \n\n{gt_pose}\n\nERROR: \n\n{error}")
 
             else:
-                QMessageBox.warning(self,"vision6D", "Clicked the wrong method")
+                QtWidgets.QMessageBox.warning(self,"vision6D", "Clicked the wrong method")
         else:
-            QMessageBox.warning(self,"vision6D", "please load a mask first")
+            QtWidgets.QMessageBox.warning(self,"vision6D", "please load a mask first")
```

### Comparing `vision6D-0.0.7/vision6D/mainwindow.py` & `vision6D-0.0.8/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.7/vision6D/run_gui.py` & `vision6D-0.0.8/vision6D/run_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from vision6D import Interface_GUI
-from PyQt5.QtCore import QFile
 import sys
 from qtpy import QtWidgets
 
 def exe():
     app = QtWidgets.QApplication(sys.argv)
     app.setStyleSheet("""
     QToolTip
```

### Comparing `vision6D-0.0.7/vision6D/utils.py` & `vision6D-0.0.8/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.7/vision6D.egg-info/PKG-INFO` & `vision6D-0.0.8/vision6D.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.0.7
+Version: 0.0.8
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

