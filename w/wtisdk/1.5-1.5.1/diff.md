# Comparing `tmp/wtisdk-1.5.tar.gz` & `tmp/wtisdk-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtisdk-1.5.tar", last modified: Fri May 26 23:41:59 2023, max compression
+gzip compressed data, was "wtisdk-1.5.1.tar", last modified: Fri May 26 23:51:13 2023, max compression
```

## Comparing `wtisdk-1.5.tar` & `wtisdk-1.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:41:59.126898 wtisdk-1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 23:41:46.000000 wtisdk-1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-05-26 23:41:59.126898 wtisdk-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-26 23:41:46.000000 wtisdk-1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 23:41:59.126898 wtisdk-1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-26 23:41:46.000000 wtisdk-1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:41:59.122898 wtisdk-1.5/wtisdk/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 23:41:46.000000 wtisdk-1.5/wtisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:41:59.126898 wtisdk-1.5/wtisdk/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 23:41:46.000000 wtisdk-1.5/wtisdk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 23:41:46.000000 wtisdk-1.5/wtisdk/tests/test_wtisdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    37138 2023-05-26 23:41:46.000000 wtisdk-1.5/wtisdk/wtisdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:41:59.126898 wtisdk-1.5/wtisdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-05-26 23:41:59.000000 wtisdk-1.5/wtisdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 23:41:59.000000 wtisdk-1.5/wtisdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 23:41:59.000000 wtisdk-1.5/wtisdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 23:41:59.000000 wtisdk-1.5/wtisdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 23:41:59.000000 wtisdk-1.5/wtisdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:13.878293 wtisdk-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 23:51:05.000000 wtisdk-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-05-26 23:51:13.878293 wtisdk-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18584 2023-05-26 23:51:05.000000 wtisdk-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 23:51:13.878293 wtisdk-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-26 23:51:05.000000 wtisdk-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:13.878293 wtisdk-1.5.1/wtisdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 23:51:05.000000 wtisdk-1.5.1/wtisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:13.878293 wtisdk-1.5.1/wtisdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:05.000000 wtisdk-1.5.1/wtisdk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 23:51:05.000000 wtisdk-1.5.1/wtisdk/tests/test_wtisdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37138 2023-05-26 23:51:05.000000 wtisdk-1.5.1/wtisdk/wtisdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:51:13.878293 wtisdk-1.5.1/wtisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-05-26 23:51:13.000000 wtisdk-1.5.1/wtisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 23:51:13.000000 wtisdk-1.5.1/wtisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 23:51:13.000000 wtisdk-1.5.1/wtisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 23:51:13.000000 wtisdk-1.5.1/wtisdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 23:51:13.000000 wtisdk-1.5.1/wtisdk.egg-info/top_level.txt
```

### Comparing `wtisdk-1.5/LICENSE` & `wtisdk-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5/PKG-INFO` & `wtisdk-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.5
+Version: 1.5.1
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI Version](https://img.shields.io/pypi/v/wtisdk.svg)](https://pypi.org/project/wtisdk/)
-[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](URL_TO_YOUR_BUILD_STATUS)
-![PyPI Downloads](https://img.shields.io/pypi/dm/wtisdk)
+[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://github.com/melihteke/wtisdk/actions/workflows/python-publish.yml)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 ![image](https://github.com/melihteke/wtisdk/assets/36086368/24e4279e-54b6-4f3c-8d57-81ce9a005c89)
 
 # WTI SDK - API Wrapper for Western Telematic Inc. (WTI)
 WTI SDK is a Python library that serves as an API wrapper for Western Telematic Inc. (WTI) devices. It provides a convenient way to interact with WTI devices and perform various actions.
```

### Comparing `wtisdk-1.5/README.md` & `wtisdk-1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [![PyPI Version](https://img.shields.io/pypi/v/wtisdk.svg)](https://pypi.org/project/wtisdk/)
-[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](URL_TO_YOUR_BUILD_STATUS)
-![PyPI Downloads](https://img.shields.io/pypi/dm/wtisdk)
+[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://github.com/melihteke/wtisdk/actions/workflows/python-publish.yml)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 ![image](https://github.com/melihteke/wtisdk/assets/36086368/24e4279e-54b6-4f3c-8d57-81ce9a005c89)
 
 # WTI SDK - API Wrapper for Western Telematic Inc. (WTI)
 WTI SDK is a Python library that serves as an API wrapper for Western Telematic Inc. (WTI) devices. It provides a convenient way to interact with WTI devices and perform various actions.
```

### Comparing `wtisdk-1.5/setup.py` & `wtisdk-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='wtisdk',
-    version='1.5',
+    version='1.5.1',
     author='Melih Teke',
     author_email='me@mteke.com',
     description='WTI SDK for interacting with WTI devices',
     long_description=f"{long_description}\n\nFor more information, visit the [PyPI page](https://pypi.org/project/wtisdk/).\n\nYou can also connect with me on [LinkedIn](https://www.linkedin.com/in/melih-teke/).",
     long_description_content_type='text/markdown',
     url='https://github.com/melihteke/wtisdk',
     packages=find_packages(),
```

### Comparing `wtisdk-1.5/wtisdk/tests/test_wtisdk.py` & `wtisdk-1.5.1/wtisdk/tests/test_wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5/wtisdk/wtisdk.py` & `wtisdk-1.5.1/wtisdk/wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5/wtisdk.egg-info/PKG-INFO` & `wtisdk-1.5.1/wtisdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.5
+Version: 1.5.1
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI Version](https://img.shields.io/pypi/v/wtisdk.svg)](https://pypi.org/project/wtisdk/)
-[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](URL_TO_YOUR_BUILD_STATUS)
-![PyPI Downloads](https://img.shields.io/pypi/dm/wtisdk)
+[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://github.com/melihteke/wtisdk/actions/workflows/python-publish.yml)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 ![image](https://github.com/melihteke/wtisdk/assets/36086368/24e4279e-54b6-4f3c-8d57-81ce9a005c89)
 
 # WTI SDK - API Wrapper for Western Telematic Inc. (WTI)
 WTI SDK is a Python library that serves as an API wrapper for Western Telematic Inc. (WTI) devices. It provides a convenient way to interact with WTI devices and perform various actions.
```

