# Comparing `tmp/mavcom-1.1.0.tar.gz` & `tmp/mavcom-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mavcom-1.1.0.tar", last modified: Sat May 27 12:53:42 2023, max compression
+gzip compressed data, was "mavcom-1.1.1.tar", last modified: Sat May 27 18:11:04 2023, max compression
```

## Comparing `mavcom-1.1.0.tar` & `mavcom-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 12:53:42.993623 mavcom-1.1.0/
--rw-rw-r--   0 main      (1000) main      (1000)     1066 2023-05-26 21:59:37.000000 mavcom-1.1.0/LICENSE
--rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 12:53:42.993623 mavcom-1.1.0/PKG-INFO
--rw-rw-r--   0 main      (1000) main      (1000)      717 2023-05-26 23:18:10.000000 mavcom-1.1.0/README.md
--rw-rw-r--   0 main      (1000) main      (1000)      886 2023-05-27 12:52:30.000000 mavcom-1.1.0/pyproject.toml
--rw-rw-r--   0 main      (1000) main      (1000)       38 2023-05-27 12:53:42.993623 mavcom-1.1.0/setup.cfg
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 12:53:42.993623 mavcom-1.1.0/src/
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 12:53:42.993623 mavcom-1.1.0/src/mavcom/
--rw-rw-r--   0 main      (1000) main      (1000)        0 2023-05-26 10:29:36.000000 mavcom-1.1.0/src/mavcom/__init__.py
--rw-rw-r--   0 main      (1000) main      (1000)     9223 2023-05-27 11:53:36.000000 mavcom-1.1.0/src/mavcom/mavcom.py
--rw-rw-r--   0 main      (1000) main      (1000)     1646 2023-05-26 10:10:28.000000 mavcom-1.1.0/src/mavcom/mavconstants.py
--rw-rw-r--   0 main      (1000) main      (1000)     4332 2023-05-27 12:36:59.000000 mavcom-1.1.0/src/mavcom/video.py
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 12:53:42.993623 mavcom-1.1.0/src/mavcom.egg-info/
--rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 12:53:42.000000 mavcom-1.1.0/src/mavcom.egg-info/PKG-INFO
--rw-rw-r--   0 main      (1000) main      (1000)      350 2023-05-27 12:53:42.000000 mavcom-1.1.0/src/mavcom.egg-info/SOURCES.txt
--rw-rw-r--   0 main      (1000) main      (1000)        1 2023-05-27 12:53:42.000000 mavcom-1.1.0/src/mavcom.egg-info/dependency_links.txt
--rw-rw-r--   0 main      (1000) main      (1000)       52 2023-05-27 12:53:42.000000 mavcom-1.1.0/src/mavcom.egg-info/entry_points.txt
--rw-rw-r--   0 main      (1000) main      (1000)       49 2023-05-27 12:53:42.000000 mavcom-1.1.0/src/mavcom.egg-info/requires.txt
--rw-rw-r--   0 main      (1000) main      (1000)        7 2023-05-27 12:53:42.000000 mavcom-1.1.0/src/mavcom.egg-info/top_level.txt
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 12:53:42.993623 mavcom-1.1.0/tests/
--rw-rw-r--   0 main      (1000) main      (1000)     1218 2023-05-27 00:25:30.000000 mavcom-1.1.0/tests/test_mavcom.py
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 18:11:04.426995 mavcom-1.1.1/
+-rw-rw-r--   0 main      (1000) main      (1000)     1066 2023-05-26 21:59:37.000000 mavcom-1.1.1/LICENSE
+-rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 18:11:04.426995 mavcom-1.1.1/PKG-INFO
+-rw-rw-r--   0 main      (1000) main      (1000)      717 2023-05-26 23:18:10.000000 mavcom-1.1.1/README.md
+-rw-rw-r--   0 main      (1000) main      (1000)      886 2023-05-27 18:10:03.000000 mavcom-1.1.1/pyproject.toml
+-rw-rw-r--   0 main      (1000) main      (1000)       38 2023-05-27 18:11:04.426995 mavcom-1.1.1/setup.cfg
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 18:11:04.426995 mavcom-1.1.1/src/
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 18:11:04.426995 mavcom-1.1.1/src/mavcom/
+-rw-rw-r--   0 main      (1000) main      (1000)        0 2023-05-26 10:29:36.000000 mavcom-1.1.1/src/mavcom/__init__.py
+-rw-rw-r--   0 main      (1000) main      (1000)     1646 2023-05-26 10:10:28.000000 mavcom-1.1.1/src/mavcom/mavconstants.py
+-rw-rw-r--   0 main      (1000) main      (1000)    12499 2023-05-27 18:09:22.000000 mavcom-1.1.1/src/mavcom/mavcontrol.py
+-rw-rw-r--   0 main      (1000) main      (1000)     4332 2023-05-27 12:36:59.000000 mavcom-1.1.1/src/mavcom/video.py
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 18:11:04.426995 mavcom-1.1.1/src/mavcom.egg-info/
+-rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 18:11:04.000000 mavcom-1.1.1/src/mavcom.egg-info/PKG-INFO
+-rw-rw-r--   0 main      (1000) main      (1000)      354 2023-05-27 18:11:04.000000 mavcom-1.1.1/src/mavcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 main      (1000) main      (1000)        1 2023-05-27 18:11:04.000000 mavcom-1.1.1/src/mavcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 main      (1000) main      (1000)       52 2023-05-27 18:11:04.000000 mavcom-1.1.1/src/mavcom.egg-info/entry_points.txt
+-rw-rw-r--   0 main      (1000) main      (1000)       49 2023-05-27 18:11:04.000000 mavcom-1.1.1/src/mavcom.egg-info/requires.txt
+-rw-rw-r--   0 main      (1000) main      (1000)        7 2023-05-27 18:11:04.000000 mavcom-1.1.1/src/mavcom.egg-info/top_level.txt
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 18:11:04.426995 mavcom-1.1.1/tests/
+-rw-rw-r--   0 main      (1000) main      (1000)     1208 2023-05-27 18:09:22.000000 mavcom-1.1.1/tests/test_mavcom.py
```

### Comparing `mavcom-1.1.0/LICENSE` & `mavcom-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.0/PKG-INFO` & `mavcom-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mavcom-1.1.0/README.md` & `mavcom-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.0/pyproject.toml` & `mavcom-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mavcom"
-version = "1.1.0"
+version = "1.1.1"
 description = "A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers"
 readme = "README.md"
 authors = [{ name = "Mavscient", email = "mavscient@xee4c.33mail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mavcom-1.1.0/src/mavcom/mavconstants.py` & `mavcom-1.1.1/src/mavcom/mavconstants.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.0/src/mavcom/video.py` & `mavcom-1.1.1/src/mavcom/video.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.0/src/mavcom.egg-info/PKG-INFO` & `mavcom-1.1.1/src/mavcom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mavcom-1.1.0/tests/test_mavcom.py` & `mavcom-1.1.1/tests/test_mavcom.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from mavcom import mavcom
+from mavcom.mavcontrol import Mavcom
 from multiprocessing import Process
 import time
 import os
-import atexit
 
 def sim_vehicle():
     os.system("gnome-terminal --tab -e 'bash -c \"sim_vehicle.py -v ArduCopter; exec bash\"'")
 
 sim = Process(target=sim_vehicle, daemon=True)
 sim.start()
 print(sim.pid)
 
-vehicle = mavcom.Mavcom(
+vehicle = Mavcom(
     connection_path="127.0.0.1:14551"
 )
 vehicle.start()
 time.sleep(1)
 
 def test_receiving_mavlink_packets():
     assert len(vehicle.current_values) > 0
```

