# Comparing `tmp/ros-d2-1.0.4.tar.gz` & `tmp/ros-d2-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ros-d2-1.0.4.tar", last modified: Wed Feb  8 10:29:06 2023, max compression
+gzip compressed data, was "ros-d2-1.0.5.tar", last modified: Sat May 27 10:59:04 2023, max compression
```

## Comparing `ros-d2-1.0.4.tar` & `ros-d2-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:29:06.914006 ros-d2-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-08 10:28:59.000000 ros-d2-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-02-08 10:29:06.914006 ros-d2-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-02-08 10:29:02.000000 ros-d2-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:29:06.914006 ros-d2-1.0.4/ros_d2/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-08 10:28:59.000000 ros-d2-1.0.4/ros_d2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-08 10:28:59.000000 ros-d2-1.0.4/ros_d2/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:29:06.914006 ros-d2-1.0.4/ros_d2/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-02-08 10:28:59.000000 ros-d2-1.0.4/ros_d2/helpers/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-02-08 10:28:59.000000 ros-d2-1.0.4/ros_d2/helpers/get_ros_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-02-08 10:28:59.000000 ros-d2-1.0.4/ros_d2/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:29:06.914006 ros-d2-1.0.4/ros_d2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-02-08 10:29:06.000000 ros-d2-1.0.4/ros_d2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-02-08 10:29:06.000000 ros-d2-1.0.4/ros_d2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 10:29:06.000000 ros-d2-1.0.4/ros_d2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-08 10:29:06.000000 ros-d2-1.0.4/ros_d2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-08 10:29:06.000000 ros-d2-1.0.4/ros_d2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-08 10:29:06.000000 ros-d2-1.0.4/ros_d2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 10:29:06.000000 ros-d2-1.0.4/ros_d2.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-02-08 10:29:06.914006 ros-d2-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-08 10:28:59.000000 ros-d2-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:59:04.684978 ros-d2-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-27 10:58:58.000000 ros-d2-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-27 10:59:04.684978 ros-d2-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-27 10:59:02.000000 ros-d2-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:59:04.684978 ros-d2-1.0.5/ros_d2/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-27 10:58:58.000000 ros-d2-1.0.5/ros_d2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-27 10:58:58.000000 ros-d2-1.0.5/ros_d2/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:59:04.684978 ros-d2-1.0.5/ros_d2/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-27 10:58:58.000000 ros-d2-1.0.5/ros_d2/helpers/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-27 10:58:58.000000 ros-d2-1.0.5/ros_d2/helpers/get_ros_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-27 10:58:58.000000 ros-d2-1.0.5/ros_d2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:59:04.684978 ros-d2-1.0.5/ros_d2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-27 10:59:04.000000 ros-d2-1.0.5/ros_d2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-27 10:59:04.000000 ros-d2-1.0.5/ros_d2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:59:04.000000 ros-d2-1.0.5/ros_d2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-27 10:59:04.000000 ros-d2-1.0.5/ros_d2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-27 10:59:04.000000 ros-d2-1.0.5/ros_d2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 10:59:04.000000 ros-d2-1.0.5/ros_d2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:59:04.000000 ros-d2-1.0.5/ros_d2.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-27 10:59:04.684978 ros-d2-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-27 10:58:58.000000 ros-d2-1.0.5/setup.py
```

### Comparing `ros-d2-1.0.4/LICENSE` & `ros-d2-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-d2-1.0.4/PKG-INFO` & `ros-d2-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-d2
-Version: 1.0.4
+Version: 1.0.5
 Summary: Exports ROS2 nodes into the .d2 diagram format
 Home-page: https://github.com/Greenroom-Robotics/ros-d2
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2022, Greenroom Robotics
```

### Comparing `ros-d2-1.0.4/README.md` & `ros-d2-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ros-d2-1.0.4/ros_d2/helpers/convert.py` & `ros-d2-1.0.5/ros_d2/helpers/convert.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 from typing import List
 
-from py_d2.D2Connection import D2Connection, Direction
-from py_d2.D2Diagram import D2Diagram
-from py_d2.D2Shape import D2Shape, D2Text, Shape
-from py_d2.D2Style import D2Style
+from py_d2 import D2Connection, D2Diagram, D2Shape, D2Style, D2Text, Direction
+from py_d2.shape import Shape
 
 from ros_d2.helpers.get_ros_architecture import RosArchitecture
 
 node_style = D2Style(
     opacity=0.6,
     three_d=True,
 )
```

### Comparing `ros-d2-1.0.4/ros_d2/helpers/get_ros_architecture.py` & `ros-d2-1.0.5/ros_d2/helpers/get_ros_architecture.py`

 * *Files identical despite different names*

### Comparing `ros-d2-1.0.4/ros_d2/main.py` & `ros-d2-1.0.5/ros_d2/main.py`

 * *Files identical despite different names*

### Comparing `ros-d2-1.0.4/ros_d2.egg-info/PKG-INFO` & `ros-d2-1.0.5/ros_d2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-d2
-Version: 1.0.4
+Version: 1.0.5
 Summary: Exports ROS2 nodes into the .d2 diagram format
 Home-page: https://github.com/Greenroom-Robotics/ros-d2
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2022, Greenroom Robotics
```

### Comparing `ros-d2-1.0.4/setup.cfg` & `ros-d2-1.0.5/setup.cfg`

 * *Files identical despite different names*

