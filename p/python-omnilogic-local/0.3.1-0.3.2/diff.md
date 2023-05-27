# Comparing `tmp/python_omnilogic_local-0.3.1.tar.gz` & `tmp/python_omnilogic_local-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.3.1.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.3.2.tar", max compression
```

## Comparing `python_omnilogic_local-0.3.1.tar` & `python_omnilogic_local-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1696 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    20177 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3931 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0        0 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     7655 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9535 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0     7903 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6304 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-27 12:47:41.348353 python_omnilogic_local-0.3.1/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-27 12:47:42.248355 python_omnilogic_local-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    20177 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3931 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0        0 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     7748 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9535 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0     7903 2023-05-27 13:43:41.352761 python_omnilogic_local-0.3.2/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6304 2023-05-27 13:43:41.352761 python_omnilogic_local-0.3.2/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-27 13:43:41.352761 python_omnilogic_local-0.3.2/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-27 13:43:42.268768 python_omnilogic_local-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.3.2/PKG-INFO
```

### Comparing `python_omnilogic_local-0.3.1/README.md` & `python_omnilogic_local-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.1/pyomnilogic_local/api.py` & `python_omnilogic_local-0.3.2/pyomnilogic_local/api.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.1/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.3.2/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.1/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.3.2/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.1/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.3.2/pyomnilogic_local/models/mspconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,18 +47,20 @@
             return
         for subdevice_name in self._sub_devices:
             subdevice = getattr(self, subdevice_name)
             # If our subdevice is a list of subdevices ...
             if isinstance(subdevice, list):
                 for device in subdevice:
                     # ... then call propagate_bow_id on each of them ...
-                    device.propagate_bow_id(bow_id)
+                    if device is not None:
+                        device.propagate_bow_id(bow_id)
             else:
                 # ... otherwise just call it on the single subdevice
-                subdevice.propagate_bow_id(bow_id)
+                if subdevice is not None:
+                    subdevice.propagate_bow_id(bow_id)
 
 
 class MSPSystem(BaseModel):
     omni_type: OmniType = OmniType.SYSTEM
     vsp_speed_format: Literal["RPM", "Percent"] = Field(alias="Msp-Vsp-Speed-Format")
     units: Literal["Standard", "Metric"] = Field(alias="Units")
```

### Comparing `python_omnilogic_local-0.3.1/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.3.2/pyomnilogic_local/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.1/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.3.2/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.1/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.3.2/pyomnilogic_local/protocol.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.1/pyomnilogic_local/types.py` & `python_omnilogic_local-0.3.2/pyomnilogic_local/types.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.1/pyproject.toml` & `python_omnilogic_local-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.3.1"
+version = "0.3.2"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.3.1/PKG-INFO` & `python_omnilogic_local-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.3.1 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.3.2 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

