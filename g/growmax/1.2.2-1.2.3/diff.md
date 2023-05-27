# Comparing `tmp/growmax-1.2.2.tar.gz` & `tmp/growmax-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "growmax-1.2.2.tar", last modified: Sat May 27 00:55:01 2023, max compression
+gzip compressed data, was "growmax-1.2.3.tar", last modified: Sat May 27 01:05:35 2023, max compression
```

## Comparing `growmax-1.2.2.tar` & `growmax-1.2.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.052908 growmax-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-27 00:54:46.000000 growmax-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-27 00:55:01.052908 growmax-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-27 00:54:46.000000 growmax-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-27 00:54:46.000000 growmax-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-27 00:55:01.052908 growmax-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.040908 growmax-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.044908 growmax-1.2.2/src/growmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.048908 growmax-1.2.2/src/growmax/atlas_ph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/import_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/set_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/uart_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.048908 growmax-1.2.2/src/growmax/displays/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/displays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/displays/sh1107.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/displays/ssd1327.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/moisture.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/ntpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/pump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.048908 growmax-1.2.2/src/growmax/relays/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/relays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/relays/i2c_relays.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/routine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.048908 growmax-1.2.2/src/growmax/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/sensors/adafruit_scd4x.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/sensors/motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.052908 growmax-1.2.2/src/growmax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/displays.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/relays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/water.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.048908 growmax-1.2.2/src/growmax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-27 00:55:01.000000 growmax-1.2.2/src/growmax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-27 00:55:01.000000 growmax-1.2.2/src/growmax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:55:01.000000 growmax-1.2.2/src/growmax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-27 00:55:01.000000 growmax-1.2.2/src/growmax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.758313 growmax-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-27 01:05:22.000000 growmax-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-27 01:05:35.758313 growmax-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-27 01:05:22.000000 growmax-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-27 01:05:22.000000 growmax-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-27 01:05:35.758313 growmax-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.754313 growmax-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.754313 growmax-1.2.3/src/growmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.754313 growmax-1.2.3/src/growmax/atlas_ph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/import_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/set_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/atlas_ph/uart_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.758313 growmax-1.2.3/src/growmax/displays/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/displays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/displays/sh1107.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/displays/ssd1327.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/moisture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/ntpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/pump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.758313 growmax-1.2.3/src/growmax/relays/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/relays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/relays/i2c_relays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/routine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.758313 growmax-1.2.3/src/growmax/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/sensors/adafruit_scd4x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/sensors/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.758313 growmax-1.2.3/src/growmax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/displays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/relays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/water.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-27 01:05:22.000000 growmax-1.2.3/src/growmax/utils/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 01:05:35.754313 growmax-1.2.3/src/growmax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-27 01:05:35.000000 growmax-1.2.3/src/growmax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-27 01:05:35.000000 growmax-1.2.3/src/growmax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 01:05:35.000000 growmax-1.2.3/src/growmax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-27 01:05:35.000000 growmax-1.2.3/src/growmax.egg-info/top_level.txt
```

### Comparing `growmax-1.2.2/LICENSE` & `growmax-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/PKG-INFO` & `growmax-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.2.2
+Version: 1.2.3
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
```

### Comparing `growmax-1.2.2/README.md` & `growmax-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/setup.cfg` & `growmax-1.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = growmax
-version = 1.2.2
+version = 1.2.3
 author = Matt Davis and OpenSensor.io
 author_email = matteius@gmail.com
 description = Micropython routines for automated plant watering and monitoring.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/opensensor/growmax
 project_urls =
```

### Comparing `growmax-1.2.2/src/growmax/atlas_ph/calibration.py` & `growmax-1.2.3/src/growmax/atlas_ph/calibration.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/atlas_ph/i2c.py` & `growmax-1.2.3/src/growmax/atlas_ph/i2c.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/config.py` & `growmax-1.2.3/src/growmax/config.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/constants.py` & `growmax-1.2.3/src/growmax/constants.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/displays/sh1107.py` & `growmax-1.2.3/src/growmax/displays/sh1107.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/displays/ssd1327.py` & `growmax-1.2.3/src/growmax/displays/ssd1327.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/moisture.py` & `growmax-1.2.3/src/growmax/moisture.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/ntpclient.py` & `growmax-1.2.3/src/growmax/ntpclient.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/pump.py` & `growmax-1.2.3/src/growmax/pump.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/relays/i2c_relays.py` & `growmax-1.2.3/src/growmax/relays/i2c_relays.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/routine.py` & `growmax-1.2.3/src/growmax/routine.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,23 +61,23 @@
             utime.sleep(get_config_value("AUTO_REFILL_DURATION", 45))
             relay_board.turn_off(get_config_value("AUTO_REFILL_RELAY_POSITION"))
 
         soil_moisture = []
         for position, soil_sensor in enumerate(soil_sensors):
             try:
                 pump_position = str(position + 1)
-                soil_moisture = soil_sensor.moisture
-                soil_moisture.append(soil_moisture)
+                reading = soil_sensor.moisture
+                soil_moisture.append(reading)
                 has_water = water_sensor and statistically_has_water(water_sensor)
                 moisture_config = get_moisture_threshold_for_position(position)
                 print("Position ", pump_position,
                       " reservoir has water ", has_water,
-                      " and moisture value ", soil_moisture, "/", moisture_config)
-                display_basic_stats(has_water, pump_position, soil_moisture, moisture_config)
-                if (config.PUMP_WHEN_DRY or has_water) and soil_moisture >= moisture_config:
+                      " and moisture value ", reading, "/", moisture_config)
+                display_basic_stats(has_water, pump_position, reading, moisture_config)
+                if (config.PUMP_WHEN_DRY or has_water) and reading >= moisture_config:
                     print("position: ", pump_position)
                     pumps[position].dose(1, config.PUMP_CYCLE_DURATION)
                 utime.sleep(2)
             except Exception as e:
                 print("Exception: ", str(e))
 
         ph_reading = None
```

### Comparing `growmax-1.2.2/src/growmax/sensors/adafruit_scd4x.py` & `growmax-1.2.3/src/growmax/sensors/adafruit_scd4x.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/sensors/motion.py` & `growmax-1.2.3/src/growmax/sensors/motion.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/utils/api.py` & `growmax-1.2.3/src/growmax/utils/api.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/utils/displays.py` & `growmax-1.2.3/src/growmax/utils/displays.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/utils/relays.py` & `growmax-1.2.3/src/growmax/utils/relays.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/utils/sensors.py` & `growmax-1.2.3/src/growmax/utils/sensors.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax/utils/wifi.py` & `growmax-1.2.3/src/growmax/utils/wifi.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.2/src/growmax.egg-info/PKG-INFO` & `growmax-1.2.3/src/growmax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.2.2
+Version: 1.2.3
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
```

### Comparing `growmax-1.2.2/src/growmax.egg-info/SOURCES.txt` & `growmax-1.2.3/src/growmax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

