# Comparing `tmp/pymorlocinternals-0.3.0.tar.gz` & `tmp/pymorlocinternals-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymorlocinternals-0.3.0.tar", last modified: Wed Oct 28 21:23:27 2020, max compression
+gzip compressed data, was "pymorlocinternals-0.4.0.tar", last modified: Sat May 27 04:08:20 2023, max compression
```

## Comparing `pymorlocinternals-0.3.0.tar` & `pymorlocinternals-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 z         (1000) z         (1000)        0 2020-10-28 21:23:27.395985 pymorlocinternals-0.3.0/
--rw-r--r--   0 z         (1000) z         (1000)      520 2020-10-28 21:23:27.395985 pymorlocinternals-0.3.0/PKG-INFO
--rw-r--r--   0 z         (1000) z         (1000)       34 2020-10-27 05:23:15.000000 pymorlocinternals-0.3.0/README.md
-drwxr-xr-x   0 z         (1000) z         (1000)        0 2020-10-28 21:23:27.392651 pymorlocinternals-0.3.0/pymorlocinternals/
--rw-r--r--   0 z         (1000) z         (1000)       68 2020-10-27 05:23:15.000000 pymorlocinternals-0.3.0/pymorlocinternals/__init__.py
--rw-r--r--   0 z         (1000) z         (1000)     2290 2020-10-28 21:13:37.000000 pymorlocinternals-0.3.0/pymorlocinternals/main.py
--rw-r--r--   0 z         (1000) z         (1000)     1001 2020-10-28 20:47:32.000000 pymorlocinternals-0.3.0/pymorlocinternals/types.py
--rw-r--r--   0 z         (1000) z         (1000)       22 2020-10-28 21:21:28.000000 pymorlocinternals-0.3.0/pymorlocinternals/version.py
-drwxr-xr-x   0 z         (1000) z         (1000)        0 2020-10-28 21:23:27.395985 pymorlocinternals-0.3.0/pymorlocinternals.egg-info/
--rw-r--r--   0 z         (1000) z         (1000)      520 2020-10-28 21:23:27.000000 pymorlocinternals-0.3.0/pymorlocinternals.egg-info/PKG-INFO
--rw-r--r--   0 z         (1000) z         (1000)      334 2020-10-28 21:23:27.000000 pymorlocinternals-0.3.0/pymorlocinternals.egg-info/SOURCES.txt
--rw-r--r--   0 z         (1000) z         (1000)        1 2020-10-28 21:23:27.000000 pymorlocinternals-0.3.0/pymorlocinternals.egg-info/dependency_links.txt
--rw-r--r--   0 z         (1000) z         (1000)        1 2020-10-28 21:23:27.000000 pymorlocinternals-0.3.0/pymorlocinternals.egg-info/not-zip-safe
--rw-r--r--   0 z         (1000) z         (1000)       18 2020-10-28 21:23:27.000000 pymorlocinternals-0.3.0/pymorlocinternals.egg-info/top_level.txt
--rw-r--r--   0 z         (1000) z         (1000)       38 2020-10-28 21:23:27.395985 pymorlocinternals-0.3.0/setup.cfg
--rw-r--r--   0 z         (1000) z         (1000)      770 2020-10-27 05:23:15.000000 pymorlocinternals-0.3.0/setup.py
+drwxr-xr-x   0 z         (1000) z         (1000)        0 2023-05-27 04:08:20.233332 pymorlocinternals-0.4.0/
+-rw-r--r--   0 z         (1000) z         (1000)      464 2023-05-27 04:08:20.233332 pymorlocinternals-0.4.0/PKG-INFO
+-rw-r--r--   0 z         (1000) z         (1000)       34 2022-02-16 21:54:00.000000 pymorlocinternals-0.4.0/README.md
+drwxr-xr-x   0 z         (1000) z         (1000)        0 2023-05-27 04:08:20.229999 pymorlocinternals-0.4.0/pymorlocinternals/
+-rw-r--r--   0 z         (1000) z         (1000)       68 2022-02-16 21:54:00.000000 pymorlocinternals-0.4.0/pymorlocinternals/__init__.py
+-rw-r--r--   0 z         (1000) z         (1000)     2471 2023-05-27 03:51:47.000000 pymorlocinternals-0.4.0/pymorlocinternals/main.py
+-rw-r--r--   0 z         (1000) z         (1000)     1003 2023-03-25 18:12:09.000000 pymorlocinternals-0.4.0/pymorlocinternals/types.py
+-rw-r--r--   0 z         (1000) z         (1000)       22 2023-05-27 04:05:31.000000 pymorlocinternals-0.4.0/pymorlocinternals/version.py
+drwxr-xr-x   0 z         (1000) z         (1000)        0 2023-05-27 04:08:20.233332 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/
+-rw-r--r--   0 z         (1000) z         (1000)      464 2023-05-27 04:08:20.000000 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/PKG-INFO
+-rw-r--r--   0 z         (1000) z         (1000)      334 2023-05-27 04:08:20.000000 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/SOURCES.txt
+-rw-r--r--   0 z         (1000) z         (1000)        1 2023-05-27 04:08:20.000000 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/dependency_links.txt
+-rw-r--r--   0 z         (1000) z         (1000)        1 2023-05-27 04:08:00.000000 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/not-zip-safe
+-rw-r--r--   0 z         (1000) z         (1000)       18 2023-05-27 04:08:20.000000 pymorlocinternals-0.4.0/pymorlocinternals.egg-info/top_level.txt
+-rw-r--r--   0 z         (1000) z         (1000)       38 2023-05-27 04:08:20.233332 pymorlocinternals-0.4.0/setup.cfg
+-rw-r--r--   0 z         (1000) z         (1000)      770 2023-05-27 03:58:51.000000 pymorlocinternals-0.4.0/setup.py
```

### Comparing `pymorlocinternals-0.3.0/pymorlocinternals/main.py` & `pymorlocinternals-0.4.0/pymorlocinternals/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,25 +37,28 @@
 def serialize_str(x, schema):
     return json.dumps(x)
 
 
 def serialize_bool(x, schema):
     return json.dumps(x)
 
+def serialize_none(x, schema):
+    return json.dumps(None)
 
-dispatch = dict(
-    list=serialize_list,
-    tuple=serialize_tuple,
-    record=serialize_record,
-    dict=serialize_record,
-    float=serialize_float,
-    int=serialize_int,
-    str=serialize_str,
-    bool=serialize_bool,
-)
+dispatch = { 
+    "list" : serialize_list,
+    "tuple" : serialize_tuple,
+    "record" : serialize_record,
+    "dict" : serialize_record,
+    "float" : serialize_float,
+    "int" : serialize_int,
+    "str" : serialize_str,
+    "bool" : serialize_bool,
+    "None" : serialize_none,
+  }
 
 
 def mlc_serialize(x, schema):
     if type(schema[0]) == str:
         return dispatch[schema[0]](x, schema[1])
     else:
         # Is the label is not a string, then it is a constructor,
@@ -76,24 +79,25 @@
     d = dict()
     for (k, v) in schema.items():
         deserializer = dispatch_deserialize[v[0]]
         d[k] = deserializer(d0[k], v[1])
     return d
 
 
-dispatch_deserialize = dict(
-    list=deserialize_list,
-    tuple=deserialize_tuple,
-    record=deserialize_record,
-    dict=deserialize_record,
-    float=lambda x, s: x,
-    int=lambda x, s: x,
-    str=lambda x, s: x,
-    bool=lambda x, s: x,
-)
+dispatch_deserialize = {
+    "list"   : deserialize_list,
+    "tuple"  : deserialize_tuple,
+    "record" : deserialize_record,
+    "dict"   : deserialize_record,
+    "float"  : lambda x, _: x,
+    "int"    : lambda x, _: x,
+    "str"    : lambda x, _: x,
+    "bool"   : lambda x, _: x,
+    "None"   : None
+}
 
 
 def mlc_deserialize(json_str, schema):
     x = json.loads(json_str)
     if type(schema[0]) == str:
         return dispatch_deserialize[schema[0]](x, schema[1])
     else:
```

### Comparing `pymorlocinternals-0.3.0/pymorlocinternals/types.py` & `pymorlocinternals-0.4.0/pymorlocinternals/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def mlc_record(**kwargs):
     """
   Helper function for building record types
 
   @param **kwargs The keyword arguments for the record
   """
-    return ("record", dict(**args))
+    return ("record", dict(**kwargs))
 
 
 def mlc_object(f, **kwargs):
     """
   Helper function for building object types
 
   @param **kwargs The keyword arguments for the record
```

### Comparing `pymorlocinternals-0.3.0/setup.py` & `pymorlocinternals-0.4.0/setup.py`

 * *Files identical despite different names*

