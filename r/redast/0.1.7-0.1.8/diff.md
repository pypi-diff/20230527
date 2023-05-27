# Comparing `tmp/redast-0.1.7.tar.gz` & `tmp/redast-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redast-0.1.7.tar", last modified: Sun Apr 23 21:35:52 2023, max compression
+gzip compressed data, was "redast-0.1.8.tar", last modified: Sat May 27 20:15:32 2023, max compression
```

## Comparing `redast-0.1.7.tar` & `redast-0.1.8.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.761614 redast-0.1.7/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1088 2022-04-08 07:02:34.000000 redast-0.1.7/LICENSE
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      148 2022-04-09 19:12:22.000000 redast-0.1.7/MANIFEST.in
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      824 2023-04-23 21:35:52.761614 redast-0.1.7/PKG-INFO
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      292 2023-04-23 21:33:19.000000 redast-0.1.7/README.md
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.757614 redast-0.1.7/redast/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      349 2023-04-23 21:33:19.000000 redast-0.1.7/redast/__init__.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       63 2023-04-23 21:35:50.000000 redast-0.1.7/redast/__init__.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      122 2023-04-23 21:35:05.000000 redast-0.1.7/redast/__version__.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:50.000000 redast-0.1.7/redast/__version__.pyi
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.757614 redast-0.1.7/redast/core/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      148 2022-06-18 03:47:52.000000 redast-0.1.7/redast/core/__init__.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       48 2023-04-23 21:35:50.000000 redast-0.1.7/redast/core/__init__.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1488 2022-06-18 03:44:49.000000 redast-0.1.7/redast/core/hash.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      248 2023-04-23 21:35:50.000000 redast-0.1.7/redast/core/hash.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     4787 2022-08-17 19:23:58.000000 redast-0.1.7/redast/core/packaging.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1283 2023-04-23 21:35:50.000000 redast-0.1.7/redast/core/packaging.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     6390 2022-08-17 19:23:58.000000 redast-0.1.7/redast/core/storage.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2070 2023-04-23 21:35:50.000000 redast-0.1.7/redast/core/storage.pyi
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.757614 redast-0.1.7/redast/local/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      186 2022-06-18 03:46:20.000000 redast-0.1.7/redast/local/__init__.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       86 2023-04-23 21:35:50.000000 redast-0.1.7/redast/local/__init__.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      621 2022-06-18 03:45:10.000000 redast-0.1.7/redast/local/cache.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      281 2023-04-23 21:35:50.000000 redast-0.1.7/redast/local/cache.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2875 2022-08-17 19:23:58.000000 redast-0.1.7/redast/local/drive.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      446 2023-04-23 21:35:50.000000 redast-0.1.7/redast/local/drive.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      593 2022-06-18 03:45:27.000000 redast-0.1.7/redast/local/memory.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      231 2023-04-23 21:35:50.000000 redast-0.1.7/redast/local/memory.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1811 2022-06-18 03:45:37.000000 redast-0.1.7/redast/local/sqlite.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      379 2023-04-23 21:35:50.000000 redast-0.1.7/redast/local/sqlite.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      225 2022-06-18 03:48:02.000000 redast-0.1.7/redast/py.typed
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.757614 redast-0.1.7/redast/remote/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      125 2022-06-18 03:47:46.000000 redast-0.1.7/redast/remote/__init__.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       25 2023-04-23 21:35:50.000000 redast-0.1.7/redast/remote/__init__.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1814 2022-06-18 03:46:03.000000 redast-0.1.7/redast/remote/megacloud.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      273 2023-04-23 21:35:50.000000 redast-0.1.7/redast/remote/megacloud.pyi
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.761614 redast-0.1.7/redast/tool/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      118 2022-06-18 03:47:14.000000 redast-0.1.7/redast/tool/__init__.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       18 2023-04-23 21:35:50.000000 redast-0.1.7/redast/tool/__init__.pyi
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      565 2022-06-18 03:46:28.000000 redast-0.1.7/redast/tool/io.py
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      113 2023-04-23 21:35:50.000000 redast-0.1.7/redast/tool/io.pyi
-drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-04-23 21:35:52.757614 redast-0.1.7/redast.egg-info/
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      824 2023-04-23 21:35:52.000000 redast-0.1.7/redast.egg-info/PKG-INFO
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      921 2023-04-23 21:35:52.000000 redast-0.1.7/redast.egg-info/SOURCES.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        1 2023-04-23 21:35:52.000000 redast-0.1.7/redast.egg-info/dependency_links.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       65 2023-04-23 21:35:52.000000 redast-0.1.7/redast.egg-info/requires.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        7 2023-04-23 21:35:52.000000 redast-0.1.7/redast.egg-info/top_level.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       65 2023-04-23 21:33:42.000000 redast-0.1.7/requirements.txt
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       38 2023-04-23 21:35:52.761614 redast-0.1.7/setup.cfg
--rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1294 2023-04-23 21:33:19.000000 redast-0.1.7/setup.py
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-27 20:15:32.994436 redast-0.1.8/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1088 2022-04-08 07:02:34.000000 redast-0.1.8/LICENSE
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      148 2022-04-09 19:12:22.000000 redast-0.1.8/MANIFEST.in
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      824 2023-05-27 20:15:32.994436 redast-0.1.8/PKG-INFO
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      292 2023-04-23 21:33:19.000000 redast-0.1.8/README.md
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-27 20:15:32.986433 redast-0.1.8/redast/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      349 2023-04-23 21:33:19.000000 redast-0.1.8/redast/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       63 2023-05-27 20:15:30.000000 redast-0.1.8/redast/__init__.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      122 2023-05-27 20:12:52.000000 redast-0.1.8/redast/__version__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-27 20:15:30.000000 redast-0.1.8/redast/__version__.pyi
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-27 20:15:32.990434 redast-0.1.8/redast/core/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      148 2022-06-18 03:47:52.000000 redast-0.1.8/redast/core/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       48 2023-05-27 20:15:30.000000 redast-0.1.8/redast/core/__init__.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1488 2022-06-18 03:44:49.000000 redast-0.1.8/redast/core/hash.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      248 2023-05-27 20:15:30.000000 redast-0.1.8/redast/core/hash.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     4787 2022-08-17 19:23:58.000000 redast-0.1.8/redast/core/packaging.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1283 2023-05-27 20:15:30.000000 redast-0.1.8/redast/core/packaging.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     6390 2022-08-17 19:23:58.000000 redast-0.1.8/redast/core/storage.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2070 2023-05-27 20:15:30.000000 redast-0.1.8/redast/core/storage.pyi
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-27 20:15:32.990434 redast-0.1.8/redast/local/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      186 2022-06-18 03:46:20.000000 redast-0.1.8/redast/local/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       86 2023-05-27 20:15:30.000000 redast-0.1.8/redast/local/__init__.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      621 2022-06-18 03:45:10.000000 redast-0.1.8/redast/local/cache.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      281 2023-05-27 20:15:30.000000 redast-0.1.8/redast/local/cache.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     2875 2022-08-17 19:23:58.000000 redast-0.1.8/redast/local/drive.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      446 2023-05-27 20:15:30.000000 redast-0.1.8/redast/local/drive.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      593 2022-06-18 03:45:27.000000 redast-0.1.8/redast/local/memory.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      231 2023-05-27 20:15:30.000000 redast-0.1.8/redast/local/memory.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1811 2022-06-18 03:45:37.000000 redast-0.1.8/redast/local/sqlite.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      379 2023-05-27 20:15:30.000000 redast-0.1.8/redast/local/sqlite.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      225 2022-06-18 03:48:02.000000 redast-0.1.8/redast/py.typed
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-27 20:15:32.990434 redast-0.1.8/redast/remote/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       99 2023-05-27 20:12:09.000000 redast-0.1.8/redast/remote/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        0 2023-05-27 20:15:30.000000 redast-0.1.8/redast/remote/__init__.pyi
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-27 20:15:32.994436 redast-0.1.8/redast/tool/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      118 2022-06-18 03:47:14.000000 redast-0.1.8/redast/tool/__init__.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       18 2023-05-27 20:15:30.000000 redast-0.1.8/redast/tool/__init__.pyi
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      565 2022-06-18 03:46:28.000000 redast-0.1.8/redast/tool/io.py
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      113 2023-05-27 20:15:30.000000 redast-0.1.8/redast/tool/io.pyi
+drwxrwxr-x   0 rilshok   (1000) rilshok   (1000)        0 2023-05-27 20:15:32.990434 redast-0.1.8/redast.egg-info/
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      824 2023-05-27 20:15:32.000000 redast-0.1.8/redast.egg-info/PKG-INFO
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)      866 2023-05-27 20:15:32.000000 redast-0.1.8/redast.egg-info/SOURCES.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        1 2023-05-27 20:15:32.000000 redast-0.1.8/redast.egg-info/dependency_links.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       50 2023-05-27 20:15:32.000000 redast-0.1.8/redast.egg-info/requires.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)        7 2023-05-27 20:15:32.000000 redast-0.1.8/redast.egg-info/top_level.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       50 2023-05-27 20:11:27.000000 redast-0.1.8/requirements.txt
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)       38 2023-05-27 20:15:32.994436 redast-0.1.8/setup.cfg
+-rw-rw-r--   0 rilshok   (1000) rilshok   (1000)     1294 2023-04-23 21:33:19.000000 redast-0.1.8/setup.py
```

### Comparing `redast-0.1.7/LICENSE` & `redast-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `redast-0.1.7/PKG-INFO` & `redast-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redast
-Version: 0.1.7
+Version: 0.1.8
 Summary: UNKNOWN
 Home-page: https://github.com/rilshok/redast
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `redast-0.1.7/redast/core/hash.py` & `redast-0.1.8/redast/core/hash.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.7/redast/core/packaging.py` & `redast-0.1.8/redast/core/packaging.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.7/redast/core/packaging.pyi` & `redast-0.1.8/redast/core/packaging.pyi`

 * *Files identical despite different names*

### Comparing `redast-0.1.7/redast/core/storage.py` & `redast-0.1.8/redast/core/storage.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.7/redast/core/storage.pyi` & `redast-0.1.8/redast/core/storage.pyi`

 * *Files identical despite different names*

### Comparing `redast-0.1.7/redast/local/cache.py` & `redast-0.1.8/redast/local/cache.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.7/redast/local/drive.py` & `redast-0.1.8/redast/local/drive.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.7/redast/local/memory.py` & `redast-0.1.8/redast/local/memory.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.7/redast/local/sqlite.py` & `redast-0.1.8/redast/local/sqlite.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.7/redast/tool/io.py` & `redast-0.1.8/redast/tool/io.py`

 * *Files identical despite different names*

### Comparing `redast-0.1.7/redast.egg-info/PKG-INFO` & `redast-0.1.8/redast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redast
-Version: 0.1.7
+Version: 0.1.8
 Summary: UNKNOWN
 Home-page: https://github.com/rilshok/redast
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `redast-0.1.7/redast.egg-info/SOURCES.txt` & `redast-0.1.8/redast.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,13 +29,11 @@
 redast/local/drive.pyi
 redast/local/memory.py
 redast/local/memory.pyi
 redast/local/sqlite.py
 redast/local/sqlite.pyi
 redast/remote/__init__.py
 redast/remote/__init__.pyi
-redast/remote/megacloud.py
-redast/remote/megacloud.pyi
 redast/tool/__init__.py
 redast/tool/__init__.pyi
 redast/tool/io.py
 redast/tool/io.pyi
```

### Comparing `redast-0.1.7/setup.py` & `redast-0.1.8/setup.py`

 * *Files identical despite different names*

