# Comparing `tmp/wtisdk-1.4.tar.gz` & `tmp/wtisdk-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtisdk-1.4.tar", last modified: Fri May 26 22:50:11 2023, max compression
+gzip compressed data, was "wtisdk-1.5.tar", last modified: Fri May 26 23:41:59 2023, max compression
```

## Comparing `wtisdk-1.4.tar` & `wtisdk-1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:50:10.997582 wtisdk-1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 22:50:00.000000 wtisdk-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-26 22:50:10.997582 wtisdk-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-05-26 22:50:00.000000 wtisdk-1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 22:50:10.997582 wtisdk-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-26 22:50:00.000000 wtisdk-1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:50:10.993581 wtisdk-1.4/wtisdk/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 22:50:00.000000 wtisdk-1.4/wtisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:50:10.993581 wtisdk-1.4/wtisdk/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 22:50:00.000000 wtisdk-1.4/wtisdk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 22:50:00.000000 wtisdk-1.4/wtisdk/tests/test_wtisdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    37138 2023-05-26 22:50:00.000000 wtisdk-1.4/wtisdk/wtisdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 22:50:10.993581 wtisdk-1.4/wtisdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-26 22:50:10.000000 wtisdk-1.4/wtisdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 22:50:10.000000 wtisdk-1.4/wtisdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 22:50:10.000000 wtisdk-1.4/wtisdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 22:50:10.000000 wtisdk-1.4/wtisdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 22:50:10.000000 wtisdk-1.4/wtisdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:41:59.126898 wtisdk-1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 23:41:46.000000 wtisdk-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-05-26 23:41:59.126898 wtisdk-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-26 23:41:46.000000 wtisdk-1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 23:41:59.126898 wtisdk-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-26 23:41:46.000000 wtisdk-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:41:59.122898 wtisdk-1.5/wtisdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 23:41:46.000000 wtisdk-1.5/wtisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:41:59.126898 wtisdk-1.5/wtisdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 23:41:46.000000 wtisdk-1.5/wtisdk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 23:41:46.000000 wtisdk-1.5/wtisdk/tests/test_wtisdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37138 2023-05-26 23:41:46.000000 wtisdk-1.5/wtisdk/wtisdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:41:59.126898 wtisdk-1.5/wtisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-05-26 23:41:59.000000 wtisdk-1.5/wtisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 23:41:59.000000 wtisdk-1.5/wtisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 23:41:59.000000 wtisdk-1.5/wtisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 23:41:59.000000 wtisdk-1.5/wtisdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 23:41:59.000000 wtisdk-1.5/wtisdk.egg-info/top_level.txt
```

### Comparing `wtisdk-1.4/LICENSE` & `wtisdk-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wtisdk-1.4/README.md` & `wtisdk-1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,25 @@
-[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)]([URL_TO_YOUR_BUILD_STATUS](https://pypi.org/project/wtisdk/))
+[![PyPI Version](https://img.shields.io/pypi/v/wtisdk.svg)](https://pypi.org/project/wtisdk/)
+[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](URL_TO_YOUR_BUILD_STATUS)
+![PyPI Downloads](https://img.shields.io/pypi/dm/wtisdk)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 ![image](https://github.com/melihteke/wtisdk/assets/36086368/24e4279e-54b6-4f3c-8d57-81ce9a005c89)
 
 # WTI SDK - API Wrapper for Western Telematic Inc. (WTI)
 WTI SDK is a Python library that serves as an API wrapper for Western Telematic Inc. (WTI) devices. It provides a convenient way to interact with WTI devices and perform various actions.
 
-Please note that this is not an official tool provided by Western Telematic Inc. It was developed by Melih Teke to simplify the integration with WTI devices.
+Please note that WTI is a vendor specializing in console and power management solutions for network equipment. Their devices offer advanced features for managing and controlling network infrastructure.
+
+This SDK, developed by Melih Teke, aims to simplify the integration with WTI devices and enhance the functionality for managing and controlling network infrastructure.
+
+Please refer to the WTI Website for more information about Western Telematic Inc. and their range of devices.
+
+Please note that this SDK is not an official tool provided by Western Telematic Inc., but an independent contribution to facilitate working with their devices.
 
 ## Features
 - Connect to WTI devices and retrieve operational data.
 - Change configuration.
 - Manage the device.
 
 ### Installation
@@ -112,15 +121,15 @@
 response = client.edit_power_plug_plugconfig(config)
 ```
 
 ### Get Specific User
 Retrieves information about a specific user from the WTI device.
 ```sh 
 client = WtiClient(host, username, password)
-user_info = client.get_specific_user("john_doe")
+user_info = client.get_specific_user("Melih Teke")
 print(user_info)
 ```
 ### Add new user
 Add a new user using the provided configuration.
 ```sh 
 client = WtiClient(host, username, password)
 new_user_config = {
@@ -218,15 +227,15 @@
     "interface": {
         "name": "eth0",
         "ietf-ipv4": {
             "address": [
                 {
                     "ip": "10.60.11.101",
                     "netmask": "255.255.255.240",
-                    "gateway": "10.60.11.97"
+                    "gateway": "10.20.11.97"
                 }
             ]
         }
     }
 }
 updated_config = client.edit_network_interface_config(new_interface_config)
 print(updated_config)
@@ -482,26 +491,26 @@
     ]
 }
 updated_snmp_access_config = client.edit_config_snmp_access(new_snmp_access_config)
 print(updated_snmp_access_config)
 
 ```
 
-# Retrieve IP Tables
+### Retrieve IP Tables
 Retrieves the IP tables configuration from the device.
 
 ```sh 
 client = WtiClient(host, username, password)
 ip_tables_config = client.get_config_ip_tables()
 print(ip_tables_config)
 
 ```
 
 
-# Edit IP Tables
+### Edit IP Tables
 Edits the IP tables configuration on the device.
 ```sh 
 config = {
     "iptables": {
         "eth0": {
             "ietf-ipv4": {
                 "clear": 1,
```

### Comparing `wtisdk-1.4/wtisdk/tests/test_wtisdk.py` & `wtisdk-1.5/wtisdk/tests/test_wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.4/wtisdk/wtisdk.py` & `wtisdk-1.5/wtisdk/wtisdk.py`

 * *Files identical despite different names*

