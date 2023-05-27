# Comparing `tmp/shinherpro-1.6.5.tar.gz` & `tmp/shinherpro-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.6.5.tar", last modified: Mon May 22 15:34:34 2023, max compression
+gzip compressed data, was "shinherpro-1.6.6.tar", last modified: Sat May 27 03:12:41 2023, max compression
```

## Comparing `shinherpro-1.6.5.tar` & `shinherpro-1.6.6.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 15:34:34.959704 shinherpro-1.6.5/
--rw-rw-rw-   0        0        0     4623 2023-05-22 15:34:34.954297 shinherpro-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2023-05-21 09:21:34.000000 shinherpro-1.6.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 15:34:34.960202 shinherpro-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-05-22 12:54:15.000000 shinherpro-1.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 15:34:34.945370 shinherpro-1.6.5/shinherpro/
--rw-rw-rw-   0        0        0    10375 2023-05-22 15:34:26.000000 shinherpro-1.6.5/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-22 15:34:31.000000 shinherpro-1.6.5/shinherpro/__init__.py
--rw-rw-rw-   0        0        0     1225 2023-05-21 09:03:22.000000 shinherpro-1.6.5/shinherpro/chormeDriver.py
--rw-rw-rw-   0        0        0     1186 2023-05-22 15:33:52.000000 shinherpro-1.6.5/shinherpro/serverLog.py
--rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.5/shinherpro/vfcModel.py
-drwxrwxrwx   0        0        0        0 2023-05-22 15:34:34.953305 shinherpro-1.6.5/shinherpro.egg-info/
--rw-rw-rw-   0        0        0     4623 2023-05-22 15:34:34.000000 shinherpro-1.6.5/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-05-22 15:34:34.000000 shinherpro-1.6.5/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 15:34:34.000000 shinherpro-1.6.5/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-22 15:34:34.000000 shinherpro-1.6.5/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 15:34:34.000000 shinherpro-1.6.5/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 03:12:41.651933 shinherpro-1.6.6/
+-rw-rw-rw-   0        0        0      178 2023-05-27 03:12:41.650941 shinherpro-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-27 03:12:41.651933 shinherpro-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-05-27 03:12:24.000000 shinherpro-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 03:12:41.632092 shinherpro-1.6.6/shinherpro/
+-rw-rw-rw-   0        0        0    19138 2023-05-27 03:00:54.000000 shinherpro-1.6.6/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:34:31.000000 shinherpro-1.6.6/shinherpro/__init__.py
+-rw-rw-rw-   0        0        0     1293 2023-05-23 15:25:54.000000 shinherpro-1.6.6/shinherpro/chormeDriver.py
+-rw-rw-rw-   0        0        0     1186 2023-05-22 15:33:52.000000 shinherpro-1.6.6/shinherpro/serverLog.py
+-rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.6/shinherpro/vfcModel.py
+drwxrwxrwx   0        0        0        0 2023-05-27 03:12:41.649949 shinherpro-1.6.6/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-05-27 03:12:41.000000 shinherpro-1.6.6/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-27 03:12:41.000000 shinherpro-1.6.6/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 03:12:41.000000 shinherpro-1.6.6/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-27 03:12:41.000000 shinherpro-1.6.6/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-27 03:12:41.000000 shinherpro-1.6.6/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.6.5/shinherpro/chormeDriver.py` & `shinherpro-1.6.6/shinherpro/chormeDriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,8 +31,11 @@
     return driver
 
 def switch_frame(reset, frame, driver):
     if reset:
         driver.switch_to.default_content()
     for frame_name in frame:
         right_frame = driver.find_element(By.NAME, frame_name)
-        driver.switch_to.frame(right_frame)
+        driver.switch_to.frame(right_frame)
+
+def reset_frame(driver):
+    driver.switch_to.default_content()
```

### Comparing `shinherpro-1.6.5/shinherpro/serverLog.py` & `shinherpro-1.6.6/shinherpro/serverLog.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.5/shinherpro/vfcModel.py` & `shinherpro-1.6.6/shinherpro/vfcModel.py`

 * *Files identical despite different names*

