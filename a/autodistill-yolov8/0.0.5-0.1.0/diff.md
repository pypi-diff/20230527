# Comparing `tmp/autodistill_yolov8-0.0.5.tar.gz` & `tmp/autodistill_yolov8-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill_yolov8-0.0.5.tar", last modified: Wed May 17 23:05:38 2023, max compression
+gzip compressed data, was "dist/autodistill_yolov8-0.1.0.tar", last modified: Sat May 27 03:02:18 2023, max compression
```

## Comparing `autodistill_yolov8-0.0.5.tar` & `autodistill_yolov8-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:05:38.922797 autodistill_yolov8-0.0.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      641 2023-05-17 23:05:38.922797 autodistill_yolov8-0.0.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3157 2023-05-15 17:30:29.000000 autodistill_yolov8-0.0.5/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:05:38.922797 autodistill_yolov8-0.0.5/autodistill_yolov8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       68 2023-05-17 21:28:40.000000 autodistill_yolov8-0.0.5/autodistill_yolov8/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      377 2023-05-17 21:28:40.000000 autodistill_yolov8-0.0.5/autodistill_yolov8/yolov8.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:05:38.922797 autodistill_yolov8-0.0.5/autodistill_yolov8.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      641 2023-05-17 23:05:38.000000 autodistill_yolov8-0.0.5/autodistill_yolov8.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      306 2023-05-17 23:05:38.000000 autodistill_yolov8-0.0.5/autodistill_yolov8.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 23:05:38.000000 autodistill_yolov8-0.0.5/autodistill_yolov8.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2023-05-17 23:05:38.000000 autodistill_yolov8-0.0.5/autodistill_yolov8.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-05-17 23:05:38.000000 autodistill_yolov8-0.0.5/autodistill_yolov8.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 23:05:38.926797 autodistill_yolov8-0.0.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1309 2023-05-17 23:05:35.000000 autodistill_yolov8-0.0.5/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:05:38.922797 autodistill_yolov8-0.0.5/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-05-17 21:20:42.000000 autodistill_yolov8-0.0.5/test/test_hello.py
+drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      594 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/PKG-INFO
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     3157 2023-05-27 02:55:33.000000 autodistill_yolov8-0.1.0/README.md
+drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8/
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       68 2023-05-27 03:02:12.000000 autodistill_yolov8-0.1.0/autodistill_yolov8/__init__.py
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      442 2023-05-27 02:55:33.000000 autodistill_yolov8-0.1.0/autodistill_yolov8/yolov8.py
+drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      594 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/PKG-INFO
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      306 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/SOURCES.txt
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)        1 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/dependency_links.txt
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       85 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/requires.txt
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       19 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/top_level.txt
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       38 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/setup.cfg
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     1309 2023-05-27 02:55:33.000000 autodistill_yolov8-0.1.0/setup.py
+drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/test/
+-rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       40 2023-05-27 02:55:33.000000 autodistill_yolov8-0.1.0/test/test_hello.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `autodistill_yolov8-0.0.5/README.md` & `autodistill_yolov8-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `autodistill_yolov8-0.0.5/autodistill_yolov8.egg-info/PKG-INFO` & `autodistill_yolov8-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
-Name: autodistill-yolov8
-Version: 0.0.5
+Name: autodistill_yolov8
+Version: 0.1.0
 Summary: Automatically distill large foundational models into smaller, in-domain models for deployment
 Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ
 Author: Roboflow
 Author-email: jacob@roboflow.com
-License: UNKNOWN
-Description: Automatically distill large foundational models into smaller, in-domain models for deployment
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+
+Automatically distill large foundational models into smaller, in-domain models for deployment
```

### Comparing `autodistill_yolov8-0.0.5/setup.py` & `autodistill_yolov8-0.1.0/setup.py`

 * *Files identical despite different names*

