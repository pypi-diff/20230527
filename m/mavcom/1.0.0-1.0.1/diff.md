# Comparing `tmp/mavcom-1.0.0.tar.gz` & `tmp/mavcom-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mavcom-1.0.0.tar", last modified: Fri May 26 23:02:05 2023, max compression
+gzip compressed data, was "mavcom-1.0.1.tar", last modified: Sat May 27 11:57:20 2023, max compression
```

## Comparing `mavcom-1.0.0.tar` & `mavcom-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-26 23:02:05.040235 mavcom-1.0.0/
--rw-rw-r--   0 main      (1000) main      (1000)     1066 2023-05-26 21:59:37.000000 mavcom-1.0.0/LICENSE
--rw-rw-r--   0 main      (1000) main      (1000)     2284 2023-05-26 23:02:05.040235 mavcom-1.0.0/PKG-INFO
--rw-rw-r--   0 main      (1000) main      (1000)      454 2023-05-26 21:22:47.000000 mavcom-1.0.0/README.md
--rw-rw-r--   0 main      (1000) main      (1000)      886 2023-05-26 23:01:46.000000 mavcom-1.0.0/pyproject.toml
--rw-rw-r--   0 main      (1000) main      (1000)       38 2023-05-26 23:02:05.040235 mavcom-1.0.0/setup.cfg
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-26 23:02:05.040235 mavcom-1.0.0/src/
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-26 23:02:05.040235 mavcom-1.0.0/src/mavcom/
--rw-rw-r--   0 main      (1000) main      (1000)        0 2023-05-26 10:29:36.000000 mavcom-1.0.0/src/mavcom/__init__.py
--rw-rw-r--   0 main      (1000) main      (1000)     9188 2023-05-26 21:19:59.000000 mavcom-1.0.0/src/mavcom/mavcom.py
--rw-rw-r--   0 main      (1000) main      (1000)     1646 2023-05-26 10:10:28.000000 mavcom-1.0.0/src/mavcom/mavconstants.py
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-26 23:02:05.040235 mavcom-1.0.0/src/mavcom.egg-info/
--rw-rw-r--   0 main      (1000) main      (1000)     2284 2023-05-26 23:02:05.000000 mavcom-1.0.0/src/mavcom.egg-info/PKG-INFO
--rw-rw-r--   0 main      (1000) main      (1000)      330 2023-05-26 23:02:05.000000 mavcom-1.0.0/src/mavcom.egg-info/SOURCES.txt
--rw-rw-r--   0 main      (1000) main      (1000)        1 2023-05-26 23:02:05.000000 mavcom-1.0.0/src/mavcom.egg-info/dependency_links.txt
--rw-rw-r--   0 main      (1000) main      (1000)       52 2023-05-26 23:02:05.000000 mavcom-1.0.0/src/mavcom.egg-info/entry_points.txt
--rw-rw-r--   0 main      (1000) main      (1000)       49 2023-05-26 23:02:05.000000 mavcom-1.0.0/src/mavcom.egg-info/requires.txt
--rw-rw-r--   0 main      (1000) main      (1000)        7 2023-05-26 23:02:05.000000 mavcom-1.0.0/src/mavcom.egg-info/top_level.txt
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-26 23:02:05.040235 mavcom-1.0.0/tests/
--rw-rw-r--   0 main      (1000) main      (1000)      769 2023-05-26 21:41:42.000000 mavcom-1.0.0/tests/test_mavcom.py
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 11:57:20.279576 mavcom-1.0.1/
+-rw-rw-r--   0 main      (1000) main      (1000)     1066 2023-05-26 21:59:37.000000 mavcom-1.0.1/LICENSE
+-rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 11:57:20.279576 mavcom-1.0.1/PKG-INFO
+-rw-rw-r--   0 main      (1000) main      (1000)      717 2023-05-26 23:18:10.000000 mavcom-1.0.1/README.md
+-rw-rw-r--   0 main      (1000) main      (1000)      886 2023-05-27 11:55:24.000000 mavcom-1.0.1/pyproject.toml
+-rw-rw-r--   0 main      (1000) main      (1000)       38 2023-05-27 11:57:20.279576 mavcom-1.0.1/setup.cfg
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 11:57:20.279576 mavcom-1.0.1/src/
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 11:57:20.279576 mavcom-1.0.1/src/mavcom/
+-rw-rw-r--   0 main      (1000) main      (1000)        0 2023-05-26 10:29:36.000000 mavcom-1.0.1/src/mavcom/__init__.py
+-rw-rw-r--   0 main      (1000) main      (1000)     9223 2023-05-27 11:53:36.000000 mavcom-1.0.1/src/mavcom/mavcom.py
+-rw-rw-r--   0 main      (1000) main      (1000)     1646 2023-05-26 10:10:28.000000 mavcom-1.0.1/src/mavcom/mavconstants.py
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 11:57:20.279576 mavcom-1.0.1/src/mavcom.egg-info/
+-rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/PKG-INFO
+-rw-rw-r--   0 main      (1000) main      (1000)      330 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 main      (1000) main      (1000)        1 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 main      (1000) main      (1000)       52 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/entry_points.txt
+-rw-rw-r--   0 main      (1000) main      (1000)       49 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/requires.txt
+-rw-rw-r--   0 main      (1000) main      (1000)        7 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/top_level.txt
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 11:57:20.279576 mavcom-1.0.1/tests/
+-rw-rw-r--   0 main      (1000) main      (1000)     1218 2023-05-27 00:25:30.000000 mavcom-1.0.1/tests/test_mavcom.py
```

### Comparing `mavcom-1.0.0/LICENSE` & `mavcom-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mavcom-1.0.0/PKG-INFO` & `mavcom-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,24 +43,35 @@
 
 ## Installation
 
 ```pip install mavcom```
 
 ## Basic Usage
 
+This is an example of how to use Mavcom with a simulated vehicle.
+
+Run SITL:
+
+```sim_vehicle.py -v ArduCopter```
+
 ```python
-import mavcom
+from mavcom import mavcom
 import time
 
 vehicle = mavcom.Mavcom(
-    connection_path = "/dev/ttyS0",
+    connection_path = "127.0.0.1:14551",
 )
 
 vehicle.start()
 
 while not vehicle.ready:
     print("Waiting for vehicle to initialise...")
     time.sleep(1)
 
 vehicle.motors_armed = True
+while not vehicle.motors_armed:
+    print("Waiting for motors to spin up...")
+    time.sleep(1)
+    
+vehicle.flight_mode = "GUIDED"
 vehicle.takeoff(alt=10)
 ```
```

### Comparing `mavcom-1.0.0/pyproject.toml` & `mavcom-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mavcom"
-version = "1.0.0"
+version = "1.0.1"
 description = "A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers"
 readme = "README.md"
 authors = [{ name = "Mavscient", email = "mavscient@xee4c.33mail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mavcom-1.0.0/src/mavcom/mavcom.py` & `mavcom-1.0.1/src/mavcom/mavcom.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,23 +28,24 @@
         self.current_values = defaultdict(lambda: None)
         self.controller = controller
         
         self._flight_mode = None
         self._motors_armed = False
         self.airframe = None
         
-        self.telemetry_thread = threading.Thread(target=self.monitor_mavlink_messages)
+        self.telemetry_thread = threading.Thread(target=self.monitor_mavlink_messages, daemon=True)
 
         self.connection = mavutil.mavlink_connection(connection_path, baud=baud)
         self.get_heartbeat()
 
     def start(self):
         """Starts listening to the Mavlink messages from the flight controller."""
         print("MAVCOM: Mavcom active")
         self.telemetry_thread.start()
+        time.sleep(3)
 
     def get_heartbeat(self):
         print("MAVCOM: Waiting for heartbeat...")
         self.connection.wait_heartbeat()
         print(f"MAVCOM: Heartbeat from system (system {self.connection.target_system} "
                     f"component {self.connection.target_component})")
         hb = self.connection.recv_match(type="HEARTBEAT", blocking = True)
```

### Comparing `mavcom-1.0.0/src/mavcom/mavconstants.py` & `mavcom-1.0.1/src/mavcom/mavconstants.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.0.0/src/mavcom.egg-info/PKG-INFO` & `mavcom-1.0.1/src/mavcom.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,24 +43,35 @@
 
 ## Installation
 
 ```pip install mavcom```
 
 ## Basic Usage
 
+This is an example of how to use Mavcom with a simulated vehicle.
+
+Run SITL:
+
+```sim_vehicle.py -v ArduCopter```
+
 ```python
-import mavcom
+from mavcom import mavcom
 import time
 
 vehicle = mavcom.Mavcom(
-    connection_path = "/dev/ttyS0",
+    connection_path = "127.0.0.1:14551",
 )
 
 vehicle.start()
 
 while not vehicle.ready:
     print("Waiting for vehicle to initialise...")
     time.sleep(1)
 
 vehicle.motors_armed = True
+while not vehicle.motors_armed:
+    print("Waiting for motors to spin up...")
+    time.sleep(1)
+    
+vehicle.flight_mode = "GUIDED"
 vehicle.takeoff(alt=10)
 ```
```

