# Comparing `tmp/tasmota-metrics-0.3.3.tar.gz` & `tmp/tasmota-metrics-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tasmota-metrics-0.3.3.tar", last modified: Fri Apr 21 15:37:08 2023, max compression
+gzip compressed data, was "tasmota-metrics-0.3.4.tar", last modified: Sat May 27 18:39:34 2023, max compression
```

## Comparing `tasmota-metrics-0.3.3.tar` & `tasmota-metrics-0.3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:37:08.766675 tasmota-metrics-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-21 15:37:08.766675 tasmota-metrics-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 15:37:08.766675 tasmota-metrics-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:37:08.762675 tasmota-metrics-0.3.3/tasmota_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/tasmota_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/tasmota_metrics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:37:08.766675 tasmota-metrics-0.3.3/tasmota_metrics/chip_info/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/tasmota_metrics/chip_info/esp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/tasmota_metrics/chip_info/esp32c2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/tasmota_metrics/chip_info/esp32c3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/tasmota_metrics/chip_info/esp32c6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/tasmota_metrics/chip_info/esp32h2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/tasmota_metrics/chip_info/esp32h4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/tasmota_metrics/chip_info/esp32s2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/tasmota_metrics/chip_info/esp32s3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    56430 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/tasmota_metrics/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:37:08.762675 tasmota-metrics-0.3.3/tasmota_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-21 15:37:08.000000 tasmota-metrics-0.3.3/tasmota_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-21 15:37:08.000000 tasmota-metrics-0.3.3/tasmota_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:37:08.000000 tasmota-metrics-0.3.3/tasmota_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 15:37:08.000000 tasmota-metrics-0.3.3/tasmota_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 15:37:08.000000 tasmota-metrics-0.3.3/tasmota_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:37:08.766675 tasmota-metrics-0.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 15:36:52.000000 tasmota-metrics-0.3.3/test/test_tasmota_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:39:34.608893 tasmota-metrics-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-27 18:39:34.608893 tasmota-metrics-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 18:39:34.608893 tasmota-metrics-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:39:34.604893 tasmota-metrics-0.3.4/tasmota_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/tasmota_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/tasmota_metrics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:39:34.608893 tasmota-metrics-0.3.4/tasmota_metrics/chip_info/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/tasmota_metrics/chip_info/esp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/tasmota_metrics/chip_info/esp32c2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/tasmota_metrics/chip_info/esp32c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/tasmota_metrics/chip_info/esp32c6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/tasmota_metrics/chip_info/esp32h2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/tasmota_metrics/chip_info/esp32h4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/tasmota_metrics/chip_info/esp32s2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/tasmota_metrics/chip_info/esp32s3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    56433 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/tasmota_metrics/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:39:34.604893 tasmota-metrics-0.3.4/tasmota_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-27 18:39:34.000000 tasmota-metrics-0.3.4/tasmota_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-27 18:39:34.000000 tasmota-metrics-0.3.4/tasmota_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 18:39:34.000000 tasmota-metrics-0.3.4/tasmota_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-27 18:39:34.000000 tasmota-metrics-0.3.4/tasmota_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 18:39:34.000000 tasmota-metrics-0.3.4/tasmota_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:39:34.608893 tasmota-metrics-0.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-27 18:39:13.000000 tasmota-metrics-0.3.4/test/test_tasmota_metrics.py
```

### Comparing `tasmota-metrics-0.3.3/LICENSE` & `tasmota-metrics-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tasmota-metrics-0.3.3/PKG-INFO` & `tasmota-metrics-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tasmota-metrics
-Version: 0.3.3
+Version: 0.3.4
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/jason2866/tasmota-metrics
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tasmota-metrics-0.3.3/setup.py` & `tasmota-metrics-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `tasmota-metrics-0.3.3/tasmota_metrics/chip_info/esp32.yaml` & `tasmota-metrics-0.3.4/tasmota_metrics/chip_info/esp32.yaml`

 * *Files identical despite different names*

### Comparing `tasmota-metrics-0.3.3/tasmota_metrics/chip_info/esp32s2.yaml` & `tasmota-metrics-0.3.4/tasmota_metrics/chip_info/esp32s2.yaml`

 * *Files identical despite different names*

### Comparing `tasmota-metrics-0.3.3/tasmota_metrics/chip_info/esp32s3.yaml` & `tasmota-metrics-0.3.4/tasmota_metrics/chip_info/esp32s3.yaml`

 * *Files identical despite different names*

### Comparing `tasmota-metrics-0.3.3/tasmota_metrics/core.py` & `tasmota-metrics-0.3.4/tasmota_metrics/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
     ''' Detect target chip based on the target archive name in the linker script part of the MAP file '''
     scan_to_header(map_file, 'Linker script and memory map')
 
     RE_TARGET = re.compile(r'IDF_TARGET_(\S*) =')
     # For back-compatible with cmake in idf version before 5.0
     RE_TARGET_CMAKEv4x = re.compile(r'project_elf_src_(\S*)\.c.obj')
     # For back-compatible with make
-    RE_TARGET_MAKE = re.compile(r'^LOAD .*?/xtensa-([^-]+)-elf/')
+    RE_TARGET_MAKE = re.compile(r'^LOAD .*?/xtensa-(esp[^-]+)-elf/')
     # For PIO and RISC-V
     RE_TARGET_PIO = re.compile(r'^LOAD .*?/framework-arduinoespressif32/tools/sdk/([^-]+)/lib/')
 
     for line in map_file:
         match_target = RE_TARGET.search(line)
         if match_target:
             return match_target.group(1).lower()
```

### Comparing `tasmota-metrics-0.3.3/tasmota_metrics.egg-info/PKG-INFO` & `tasmota-metrics-0.3.4/tasmota_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tasmota-metrics
-Version: 0.3.3
+Version: 0.3.4
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/jason2866/tasmota-metrics
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tasmota-metrics-0.3.3/tasmota_metrics.egg-info/SOURCES.txt` & `tasmota-metrics-0.3.4/tasmota_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tasmota-metrics-0.3.3/test/test_tasmota_metrics.py` & `tasmota-metrics-0.3.4/test/test_tasmota_metrics.py`

 * *Files identical despite different names*

