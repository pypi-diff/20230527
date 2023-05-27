# Comparing `tmp/growmax-1.2.3.tar.gz` & `tmp/growmax-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "growmax-1.2.3.tar", last modified: Sat May 27 01:05:35 2023, max compression
+gzip compressed data, was "growmax-1.2.4.tar", last modified: Sat May 27 01:18:23 2023, max compression
```

## Comparing `growmax-1.2.3.tar` & `growmax-1.2.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.758313 growmax-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-27 01:05:22.000000 growmax-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-27 01:05:35.758313 growmax-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-27 01:05:22.000000 growmax-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-27 01:05:22.000000 growmax-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-27 01:05:35.758313 growmax-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.754313 growmax-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.754313 growmax-1.2.3/src/growmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.754313 growmax-1.2.3/src/growmax/atlas_ph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/import_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/set_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/uart_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.758313 growmax-1.2.3/src/growmax/displays/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/displays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/displays/sh1107.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/displays/ssd1327.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/moisture.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/ntpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/pump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.758313 growmax-1.2.3/src/growmax/relays/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/relays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/relays/i2c_relays.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/routine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.758313 growmax-1.2.3/src/growmax/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/sensors/adafruit_scd4x.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/sensors/motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.758313 growmax-1.2.3/src/growmax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/displays.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/relays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/water.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.754313 growmax-1.2.3/src/growmax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-27 01:05:35.000000 growmax-1.2.3/src/growmax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-27 01:05:35.000000 growmax-1.2.3/src/growmax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 01:05:35.000000 growmax-1.2.3/src/growmax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-27 01:05:35.000000 growmax-1.2.3/src/growmax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:23.442938 growmax-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-27 01:18:12.000000 growmax-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-27 01:18:23.442938 growmax-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-27 01:18:12.000000 growmax-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-27 01:18:12.000000 growmax-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-27 01:18:23.446938 growmax-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:23.438938 growmax-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:23.438938 growmax-1.2.4/src/growmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:23.442938 growmax-1.2.4/src/growmax/atlas_ph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/atlas_ph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/atlas_ph/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/atlas_ph/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/atlas_ph/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/atlas_ph/import_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/atlas_ph/set_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/atlas_ph/uart_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:23.442938 growmax-1.2.4/src/growmax/displays/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/displays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/displays/sh1107.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/displays/ssd1327.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/moisture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/ntpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/pump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:23.442938 growmax-1.2.4/src/growmax/relays/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/relays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/relays/i2c_relays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/routine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:23.442938 growmax-1.2.4/src/growmax/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/sensors/adafruit_scd4x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/sensors/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:23.442938 growmax-1.2.4/src/growmax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/utils/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/utils/displays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/utils/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/utils/relays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/utils/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/utils/water.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-27 01:18:12.000000 growmax-1.2.4/src/growmax/utils/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:18:23.442938 growmax-1.2.4/src/growmax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-27 01:18:23.000000 growmax-1.2.4/src/growmax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-27 01:18:23.000000 growmax-1.2.4/src/growmax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 01:18:23.000000 growmax-1.2.4/src/growmax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-27 01:18:23.000000 growmax-1.2.4/src/growmax.egg-info/top_level.txt
```

### Comparing `growmax-1.2.3/LICENSE` & `growmax-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/PKG-INFO` & `growmax-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.2.3
+Version: 1.2.4
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
```

### Comparing `growmax-1.2.3/README.md` & `growmax-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/setup.cfg` & `growmax-1.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = growmax
-version = 1.2.3
+version = 1.2.4
 author = Matt Davis and OpenSensor.io
 author_email = matteius@gmail.com
 description = Micropython routines for automated plant watering and monitoring.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/opensensor/growmax
 project_urls =
```

### Comparing `growmax-1.2.3/src/growmax/atlas_ph/calibration.py` & `growmax-1.2.4/src/growmax/atlas_ph/calibration.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/atlas_ph/i2c.py` & `growmax-1.2.4/src/growmax/atlas_ph/i2c.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/config.py` & `growmax-1.2.4/src/growmax/config.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/constants.py` & `growmax-1.2.4/src/growmax/constants.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/displays/sh1107.py` & `growmax-1.2.4/src/growmax/displays/sh1107.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/displays/ssd1327.py` & `growmax-1.2.4/src/growmax/displays/ssd1327.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/moisture.py` & `growmax-1.2.4/src/growmax/moisture.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/ntpclient.py` & `growmax-1.2.4/src/growmax/ntpclient.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/pump.py` & `growmax-1.2.4/src/growmax/pump.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/relays/i2c_relays.py` & `growmax-1.2.4/src/growmax/relays/i2c_relays.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,23 @@
         self.num_relays = num_relays
         # Initialize all relays to off (0)
         self.state = [0]*8
 
     def turn_on(self, position):
         # Turn on relay at the specified position
         position -= 1
-        if self.num_relays == 4:
-            position += 4
         self.state[position] = 1
         self._write_state()
 
     def turn_off(self, position):
         # Turn off relay at the specified position
         position -= 1
-        if self.num_relays == 4:
-            position += 4
         self.state[position] = 0
         self._write_state()
 
     def _write_state(self):
         # Convert state list to integer
         state_as_int = int(''.join(map(str, self.state)), 2)
         # If relay board uses active low, invert the bits before sending
         inverted_state = ~state_as_int & 0xFF
-        print(f"Writing state to board: {bin(inverted_state)}")
+        print(f"Writing state to relay board: {bin(inverted_state)}")
         self.i2c.writeto(self.addr, inverted_state.to_bytes(1, "big"))
```

### Comparing `growmax-1.2.3/src/growmax/routine.py` & `growmax-1.2.4/src/growmax/routine.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/sensors/adafruit_scd4x.py` & `growmax-1.2.4/src/growmax/sensors/adafruit_scd4x.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/sensors/motion.py` & `growmax-1.2.4/src/growmax/sensors/motion.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/utils/api.py` & `growmax-1.2.4/src/growmax/utils/api.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/utils/displays.py` & `growmax-1.2.4/src/growmax/utils/displays.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/utils/relays.py` & `growmax-1.2.4/src/growmax/utils/relays.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/utils/sensors.py` & `growmax-1.2.4/src/growmax/utils/sensors.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax/utils/wifi.py` & `growmax-1.2.4/src/growmax/utils/wifi.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.3/src/growmax.egg-info/PKG-INFO` & `growmax-1.2.4/src/growmax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.2.3
+Version: 1.2.4
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
```

### Comparing `growmax-1.2.3/src/growmax.egg-info/SOURCES.txt` & `growmax-1.2.4/src/growmax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

