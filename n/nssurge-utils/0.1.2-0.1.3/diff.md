# Comparing `tmp/nssurge_utils-0.1.2.tar.gz` & `tmp/nssurge_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nssurge_utils-0.1.2.tar", max compression
+gzip compressed data, was "nssurge_utils-0.1.3.tar", max compression
```

## Comparing `nssurge_utils-0.1.2.tar` & `nssurge_utils-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-24 03:07:21.792499 nssurge_utils-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-05-24 14:04:00.568417 nssurge_utils-0.1.2/nssurge_utils/__init__.py
--rw-r--r--   0        0        0      624 2023-05-24 13:22:53.300899 nssurge_utils-0.1.2/nssurge_utils/config.py
--rwxr-xr-x   0        0        0     7623 2023-05-24 13:53:38.873303 nssurge_utils-0.1.2/nssurge_utils/extract_proxy.py
--rw-r--r--   0        0        0     1809 2023-05-24 12:59:45.993775 nssurge_utils-0.1.2/nssurge_utils/parsers.py
--rw-r--r--   0        0        0      880 2023-05-24 12:09:19.509286 nssurge_utils-0.1.2/nssurge_utils/predicates.py
--rw-r--r--   0        0        0     1098 2023-05-24 14:00:56.636289 nssurge_utils-0.1.2/nssurge_utils/transform.py
--rw-r--r--   0        0        0      298 2023-05-24 03:20:15.526307 nssurge_utils-0.1.2/nssurge_utils/types.py
--rw-r--r--   0        0        0     7790 2023-05-24 13:39:00.489727 nssurge_utils-0.1.2/nssurge_utils/utils.py
--rw-r--r--   0        0        0      861 2023-05-24 14:04:00.567261 nssurge_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 nssurge_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-24 03:07:21.792499 nssurge_utils-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-05-27 01:07:04.417682 nssurge_utils-0.1.3/nssurge_utils/__init__.py
+-rw-r--r--   0        0        0      624 2023-05-24 13:22:53.300899 nssurge_utils-0.1.3/nssurge_utils/config.py
+-rwxr-xr-x   0        0        0     7623 2023-05-24 13:53:38.873303 nssurge_utils-0.1.3/nssurge_utils/extract_proxy.py
+-rw-r--r--   0        0        0     1809 2023-05-24 12:59:45.993775 nssurge_utils-0.1.3/nssurge_utils/parsers.py
+-rw-r--r--   0        0        0      880 2023-05-24 12:09:19.509286 nssurge_utils-0.1.3/nssurge_utils/predicates.py
+-rw-r--r--   0        0        0     1098 2023-05-24 14:00:56.636289 nssurge_utils-0.1.3/nssurge_utils/transform.py
+-rw-r--r--   0        0        0      298 2023-05-24 03:20:15.526307 nssurge_utils-0.1.3/nssurge_utils/types.py
+-rw-r--r--   0        0        0     7790 2023-05-24 13:39:00.489727 nssurge_utils-0.1.3/nssurge_utils/utils.py
+-rw-r--r--   0        0        0      861 2023-05-27 01:07:04.416298 nssurge_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 nssurge_utils-0.1.3/PKG-INFO
```

### Comparing `nssurge_utils-0.1.2/nssurge_utils/config.py` & `nssurge_utils-0.1.3/nssurge_utils/config.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.2/nssurge_utils/extract_proxy.py` & `nssurge_utils-0.1.3/nssurge_utils/extract_proxy.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.2/nssurge_utils/parsers.py` & `nssurge_utils-0.1.3/nssurge_utils/parsers.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.2/nssurge_utils/predicates.py` & `nssurge_utils-0.1.3/nssurge_utils/predicates.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.2/nssurge_utils/transform.py` & `nssurge_utils-0.1.3/nssurge_utils/transform.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.2/nssurge_utils/utils.py` & `nssurge_utils-0.1.3/nssurge_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.2/pyproject.toml` & `nssurge_utils-0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nssurge-utils"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "nssurge_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/nssurge-utils"
 repository = "https://github.com/tddschn/nssurge-utils"
```

### Comparing `nssurge_utils-0.1.2/PKG-INFO` & `nssurge_utils-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nssurge-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/tddschn/nssurge-utils
 License: MIT
 Keywords: nssurge,surge,utils
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

