# Comparing `tmp/jao-py-0.3.6.tar.gz` & `tmp/jao-py-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jao-py-0.3.6.tar", last modified: Sun May 21 21:58:45 2023, max compression
+gzip compressed data, was "jao-py-0.3.7.tar", last modified: Sat May 27 20:19:50 2023, max compression
```

## Comparing `jao-py-0.3.6.tar` & `jao-py-0.3.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:45.848231 jao-py-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-21 21:58:34.000000 jao-py-0.3.6/LICENSE.MD
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-21 21:58:45.848231 jao-py-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-21 21:58:34.000000 jao-py-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:45.844231 jao-py-0.3.6/jao/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:45.844231 jao-py-0.3.6/jao/CWE/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/CWE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/CWE/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/CWE/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/CWE/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/CWE/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:45.844231 jao-py-0.3.6/jao/beta/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/beta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/beta/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/webservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:45.848231 jao-py-0.3.6/jao_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-21 21:58:45.000000 jao-py-0.3.6/jao_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-21 21:58:45.000000 jao-py-0.3.6/jao_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:58:45.000000 jao-py-0.3.6/jao_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 21:58:45.000000 jao-py-0.3.6/jao_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-21 21:58:45.000000 jao-py-0.3.6/jao_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-21 21:58:45.848231 jao-py-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-21 21:58:34.000000 jao-py-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:50.689649 jao-py-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-27 20:19:41.000000 jao-py-0.3.7/LICENSE.MD
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-27 20:19:50.689649 jao-py-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-27 20:19:41.000000 jao-py-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:50.689649 jao-py-0.3.7/jao/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:50.689649 jao-py-0.3.7/jao/CWE/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/CWE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/CWE/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/CWE/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/CWE/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/CWE/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:50.689649 jao-py-0.3.7/jao/beta/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/beta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/beta/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-27 20:19:41.000000 jao-py-0.3.7/jao/webservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:19:50.689649 jao-py-0.3.7/jao_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-27 20:19:50.000000 jao-py-0.3.7/jao_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-27 20:19:50.000000 jao-py-0.3.7/jao_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 20:19:50.000000 jao-py-0.3.7/jao_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-27 20:19:50.000000 jao-py-0.3.7/jao_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-27 20:19:50.000000 jao-py-0.3.7/jao_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-27 20:19:50.693649 jao-py-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-27 20:19:41.000000 jao-py-0.3.7/setup.py
```

### Comparing `jao-py-0.3.6/LICENSE.MD` & `jao-py-0.3.7/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.6/PKG-INFO` & `jao-py-0.3.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.3.6
+Version: 0.3.7
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jao-py-0.3.6/README.md` & `jao-py-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.6/jao/CWE/jao.py` & `jao-py-0.3.7/jao/CWE/jao.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.6/jao/CWE/parsers.py` & `jao-py-0.3.7/jao/CWE/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.6/jao/beta/jao.py` & `jao-py-0.3.7/jao/beta/jao.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.6/jao/jao.py` & `jao-py-0.3.7/jao/jao.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import itertools
 from .exceptions import NoMatchingDataError
 from .parsers import parse_final_domain, parse_base_output
 from typing import List, Dict
 from .util import to_snake_case
 
 __title__ = "jao-py"
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 __author__ = "Frank Boerman"
 __license__ = "MIT"
 
 
 class JaoPublicationToolClient:
     BASEURL = "https://publicationtool.jao.eu/core/api/core/"
     BASEURL2 = "https://publicationtool.jao.eu/core/api/data/"
@@ -131,14 +131,17 @@
 
     def query_minmax_np(self, day: pd.Timestamp) -> List[Dict]:
         return self._query_base(day, 'maxNetPos')
 
     def query_allocationconstraint(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> List[Dict]:
         return self._query_base_fromto(d_from, d_to, 'allocationConstraint')
 
+    def query_status(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> List[Dict]:
+        return self._query_base_fromto(d_from, d_to, 'spanningDefaultFBP')
+
 
 class JaoPublicationToolPandasClient(JaoPublicationToolClient):
     def query_final_domain(self, mtu: pd.Timestamp, presolved: bool = None, cne: str = None,
                            co: str = None) -> pd.DataFrame:
         return parse_final_domain(
             super().query_final_domain(mtu=mtu, presolved=presolved, cne=cne, co=co)
         )
@@ -181,8 +184,13 @@
 
     def query_validations(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> pd.DataFrame:
         df = parse_base_output(
             super().query_validations(d_from=d_from, d_to=d_to)
         ).rename(columns=to_snake_case)
         df['last_modified_on'] = pd.to_datetime(df['last_modified_on'], utc=True).dt.tz_convert('europe/amsterdam')
 
-        return df
+        return df
+
+    def query_status(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> pd.DataFrame:
+        return parse_base_output(
+            super().query_status(d_from=d_from, d_to=d_to)
+        ).drop(columns=['lastModifiedOn'])
```

### Comparing `jao-py-0.3.6/jao/parsers.py` & `jao-py-0.3.7/jao/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.6/jao/webservice.py` & `jao-py-0.3.7/jao/webservice.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.6/jao_py.egg-info/PKG-INFO` & `jao-py-0.3.7/jao_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.3.6
+Version: 0.3.7
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jao-py-0.3.6/setup.py` & `jao-py-0.3.7/setup.py`

 * *Files identical despite different names*

