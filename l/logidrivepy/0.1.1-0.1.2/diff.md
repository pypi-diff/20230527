# Comparing `tmp/logidrivepy-0.1.1.tar.gz` & `tmp/logidrivepy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logidrivepy-0.1.1.tar", last modified: Sat May 27 09:44:06 2023, max compression
+gzip compressed data, was "logidrivepy-0.1.2.tar", last modified: Sat May 27 10:05:13 2023, max compression
```

## Comparing `logidrivepy-0.1.1.tar` & `logidrivepy-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 09:44:06.277952 logidrivepy-0.1.1/
--rw-rw-rw-   0        0        0     1087 2023-05-23 22:21:13.000000 logidrivepy-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3467 2023-05-27 09:44:06.276952 logidrivepy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2770 2023-05-27 09:41:01.000000 logidrivepy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 09:44:06.248945 logidrivepy-0.1.1/logidrivepy/
--rw-rw-rw-   0        0        0      196 2023-05-27 04:08:39.000000 logidrivepy-0.1.1/logidrivepy/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-05-27 03:38:07.000000 logidrivepy-0.1.1/logidrivepy/constants.py
--rw-rw-rw-   0        0        0      760 2023-05-27 09:04:30.000000 logidrivepy-0.1.1/logidrivepy/controller.py
--rw-rw-rw-   0        0        0    16701 2023-05-27 08:42:15.000000 logidrivepy-0.1.1/logidrivepy/functions.py
--rw-rw-rw-   0        0        0     1865 2023-05-27 03:39:18.000000 logidrivepy-0.1.1/logidrivepy/structs.py
-drwxrwxrwx   0        0        0        0 2023-05-27 09:44:06.266949 logidrivepy-0.1.1/logidrivepy.egg-info/
--rw-rw-rw-   0        0        0     3467 2023-05-27 09:44:06.000000 logidrivepy-0.1.1/logidrivepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-05-27 09:44:06.000000 logidrivepy-0.1.1/logidrivepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:44:06.000000 logidrivepy-0.1.1/logidrivepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-27 09:44:06.000000 logidrivepy-0.1.1/logidrivepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-27 09:44:06.000000 logidrivepy-0.1.1/logidrivepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 09:44:06.278952 logidrivepy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      964 2023-05-27 09:42:33.000000 logidrivepy-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 09:44:06.273952 logidrivepy-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-05-23 21:56:36.000000 logidrivepy-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      743 2023-05-27 09:01:48.000000 logidrivepy-0.1.1/tests/run_controller_test.py
--rw-rw-rw-   0        0        0      585 2023-05-27 09:26:43.000000 logidrivepy-0.1.1/tests/spin_wheel_test.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:05:13.338046 logidrivepy-0.1.2/
+-rw-rw-rw-   0        0        0     1087 2023-05-23 22:21:13.000000 logidrivepy-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3469 2023-05-27 10:05:13.337045 logidrivepy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2770 2023-05-27 10:03:51.000000 logidrivepy-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 10:05:13.295035 logidrivepy-0.1.2/logidrivepy/
+-rw-rw-rw-   0        0        0      196 2023-05-27 04:08:39.000000 logidrivepy-0.1.2/logidrivepy/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-05-27 03:38:07.000000 logidrivepy-0.1.2/logidrivepy/constants.py
+-rw-rw-rw-   0        0        0      760 2023-05-27 09:04:30.000000 logidrivepy-0.1.2/logidrivepy/controller.py
+-rw-rw-rw-   0        0        0    16701 2023-05-27 08:42:15.000000 logidrivepy-0.1.2/logidrivepy/functions.py
+-rw-rw-rw-   0        0        0     1865 2023-05-27 03:39:18.000000 logidrivepy-0.1.2/logidrivepy/structs.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:05:13.326044 logidrivepy-0.1.2/logidrivepy.egg-info/
+-rw-rw-rw-   0        0        0     3469 2023-05-27 10:05:13.000000 logidrivepy-0.1.2/logidrivepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-05-27 10:05:13.000000 logidrivepy-0.1.2/logidrivepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 10:05:13.000000 logidrivepy-0.1.2/logidrivepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-27 10:05:13.000000 logidrivepy-0.1.2/logidrivepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 10:05:13.339046 logidrivepy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-05-27 10:04:05.000000 logidrivepy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:05:13.334045 logidrivepy-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-23 21:56:36.000000 logidrivepy-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-05-27 09:01:48.000000 logidrivepy-0.1.2/tests/run_controller_test.py
+-rw-rw-rw-   0        0        0      585 2023-05-27 09:26:43.000000 logidrivepy-0.1.2/tests/spin_wheel_test.py
```

### Comparing `logidrivepy-0.1.1/LICENSE.txt` & `logidrivepy-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.1/PKG-INFO` & `logidrivepy-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,10 @@
-Metadata-Version: 2.1
-Name: logidrivepy
-Version: 0.1.1
-Summary: A Python library for interfacing with Logitech Steering Wheel.
-Home-page: https://github.com/cengizozel/logidrivepy
-Author: Cengiz Ozel
-Author-email: cozel@cs.rochester.edu
-License: MIT
-Keywords: logitech,g920,driving,wheel,controller
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # LogiDrivePy - Logitech Controller Python Module
 
-A Python module for interfacing with a Logitech Steering Wheel. This module was tested on a Logitech G920 Driving Force Racing Wheel.
+A Python module for interfacing with a Logitech steering wheel. This module was tested on a Logitech G920 Driving Force Racing Wheel.
 
 ## Introduction
 
 This Python module facilitates interaction with the Logitech G920 Driving Force Racing Wheel, serving as a bridge between Python and the Logitech Steering Wheel's software components.
 
 The original functionality was provided in the form of a C# implementation as part of the Logitech Steering Wheel SDK (Software Development Kit) for the Unity Game Engine, designed by Logitech's developers. The SDK includes APIs (Application Programming Interfaces), which are sets of protocols and tools that allow developers to interact with Logitech's steering wheel hardware.
 
@@ -81,9 +62,7 @@
 This library uses the `ctypes` Python library to load and call functions from the Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll). The ctypes library is part of the standard Python library and should be installed by default with a standard Python installation.
 
 This library also requires `Tkinter`, a Python binding to the Tk GUI toolkit. Tkinter is part of the standard Python library for Python 3 and should be installed by default with a standard Python installation.
 
 ### License
 
 This project is licensed under the terms of the MIT license. For more details, see the `LICENSE.txt` file.
-
-
```

### Comparing `logidrivepy-0.1.1/README.md` & `logidrivepy-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,29 @@
+Metadata-Version: 2.1
+Name: logidrivepy
+Version: 0.1.2
+Summary: A Python library for interfacing with a Logitech steering wheel.
+Home-page: https://github.com/cengizozel/logidrivepy
+Author: Cengiz Ozel
+Author-email: cozel@cs.rochester.edu
+License: MIT
+Keywords: logitech,g920,driving,wheel,controller
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # LogiDrivePy - Logitech Controller Python Module
 
-A Python module for interfacing with a Logitech Steering Wheel. This module was tested on a Logitech G920 Driving Force Racing Wheel.
+A Python module for interfacing with a Logitech steering wheel. This module was tested on a Logitech G920 Driving Force Racing Wheel.
 
 ## Introduction
 
 This Python module facilitates interaction with the Logitech G920 Driving Force Racing Wheel, serving as a bridge between Python and the Logitech Steering Wheel's software components.
 
 The original functionality was provided in the form of a C# implementation as part of the Logitech Steering Wheel SDK (Software Development Kit) for the Unity Game Engine, designed by Logitech's developers. The SDK includes APIs (Application Programming Interfaces), which are sets of protocols and tools that allow developers to interact with Logitech's steering wheel hardware.
 
@@ -62,7 +81,9 @@
 This library uses the `ctypes` Python library to load and call functions from the Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll). The ctypes library is part of the standard Python library and should be installed by default with a standard Python installation.
 
 This library also requires `Tkinter`, a Python binding to the Tk GUI toolkit. Tkinter is part of the standard Python library for Python 3 and should be installed by default with a standard Python installation.
 
 ### License
 
 This project is licensed under the terms of the MIT license. For more details, see the `LICENSE.txt` file.
+
+
```

### Comparing `logidrivepy-0.1.1/logidrivepy/constants.py` & `logidrivepy-0.1.2/logidrivepy/constants.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.1/logidrivepy/controller.py` & `logidrivepy-0.1.2/logidrivepy/controller.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.1/logidrivepy/functions.py` & `logidrivepy-0.1.2/logidrivepy/functions.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.1/logidrivepy/structs.py` & `logidrivepy-0.1.2/logidrivepy/structs.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.1/logidrivepy.egg-info/PKG-INFO` & `logidrivepy-0.1.2/logidrivepy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: logidrivepy
-Version: 0.1.1
-Summary: A Python library for interfacing with Logitech Steering Wheel.
+Version: 0.1.2
+Summary: A Python library for interfacing with a Logitech steering wheel.
 Home-page: https://github.com/cengizozel/logidrivepy
 Author: Cengiz Ozel
 Author-email: cozel@cs.rochester.edu
 License: MIT
 Keywords: logitech,g920,driving,wheel,controller
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # LogiDrivePy - Logitech Controller Python Module
 
-A Python module for interfacing with a Logitech Steering Wheel. This module was tested on a Logitech G920 Driving Force Racing Wheel.
+A Python module for interfacing with a Logitech steering wheel. This module was tested on a Logitech G920 Driving Force Racing Wheel.
 
 ## Introduction
 
 This Python module facilitates interaction with the Logitech G920 Driving Force Racing Wheel, serving as a bridge between Python and the Logitech Steering Wheel's software components.
 
 The original functionality was provided in the form of a C# implementation as part of the Logitech Steering Wheel SDK (Software Development Kit) for the Unity Game Engine, designed by Logitech's developers. The SDK includes APIs (Application Programming Interfaces), which are sets of protocols and tools that allow developers to interact with Logitech's steering wheel hardware.
```

### Comparing `logidrivepy-0.1.1/setup.py` & `logidrivepy-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='logidrivepy',
-    version='0.1.1',
-    description='A Python library for interfacing with Logitech Steering Wheel.',
+    version='0.1.2',
+    description='A Python library for interfacing with a Logitech steering wheel.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/cengizozel/logidrivepy',
     author='Cengiz Ozel',
     author_email='cozel@cs.rochester.edu',
     license='MIT',
     packages=find_packages(),
@@ -18,12 +18,9 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     keywords='logitech, g920, driving, wheel, controller',
     install_requires=[
-        'tkinter',
-        'ctypes',
-        'pathlib',
     ],
 )
```

### Comparing `logidrivepy-0.1.1/tests/run_controller_test.py` & `logidrivepy-0.1.2/tests/run_controller_test.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.1/tests/spin_wheel_test.py` & `logidrivepy-0.1.2/tests/spin_wheel_test.py`

 * *Files identical despite different names*

