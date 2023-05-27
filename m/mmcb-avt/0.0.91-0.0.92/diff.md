# Comparing `tmp/mmcb-avt-0.0.91.tar.gz` & `tmp/mmcb-avt-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.91.tar", last modified: Sat May 27 07:54:48 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.92.tar", last modified: Sat May 27 08:08:05 2023, max compression
```

## Comparing `mmcb-avt-0.0.91.tar` & `mmcb-avt-0.0.92.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 07:54:48.591572 mmcb-avt-0.0.91/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.91/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-27 07:54:48.589969 mmcb-avt-0.0.91/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.91/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb-avt-0.0.91/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-27 07:54:48.591864 mmcb-avt-0.0.91/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-27 07:54:35.000000 mmcb-avt-0.0.91/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 07:54:48.547898 mmcb-avt-0.0.91/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 07:54:48.580356 mmcb-avt-0.0.91/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.91/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93158 2023-05-27 07:42:26.000000 mmcb-avt-0.0.91/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    32486 2023-05-27 07:52:17.000000 mmcb-avt-0.0.91/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.91/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.91/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33782 2023-05-17 14:29:51.000000 mmcb-avt-0.0.91/src/mmcb/detect.py
--rwx------   0 avt        (501) staff       (20)     3235 2023-05-17 14:42:59.000000 mmcb-avt-0.0.91/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4688 2023-05-17 14:29:45.000000 mmcb-avt-0.0.91/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.91/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.91/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.91/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.91/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.91/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.91/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.91/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-05-27 07:52:28.000000 mmcb-avt-0.0.91/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.91/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.91/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.91/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.91/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 07:54:48.587834 mmcb-avt-0.0.91/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-27 07:54:48.000000 mmcb-avt-0.0.91/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      694 2023-05-27 07:54:48.000000 mmcb-avt-0.0.91/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-27 07:54:48.000000 mmcb-avt-0.0.91/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-27 07:54:48.000000 mmcb-avt-0.0.91/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-27 07:54:48.000000 mmcb-avt-0.0.91/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-27 07:54:48.000000 mmcb-avt-0.0.91/src/mmcb_avt.egg-info/top_level.txt
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 07:54:48.588683 mmcb-avt-0.0.91/tests/
--rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb-avt-0.0.91/tests/test_lexicon.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 08:08:05.315344 mmcb-avt-0.0.92/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.92/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-27 08:08:05.314521 mmcb-avt-0.0.92/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.92/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb-avt-0.0.92/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-27 08:08:05.315523 mmcb-avt-0.0.92/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2593 2023-05-27 08:07:41.000000 mmcb-avt-0.0.92/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 08:08:05.284690 mmcb-avt-0.0.92/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 08:08:05.307148 mmcb-avt-0.0.92/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.92/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93158 2023-05-27 07:42:26.000000 mmcb-avt-0.0.92/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    32486 2023-05-27 07:52:17.000000 mmcb-avt-0.0.92/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.92/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.92/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33782 2023-05-17 14:29:51.000000 mmcb-avt-0.0.92/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     3235 2023-05-17 14:42:59.000000 mmcb-avt-0.0.92/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4688 2023-05-17 14:29:45.000000 mmcb-avt-0.0.92/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.92/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.92/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.92/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.92/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.92/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.92/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.92/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-05-27 07:52:28.000000 mmcb-avt-0.0.92/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.92/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.92/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.92/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.92/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 08:08:05.312584 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      694 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      228 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-27 08:08:05.000000 mmcb-avt-0.0.92/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-27 08:08:05.313412 mmcb-avt-0.0.92/tests/
+-rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb-avt-0.0.92/tests/test_lexicon.py
```

### Comparing `mmcb-avt-0.0.91/LICENSE` & `mmcb-avt-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/PKG-INFO` & `mmcb-avt-0.0.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.91
+Version: 0.0.92
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.91/README.md` & `mmcb-avt-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/setup.py` & `mmcb-avt-0.0.92/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.91",
+    version="0.0.92",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -22,15 +22,15 @@
     include_package_data=True,
     python_requires=">=3.6",
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "zmq",
-        "pyserial==3.4",
+        "pyserial==3.4.*",
         "smbus",
         "tables",
         "Adafruit-Blinka",
         "adafruit-circuitpython-ads1x15",
         "adafruit-circuitpython-bme680",
         "adafruit-circuitpython-pcf8591",
         "adafruit-circuitpython-shtc3",
```

### Comparing `mmcb-avt-0.0.91/src/mmcb/common.py` & `mmcb-avt-0.0.92/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.92/src/mmcb/configure_environment.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.92/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/dat2root.py` & `mmcb-avt-0.0.92/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/detect.py` & `mmcb-avt-0.0.92/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/dmm.py` & `mmcb-avt-0.0.92/src/mmcb/dmm.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/dmm_interface.py` & `mmcb-avt-0.0.92/src/mmcb/dmm_interface.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/iv.py` & `mmcb-avt-0.0.92/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/lexicon.py` & `mmcb-avt-0.0.92/src/mmcb/lexicon.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/liveplot.py` & `mmcb-avt-0.0.92/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/log2dat.py` & `mmcb-avt-0.0.92/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/peltier.py` & `mmcb-avt-0.0.92/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/psuset.py` & `mmcb-avt-0.0.92/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/psustat.py` & `mmcb-avt-0.0.92/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/sense.py` & `mmcb-avt-0.0.92/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/sensors.py` & `mmcb-avt-0.0.92/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/sensors_mod.py` & `mmcb-avt-0.0.92/src/mmcb/sensors_mod.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/sequence.py` & `mmcb-avt-0.0.92/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb/ult80.py` & `mmcb-avt-0.0.92/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.91/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.92/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.91
+Version: 0.0.92
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.91/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.92/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

