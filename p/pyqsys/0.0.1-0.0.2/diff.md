# Comparing `tmp/pyqsys-0.0.1.tar.gz` & `tmp/pyqsys-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqsys-0.0.1.tar", last modified: Sat May 27 18:53:36 2023, max compression
+gzip compressed data, was "/home/runner/work/pyqsys/pyqsys/dist/.tmp-3_m9okwn/pyqsys-0.0.2.tar", last modified: Sat May 27 19:42:13 2023, max compression
```

## Comparing `pyqsys-0.0.1.tar` & `pyqsys-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:53:36.955878 pyqsys-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-27 18:53:24.000000 pyqsys-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-27 18:53:24.000000 pyqsys-0.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-27 18:53:36.955878 pyqsys-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-27 18:53:24.000000 pyqsys-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-27 18:53:24.000000 pyqsys-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 18:53:36.955878 pyqsys-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:53:36.955878 pyqsys-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:53:36.955878 pyqsys-0.0.1/src/pyqsys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:53:24.000000 pyqsys-0.0.1/src/pyqsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-05-27 18:53:24.000000 pyqsys-0.0.1/src/pyqsys/qrc_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     9034 2023-05-27 18:53:24.000000 pyqsys-0.0.1/src/pyqsys/qsc_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:53:36.955878 pyqsys-0.0.1/src/pyqsys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-27 18:53:36.000000 pyqsys-0.0.1/src/pyqsys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 18:53:36.000000 pyqsys-0.0.1/src/pyqsys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 18:53:36.000000 pyqsys-0.0.1/src/pyqsys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 18:53:36.000000 pyqsys-0.0.1/src/pyqsys.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:42:13.000000 pyqsys-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-27 19:41:54.000000 pyqsys-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-27 19:41:54.000000 pyqsys-0.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-27 19:42:13.000000 pyqsys-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-27 19:41:54.000000 pyqsys-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-27 19:41:54.000000 pyqsys-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 19:42:13.000000 pyqsys-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:42:13.000000 pyqsys-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:42:13.000000 pyqsys-0.0.2/src/pyqsys/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 19:41:54.000000 pyqsys-0.0.2/src/pyqsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-05-27 19:41:54.000000 pyqsys-0.0.2/src/pyqsys/qrc_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-05-27 19:41:54.000000 pyqsys-0.0.2/src/pyqsys/qsc_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 19:42:13.000000 pyqsys-0.0.2/src/pyqsys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-27 19:42:13.000000 pyqsys-0.0.2/src/pyqsys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 19:42:13.000000 pyqsys-0.0.2/src/pyqsys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 19:42:13.000000 pyqsys-0.0.2/src/pyqsys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 19:42:13.000000 pyqsys-0.0.2/src/pyqsys.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyqsys-0.0.1/LICENSE` & `pyqsys-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqsys-0.0.1/NOTICE` & `pyqsys-0.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `pyqsys-0.0.1/PKG-INFO` & `pyqsys-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqsys
-Version: 0.0.1
+Version: 0.0.2
 Summary: An attempt to create a Python library to communicate with QSYS Cores via their QRC (JSONRPC 2.0) protocol.
 Author-email: Maximilian Schöberl <maxschoeberl@gmail.com>
 Project-URL: Homepage, https://github.com/mexxs/pyqsys
 Project-URL: Bug Tracker, https://github.com/mexxs/pyqsys/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 - [x] Bare QRC methods
 - [ ] High level interface
 
 ## Usage
 Create a Core object and just call the methods with the correct [arguments](https://q-syshelp.qsc.com/#External_Control_APIs/QRC/QRC_Commands.htm).
 
 ```python
-from qsc_core import Core
+from pyqsys import Core
 
 core = Core("192.168.0.135")
 core.connect()
 
 # If you need to log on to your QSC core use
 core.logon("username", "password")
```

### Comparing `pyqsys-0.0.1/README.md` & `pyqsys-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - [x] Bare QRC methods
 - [ ] High level interface
 
 ## Usage
 Create a Core object and just call the methods with the correct [arguments](https://q-syshelp.qsc.com/#External_Control_APIs/QRC/QRC_Commands.htm).
 
 ```python
-from qsc_core import Core
+from pyqsys import Core
 
 core = Core("192.168.0.135")
 core.connect()
 
 # If you need to log on to your QSC core use
 core.logon("username", "password")
```

### Comparing `pyqsys-0.0.1/pyproject.toml` & `pyqsys-0.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyqsys"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Maximilian Schöberl", email="maxschoeberl@gmail.com" },
 ]
 description = "An attempt to create a Python library to communicate with QSYS Cores via their QRC (JSONRPC 2.0) protocol."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyqsys-0.0.1/src/pyqsys/qrc_methods.py` & `pyqsys-0.0.2/src/pyqsys/qrc_methods.py`

 * *Files identical despite different names*

### Comparing `pyqsys-0.0.1/src/pyqsys/qsc_core.py` & `pyqsys-0.0.2/src/pyqsys/qsc_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import queue
 import socket
 import threading
 import time
 
 import xml.etree.ElementTree as Et
 from jsonrpcclient import request, parse_json, Ok, Error
-from qrc_methods import ControlMethods, ComponentMethods, ChangeGroupMethods, MixerMethods, LoopPlayerMethods, \
+from .qrc_methods import ControlMethods, ComponentMethods, ChangeGroupMethods, MixerMethods, LoopPlayerMethods, \
     SnapshotMethods
 
 
 class Core(object):
     """
     Class representing a QSC Core device
```

### Comparing `pyqsys-0.0.1/src/pyqsys.egg-info/PKG-INFO` & `pyqsys-0.0.2/src/pyqsys.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqsys
-Version: 0.0.1
+Version: 0.0.2
 Summary: An attempt to create a Python library to communicate with QSYS Cores via their QRC (JSONRPC 2.0) protocol.
 Author-email: Maximilian Schöberl <maxschoeberl@gmail.com>
 Project-URL: Homepage, https://github.com/mexxs/pyqsys
 Project-URL: Bug Tracker, https://github.com/mexxs/pyqsys/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 - [x] Bare QRC methods
 - [ ] High level interface
 
 ## Usage
 Create a Core object and just call the methods with the correct [arguments](https://q-syshelp.qsc.com/#External_Control_APIs/QRC/QRC_Commands.htm).
 
 ```python
-from qsc_core import Core
+from pyqsys import Core
 
 core = Core("192.168.0.135")
 core.connect()
 
 # If you need to log on to your QSC core use
 core.logon("username", "password")
```

