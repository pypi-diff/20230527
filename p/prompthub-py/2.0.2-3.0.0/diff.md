# Comparing `tmp/prompthub_py-2.0.2.tar.gz` & `tmp/prompthub_py-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompthub_py-2.0.2.tar", max compression
+gzip compressed data, was "prompthub_py-3.0.0.tar", max compression
```

## Comparing `prompthub_py-2.0.2.tar` & `prompthub_py-3.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11343 2023-05-11 11:45:57.029591 prompthub_py-2.0.2/LICENSE
--rw-r--r--   0        0        0     1639 2023-05-11 11:45:57.029591 prompthub_py-2.0.2/README.md
--rw-r--r--   0        0        0       65 2023-05-11 11:45:57.029591 prompthub_py-2.0.2/prompthub/__init__.py
--rw-r--r--   0        0        0     1669 2023-05-11 11:45:57.029591 prompthub_py-2.0.2/prompthub/prompt.py
--rw-r--r--   0        0        0      439 2023-05-11 11:45:57.029591 prompthub_py-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 prompthub_py-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-05-27 16:38:40.125084 prompthub_py-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1639 2023-05-27 16:38:40.125084 prompthub_py-3.0.0/README.md
+-rw-r--r--   0        0        0       65 2023-05-27 16:38:40.125084 prompthub_py-3.0.0/prompthub/__init__.py
+-rw-r--r--   0        0        0     1670 2023-05-27 16:38:40.125084 prompthub_py-3.0.0/prompthub/prompt.py
+-rw-r--r--   0        0        0      439 2023-05-27 16:38:40.125084 prompthub_py-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 prompthub_py-3.0.0/PKG-INFO
```

### Comparing `prompthub_py-2.0.2/LICENSE` & `prompthub_py-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prompthub_py-2.0.2/README.md` & `prompthub_py-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `prompthub_py-2.0.2/prompthub/prompt.py` & `prompthub_py-3.0.0/prompthub/prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import os
 
 import yaml
 import requests
 
 
-MAIN_ENDPOINT = os.getenv("PROMPTHUB_MAIN_ENDPOINT", "http://api.prompthub.deepset.ai")
+MAIN_ENDPOINT = os.getenv("PROMPTHUB_MAIN_ENDPOINT", "https://api.prompthub.deepset.ai")
 
 
 @dataclass
 class Prompt:
     """
     Prompt stores all the information of a single prompt.
     """
```

### Comparing `prompthub_py-2.0.2/PKG-INFO` & `prompthub_py-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompthub-py
-Version: 2.0.2
+Version: 3.0.0
 Summary: 
 License: Apache-2.0
 Author: deepset.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

