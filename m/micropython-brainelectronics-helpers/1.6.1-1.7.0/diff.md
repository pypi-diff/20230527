# Comparing `tmp/micropython-brainelectronics-helpers-1.6.1.tar.gz` & `tmp/micropython-brainelectronics-helpers-1.7.0.tar.gz`

## Comparing `micropython-brainelectronics-helpers-1.6.1.tar` & `micropython-brainelectronics-helpers-1.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-29 13:01:54.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-01-29 13:01:54.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/generic_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19680 2023-01-29 13:01:54.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/led_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-01-29 13:01:54.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    41522 2023-01-29 13:01:54.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/modbus_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-01-29 13:01:54.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/path_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-01-29 13:01:54.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-01-29 13:01:54.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/time_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-01-29 13:01:54.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-01-29 13:01:54.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/update_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-29 13:02:01.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-01-29 13:01:54.000000 micropython-brainelectronics-helpers-1.6.1/be_helpers/wifi_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-01-29 13:02:01.000000 micropython-brainelectronics-helpers-1.6.1/micropython_brainelectronics_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-29 13:02:01.000000 micropython-brainelectronics-helpers-1.6.1/micropython_brainelectronics_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/generic_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19680 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/led_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41522 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/modbus_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/path_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/time_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/ulogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/update_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-27 10:51:58.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-05-27 10:51:50.000000 micropython-brainelectronics-helpers-1.7.0/be_helpers/wifi_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-05-27 10:51:59.000000 micropython-brainelectronics-helpers-1.7.0/micropython_brainelectronics_helpers.egg-info/PKG-INFO
```

### Comparing `micropython-brainelectronics-helpers-1.6.1/be_helpers/generic_helper.py` & `micropython-brainelectronics-helpers-1.7.0/be_helpers/generic_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 Generic helper
 
 Collection of helper functions for Micropython boards like BE32-01 and others
 """
 
 import gc
 import json
-import ulogging as logging
 import machine
 import os
 import random
 import time
 import ubinascii
 
 # custom packages
 # typing not natively supported on MicroPython
 from .typing import Optional, Union
+from . import ulogging as logging
 
 
 class GenericHelper(object):
     """docstring for GenericHelper"""
     def __init__(self):
         pass
```

### Comparing `micropython-brainelectronics-helpers-1.6.1/be_helpers/led_helper.py` & `micropython-brainelectronics-helpers-1.7.0/be_helpers/led_helper.py`

 * *Files identical despite different names*

### Comparing `micropython-brainelectronics-helpers-1.6.1/be_helpers/message.py` & `micropython-brainelectronics-helpers-1.7.0/be_helpers/message.py`

 * *Files identical despite different names*

### Comparing `micropython-brainelectronics-helpers-1.6.1/be_helpers/modbus_bridge.py` & `micropython-brainelectronics-helpers-1.7.0/be_helpers/modbus_bridge.py`

 * *Files identical despite different names*

### Comparing `micropython-brainelectronics-helpers-1.6.1/be_helpers/path_helper.py` & `micropython-brainelectronics-helpers-1.7.0/be_helpers/path_helper.py`

 * *Files identical despite different names*

### Comparing `micropython-brainelectronics-helpers-1.6.1/be_helpers/queue.py` & `micropython-brainelectronics-helpers-1.7.0/be_helpers/queue.py`

 * *Files identical despite different names*

### Comparing `micropython-brainelectronics-helpers-1.6.1/be_helpers/time_helper.py` & `micropython-brainelectronics-helpers-1.7.0/be_helpers/time_helper.py`

 * *Files identical despite different names*

### Comparing `micropython-brainelectronics-helpers-1.6.1/be_helpers/typing.py` & `micropython-brainelectronics-helpers-1.7.0/be_helpers/typing.py`

 * *Files identical despite different names*

### Comparing `micropython-brainelectronics-helpers-1.6.1/be_helpers/update_helper.py` & `micropython-brainelectronics-helpers-1.7.0/be_helpers/update_helper.py`

 * *Files identical despite different names*

### Comparing `micropython-brainelectronics-helpers-1.6.1/be_helpers/wifi_helper.py` & `micropython-brainelectronics-helpers-1.7.0/be_helpers/wifi_helper.py`

 * *Files identical despite different names*

### Comparing `micropython-brainelectronics-helpers-1.6.1/micropython_brainelectronics_helpers.egg-info/PKG-INFO` & `micropython-brainelectronics-helpers-1.7.0/micropython_brainelectronics_helpers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: micropython-brainelectronics-helpers
-Version: 1.6.1
+Version: 1.7.0
 Summary: MicroPython brainelectronics helpers library
 Home-page: https://github.com/brainelectronics/micropython-modules
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-modules/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-modules
 Keywords: micropython,brainelectronics,modules,library
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MicroPython modules
 
 [![Downloads](https://pepy.tech/badge/micropython-brainelectronics-helpers)](https://pepy.tech/project/micropython-brainelectronics-helpers)
 ![Release](https://img.shields.io/github/v/release/brainelectronics/micropython-modules?include_prereleases&color=success)
@@ -35,15 +36,18 @@
 
 <!-- MarkdownTOC -->
 
 - [Available generators](#available-generators)
 - [Installation](#installation)
     - [Install required tools](#install-required-tools)
 - [Setup](#setup)
-    - [Install package with pip](#install-package-with-pip)
+    - [Install package](#install-package)
+        - [General](#general)
+        - [Specific version](#specific-version)
+        - [Test version](#test-version)
     - [Manually](#manually)
     - [Generic Helper](#generic-helper)
     - [LED Helper](#led-helper)
         - [Onboard LED](#onboard-led)
             - [Basics](#basics)
             - [Advanced](#advanced)
         - [Neopixel](#neopixel)
@@ -81,34 +85,78 @@
 source .venv/bin/activate
 
 pip install -r requirements.txt
 ```
 
 ## Setup
 
-### Install package with pip
+### Install package
 
 Connect your MicroPython board to a network
 
 ```python
 import network
 station = network.WLAN(network.STA_IF)
 station.active(True)
 station.connect('SSID', 'PASSWORD')
 station.isconnected()
 ```
 
-and install this lib on the MicroPython device like this
+#### General
+
+Install the latest package version of this lib on the MicroPython device
+
+```python
+import mip
+mip.install("github:brainelectronics/micropython-modules")
+```
+
+For MicroPython versions below 1.19.1 use the `upip` package instead of `mip`
 
 ```python
 import upip
 upip.install('micropython-brainelectronics-helpers')
-# its dependencies will be installed alongside
 ```
 
+#### Specific version
+
+Install a specific, fixed package version of this lib on the MicroPython device
+
+```python
+import mip
+# install a verions of a specific branch
+mip.install("github:brainelectronics/micropython-modules", version="feature/support-mip")
+# install a tag version
+mip.install("github:brainelectronics/micropython-modules", version="1.7.0")
+```
+
+#### Test version
+
+Install a specific release candidate version uploaded to
+[Test Python Package Index](https://test.pypi.org/) on every PR on the
+MicroPython device. If no specific version is set, the latest stable version
+will be used.
+
+```python
+import mip
+mip.install("github:brainelectronics/micropython-modules", version="1.7.0-rc5.dev22")
+```
+
+For MicroPython versions below 1.19.1 use the `upip` package instead of `mip`
+
+```python
+import upip
+# overwrite index_urls to only take artifacts from test.pypi.org
+upip.index_urls = ['https://test.pypi.org/pypi']
+upip.install('micropython-brainelectronics-helpers')
+```
+
+See also [brainelectronics Test PyPi Server in Docker][ref-brainelectronics-test-pypiserver]
+for a test PyPi server running on Docker.
+
 ### Manually
 
 Copy the module to the MicroPython board and import them as shown below
 using [Remote MicroPython shell][ref-remote-upy-shell]
 
 Open the remote shell with the following command. Additionally use `-b 115200`
 in case no CP210x is used but a CH34x.
@@ -124,19 +172,14 @@
 mkdir /pyboard/lib/be_helpers
 cp be_helpers/* /pyboard/lib/be_helpers
 ```
 
 Install required dependencies (requires network connection, see may use the
 [`WifiHelper`][ref-wifi-helper])
 
-```python
-import upip
-upip.install('micropython-ulogging')
-```
-
 ### Generic Helper
 
 Generic helper class with different usecases and functions.
 
 ```python
 from be_helpers.generic_helper import GenericHelper
 
@@ -198,14 +241,19 @@
 #### Onboard LED
 
 This example demonstrates how to interact with the onboard LED on the BE32-01
 
 ##### Basics
 
 The onboard LED is availabe on Pin 4 on the BE32-01 board in inverted mode.
+For the Raspberry Pi Pico (W) initialise the LED like this:
+```python
+from be_helpers.led_helper import Led
+led = Led(led_pin="LED", inverted=False)
+```
 
 ```python
 from be_helpers.led_helper import Led
 
 # Onboard LED is availabe on Pin 4 on BE32-01 in inverted mode
 led = Led()
 print('Onboard LED is ON: {}'.format(led.on))
@@ -354,15 +402,23 @@
 ```
 
 ### Modbus Bridge
 
 This requires [brainelectronics MicroPython Modbus][ref-be-upy-modbus]. Forked
 and extended from [SFERALABS Exo Sense Py][ref-sferalabs-exo-sense].
 
-Connect the board to a network and install the package like this
+Connect the board to a network and install the package like this for
+MicroPython 1.20.0 or never
+
+```python
+import mip
+mip.install("github:brainelectronics/micropython-modbus")
+```
+
+For MicroPython versions below 1.19.1 use the `upip` package instead of `mip`
 
 ```python
 import upip
 upip.install('micropython-modbus')
 ```
 
 ```python
@@ -483,12 +539,13 @@
 # convert dBm (RRSI) to quality index in percent
 quality = WifiHelper.dbm_to_quality(dBm=wh.networks[0].RSSI)
 print('Quality of strongest network {}: {}%'.format(strongest_net, quality))
 ```
 
 <!-- Links -->
 [ref-remote-upy-shell]: https://github.com/dhylands/rshell
+[ref-brainelectronics-test-pypiserver]: https://github.com/brainelectronics/test-pypiserver
 [ref-wifi-helper]: wifi_helper.py
 [ref-be-upy-modbus]: https://github.com/brainelectronics/micropython-modbus
 [ref-sferalabs-exo-sense]: https://github.com/sfera-labs/exo-sense-py-modbus
```

