# Comparing `tmp/mavcom-1.0.1.tar.gz` & `tmp/mavcom-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mavcom-1.0.1.tar", last modified: Sat May 27 11:57:20 2023, max compression
+gzip compressed data, was "mavcom-1.0.2.tar", last modified: Sat May 27 12:38:22 2023, max compression
```

## Comparing `mavcom-1.0.1.tar` & `mavcom-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 11:57:20.279576 mavcom-1.0.1/
--rw-rw-r--   0 main      (1000) main      (1000)     1066 2023-05-26 21:59:37.000000 mavcom-1.0.1/LICENSE
--rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 11:57:20.279576 mavcom-1.0.1/PKG-INFO
--rw-rw-r--   0 main      (1000) main      (1000)      717 2023-05-26 23:18:10.000000 mavcom-1.0.1/README.md
--rw-rw-r--   0 main      (1000) main      (1000)      886 2023-05-27 11:55:24.000000 mavcom-1.0.1/pyproject.toml
--rw-rw-r--   0 main      (1000) main      (1000)       38 2023-05-27 11:57:20.279576 mavcom-1.0.1/setup.cfg
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 11:57:20.279576 mavcom-1.0.1/src/
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 11:57:20.279576 mavcom-1.0.1/src/mavcom/
--rw-rw-r--   0 main      (1000) main      (1000)        0 2023-05-26 10:29:36.000000 mavcom-1.0.1/src/mavcom/__init__.py
--rw-rw-r--   0 main      (1000) main      (1000)     9223 2023-05-27 11:53:36.000000 mavcom-1.0.1/src/mavcom/mavcom.py
--rw-rw-r--   0 main      (1000) main      (1000)     1646 2023-05-26 10:10:28.000000 mavcom-1.0.1/src/mavcom/mavconstants.py
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 11:57:20.279576 mavcom-1.0.1/src/mavcom.egg-info/
--rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/PKG-INFO
--rw-rw-r--   0 main      (1000) main      (1000)      330 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/SOURCES.txt
--rw-rw-r--   0 main      (1000) main      (1000)        1 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/dependency_links.txt
--rw-rw-r--   0 main      (1000) main      (1000)       52 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/entry_points.txt
--rw-rw-r--   0 main      (1000) main      (1000)       49 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/requires.txt
--rw-rw-r--   0 main      (1000) main      (1000)        7 2023-05-27 11:57:20.000000 mavcom-1.0.1/src/mavcom.egg-info/top_level.txt
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 11:57:20.279576 mavcom-1.0.1/tests/
--rw-rw-r--   0 main      (1000) main      (1000)     1218 2023-05-27 00:25:30.000000 mavcom-1.0.1/tests/test_mavcom.py
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 12:38:22.102642 mavcom-1.0.2/
+-rw-rw-r--   0 main      (1000) main      (1000)     1066 2023-05-26 21:59:37.000000 mavcom-1.0.2/LICENSE
+-rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 12:38:22.102642 mavcom-1.0.2/PKG-INFO
+-rw-rw-r--   0 main      (1000) main      (1000)      717 2023-05-26 23:18:10.000000 mavcom-1.0.2/README.md
+-rw-rw-r--   0 main      (1000) main      (1000)      886 2023-05-27 12:36:34.000000 mavcom-1.0.2/pyproject.toml
+-rw-rw-r--   0 main      (1000) main      (1000)       38 2023-05-27 12:38:22.102642 mavcom-1.0.2/setup.cfg
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 12:38:22.102642 mavcom-1.0.2/src/
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 12:38:22.102642 mavcom-1.0.2/src/mavcom/
+-rw-rw-r--   0 main      (1000) main      (1000)        0 2023-05-26 10:29:36.000000 mavcom-1.0.2/src/mavcom/__init__.py
+-rw-rw-r--   0 main      (1000) main      (1000)     9223 2023-05-27 11:53:36.000000 mavcom-1.0.2/src/mavcom/mavcom.py
+-rw-rw-r--   0 main      (1000) main      (1000)     1646 2023-05-26 10:10:28.000000 mavcom-1.0.2/src/mavcom/mavconstants.py
+-rw-rw-r--   0 main      (1000) main      (1000)     4332 2023-05-27 12:36:59.000000 mavcom-1.0.2/src/mavcom/video.py
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 12:38:22.102642 mavcom-1.0.2/src/mavcom.egg-info/
+-rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 12:38:22.000000 mavcom-1.0.2/src/mavcom.egg-info/PKG-INFO
+-rw-rw-r--   0 main      (1000) main      (1000)      350 2023-05-27 12:38:22.000000 mavcom-1.0.2/src/mavcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 main      (1000) main      (1000)        1 2023-05-27 12:38:22.000000 mavcom-1.0.2/src/mavcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 main      (1000) main      (1000)       52 2023-05-27 12:38:22.000000 mavcom-1.0.2/src/mavcom.egg-info/entry_points.txt
+-rw-rw-r--   0 main      (1000) main      (1000)       49 2023-05-27 12:38:22.000000 mavcom-1.0.2/src/mavcom.egg-info/requires.txt
+-rw-rw-r--   0 main      (1000) main      (1000)        7 2023-05-27 12:38:22.000000 mavcom-1.0.2/src/mavcom.egg-info/top_level.txt
+drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 12:38:22.102642 mavcom-1.0.2/tests/
+-rw-rw-r--   0 main      (1000) main      (1000)     1218 2023-05-27 00:25:30.000000 mavcom-1.0.2/tests/test_mavcom.py
```

### Comparing `mavcom-1.0.1/LICENSE` & `mavcom-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mavcom-1.0.1/PKG-INFO` & `mavcom-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mavcom-1.0.1/README.md` & `mavcom-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mavcom-1.0.1/pyproject.toml` & `mavcom-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mavcom"
-version = "1.0.1"
+version = "1.0.2"
 description = "A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers"
 readme = "README.md"
 authors = [{ name = "Mavscient", email = "mavscient@xee4c.33mail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mavcom-1.0.1/src/mavcom/mavcom.py` & `mavcom-1.0.2/src/mavcom/mavcom.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.0.1/src/mavcom/mavconstants.py` & `mavcom-1.0.2/src/mavcom/mavconstants.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.0.1/src/mavcom.egg-info/PKG-INFO` & `mavcom-1.0.2/src/mavcom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mavcom-1.0.1/tests/test_mavcom.py` & `mavcom-1.0.2/tests/test_mavcom.py`

 * *Files identical despite different names*

