# Comparing `tmp/wtisdk-1.5.1.tar.gz` & `tmp/wtisdk-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtisdk-1.5.1.tar", last modified: Fri May 26 23:51:13 2023, max compression
+gzip compressed data, was "wtisdk-1.5.2.tar", last modified: Sat May 27 00:18:22 2023, max compression
```

## Comparing `wtisdk-1.5.1.tar` & `wtisdk-1.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:13.878293 wtisdk-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 23:51:05.000000 wtisdk-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-05-26 23:51:13.878293 wtisdk-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18584 2023-05-26 23:51:05.000000 wtisdk-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 23:51:13.878293 wtisdk-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-26 23:51:05.000000 wtisdk-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:13.878293 wtisdk-1.5.1/wtisdk/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 23:51:05.000000 wtisdk-1.5.1/wtisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:13.878293 wtisdk-1.5.1/wtisdk/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:05.000000 wtisdk-1.5.1/wtisdk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 23:51:05.000000 wtisdk-1.5.1/wtisdk/tests/test_wtisdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    37138 2023-05-26 23:51:05.000000 wtisdk-1.5.1/wtisdk/wtisdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:13.878293 wtisdk-1.5.1/wtisdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-05-26 23:51:13.000000 wtisdk-1.5.1/wtisdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 23:51:13.000000 wtisdk-1.5.1/wtisdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 23:51:13.000000 wtisdk-1.5.1/wtisdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 23:51:13.000000 wtisdk-1.5.1/wtisdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 23:51:13.000000 wtisdk-1.5.1/wtisdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:18:22.140042 wtisdk-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-27 00:18:04.000000 wtisdk-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-05-27 00:18:22.140042 wtisdk-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18877 2023-05-27 00:18:04.000000 wtisdk-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 00:18:22.140042 wtisdk-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-27 00:18:04.000000 wtisdk-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:18:22.140042 wtisdk-1.5.2/wtisdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-27 00:18:04.000000 wtisdk-1.5.2/wtisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:18:22.140042 wtisdk-1.5.2/wtisdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:18:04.000000 wtisdk-1.5.2/wtisdk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-27 00:18:04.000000 wtisdk-1.5.2/wtisdk/tests/test_wtisdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37138 2023-05-27 00:18:04.000000 wtisdk-1.5.2/wtisdk/wtisdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:18:22.140042 wtisdk-1.5.2/wtisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-05-27 00:18:22.000000 wtisdk-1.5.2/wtisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-27 00:18:22.000000 wtisdk-1.5.2/wtisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:18:22.000000 wtisdk-1.5.2/wtisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 00:18:22.000000 wtisdk-1.5.2/wtisdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 00:18:22.000000 wtisdk-1.5.2/wtisdk.egg-info/top_level.txt
```

### Comparing `wtisdk-1.5.1/LICENSE` & `wtisdk-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5.1/PKG-INFO` & `wtisdk-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.5.1
+Version: 1.5.2
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,14 +34,18 @@
 
 This SDK, developed by Melih Teke, aims to simplify the integration with WTI devices and enhance the functionality for managing and controlling network infrastructure.
 
 Please refer to the WTI Website for more information about Western Telematic Inc. and their range of devices.
 
 Please note that this SDK is not an official tool provided by Western Telematic Inc., but an independent contribution to facilitate working with their devices.
 
+**Disclaimer: All risks associated with the usage of this SDK are the responsibility of the users. It is recommended to thoroughly test the SDK in a non-production environment before deploying it in a production environment.**
+
+For any questions or support, please contact me at me@mteke.com
+
 ## Features
 - Connect to WTI devices and retrieve operational data.
 - Change configuration.
 - Manage the device.
 
 ### Installation
 ```sh
```

### Comparing `wtisdk-1.5.1/README.md` & `wtisdk-1.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 
 This SDK, developed by Melih Teke, aims to simplify the integration with WTI devices and enhance the functionality for managing and controlling network infrastructure.
 
 Please refer to the WTI Website for more information about Western Telematic Inc. and their range of devices.
 
 Please note that this SDK is not an official tool provided by Western Telematic Inc., but an independent contribution to facilitate working with their devices.
 
+**Disclaimer: All risks associated with the usage of this SDK are the responsibility of the users. It is recommended to thoroughly test the SDK in a non-production environment before deploying it in a production environment.**
+
+For any questions or support, please contact me at me@mteke.com
+
 ## Features
 - Connect to WTI devices and retrieve operational data.
 - Change configuration.
 - Manage the device.
 
 ### Installation
 ```sh
```

### Comparing `wtisdk-1.5.1/setup.py` & `wtisdk-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='wtisdk',
-    version='1.5.1',
+    version='1.5.2',
     author='Melih Teke',
     author_email='me@mteke.com',
     description='WTI SDK for interacting with WTI devices',
     long_description=f"{long_description}\n\nFor more information, visit the [PyPI page](https://pypi.org/project/wtisdk/).\n\nYou can also connect with me on [LinkedIn](https://www.linkedin.com/in/melih-teke/).",
     long_description_content_type='text/markdown',
     url='https://github.com/melihteke/wtisdk',
     packages=find_packages(),
```

### Comparing `wtisdk-1.5.1/wtisdk/tests/test_wtisdk.py` & `wtisdk-1.5.2/wtisdk/tests/test_wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5.1/wtisdk/wtisdk.py` & `wtisdk-1.5.2/wtisdk/wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5.1/wtisdk.egg-info/PKG-INFO` & `wtisdk-1.5.2/wtisdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.5.1
+Version: 1.5.2
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,14 +34,18 @@
 
 This SDK, developed by Melih Teke, aims to simplify the integration with WTI devices and enhance the functionality for managing and controlling network infrastructure.
 
 Please refer to the WTI Website for more information about Western Telematic Inc. and their range of devices.
 
 Please note that this SDK is not an official tool provided by Western Telematic Inc., but an independent contribution to facilitate working with their devices.
 
+**Disclaimer: All risks associated with the usage of this SDK are the responsibility of the users. It is recommended to thoroughly test the SDK in a non-production environment before deploying it in a production environment.**
+
+For any questions or support, please contact me at me@mteke.com
+
 ## Features
 - Connect to WTI devices and retrieve operational data.
 - Change configuration.
 - Manage the device.
 
 ### Installation
 ```sh
```

