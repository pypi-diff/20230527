# Comparing `tmp/jutl-0.5.2.tar.gz` & `tmp/jutl-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jutl-0.5.2.tar", last modified: Wed Mar  8 08:23:04 2023, max compression
+gzip compressed data, was "jutl-0.5.3.tar", last modified: Sat May 27 05:18:49 2023, max compression
```

## Comparing `jutl-0.5.2.tar` & `jutl-0.5.3.tar`

### file list

```diff
@@ -1,60 +1,64 @@
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.610969 jutl-0.5.2/
--rw-r--r--   0 jordan     (502) staff       (20)     1073 2023-02-17 20:26:46.000000 jutl-0.5.2/LICENSE.md
--rw-r--r--   0 jordan     (502) staff       (20)     5819 2023-03-08 08:23:04.610817 jutl-0.5.2/PKG-INFO
--rw-r--r--   0 jordan     (502) staff       (20)     4537 2023-02-20 01:03:52.000000 jutl-0.5.2/README.md
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.600809 jutl-0.5.2/jutl/
--rw-r--r--   0 jordan     (502) staff       (20)      140 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/__init__.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.601928 jutl-0.5.2/jutl/averages/
--rw-r--r--   0 jordan     (502) staff       (20)        0 2023-01-12 10:17:39.000000 jutl-0.5.2/jutl/averages/__init__.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.602353 jutl-0.5.2/jutl/benchmarking/
--rw-r--r--   0 jordan     (502) staff       (20)      481 2023-03-04 17:38:54.000000 jutl-0.5.2/jutl/benchmarking/__init__.py
--rw-r--r--   0 jordan     (502) staff       (20)      666 2023-03-04 17:38:54.000000 jutl-0.5.2/jutl/benchmarking/latency.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.602555 jutl-0.5.2/jutl/calculators/
--rw-r--r--   0 jordan     (502) staff       (20)        0 2023-01-12 10:17:39.000000 jutl-0.5.2/jutl/calculators/__init__.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.602728 jutl-0.5.2/jutl/converters/
--rw-r--r--   0 jordan     (502) staff       (20)        0 2023-01-12 10:17:39.000000 jutl-0.5.2/jutl/converters/__init__.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.602879 jutl-0.5.2/jutl/cryptography/
--rw-r--r--   0 jordan     (502) staff       (20)        0 2023-01-12 10:17:39.000000 jutl-0.5.2/jutl/cryptography/__init__.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.603719 jutl-0.5.2/jutl/datastructures/
--rw-r--r--   0 jordan     (502) staff       (20)      252 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/datastructures/__init__.py
--rw-r--r--   0 jordan     (502) staff       (20)     5000 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/datastructures/queue.py
--rw-r--r--   0 jordan     (502) staff       (20)     4858 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/datastructures/stack.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.606300 jutl-0.5.2/jutl/exceptions/
--rw-r--r--   0 jordan     (502) staff       (20)      534 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/exceptions/__init__.py
--rw-r--r--   0 jordan     (502) staff       (20)      174 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/exceptions/emptypipeline.py
--rw-r--r--   0 jordan     (502) staff       (20)      168 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/exceptions/emptyqueue.py
--rw-r--r--   0 jordan     (502) staff       (20)      168 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/exceptions/emptystack.py
--rw-r--r--   0 jordan     (502) staff       (20)      166 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/exceptions/fullqueue.py
--rw-r--r--   0 jordan     (502) staff       (20)      166 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/exceptions/fullstack.py
--rw-r--r--   0 jordan     (502) staff       (20)      182 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/exceptions/invalidformatting.py
--rw-r--r--   0 jordan     (502) staff       (20)      174 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/exceptions/jutlexception.py
--rw-r--r--   0 jordan     (502) staff       (20)      172 2023-03-08 08:22:34.000000 jutl-0.5.2/jutl/exceptions/missinginput.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.607675 jutl-0.5.2/jutl/formatting/
--rw-r--r--   0 jordan     (502) staff       (20)      318 2023-01-12 10:17:39.000000 jutl-0.5.2/jutl/formatting/__init__.py
--rw-r--r--   0 jordan     (502) staff       (20)     3273 2023-02-02 08:49:08.000000 jutl-0.5.2/jutl/formatting/color.py
--rw-r--r--   0 jordan     (502) staff       (20)     1705 2023-01-12 10:17:39.000000 jutl-0.5.2/jutl/formatting/text.py
--rw-r--r--   0 jordan     (502) staff       (20)     1214 2023-02-20 01:03:52.000000 jutl-0.5.2/jutl/formatting/utils.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.607960 jutl-0.5.2/jutl/language/
--rw-r--r--   0 jordan     (502) staff       (20)        0 2023-01-12 10:17:39.000000 jutl-0.5.2/jutl/language/__init__.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.608305 jutl-0.5.2/jutl/logic/
--rw-r--r--   0 jordan     (502) staff       (20)        0 2023-01-12 10:17:39.000000 jutl-0.5.2/jutl/logic/__init__.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.608976 jutl-0.5.2/jutl/pipelining/
--rw-r--r--   0 jordan     (502) staff       (20)      306 2023-02-16 05:47:57.000000 jutl-0.5.2/jutl/pipelining/__init__.py
--rw-r--r--   0 jordan     (502) staff       (20)     1638 2023-02-20 01:03:52.000000 jutl-0.5.2/jutl/pipelining/datapipeline.py
--rw-r--r--   0 jordan     (502) staff       (20)     2901 2023-02-20 07:27:58.000000 jutl-0.5.2/jutl/pipelining/instructionpipeline.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.609230 jutl-0.5.2/jutl/sorters/
--rw-r--r--   0 jordan     (502) staff       (20)        0 2023-01-12 10:17:39.000000 jutl-0.5.2/jutl/sorters/__init__.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.609947 jutl-0.5.2/jutl/timers/
--rw-r--r--   0 jordan     (502) staff       (20)      267 2023-02-16 05:47:57.000000 jutl-0.5.2/jutl/timers/__init__.py
--rw-r--r--   0 jordan     (502) staff       (20)     5926 2023-02-20 01:03:52.000000 jutl-0.5.2/jutl/timers/stopwatch.py
--rw-r--r--   0 jordan     (502) staff       (20)     6003 2023-02-20 01:03:52.000000 jutl-0.5.2/jutl/timers/timer.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.610513 jutl-0.5.2/jutl/utilities/
--rw-r--r--   0 jordan     (502) staff       (20)      222 2023-02-16 05:47:57.000000 jutl-0.5.2/jutl/utilities/__init__.py
--rw-r--r--   0 jordan     (502) staff       (20)      495 2023-02-16 05:47:57.000000 jutl-0.5.2/jutl/utilities/helloworld.py
-drwxr-xr-x   0 jordan     (502) staff       (20)        0 2023-03-08 08:23:04.601725 jutl-0.5.2/jutl.egg-info/
--rw-r--r--   0 jordan     (502) staff       (20)     5819 2023-03-08 08:23:04.000000 jutl-0.5.2/jutl.egg-info/PKG-INFO
--rw-r--r--   0 jordan     (502) staff       (20)     1102 2023-03-08 08:23:04.000000 jutl-0.5.2/jutl.egg-info/SOURCES.txt
--rw-r--r--   0 jordan     (502) staff       (20)        1 2023-03-08 08:23:04.000000 jutl-0.5.2/jutl.egg-info/dependency_links.txt
--rw-r--r--   0 jordan     (502) staff       (20)        5 2023-03-08 08:23:04.000000 jutl-0.5.2/jutl.egg-info/top_level.txt
--rw-r--r--   0 jordan     (502) staff       (20)       38 2023-03-08 08:23:04.611019 jutl-0.5.2/setup.cfg
--rw-r--r--   0 jordan     (502) staff       (20)     2040 2023-03-08 08:22:34.000000 jutl-0.5.2/setup.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.559087 jutl-0.5.3/
+-rw-r--r--   0 welsman    (504) staff       (20)     1073 2023-03-09 03:13:40.000000 jutl-0.5.3/LICENSE.md
+-rw-r--r--   0 welsman    (504) staff       (20)     6047 2023-05-27 05:18:49.558761 jutl-0.5.3/PKG-INFO
+-rw-r--r--   0 welsman    (504) staff       (20)     4765 2023-03-22 18:49:37.000000 jutl-0.5.3/README.md
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.490571 jutl-0.5.3/jutl/
+-rw-r--r--   0 welsman    (504) staff       (20)      140 2023-05-27 05:14:40.000000 jutl-0.5.3/jutl/__init__.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.492488 jutl-0.5.3/jutl/averages/
+-rw-r--r--   0 welsman    (504) staff       (20)        0 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/averages/__init__.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.498397 jutl-0.5.3/jutl/benchmarking/
+-rw-r--r--   0 welsman    (504) staff       (20)      481 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/benchmarking/__init__.py
+-rw-r--r--   0 welsman    (504) staff       (20)      666 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/benchmarking/latency.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.499197 jutl-0.5.3/jutl/calculators/
+-rw-r--r--   0 welsman    (504) staff       (20)        0 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/calculators/__init__.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.499480 jutl-0.5.3/jutl/converters/
+-rw-r--r--   0 welsman    (504) staff       (20)        0 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/converters/__init__.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.500755 jutl-0.5.3/jutl/cryptography/
+-rw-r--r--   0 welsman    (504) staff       (20)      339 2023-04-10 22:45:33.000000 jutl-0.5.3/jutl/cryptography/__init__.py
+-rw-r--r--   0 welsman    (504) staff       (20)       58 2023-04-10 23:02:41.000000 jutl-0.5.3/jutl/cryptography/caesarcipher.py
+-rw-r--r--   0 welsman    (504) staff       (20)       58 2023-04-10 23:02:47.000000 jutl-0.5.3/jutl/cryptography/rot13cipher.py
+-rw-r--r--   0 welsman    (504) staff       (20)     1645 2023-04-10 23:33:07.000000 jutl-0.5.3/jutl/cryptography/substitutioncipher.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.501726 jutl-0.5.3/jutl/datastructures/
+-rw-r--r--   0 welsman    (504) staff       (20)      252 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/datastructures/__init__.py
+-rw-r--r--   0 welsman    (504) staff       (20)     5000 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/datastructures/queue.py
+-rw-r--r--   0 welsman    (504) staff       (20)     4858 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/datastructures/stack.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.520225 jutl-0.5.3/jutl/exceptions/
+-rw-r--r--   0 welsman    (504) staff       (20)      534 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/exceptions/__init__.py
+-rw-r--r--   0 welsman    (504) staff       (20)      174 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/exceptions/emptypipeline.py
+-rw-r--r--   0 welsman    (504) staff       (20)      168 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/exceptions/emptyqueue.py
+-rw-r--r--   0 welsman    (504) staff       (20)      168 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/exceptions/emptystack.py
+-rw-r--r--   0 welsman    (504) staff       (20)      166 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/exceptions/fullqueue.py
+-rw-r--r--   0 welsman    (504) staff       (20)      166 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/exceptions/fullstack.py
+-rw-r--r--   0 welsman    (504) staff       (20)      182 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/exceptions/invalidformatting.py
+-rw-r--r--   0 welsman    (504) staff       (20)      174 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/exceptions/jutlexception.py
+-rw-r--r--   0 welsman    (504) staff       (20)      172 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/exceptions/missinginput.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.523076 jutl-0.5.3/jutl/formatting/
+-rw-r--r--   0 welsman    (504) staff       (20)      318 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/formatting/__init__.py
+-rw-r--r--   0 welsman    (504) staff       (20)     3273 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/formatting/color.py
+-rw-r--r--   0 welsman    (504) staff       (20)     1705 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/formatting/text.py
+-rw-r--r--   0 welsman    (504) staff       (20)     1214 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/formatting/utils.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.524024 jutl-0.5.3/jutl/language/
+-rw-r--r--   0 welsman    (504) staff       (20)        0 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/language/__init__.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.524324 jutl-0.5.3/jutl/logic/
+-rw-r--r--   0 welsman    (504) staff       (20)        0 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/logic/__init__.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.533422 jutl-0.5.3/jutl/pipelining/
+-rw-r--r--   0 welsman    (504) staff       (20)      306 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/pipelining/__init__.py
+-rw-r--r--   0 welsman    (504) staff       (20)     1638 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/pipelining/datapipeline.py
+-rw-r--r--   0 welsman    (504) staff       (20)     2901 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/pipelining/instructionpipeline.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.555235 jutl-0.5.3/jutl/sorters/
+-rw-r--r--   0 welsman    (504) staff       (20)        0 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/sorters/__init__.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.557427 jutl-0.5.3/jutl/timers/
+-rw-r--r--   0 welsman    (504) staff       (20)      309 2023-05-10 13:45:17.000000 jutl-0.5.3/jutl/timers/__init__.py
+-rw-r--r--   0 welsman    (504) staff       (20)     6067 2023-05-10 14:49:28.000000 jutl-0.5.3/jutl/timers/reporter.py
+-rw-r--r--   0 welsman    (504) staff       (20)     5926 2023-05-10 14:36:09.000000 jutl-0.5.3/jutl/timers/stopwatch.py
+-rw-r--r--   0 welsman    (504) staff       (20)     6039 2023-05-27 05:07:06.000000 jutl-0.5.3/jutl/timers/timer.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.558118 jutl-0.5.3/jutl/utilities/
+-rw-r--r--   0 welsman    (504) staff       (20)      222 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/utilities/__init__.py
+-rw-r--r--   0 welsman    (504) staff       (20)      495 2023-03-09 03:13:40.000000 jutl-0.5.3/jutl/utilities/helloworld.py
+drwxr-xr-x   0 welsman    (504) staff       (20)        0 2023-05-27 05:18:49.492160 jutl-0.5.3/jutl.egg-info/
+-rw-r--r--   0 welsman    (504) staff       (20)     6047 2023-05-27 05:18:48.000000 jutl-0.5.3/jutl.egg-info/PKG-INFO
+-rw-r--r--   0 welsman    (504) staff       (20)     1233 2023-05-27 05:18:49.000000 jutl-0.5.3/jutl.egg-info/SOURCES.txt
+-rw-r--r--   0 welsman    (504) staff       (20)        1 2023-05-27 05:18:48.000000 jutl-0.5.3/jutl.egg-info/dependency_links.txt
+-rw-r--r--   0 welsman    (504) staff       (20)        5 2023-05-27 05:18:48.000000 jutl-0.5.3/jutl.egg-info/top_level.txt
+-rw-r--r--   0 welsman    (504) staff       (20)       38 2023-05-27 05:18:49.559197 jutl-0.5.3/setup.cfg
+-rw-r--r--   0 welsman    (504) staff       (20)     2040 2023-05-27 05:14:22.000000 jutl-0.5.3/setup.py
```

### Comparing `jutl-0.5.2/LICENSE.md` & `jutl-0.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jutl-0.5.2/PKG-INFO` & `jutl-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jutl
-Version: 0.5.2
+Version: 0.5.3
 Summary: A Python package of useful tools and utilities.
 Home-page: https://pypi.org/project/jutl/
 Download-URL: https://github.com/JordanWelsman/jutils/tags
 Author: Jordan Welsman
 Author-email: jordan.welsman@outlook.com
 License: MIT
 Keywords: python,averages,calculators,converters,cryptography,formatting,language,logic,pipelining,sorters,timers,utilities
@@ -41,16 +41,17 @@
 
 ------------------------------------------------------
 
 <div align="center">
 
 [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/tags)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/releases)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/JordanWelsman/jutils/pytest.yaml?label=pytest&style=for-the-badge)](https://github.com/JordanWelsman/jutils/actions/workflows/pytest.yaml)
 [![GitHub Release Date](https://img.shields.io/github/release-date/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/wiki/Version-History)
-[![GitHub](https://img.shields.io/github/license/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/blob/main/LICENSE.md)
+[![GitHub License](https://img.shields.io/github/license/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/blob/main/LICENSE.md)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/commits/main)
 [![GitHub wiki](https://img.shields.io/badge/wiki-jutils-blueviolet?style=for-the-badge)](https://github.com/JordanWelsman/jutils/wiki)
 
 </div>
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/jutl?style=for-the-badge)](https://pypi.org/project/jutl)
```

### Comparing `jutl-0.5.2/README.md` & `jutl-0.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 ------------------------------------------------------
 
 <div align="center">
 
 [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/tags)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/releases)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/JordanWelsman/jutils/pytest.yaml?label=pytest&style=for-the-badge)](https://github.com/JordanWelsman/jutils/actions/workflows/pytest.yaml)
 [![GitHub Release Date](https://img.shields.io/github/release-date/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/wiki/Version-History)
-[![GitHub](https://img.shields.io/github/license/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/blob/main/LICENSE.md)
+[![GitHub License](https://img.shields.io/github/license/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/blob/main/LICENSE.md)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/commits/main)
 [![GitHub wiki](https://img.shields.io/badge/wiki-jutils-blueviolet?style=for-the-badge)](https://github.com/JordanWelsman/jutils/wiki)
 
 </div>
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/jutl?style=for-the-badge)](https://pypi.org/project/jutl)
```

### Comparing `jutl-0.5.2/jutl/benchmarking/latency.py` & `jutl-0.5.3/jutl/benchmarking/latency.py`

 * *Files identical despite different names*

### Comparing `jutl-0.5.2/jutl/datastructures/queue.py` & `jutl-0.5.3/jutl/datastructures/queue.py`

 * *Files identical despite different names*

### Comparing `jutl-0.5.2/jutl/datastructures/stack.py` & `jutl-0.5.3/jutl/datastructures/stack.py`

 * *Files identical despite different names*

### Comparing `jutl-0.5.2/jutl/exceptions/__init__.py` & `jutl-0.5.3/jutl/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `jutl-0.5.2/jutl/formatting/color.py` & `jutl-0.5.3/jutl/formatting/color.py`

 * *Files identical despite different names*

### Comparing `jutl-0.5.2/jutl/formatting/text.py` & `jutl-0.5.3/jutl/formatting/text.py`

 * *Files identical despite different names*

### Comparing `jutl-0.5.2/jutl/formatting/utils.py` & `jutl-0.5.3/jutl/formatting/utils.py`

 * *Files identical despite different names*

### Comparing `jutl-0.5.2/jutl/pipelining/datapipeline.py` & `jutl-0.5.3/jutl/pipelining/datapipeline.py`

 * *Files identical despite different names*

### Comparing `jutl-0.5.2/jutl/pipelining/instructionpipeline.py` & `jutl-0.5.3/jutl/pipelining/instructionpipeline.py`

 * *Files identical despite different names*

### Comparing `jutl-0.5.2/jutl/timers/stopwatch.py` & `jutl-0.5.3/jutl/timers/stopwatch.py`

 * *Files identical despite different names*

### Comparing `jutl-0.5.2/jutl/timers/timer.py` & `jutl-0.5.3/jutl/timers/timer.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,25 +32,25 @@
                 return f"Timer({round(self.total_time, 2)}s)"
         else:
             if self.total_time is None:
                 return f"Timer({self.name})"
             else:
                 return f"Timer({self.name}, {round(self.total_time, 2)}s)"
     
-    def __call__(self, color: str = None):
+    def __call__(self, precision: int = 2, color: str = None):
         """
         Tells the interpreter what to
         do when an object of this
         class is called directly.
         """
         if self.total_time:
             if color:
-                print(apply(text=f"{self.name} total time: {round(self.total_time, 2)}s", text_color=color))
+                print(apply(text=f"{self.name} total time: {round(self.total_time, precision)}s", text_color=color))
             else:
-                print(f"{self.name} total time: {round(self.total_time, 2)}s")
+                print(f"{self.name} total time: {round(self.total_time, precision)}s")
         else:
             print("There is no recorded time.")
     
     def __len__(self):
         """
         Tells the interpreter what to
         consider this class' length.
```

### Comparing `jutl-0.5.2/jutl.egg-info/PKG-INFO` & `jutl-0.5.3/jutl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jutl
-Version: 0.5.2
+Version: 0.5.3
 Summary: A Python package of useful tools and utilities.
 Home-page: https://pypi.org/project/jutl/
 Download-URL: https://github.com/JordanWelsman/jutils/tags
 Author: Jordan Welsman
 Author-email: jordan.welsman@outlook.com
 License: MIT
 Keywords: python,averages,calculators,converters,cryptography,formatting,language,logic,pipelining,sorters,timers,utilities
@@ -41,16 +41,17 @@
 
 ------------------------------------------------------
 
 <div align="center">
 
 [![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/tags)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/releases)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/JordanWelsman/jutils/pytest.yaml?label=pytest&style=for-the-badge)](https://github.com/JordanWelsman/jutils/actions/workflows/pytest.yaml)
 [![GitHub Release Date](https://img.shields.io/github/release-date/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/wiki/Version-History)
-[![GitHub](https://img.shields.io/github/license/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/blob/main/LICENSE.md)
+[![GitHub License](https://img.shields.io/github/license/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/blob/main/LICENSE.md)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/JordanWelsman/jutils?style=for-the-badge)](https://github.com/JordanWelsman/jutils/commits/main)
 [![GitHub wiki](https://img.shields.io/badge/wiki-jutils-blueviolet?style=for-the-badge)](https://github.com/JordanWelsman/jutils/wiki)
 
 </div>
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/jutl?style=for-the-badge)](https://pypi.org/project/jutl)
```

### Comparing `jutl-0.5.2/jutl.egg-info/SOURCES.txt` & `jutl-0.5.3/jutl.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 jutl.egg-info/top_level.txt
 jutl/averages/__init__.py
 jutl/benchmarking/__init__.py
 jutl/benchmarking/latency.py
 jutl/calculators/__init__.py
 jutl/converters/__init__.py
 jutl/cryptography/__init__.py
+jutl/cryptography/caesarcipher.py
+jutl/cryptography/rot13cipher.py
+jutl/cryptography/substitutioncipher.py
 jutl/datastructures/__init__.py
 jutl/datastructures/queue.py
 jutl/datastructures/stack.py
 jutl/exceptions/__init__.py
 jutl/exceptions/emptypipeline.py
 jutl/exceptions/emptyqueue.py
 jutl/exceptions/emptystack.py
@@ -31,11 +34,12 @@
 jutl/language/__init__.py
 jutl/logic/__init__.py
 jutl/pipelining/__init__.py
 jutl/pipelining/datapipeline.py
 jutl/pipelining/instructionpipeline.py
 jutl/sorters/__init__.py
 jutl/timers/__init__.py
+jutl/timers/reporter.py
 jutl/timers/stopwatch.py
 jutl/timers/timer.py
 jutl/utilities/__init__.py
 jutl/utilities/helloworld.py
```

### Comparing `jutl-0.5.2/setup.py` & `jutl-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Module imports
 from setuptools import setup
 
 # Arguments
 git_name = "jutils"
 pypi_name = "jutl"
-version = "0.5.2" # update __init__.py
+version = "0.5.3" # update __init__.py
 python_version = ">=3.10"
 
 # Long description from README.md
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # jutils package data
```

