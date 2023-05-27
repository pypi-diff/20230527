# Comparing `tmp/pogt-1.0.0.tar.gz` & `tmp/pogt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pogt-1.0.0.tar", last modified: Sat May 27 03:56:23 2023, max compression
+gzip compressed data, was "pogt-1.0.1.tar", last modified: Sat May 27 04:10:59 2023, max compression
```

## Comparing `pogt-1.0.0.tar` & `pogt-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxr-xr-x   0 pc         (501) staff       (20)        0 2023-05-27 03:56:23.598532 pogt-1.0.0/
--rw-r--r--   0 pc         (501) staff       (20)      322 2023-05-27 03:56:23.597573 pogt-1.0.0/PKG-INFO
-drwxr-xr-x   0 pc         (501) staff       (20)        0 2023-05-27 03:56:23.595208 pogt-1.0.0/pogt.egg-info/
--rw-r--r--   0 pc         (501) staff       (20)      322 2023-05-27 03:56:23.000000 pogt-1.0.0/pogt.egg-info/PKG-INFO
--rw-r--r--   0 pc         (501) staff       (20)      120 2023-05-27 03:56:23.000000 pogt-1.0.0/pogt.egg-info/SOURCES.txt
--rw-r--r--   0 pc         (501) staff       (20)        1 2023-05-27 03:56:23.000000 pogt-1.0.0/pogt.egg-info/dependency_links.txt
--rw-r--r--   0 pc         (501) staff       (20)        1 2023-05-27 03:56:23.000000 pogt-1.0.0/pogt.egg-info/top_level.txt
--rw-r--r--   0 pc         (501) staff       (20)       38 2023-05-27 03:56:23.598877 pogt-1.0.0/setup.cfg
--rw-r--r--   0 pc         (501) staff       (20)      449 2023-05-27 03:55:20.000000 pogt-1.0.0/setup.py
+drwxr-xr-x   0 pc         (501) staff       (20)        0 2023-05-27 04:10:59.032340 pogt-1.0.1/
+-rw-r--r--   0 pc         (501) staff       (20)      322 2023-05-27 04:10:59.031651 pogt-1.0.1/PKG-INFO
+drwxr-xr-x   0 pc         (501) staff       (20)        0 2023-05-27 04:10:59.030196 pogt-1.0.1/pogt.egg-info/
+-rw-r--r--   0 pc         (501) staff       (20)      322 2023-05-27 04:10:59.000000 pogt-1.0.1/pogt.egg-info/PKG-INFO
+-rw-r--r--   0 pc         (501) staff       (20)      142 2023-05-27 04:10:59.000000 pogt-1.0.1/pogt.egg-info/SOURCES.txt
+-rw-r--r--   0 pc         (501) staff       (20)        1 2023-05-27 04:10:59.000000 pogt-1.0.1/pogt.egg-info/dependency_links.txt
+-rw-r--r--   0 pc         (501) staff       (20)      255 2023-05-27 04:10:36.000000 pogt-1.0.1/pogt.egg-info/main.py
+-rw-r--r--   0 pc         (501) staff       (20)        1 2023-05-27 04:10:59.000000 pogt-1.0.1/pogt.egg-info/top_level.txt
+-rw-r--r--   0 pc         (501) staff       (20)       38 2023-05-27 04:10:59.032609 pogt-1.0.1/setup.cfg
+-rw-r--r--   0 pc         (501) staff       (20)      449 2023-05-27 04:10:36.000000 pogt-1.0.1/setup.py
```

