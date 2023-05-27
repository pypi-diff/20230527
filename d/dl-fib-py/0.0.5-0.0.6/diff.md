# Comparing `tmp/dl_fib_py-0.0.5.tar.gz` & `tmp/dl_fib_py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_fib_py-0.0.5.tar", last modified: Fri May 26 16:25:00 2023, max compression
+gzip compressed data, was "dl_fib_py-0.0.6.tar", last modified: Sat May 27 06:14:57 2023, max compression
```

## Comparing `dl_fib_py-0.0.5.tar` & `dl_fib_py-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.744532 dl_fib_py-0.0.5/
--rw-r--r--   0 dimalurie   (501) staff       (20)     1067 2023-05-26 13:48:50.000000 dl_fib_py-0.0.5/LICENSE
--rw-r--r--   0 dimalurie   (501) staff       (20)      486 2023-05-26 16:25:00.744298 dl_fib_py-0.0.5/PKG-INFO
--rw-r--r--   0 dimalurie   (501) staff       (20)       41 2023-05-26 13:48:50.000000 dl_fib_py-0.0.5/README.md
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.742165 dl_fib_py-0.0.5/dl_fib_py/
--rw-r--r--   0 dimalurie   (501) staff       (20)       69 2023-05-26 14:03:24.000000 dl_fib_py-0.0.5/dl_fib_py/__init__.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.743143 dl_fib_py-0.0.5/dl_fib_py/cmd/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 14:12:56.000000 dl_fib_py-0.0.5/dl_fib_py/cmd/__init__.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      504 2023-05-26 14:14:31.000000 dl_fib_py-0.0.5/dl_fib_py/cmd/fib_numb.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.743580 dl_fib_py-0.0.5/dl_fib_py/fib_calcs/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 14:05:34.000000 dl_fib_py-0.0.5/dl_fib_py/fib_calcs/__init__.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      345 2023-05-26 15:38:29.000000 dl_fib_py-0.0.5/dl_fib_py/fib_calcs/fib_number.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      200 2023-05-26 14:06:36.000000 dl_fib_py-0.0.5/dl_fib_py/fib_calcs/fib_numbers.py
--rw-r--r--   0 dimalurie   (501) staff       (20)       15 2023-05-26 16:24:50.000000 dl_fib_py-0.0.5/dl_fib_py/version.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.742771 dl_fib_py-0.0.5/dl_fib_py.egg-info/
--rw-r--r--   0 dimalurie   (501) staff       (20)      486 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/PKG-INFO
--rw-r--r--   0 dimalurie   (501) staff       (20)      579 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/SOURCES.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)        1 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/dependency_links.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)       63 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/entry_points.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)       37 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/requires.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)       16 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/top_level.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)       38 2023-05-26 16:25:00.744571 dl_fib_py-0.0.5/setup.cfg
--rw-r--r--   0 dimalurie   (501) staff       (20)     1099 2023-05-26 16:24:44.000000 dl_fib_py-0.0.5/setup.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.741549 dl_fib_py-0.0.5/tests/
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.743751 dl_fib_py-0.0.5/tests/dl_fib_py/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:04:16.000000 dl_fib_py-0.0.5/tests/dl_fib_py/__init__.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.744100 dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:04:34.000000 dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/__init__.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      684 2023-05-26 15:49:50.000000 dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/test_fib_number.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      804 2023-05-26 15:18:31.000000 dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/test_fib_numbers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:57.002194 dl_fib_py-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-27 06:14:57.002194 dl_fib_py-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:56.998194 dl_fib_py-0.0.6/dl_fib_py/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/dl_fib_py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:56.998194 dl_fib_py-0.0.6/dl_fib_py/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/dl_fib_py/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/dl_fib_py/cmd/fib_numb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:57.002194 dl_fib_py-0.0.6/dl_fib_py/fib_calcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/dl_fib_py/fib_calcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/dl_fib_py/fib_calcs/fib_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/dl_fib_py/fib_calcs/fib_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-27 06:14:52.000000 dl_fib_py-0.0.6/dl_fib_py/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:56.998194 dl_fib_py-0.0.6/dl_fib_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-27 06:14:56.000000 dl_fib_py-0.0.6/dl_fib_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-27 06:14:56.000000 dl_fib_py-0.0.6/dl_fib_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:14:56.000000 dl_fib_py-0.0.6/dl_fib_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-27 06:14:56.000000 dl_fib_py-0.0.6/dl_fib_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-27 06:14:56.000000 dl_fib_py-0.0.6/dl_fib_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 06:14:56.000000 dl_fib_py-0.0.6/dl_fib_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 06:14:57.002194 dl_fib_py-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:56.998194 dl_fib_py-0.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:57.002194 dl_fib_py-0.0.6/tests/dl_fib_py/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/tests/dl_fib_py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:57.002194 dl_fib_py-0.0.6/tests/dl_fib_py/fib_calcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/tests/dl_fib_py/fib_calcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/tests/dl_fib_py/fib_calcs/test_fib_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-27 06:14:34.000000 dl_fib_py-0.0.6/tests/dl_fib_py/fib_calcs/test_fib_numbers.py
```

### Comparing `dl_fib_py-0.0.5/LICENSE` & `dl_fib_py-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_fib_py-0.0.5/dl_fib_py.egg-info/SOURCES.txt` & `dl_fib_py-0.0.6/dl_fib_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dl_fib_py-0.0.5/setup.py` & `dl_fib_py-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/test_fib_number.py` & `dl_fib_py-0.0.6/tests/dl_fib_py/fib_calcs/test_fib_number.py`

 * *Files identical despite different names*

### Comparing `dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/test_fib_numbers.py` & `dl_fib_py-0.0.6/tests/dl_fib_py/fib_calcs/test_fib_numbers.py`

 * *Files identical despite different names*

