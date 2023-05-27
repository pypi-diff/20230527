# Comparing `tmp/growmax-1.2.1.tar.gz` & `tmp/growmax-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "growmax-1.2.1.tar", last modified: Sun May 21 22:01:45 2023, max compression
+gzip compressed data, was "growmax-1.2.2.tar", last modified: Sat May 27 00:55:01 2023, max compression
```

## Comparing `growmax-1.2.1.tar` & `growmax-1.2.2.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.581334 growmax-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-21 22:01:34.000000 growmax-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-21 22:01:45.585334 growmax-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-21 22:01:34.000000 growmax-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-21 22:01:34.000000 growmax-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-21 22:01:45.585334 growmax-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.573334 growmax-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.577334 growmax-1.2.1/src/growmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.577334 growmax-1.2.1/src/growmax/atlas_ph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/import_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/set_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/uart_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.581334 growmax-1.2.1/src/growmax/displays/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/displays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/displays/sh1107.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/displays/ssd1327.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/moisture.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/ntpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/pump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/routine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.581334 growmax-1.2.1/src/growmax/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/sensors/adafruit_scd4x.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/sensors/motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.581334 growmax-1.2.1/src/growmax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/displays.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/water.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.577334 growmax-1.2.1/src/growmax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-21 22:01:45.000000 growmax-1.2.1/src/growmax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-21 22:01:45.000000 growmax-1.2.1/src/growmax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 22:01:45.000000 growmax-1.2.1/src/growmax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 22:01:45.000000 growmax-1.2.1/src/growmax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.052908 growmax-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-27 00:54:46.000000 growmax-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-27 00:55:01.052908 growmax-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-27 00:54:46.000000 growmax-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-27 00:54:46.000000 growmax-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-27 00:55:01.052908 growmax-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.040908 growmax-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.044908 growmax-1.2.2/src/growmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.048908 growmax-1.2.2/src/growmax/atlas_ph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/import_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/set_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/atlas_ph/uart_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.048908 growmax-1.2.2/src/growmax/displays/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/displays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/displays/sh1107.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/displays/ssd1327.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/moisture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/ntpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/pump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.048908 growmax-1.2.2/src/growmax/relays/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/relays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/relays/i2c_relays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/routine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.048908 growmax-1.2.2/src/growmax/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/sensors/adafruit_scd4x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/sensors/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.052908 growmax-1.2.2/src/growmax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/displays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/relays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/water.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-27 00:54:46.000000 growmax-1.2.2/src/growmax/utils/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:01.048908 growmax-1.2.2/src/growmax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-27 00:55:01.000000 growmax-1.2.2/src/growmax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-27 00:55:01.000000 growmax-1.2.2/src/growmax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:55:01.000000 growmax-1.2.2/src/growmax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-27 00:55:01.000000 growmax-1.2.2/src/growmax.egg-info/top_level.txt
```

### Comparing `growmax-1.2.1/LICENSE` & `growmax-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/PKG-INFO` & `growmax-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.2.1
+Version: 1.2.2
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
```

### Comparing `growmax-1.2.1/README.md` & `growmax-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/setup.cfg` & `growmax-1.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = growmax
-version = 1.2.1
+version = 1.2.2
 author = Matt Davis and OpenSensor.io
 author_email = matteius@gmail.com
 description = Micropython routines for automated plant watering and monitoring.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/opensensor/growmax
 project_urls =
```

### Comparing `growmax-1.2.1/src/growmax/atlas_ph/calibration.py` & `growmax-1.2.2/src/growmax/atlas_ph/calibration.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/atlas_ph/i2c.py` & `growmax-1.2.2/src/growmax/atlas_ph/i2c.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/constants.py` & `growmax-1.2.2/src/growmax/constants.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/displays/sh1107.py` & `growmax-1.2.2/src/growmax/displays/sh1107.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/displays/ssd1327.py` & `growmax-1.2.2/src/growmax/displays/ssd1327.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/moisture.py` & `growmax-1.2.2/src/growmax/moisture.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/ntpclient.py` & `growmax-1.2.2/src/growmax/ntpclient.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/pump.py` & `growmax-1.2.2/src/growmax/pump.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/routine.py` & `growmax-1.2.2/src/growmax/routine.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import utime
 from machine import Pin
 
 from growmax.atlas_ph.i2c import AtlasPHI2C
 from growmax.moisture import Moisture
 from growmax.pump import Pump
 from growmax.utils import api
-from growmax.utils.configs import get_moisture_threshold_for_position
+from growmax.utils.configs import get_config_value, get_moisture_threshold_for_position
 from growmax.utils.displays import boot_sequence, display_basic_stats, display_ph_reading, display_scd4x_reading
 from growmax.utils.mcu import get_gpio_for_mcu
+from growmax.utils.relays import initialize_relay_board
 from growmax.utils.sensors import init_adafruit_scd4x, read_adafruit_scd4x
 from growmax.utils.water import statistically_has_water
 from growmax.utils.wifi import ensure_wifi_connected
 
 # User's config file
 import config
 
@@ -21,18 +22,19 @@
 random.seed()
 
 
 def main():
     boot_sequence()
 
     water_sensor = None
-    if config.WATER_SENSOR_LOW_ENABLED:
+    if get_config_value("WATER_SENSOR_LOW_ENABLED"):
         water_sensor = Pin(get_gpio_for_mcu(config.WATER_SENSOR_LOW), Pin.IN, Pin.PULL_DOWN)
     scd40x = None
     atlas_ph = None
+    relay_board = initialize_relay_board()
 
     soil_sensors = [Moisture(channel=1), Moisture(channel=2), Moisture(channel=3), Moisture(channel=4),
                     Moisture(channel=5), Moisture(channel=6), Moisture(channel=7), Moisture(channel=8)]
     pumps = [Pump(channel=1), Pump(channel=2), Pump(channel=3), Pump(channel=4),
              Pump(channel=5), Pump(channel=6), Pump(channel=7), Pump(channel=8)]
 
     while True:
@@ -43,26 +45,32 @@
         except Exception:
             # Potentially no wi-fi
             pass
 
         if config.ADAFRUIT_SCD4X_ENABLED and scd40x is None:
             scd40x = init_adafruit_scd4x(config.ADAFRUIT_SCD4X_I2C_CHANNEL)
 
-        if hasattr(config, "ATLAS_PH_METER_ENABLED") and config.ATLAS_PH_METER_ENABLED:
+        if get_config_value("ATLAS_PH_METER_ENABLED"):
             try:
                 atlas_ph = AtlasPHI2C(config.ATLAS_PH_I2C_CHANNEL)
             except Exception as e:
                 print(f"Error initializing Atlas pH probe: {e}")
 
-        soil_moistures = []
+        has_water = water_sensor and statistically_has_water(water_sensor)
+        if not has_water and relay_board and get_config_value("AUTO_REFILL_RELAY_POSITION"):
+            relay_board.turn_on(get_config_value("AUTO_REFILL_RELAY_POSITION"))
+            utime.sleep(get_config_value("AUTO_REFILL_DURATION", 45))
+            relay_board.turn_off(get_config_value("AUTO_REFILL_RELAY_POSITION"))
+
+        soil_moisture = []
         for position, soil_sensor in enumerate(soil_sensors):
             try:
                 pump_position = str(position + 1)
                 soil_moisture = soil_sensor.moisture
-                soil_moistures.append(soil_moisture)
+                soil_moisture.append(soil_moisture)
                 has_water = water_sensor and statistically_has_water(water_sensor)
                 moisture_config = get_moisture_threshold_for_position(position)
                 print("Position ", pump_position,
                       " reservoir has water ", has_water,
                       " and moisture value ", soil_moisture, "/", moisture_config)
                 display_basic_stats(has_water, pump_position, soil_moisture, moisture_config)
                 if (config.PUMP_WHEN_DRY or has_water) and soil_moisture >= moisture_config:
@@ -80,32 +88,32 @@
         if scd40x:
             temp, rh, ppm_carbon_dioxide = read_adafruit_scd4x(scd40x)
         if config.OPEN_SENSOR_COLLECT_DATA:
             report_data = api.get_device_metadata()
             if scd40x:
                 api.add_adafruit_scd4x_data_to_report(report_data, temp, rh, ppm_carbon_dioxide)
             report_data["moisture"] = {
-                "readings": soil_moistures
+                "readings": soil_moisture
             }
             if atlas_ph and ph_reading:
                 report_data["pH"] = {
                     "pH": ph_reading
                 }
             api.report_environment_data(report_data)
-        if config.OPEN_SENSOR_RETRIEVE_COMMANDS:
+        has_water = water_sensor and statistically_has_water(water_sensor)
+        if get_config_value("OPEN_SENSOR_RETRIEVE_COMMANDS") and (config.PUMP_WHEN_DRY or has_water):
             command_parts = api.retrieve_command()  # Experimental
             if command_parts and len(command_parts) == 3 and command_parts[0] == "WATER":
-                print("WATER", command_parts[1], command_parts[2])
                 pos = int(command_parts[1]) - 1
                 duration = int(command_parts[2])
                 pumps[pos].dose(1, duration)
         if scd40x:
             display_scd4x_reading(temp, rh, ppm_carbon_dioxide)
             utime.sleep(3)
         if atlas_ph:
             display_ph_reading(ph_reading)
             utime.sleep(3)
 
-        print("Completed iteration; soil_moisture's = ", str(soil_moistures))
+        print("Completed iteration; soil_moisture's = ", str(soil_moisture))
         print("Free mem before garbage collection: ", str(gc.mem_free()))
         gc.collect()
         print("Free mem after garbage collection: ", str(gc.mem_free()))
```

### Comparing `growmax-1.2.1/src/growmax/sensors/adafruit_scd4x.py` & `growmax-1.2.2/src/growmax/sensors/adafruit_scd4x.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/sensors/motion.py` & `growmax-1.2.2/src/growmax/sensors/motion.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/utils/api.py` & `growmax-1.2.2/src/growmax/utils/api.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/utils/displays.py` & `growmax-1.2.2/src/growmax/utils/displays.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/utils/sensors.py` & `growmax-1.2.2/src/growmax/utils/sensors.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax/utils/wifi.py` & `growmax-1.2.2/src/growmax/utils/wifi.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.1/src/growmax.egg-info/PKG-INFO` & `growmax-1.2.2/src/growmax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.2.1
+Version: 1.2.2
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
```

### Comparing `growmax-1.2.1/src/growmax.egg-info/SOURCES.txt` & `growmax-1.2.2/src/growmax.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -19,18 +19,21 @@
 src/growmax/atlas_ph/i2c.py
 src/growmax/atlas_ph/import_config.py
 src/growmax/atlas_ph/set_i2c.py
 src/growmax/atlas_ph/uart_read.py
 src/growmax/displays/__init__.py
 src/growmax/displays/sh1107.py
 src/growmax/displays/ssd1327.py
+src/growmax/relays/__init__.py
+src/growmax/relays/i2c_relays.py
 src/growmax/sensors/__init__.py
 src/growmax/sensors/adafruit_scd4x.py
 src/growmax/sensors/motion.py
 src/growmax/utils/__init__.py
 src/growmax/utils/api.py
 src/growmax/utils/configs.py
 src/growmax/utils/displays.py
 src/growmax/utils/mcu.py
+src/growmax/utils/relays.py
 src/growmax/utils/sensors.py
 src/growmax/utils/water.py
 src/growmax/utils/wifi.py
```

