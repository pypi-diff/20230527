# Comparing `tmp/logidrivepy-0.0.1.tar.gz` & `tmp/logidrivepy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logidrivepy-0.0.1.tar", last modified: Wed May 24 00:28:51 2023, max compression
+gzip compressed data, was "logidrivepy-0.1.1.tar", last modified: Sat May 27 09:44:06 2023, max compression
```

## Comparing `logidrivepy-0.0.1.tar` & `logidrivepy-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 00:28:51.971466 logidrivepy-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-05-23 22:21:13.000000 logidrivepy-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2540 2023-05-24 00:28:51.970466 logidrivepy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1710 2023-05-23 22:31:31.000000 logidrivepy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 00:28:51.920454 logidrivepy-0.0.1/logidrivepy/
--rw-rw-rw-   0        0        0       51 2023-05-23 22:13:28.000000 logidrivepy-0.0.1/logidrivepy/__init__.py
--rw-rw-rw-   0        0        0    16720 2023-05-24 00:00:50.000000 logidrivepy-0.0.1/logidrivepy/logitech_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-24 00:28:51.958463 logidrivepy-0.0.1/logidrivepy.egg-info/
--rw-rw-rw-   0        0        0     2540 2023-05-24 00:28:51.000000 logidrivepy-0.0.1/logidrivepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-24 00:28:51.000000 logidrivepy-0.0.1/logidrivepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 00:28:51.000000 logidrivepy-0.0.1/logidrivepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-24 00:28:51.000000 logidrivepy-0.0.1/logidrivepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 00:28:51.972466 logidrivepy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      905 2023-05-24 00:27:41.000000 logidrivepy-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 00:28:51.965465 logidrivepy-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-05-23 21:56:36.000000 logidrivepy-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      552 2023-05-23 23:44:31.000000 logidrivepy-0.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:44:06.277952 logidrivepy-0.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-05-23 22:21:13.000000 logidrivepy-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3467 2023-05-27 09:44:06.276952 logidrivepy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2770 2023-05-27 09:41:01.000000 logidrivepy-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 09:44:06.248945 logidrivepy-0.1.1/logidrivepy/
+-rw-rw-rw-   0        0        0      196 2023-05-27 04:08:39.000000 logidrivepy-0.1.1/logidrivepy/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-05-27 03:38:07.000000 logidrivepy-0.1.1/logidrivepy/constants.py
+-rw-rw-rw-   0        0        0      760 2023-05-27 09:04:30.000000 logidrivepy-0.1.1/logidrivepy/controller.py
+-rw-rw-rw-   0        0        0    16701 2023-05-27 08:42:15.000000 logidrivepy-0.1.1/logidrivepy/functions.py
+-rw-rw-rw-   0        0        0     1865 2023-05-27 03:39:18.000000 logidrivepy-0.1.1/logidrivepy/structs.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:44:06.266949 logidrivepy-0.1.1/logidrivepy.egg-info/
+-rw-rw-rw-   0        0        0     3467 2023-05-27 09:44:06.000000 logidrivepy-0.1.1/logidrivepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-05-27 09:44:06.000000 logidrivepy-0.1.1/logidrivepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 09:44:06.000000 logidrivepy-0.1.1/logidrivepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-27 09:44:06.000000 logidrivepy-0.1.1/logidrivepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-27 09:44:06.000000 logidrivepy-0.1.1/logidrivepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 09:44:06.278952 logidrivepy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      964 2023-05-27 09:42:33.000000 logidrivepy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:44:06.273952 logidrivepy-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-23 21:56:36.000000 logidrivepy-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-05-27 09:01:48.000000 logidrivepy-0.1.1/tests/run_controller_test.py
+-rw-rw-rw-   0        0        0      585 2023-05-27 09:26:43.000000 logidrivepy-0.1.1/tests/spin_wheel_test.py
```

### Comparing `logidrivepy-0.0.1/LICENSE.txt` & `logidrivepy-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.0.1/PKG-INFO` & `logidrivepy-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logidrivepy
-Version: 0.0.1
+Version: 0.1.1
 Summary: A Python library for interfacing with Logitech Steering Wheel.
 Home-page: https://github.com/cengizozel/logidrivepy
 Author: Cengiz Ozel
 Author-email: cozel@cs.rochester.edu
 License: MIT
 Keywords: logitech,g920,driving,wheel,controller
 Platform: UNKNOWN
@@ -15,68 +15,75 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # LogiDrivePy - Logitech Controller Python Module
 
-A Python module for interfacing with Logitech Steering Wheel using the Logitech Steering Wheel Engine. This module was tested on a Logitech G920 Driving Force Racing Wheel.
+A Python module for interfacing with a Logitech Steering Wheel. This module was tested on a Logitech G920 Driving Force Racing Wheel.
 
 ## Introduction
 
-This module is an implementation of the Logitech Steering Wheel Engine's interface. It uses the `ctypes` Python library to load and call functions from the Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll). This module provides an easy-to-use Pythonic interface allowing users to interact with the Logitech Steering Wheel.
+This Python module facilitates interaction with the Logitech G920 Driving Force Racing Wheel, serving as a bridge between Python and the Logitech Steering Wheel's software components.
 
-## Installation
+The original functionality was provided in the form of a C# implementation as part of the Logitech Steering Wheel SDK (Software Development Kit) for the Unity Game Engine, designed by Logitech's developers. The SDK includes APIs (Application Programming Interfaces), which are sets of protocols and tools that allow developers to interact with Logitech's steering wheel hardware.
+
+Seeing the potential to extend this functionality to the Python community, this module was developed to enable the same capabilities for Python developers. By utilizing the `ctypes` Python library, the module can load and call functions from Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll), effectively enabling Python scripts to control and interact with the Logitech G920 Driving Force Racing Wheel.
 
-To install the package, clone the repository and use the `setup.py` file: 
+## Installation
 
+To install the package, simply use pip:
 ```
-git clone https://github.com/cengizozel/LogiDrivePy.git
-cd LogiDrivePy
-python setup.py install
+pip install logidrivepy
 ```
 
-Your project structure should look like this:
-
+The package directory layout is organized as follows:
 ```
 LogiDrivePy
-â”‚   .gitignore
-â”‚   LICENSE.txt
-â”‚   README.md
-â”‚   setup.py
-â”‚
-â”œâ”€â”€â”€logidrivepy
-â”‚   â”‚   logitech_controller.py
-â”‚   â”‚   __init__.py
-â”‚   â”‚
-â”‚   â”œâ”€â”€â”€dll
-â”‚   â”‚       LogitechSteeringWheelEnginesWrapper.dll
-â”‚
-â””â”€â”€â”€tests
-        test.py
-        __init__.py
+|   .gitignore
+|   LICENSE.txt
+|   README.md
+|   setup.py
+|
++---logidrivepy
+|   |   constants.py
+|   |   controller.py
+|   |   functions.py
+|   |   structs.py
+|   |   __init__.py
+|   |
+|   +---dll
+|   |       LogitechSteeringWheelEnginesWrapper.dll
+|
++---tests
+    |   run_controller_test.py
+    |   spin_wheel_test.py
+    |   __init__.py
 ```
 
 ## Usage
 
 Here's a simple example on how to use the Logitech Controller module in your Python script.
 
 ```python
 from logidrivepy import LogitechController
 
-def main():
-    dll_path = "logidrivepy/dll/LogitechSteeringWheelEnginesWrapper.dll"
-    controller = LogitechController(dll_path)
+controller = LogitechController()
+
+print(f"steering_initialize: {controller.steering_initialize()}")
+print(f"logi_update: {controller.logi_update()}")
+print(f"is_connected: {controller.is_connected(0)}")
 
-    # Test initialization
-    controller.initialize()
+controller.steering_shutdown()
+```
 
-    # Give the controller some time to initialize
-    time.sleep(1)
+## Dependencies
 
-    # Test update
-    controller.update(repetitions=100)
+This library uses the `ctypes` Python library to load and call functions from the Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll). The ctypes library is part of the standard Python library and should be installed by default with a standard Python installation.
+
+This library also requires `Tkinter`, a Python binding to the Tk GUI toolkit. Tkinter is part of the standard Python library for Python 3 and should be installed by default with a standard Python installation.
+
+### License
+
+This project is licensed under the terms of the MIT license. For more details, see the `LICENSE.txt` file.
 
-if __name__ == "__main__":
-    main()
-```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `logidrivepy-0.0.1/logidrivepy/logitech_controller.py` & `logidrivepy-0.1.1/logidrivepy/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,154 +1,39 @@
-import tkinter as tk
 import ctypes
-import time
-
+import tkinter as tk
 
-class LogitechController:
-    def __init__(self, dll_path):
-        self.dll_path = dll_path
+class LogitechControllerFunctions:
+    def __init__(self, dll_path, structs, use_gui=True):
+        self.structs = structs
         self.logi_dll = ctypes.cdll.LoadLibrary(dll_path)
 
-        # CONSTANTS
-        self.LOGI_MAX_CONTROLLERS = 4
-       
-        # Force types
-        self.LOGI_FORCE_NONE = -1
-        self.LOGI_FORCE_SPRING = 0
-        self.LOGI_FORCE_CONSTANT = 1
-        self.LOGI_FORCE_DAMPER = 2
-        self.LOGI_FORCE_SIDE_COLLISION = 3
-        self.LOGI_FORCE_FRONTAL_COLLISION = 4
-        self.LOGI_FORCE_DIRT_ROAD = 5
-        self.LOGI_FORCE_BUMPY_ROAD = 6
-        self.LOGI_FORCE_SLIPPERY_ROAD = 7
-        self.LOGI_FORCE_SURFACE_EFFECT = 8
-        self.LOGI_NUMBER_FORCE_EFFECTS = 9
-        self.LOGI_FORCE_SOFTSTOP = 10
-        self.LOGI_FORCE_CAR_AIRBORNE = 11
-
-        # Periodic types for surface effect
-        self.LOGI_PERIODICTYPE_NONE = -1
-        self.LOGI_PERIODICTYPE_SINE = 0
-        self.LOGI_PERIODICTYPE_SQUARE = 1
-        self.LOGI_PERIODICTYPE_TRIANGLE = 2
-
-        # Device types
-        self.LOGI_DEVICE_TYPE_NONE = -1
-        self.LOGI_DEVICE_TYPE_WHEEL = 0
-        self.LOGI_DEVICE_TYPE_JOYSTICK = 1
-        self.LOGI_DEVICE_TYPE_GAMEPAD = 2
-        self.LOGI_DEVICE_TYPE_OTHER = 3
-        self.LOGI_NUMBER_DEVICE_TYPES = 4
-
-        # Manufacturer types
-        self.LOGI_MANUFACTURER_NONE = -1
-        self.LOGI_MANUFACTURER_LOGITECH = 0
-        self.LOGI_MANUFACTURER_MICROSOFT = 1
-        self.LOGI_MANUFACTURER_OTHER = 2
-
-        # Model types
-        self.LOGI_MODEL_G27 = 0
-        self.LOGI_MODEL_DRIVING_FORCE_GT = 1
-        self.LOGI_MODEL_G25 = 2
-        self.LOGI_MODEL_MOMO_RACING = 3
-        self.LOGI_MODEL_MOMO_FORCE = 4
-        self.LOGI_MODEL_DRIVING_FORCE_PRO = 5
-        self.LOGI_MODEL_DRIVING_FORCE = 6
-        self.LOGI_MODEL_NASCAR_RACING_WHEEL = 7
-        self.LOGI_MODEL_FORMULA_FORCE = 8
-        self.LOGI_MODEL_FORMULA_FORCE_GP = 9
-        self.LOGI_MODEL_FORCE_3D_PRO = 10
-        self.LOGI_MODEL_EXTREME_3D_PRO = 11
-        self.LOGI_MODEL_FREEDOM_24 = 12
-        self.LOGI_MODEL_ATTACK_3 = 13
-        self.LOGI_MODEL_FORCE_3D = 14
-        self.LOGI_MODEL_STRIKE_FORCE_3D = 15
-        self.LOGI_MODEL_G940_JOYSTICK = 16
-        self.LOGI_MODEL_G940_THROTTLE = 17
-        self.LOGI_MODEL_G940_PEDALS = 18
-        self.LOGI_MODEL_RUMBLEPAD = 19
-        self.LOGI_MODEL_RUMBLEPAD_2 = 20
-        self.LOGI_MODEL_CORDLESS_RUMBLEPAD_2 = 21
-        self.LOGI_MODEL_CORDLESS_GAMEPAD = 22
-        self.LOGI_MODEL_DUAL_ACTION_GAMEPAD = 23
-        self.LOGI_MODEL_PRECISION_GAMEPAD_2 = 24
-        self.LOGI_MODEL_CHILLSTREAM = 25
-        self.LOGI_MODEL_G29 = 26
-        self.LOGI_MODEL_G920 = 27
-        self.LOGI_NUMBER_MODELS = 28
-
-        # Structs
-        class LogiControllerPropertiesData(ctypes.Structure):
-            _fields_ = [
-                ("forceEnable", ctypes.c_bool),
-                ("overallGain", ctypes.c_int),
-                ("springGain", ctypes.c_int),
-                ("damperGain", ctypes.c_int),
-                ("defaultSpringEnabled", ctypes.c_bool),
-                ("defaultSpringGain", ctypes.c_int),
-                ("combinePedals", ctypes.c_bool),
-                ("wheelRange", ctypes.c_int),
-                ("gameSettingsEnabled", ctypes.c_bool),
-                ("allowGameSettings", ctypes.c_bool)
-            ]
-
-        class DIJOYSTATE2ENGINES(ctypes.Structure):
-            _fields_ = [
-                ("lX", ctypes.c_int),
-                ("lY", ctypes.c_int),
-                ("lZ", ctypes.c_int),
-                ("lRx", ctypes.c_int),
-                ("lRy", ctypes.c_int),
-                ("lRz", ctypes.c_int),
-                ("rglSlider", ctypes.c_int * 2),
-                ("rgdwPOV", ctypes.c_uint * 4),
-                ("rgbButtons", ctypes.c_byte * 128),
-                ("lVX", ctypes.c_int),
-                ("lVY", ctypes.c_int),
-                ("lVZ", ctypes.c_int),
-                ("lVRx", ctypes.c_int),
-                ("lVRy", ctypes.c_int),
-                ("lVRz", ctypes.c_int),
-                ("rglVSlider", ctypes.c_int * 2),
-                ("lAX", ctypes.c_int),
-                ("lAY", ctypes.c_int),
-                ("lAZ", ctypes.c_int),
-                ("lARx", ctypes.c_int),
-                ("lARy", ctypes.c_int),
-                ("lARz", ctypes.c_int),
-                ("rglASlider", ctypes.c_int * 2),
-                ("lFX", ctypes.c_int),
-                ("lFY", ctypes.c_int),
-                ("lFZ", ctypes.c_int),
-                ("lFRx", ctypes.c_int),
-                ("lFRy", ctypes.c_int),
-                ("lFRz", ctypes.c_int),
-                ("rglFSlider", ctypes.c_int * 2)
-            ]
+        # If use_gui flag is True, then create a hidden Tkinter window
+        if use_gui:
+            self.root = tk.Tk()
+            self.root.withdraw()
+            self.root.update()
 
         # Function Definitions
-
         # LogiSteeringInitialize
         self.LogiSteeringInitialize = self.logi_dll.LogiSteeringInitialize
         self.LogiSteeringInitialize.argtypes = [ctypes.c_bool]
         self.LogiSteeringInitialize.restype = ctypes.c_bool
 
         # LogiUpdate
         self.LogiUpdate = self.logi_dll.LogiUpdate
         self.LogiUpdate.argtypes = []
         self.LogiUpdate.restype = ctypes.c_bool
 
         # LogiGetStateENGINES
         self.LogiGetStateENGINES = self.logi_dll.LogiGetStateENGINES
         self.LogiGetStateENGINES.argtypes = [ctypes.c_int]
-        self.LogiGetStateENGINES.restype = ctypes.POINTER(DIJOYSTATE2ENGINES)
+        self.LogiGetStateENGINES.restype = ctypes.POINTER(self.structs.DIJOYSTATE2ENGINES)
 
         def LogiGetStateCSharp(index):
-            ret = DIJOYSTATE2ENGINES()
+            ret = self.structs.DIJOYSTATE2ENGINES()
             ret.rglSlider = (ctypes.c_int * 2)()
             ret.rgdwPOV = (ctypes.c_uint * 4)()
             ret.rgbButtons = (ctypes.c_byte * 128)()
             ret.rglVSlider = (ctypes.c_int * 2)()
             ret.rglASlider = (ctypes.c_int * 2)()
             ret.rglFSlider = (ctypes.c_int * 2)()
             try:
@@ -320,20 +205,20 @@
         # LogiStopSoftstopForce
         self.LogiStopSoftstopForce = self.logi_dll.LogiStopSoftstopForce
         self.LogiStopSoftstopForce.argtypes = [ctypes.c_int]
         self.LogiStopSoftstopForce.restype = ctypes.c_bool
 
         # LogiSetPreferredControllerProperties
         self.LogiSetPreferredControllerProperties = self.logi_dll.LogiSetPreferredControllerProperties
-        self.LogiSetPreferredControllerProperties.argtypes = [LogiControllerPropertiesData]
+        self.LogiSetPreferredControllerProperties.argtypes = [self.structs.LogiControllerPropertiesData]
         self.LogiSetPreferredControllerProperties.restype = ctypes.c_bool
 
         # LogiGetCurrentControllerProperties
         self.LogiGetCurrentControllerProperties = self.logi_dll.LogiGetCurrentControllerProperties
-        self.LogiGetCurrentControllerProperties.argtypes = [ctypes.c_int, ctypes.POINTER(LogiControllerPropertiesData)]
+        self.LogiGetCurrentControllerProperties.argtypes = [ctypes.c_int, ctypes.POINTER(self.structs.LogiControllerPropertiesData)]
         self.LogiGetCurrentControllerProperties.restype = ctypes.c_bool
 
         # LogiGetShifterMode
         self.LogiGetShifterMode = self.logi_dll.LogiGetShifterMode
         self.LogiGetShifterMode.argtypes = [ctypes.c_int, ctypes.POINTER(ctypes.c_int)]
         self.LogiGetShifterMode.restype = ctypes.c_bool
 
@@ -353,29 +238,138 @@
         self.LogiPlayLeds.restype = ctypes.c_bool
 
         # LogiSteeringShutdown
         self.LogiSteeringShutdown = self.logi_dll.LogiSteeringShutdown
         self.LogiSteeringShutdown.argtypes = []
         self.LogiSteeringShutdown.restype = None
 
-    def initialize(self, ignore_xinput_controllers=True):
-        result = self.LogiSteeringInitialize(ignore_xinput_controllers)
-        print(f"\nLogiSteeringInitialize output: {result}\n")
-
-    def update(self, repetitions=100):
-        root = tk.Tk()
-        root.withdraw()
-
-        for i in range(repetitions):
-            print(f"LogiUpdate output: {self.LogiUpdate()}", end=", ")
-            print(f"LogiIsConnected output: {self.LogiIsConnected(0)}   ", end="\r")
-
-            self.LogiPlaySpringForce(0, i, 100, 40)
-            time.sleep(0.1)
-            root.update()
-
-
-if __name__ == "__main__":
-    dll_path = "dll/LogitechSteeringWheelEnginesWrapper.dll"
-    controller = LogitechController(dll_path)
-    controller.initialize()
-    controller.update()
+    def steering_initialize(self, ignore_xinput_controllers=True):
+        return self.LogiSteeringInitialize(ignore_xinput_controllers)
+    
+    def logi_update(self):
+        return self.LogiUpdate()
+    
+    def get_state_engines(self, index):
+        return self.LogiGetStateENGINES(index)
+    
+    def get_device_path(self, index, string, number):
+        return self.LogiGetDevicePath(index, string, number)
+    
+    def get_friendly_product_name(self, index, string, number):
+        return self.LogiGetFriendlyProductName(index, string, number)
+    
+    def is_connected(self, index):
+        return self.LogiIsConnected(index)
+    
+    def is_device_connected(self, index, number):
+        return self.LogiIsDeviceConnected(index, number)
+    
+    def is_manufacturer_connected(self, index, number):
+        return self.LogiIsManufacturerConnected(index, number)
+
+    def is_model_connected(self, index, number):
+        return self.LogiIsModelConnected(index, number)
+
+    def button_triggered(self, index, button_number):
+        return self.LogiButtonTriggered(index, button_number)
+
+    def button_released(self, index, button_number):
+        return self.LogiButtonReleased(index, button_number)
+
+    def button_is_pressed(self, index, button_number):
+        return self.LogiButtonIsPressed(index, button_number)
+
+    def generate_non_linear_values(self, index, non_linear_values):
+        return self.LogiGenerateNonLinearValues(index, non_linear_values)
+
+    def get_non_linear_value(self, index, value):
+        return self.LogiGetNonLinearValue(index, value)
+
+    def has_force_feedback(self, index):
+        return self.LogiHasForceFeedback(index)
+
+    def is_playing(self, index, force_type):
+        return self.LogiIsPlaying(index, force_type)
+
+    def play_spring_force(self, index, offset, saturation, coefficient):
+        return self.LogiPlaySpringForce(index, offset, saturation, coefficient)
+
+    def stop_spring_force(self, index):
+        return self.LogiStopSpringForce(index)
+
+    def play_constant_force(self, index, magnitude):
+        return self.LogiPlayConstantForce(index, magnitude)
+
+    def stop_constant_force(self, index):
+        return self.LogiStopConstantForce(index)
+
+    def play_damper_force(self, index, coefficient):
+        return self.LogiPlayDamperForce(index, coefficient)
+
+    def stop_damper_force(self, index):
+        return self.LogiStopDamperForce(index)
+
+    def play_side_collision_force(self, index, magnitude):
+        return self.LogiPlaySideCollisionForce(index, magnitude)
+
+    def play_frontal_collision_force(self, index, magnitude):
+        return self.LogiPlayFrontalCollisionForce(index, magnitude)
+
+    def play_dirt_road_effect(self, index, magnitude):
+        return self.LogiPlayDirtRoadEffect(index, magnitude)
+
+    def stop_dirt_road_effect(self, index):
+        return self.LogiStopDirtRoadEffect(index)
+
+    def play_bumpy_road_effect(self, index, magnitude):
+        return self.LogiPlayBumpyRoadEffect(index, magnitude)
+
+    def stop_bumpy_road_effect(self, index):
+        return self.LogiStopBumpyRoadEffect(index)
+
+    def play_slippery_road_effect(self, index, magnitude):
+        return self.LogiPlaySlipperyRoadEffect(index, magnitude)
+
+    def stop_slippery_road_effect(self, index):
+        return self.LogiStopSlipperyRoadEffect(index)
+
+    def play_surface_effect(self, index, type, magnitude, period):
+        return self.LogiPlaySurfaceEffect(index, type, magnitude, period)
+
+    def stop_surface_effect(self, index):
+        return self.LogiStopSurfaceEffect(index)
+
+    def play_car_airborne(self, index):
+        return self.LogiPlayCarAirborne(index)
+
+    def stop_car_airborne(self, index):
+        return self.LogiStopCarAirborne(index)
+
+    def play_softstop_force(self, index, usableRange):
+        return self.LogiPlaySoftstopForce(index, usableRange)
+
+    def stop_softstop_force(self, index):
+        return self.LogiStopSoftstopForce(index)
+
+    def set_preferred_controller_properties(self, properties_data):
+        return self.LogiSetPreferredControllerProperties(properties_data)
+
+    def get_current_controller_properties(self, index, properties_data_pointer):
+        return self.LogiGetCurrentControllerProperties(index, properties_data_pointer)
+
+    def get_shifter_mode(self, index, shifter_mode_pointer):
+        return self.LogiGetShifterMode(index, shifter_mode_pointer)
+
+    def get_operating_range(self, index, range_pointer):
+        return self.LogiGetOperatingRange(index, range_pointer)
+
+    def set_operating_range(self, index, range):
+        return self.LogiSetOperatingRange(index, range)
+
+    def play_leds(self, index, currentRPM, rpmFirstLedTurnsOn, rpmRedLine):
+        return self.LogiPlayLeds(index, currentRPM, rpmFirstLedTurnsOn, rpmRedLine)
+
+    def steering_shutdown(self):
+        # Destroy the GUI window if it exists
+        if hasattr(self, 'root'):
+            self.root.destroy()
+        return self.LogiSteeringShutdown()
```

### Comparing `logidrivepy-0.0.1/logidrivepy.egg-info/PKG-INFO` & `logidrivepy-0.1.1/logidrivepy.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logidrivepy
-Version: 0.0.1
+Version: 0.1.1
 Summary: A Python library for interfacing with Logitech Steering Wheel.
 Home-page: https://github.com/cengizozel/logidrivepy
 Author: Cengiz Ozel
 Author-email: cozel@cs.rochester.edu
 License: MIT
 Keywords: logitech,g920,driving,wheel,controller
 Platform: UNKNOWN
@@ -15,68 +15,75 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # LogiDrivePy - Logitech Controller Python Module
 
-A Python module for interfacing with Logitech Steering Wheel using the Logitech Steering Wheel Engine. This module was tested on a Logitech G920 Driving Force Racing Wheel.
+A Python module for interfacing with a Logitech Steering Wheel. This module was tested on a Logitech G920 Driving Force Racing Wheel.
 
 ## Introduction
 
-This module is an implementation of the Logitech Steering Wheel Engine's interface. It uses the `ctypes` Python library to load and call functions from the Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll). This module provides an easy-to-use Pythonic interface allowing users to interact with the Logitech Steering Wheel.
+This Python module facilitates interaction with the Logitech G920 Driving Force Racing Wheel, serving as a bridge between Python and the Logitech Steering Wheel's software components.
 
-## Installation
+The original functionality was provided in the form of a C# implementation as part of the Logitech Steering Wheel SDK (Software Development Kit) for the Unity Game Engine, designed by Logitech's developers. The SDK includes APIs (Application Programming Interfaces), which are sets of protocols and tools that allow developers to interact with Logitech's steering wheel hardware.
+
+Seeing the potential to extend this functionality to the Python community, this module was developed to enable the same capabilities for Python developers. By utilizing the `ctypes` Python library, the module can load and call functions from Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll), effectively enabling Python scripts to control and interact with the Logitech G920 Driving Force Racing Wheel.
 
-To install the package, clone the repository and use the `setup.py` file: 
+## Installation
 
+To install the package, simply use pip:
 ```
-git clone https://github.com/cengizozel/LogiDrivePy.git
-cd LogiDrivePy
-python setup.py install
+pip install logidrivepy
 ```
 
-Your project structure should look like this:
-
+The package directory layout is organized as follows:
 ```
 LogiDrivePy
-â”‚   .gitignore
-â”‚   LICENSE.txt
-â”‚   README.md
-â”‚   setup.py
-â”‚
-â”œâ”€â”€â”€logidrivepy
-â”‚   â”‚   logitech_controller.py
-â”‚   â”‚   __init__.py
-â”‚   â”‚
-â”‚   â”œâ”€â”€â”€dll
-â”‚   â”‚       LogitechSteeringWheelEnginesWrapper.dll
-â”‚
-â””â”€â”€â”€tests
-        test.py
-        __init__.py
+|   .gitignore
+|   LICENSE.txt
+|   README.md
+|   setup.py
+|
++---logidrivepy
+|   |   constants.py
+|   |   controller.py
+|   |   functions.py
+|   |   structs.py
+|   |   __init__.py
+|   |
+|   +---dll
+|   |       LogitechSteeringWheelEnginesWrapper.dll
+|
++---tests
+    |   run_controller_test.py
+    |   spin_wheel_test.py
+    |   __init__.py
 ```
 
 ## Usage
 
 Here's a simple example on how to use the Logitech Controller module in your Python script.
 
 ```python
 from logidrivepy import LogitechController
 
-def main():
-    dll_path = "logidrivepy/dll/LogitechSteeringWheelEnginesWrapper.dll"
-    controller = LogitechController(dll_path)
+controller = LogitechController()
+
+print(f"steering_initialize: {controller.steering_initialize()}")
+print(f"logi_update: {controller.logi_update()}")
+print(f"is_connected: {controller.is_connected(0)}")
 
-    # Test initialization
-    controller.initialize()
+controller.steering_shutdown()
+```
 
-    # Give the controller some time to initialize
-    time.sleep(1)
+## Dependencies
 
-    # Test update
-    controller.update(repetitions=100)
+This library uses the `ctypes` Python library to load and call functions from the Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll). The ctypes library is part of the standard Python library and should be installed by default with a standard Python installation.
+
+This library also requires `Tkinter`, a Python binding to the Tk GUI toolkit. Tkinter is part of the standard Python library for Python 3 and should be installed by default with a standard Python installation.
+
+### License
+
+This project is licensed under the terms of the MIT license. For more details, see the `LICENSE.txt` file.
 
-if __name__ == "__main__":
-    main()
-```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `logidrivepy-0.0.1/setup.py` & `logidrivepy-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='logidrivepy',
-    version='0.0.1',
+    version='0.1.1',
     description='A Python library for interfacing with Logitech Steering Wheel.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/cengizozel/logidrivepy',
     author='Cengiz Ozel',
     author_email='cozel@cs.rochester.edu',
     license='MIT',
@@ -18,9 +18,12 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     keywords='logitech, g920, driving, wheel, controller',
     install_requires=[
+        'tkinter',
+        'ctypes',
+        'pathlib',
     ],
 )
```

### Comparing `logidrivepy-0.0.1/tests/test.py` & `logidrivepy-0.1.1/tests/spin_wheel_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import sys
-import time
-
-sys.path.append('..\\logidrivepy')
-
+sys.path.append('../logidrivepy')
 from logidrivepy import LogitechController
+import time
 
-def test_logitech_controller():
-    dll_path = "logidrivepy/dll/LogitechSteeringWheelEnginesWrapper.dll"
-    controller = LogitechController(dll_path)
-
-    # Test initialization
-    controller.initialize()
-
-    # Give the controller some time to initialize
-    time.sleep(1)
+def spin_controller(controller):
+    for i in range(-100, 102, 2):
+        controller.LogiPlaySpringForce(0, i, 100, 40)
+        controller.logi_update()
+        time.sleep(0.1)
+
+
+def spin_test():
+    controller = LogitechController()
+
+    controller.steering_initialize()
+    print("\n---Logitech Spin Test---")
+    spin_controller(controller)
+    print("Spin test passed.\n")
 
-    # Test update
-    controller.update(repetitions=100)
+    controller.steering_shutdown()
 
-    print("All tests passed.")
 
 if __name__ == "__main__":
-    test_logitech_controller()
+    spin_test()
```

