# Comparing `tmp/vessel-3.3.0.tar.gz` & `tmp/vessel-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vessel-3.3.0.tar", last modified: Tue May  4 09:56:42 2021, max compression
+gzip compressed data, was "vessel-4.0.0.tar", last modified: Sat May 27 16:07:55 2023, max compression
```

## Comparing `vessel-3.3.0.tar` & `vessel-4.0.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 09:56:42.635381 vessel-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-05-04 09:56:42.635381 vessel-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      336 2021-05-04 09:56:32.000000 vessel-3.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-04 09:56:42.635381 vessel-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      493 2021-05-04 09:56:32.000000 vessel-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 09:56:42.635381 vessel-3.3.0/vessel/
--rw-r--r--   0 runner    (1001) docker     (121)     8678 2021-05-04 09:56:32.000000 vessel-3.3.0/vessel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5882 2021-05-04 09:56:32.000000 vessel-3.3.0/vessel/_builds.py
--rw-r--r--   0 runner    (1001) docker     (121)     1585 2021-05-04 09:56:32.000000 vessel-3.3.0/vessel/_modifies.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2021-05-04 09:56:32.000000 vessel-3.3.0/vessel/_share.py
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2021-05-04 09:56:32.000000 vessel-3.3.0/vessel/_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 09:56:42.635381 vessel-3.3.0/vessel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-05-04 09:56:42.000000 vessel-3.3.0/vessel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-05-04 09:56:42.000000 vessel-3.3.0/vessel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 09:56:42.000000 vessel-3.3.0/vessel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-05-04 09:56:42.000000 vessel-3.3.0/vessel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-05-04 09:56:42.000000 vessel-3.3.0/vessel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:07:55.548474 vessel-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 16:07:55.548474 vessel-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-27 16:07:42.000000 vessel-4.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 16:07:55.548474 vessel-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-27 16:07:42.000000 vessel-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:07:55.548474 vessel-4.0.0/vessel/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-27 16:07:42.000000 vessel-4.0.0/vessel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-27 16:07:42.000000 vessel-4.0.0/vessel/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16924 2023-05-27 16:07:42.000000 vessel-4.0.0/vessel/_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-27 16:07:42.000000 vessel-4.0.0/vessel/_manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 16:07:55.548474 vessel-4.0.0/vessel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 16:07:55.000000 vessel-4.0.0/vessel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-27 16:07:55.000000 vessel-4.0.0/vessel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 16:07:55.000000 vessel-4.0.0/vessel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-27 16:07:55.000000 vessel-4.0.0/vessel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 16:07:55.000000 vessel-4.0.0/vessel.egg-info/top_level.txt
```

