# Comparing `tmp/s5-pytorch-0.1.7.tar.gz` & `tmp/s5-pytorch-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5-pytorch-0.1.7.tar", last modified: Tue Mar 21 00:10:56 2023, max compression
+gzip compressed data, was "s5-pytorch-0.1.8.tar", last modified: Sat May 27 11:43:28 2023, max compression
```

## Comparing `s5-pytorch-0.1.7.tar` & `s5-pytorch-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-03-21 00:10:56.450941 s5-pytorch-0.1.7/
--rw-r--r--   0 null      (1000) null      (1000)    16727 2023-03-21 00:02:05.000000 s5-pytorch-0.1.7/LICENSE
--rw-r--r--   0 null      (1000) null      (1000)      685 2023-03-21 00:10:56.449941 s5-pytorch-0.1.7/PKG-INFO
--rw-r--r--   0 null      (1000) null      (1000)      666 2023-01-16 11:22:05.000000 s5-pytorch-0.1.7/README.md
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-03-21 00:10:56.449941 s5-pytorch-0.1.7/s5/
--rw-r--r--   0 null      (1000) null      (1000)       24 2023-01-16 11:22:05.000000 s5-pytorch-0.1.7/s5/__init__.py
--rw-r--r--   0 null      (1000) null      (1000)     8786 2023-02-08 11:34:23.000000 s5-pytorch-0.1.7/s5/init.py
--rw-r--r--   0 null      (1000) null      (1000)    15899 2023-02-08 11:34:23.000000 s5-pytorch-0.1.7/s5/jax_compat.py
--rw-r--r--   0 null      (1000) null      (1000)    17510 2023-03-21 00:02:54.000000 s5-pytorch-0.1.7/s5/s5_model.py
-drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-03-21 00:10:56.449941 s5-pytorch-0.1.7/s5_pytorch.egg-info/
--rw-r--r--   0 null      (1000) null      (1000)      685 2023-03-21 00:10:56.000000 s5-pytorch-0.1.7/s5_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 null      (1000) null      (1000)      253 2023-03-21 00:10:56.000000 s5-pytorch-0.1.7/s5_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 null      (1000) null      (1000)        1 2023-03-21 00:10:56.000000 s5-pytorch-0.1.7/s5_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 null      (1000) null      (1000)       34 2023-03-21 00:10:56.000000 s5-pytorch-0.1.7/s5_pytorch.egg-info/requires.txt
--rw-r--r--   0 null      (1000) null      (1000)        3 2023-03-21 00:10:56.000000 s5-pytorch-0.1.7/s5_pytorch.egg-info/top_level.txt
--rw-r--r--   0 null      (1000) null      (1000)       38 2023-03-21 00:10:56.450941 s5-pytorch-0.1.7/setup.cfg
--rw-r--r--   0 null      (1000) null      (1000)      912 2023-03-21 00:02:54.000000 s5-pytorch-0.1.7/setup.py
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-05-27 11:43:28.786533 s5-pytorch-0.1.8/
+-rw-r--r--   0 null      (1000) null      (1000)    16727 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/LICENSE
+-rw-r--r--   0 null      (1000) null      (1000)     2122 2023-05-27 11:43:28.786533 s5-pytorch-0.1.8/PKG-INFO
+-rw-r--r--   0 null      (1000) null      (1000)     1444 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/README.md
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-05-27 11:43:28.785534 s5-pytorch-0.1.8/s5/
+-rw-r--r--   0 null      (1000) null      (1000)       24 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/s5/__init__.py
+-rw-r--r--   0 null      (1000) null      (1000)     8786 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/s5/init.py
+-rw-r--r--   0 null      (1000) null      (1000)    15899 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/s5/jax_compat.py
+-rw-r--r--   0 null      (1000) null      (1000)    17510 2023-05-27 11:40:20.000000 s5-pytorch-0.1.8/s5/s5_model.py
+drwxr-xr-x   0 null      (1000) null      (1000)        0 2023-05-27 11:43:28.786533 s5-pytorch-0.1.8/s5_pytorch.egg-info/
+-rw-r--r--   0 null      (1000) null      (1000)     2122 2023-05-27 11:43:28.000000 s5-pytorch-0.1.8/s5_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 null      (1000) null      (1000)      253 2023-05-27 11:43:28.000000 s5-pytorch-0.1.8/s5_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 null      (1000) null      (1000)        1 2023-05-27 11:43:28.000000 s5-pytorch-0.1.8/s5_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 null      (1000) null      (1000)       34 2023-05-27 11:43:28.000000 s5-pytorch-0.1.8/s5_pytorch.egg-info/requires.txt
+-rw-r--r--   0 null      (1000) null      (1000)        3 2023-05-27 11:43:28.000000 s5-pytorch-0.1.8/s5_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 null      (1000) null      (1000)       38 2023-05-27 11:43:28.786533 s5-pytorch-0.1.8/setup.cfg
+-rw-r--r--   0 null      (1000) null      (1000)     1023 2023-05-27 11:41:40.000000 s5-pytorch-0.1.8/setup.py
```

### Comparing `s5-pytorch-0.1.7/LICENSE` & `s5-pytorch-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `s5-pytorch-0.1.7/s5/init.py` & `s5-pytorch-0.1.8/s5/init.py`

 * *Files identical despite different names*

### Comparing `s5-pytorch-0.1.7/s5/jax_compat.py` & `s5-pytorch-0.1.8/s5/jax_compat.py`

 * *Files identical despite different names*

### Comparing `s5-pytorch-0.1.7/s5/s5_model.py` & `s5-pytorch-0.1.8/s5/s5_model.py`

 * *Files identical despite different names*

