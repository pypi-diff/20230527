# Comparing `tmp/ducktables-0.1.1.tar.gz` & `tmp/ducktables-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ducktables-0.1.1.tar", last modified: Fri May 19 19:37:24 2023, max compression
+gzip compressed data, was "ducktables-0.1.2.tar", last modified: Fri May 26 22:17:44 2023, max compression
```

## Comparing `ducktables-0.1.1.tar` & `ducktables-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,18 @@
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-19 19:37:24.321740 ducktables-0.1.1/
--rw-rw-r--   0 mark      (4000) mark      (4000)      210 2023-05-19 19:37:24.321740 ducktables-0.1.1/PKG-INFO
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-19 19:37:24.321740 ducktables-0.1.1/ducktables.egg-info/
--rw-rw-r--   0 mark      (4000) mark      (4000)      210 2023-05-19 19:37:24.000000 ducktables-0.1.1/ducktables.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (4000) mark      (4000)      177 2023-05-19 19:37:24.000000 ducktables-0.1.1/ducktables.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)        1 2023-05-19 19:37:24.000000 ducktables-0.1.1/ducktables.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)      267 2023-05-19 19:37:24.000000 ducktables-0.1.1/ducktables.egg-info/requires.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)        1 2023-05-19 19:37:24.000000 ducktables-0.1.1/ducktables.egg-info/top_level.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)       38 2023-05-19 19:37:24.321740 ducktables-0.1.1/setup.cfg
--rw-rw-r--   0 mark      (4000) mark      (4000)      252 2023-05-19 19:35:38.000000 ducktables-0.1.1/setup.py
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-26 22:17:44.984170 ducktables-0.1.2/
+-rw-rw-r--   0 mark      (4000) mark      (4000)      210 2023-05-26 22:17:44.984170 ducktables-0.1.2/PKG-INFO
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-26 22:17:44.984170 ducktables-0.1.2/ducktables/
+-rw-rw-r--   0 mark      (4000) mark      (4000)        3 2023-05-26 22:15:50.000000 ducktables-0.1.2/ducktables/__init__.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)     3922 2023-05-19 16:52:49.000000 ducktables-0.1.2/ducktables/aws.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)      358 2023-05-23 17:02:10.000000 ducktables-0.1.2/ducktables/github.py
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-26 22:17:44.984170 ducktables-0.1.2/ducktables/google/
+-rw-rw-r--   0 mark      (4000) mark      (4000)     3918 2023-05-19 19:34:59.000000 ducktables-0.1.2/ducktables/google/__init__.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)     3479 2023-05-19 19:34:59.000000 ducktables-0.1.2/ducktables/google/analytics.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)     1039 2023-05-19 16:52:49.000000 ducktables-0.1.2/ducktables/openai.py
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-26 22:17:44.984170 ducktables-0.1.2/ducktables.egg-info/
+-rw-rw-r--   0 mark      (4000) mark      (4000)      210 2023-05-26 22:17:44.000000 ducktables-0.1.2/ducktables.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (4000) mark      (4000)      321 2023-05-26 22:17:44.000000 ducktables-0.1.2/ducktables.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)        1 2023-05-26 22:17:44.000000 ducktables-0.1.2/ducktables.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)      267 2023-05-26 22:17:44.000000 ducktables-0.1.2/ducktables.egg-info/requires.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)       11 2023-05-26 22:17:44.000000 ducktables-0.1.2/ducktables.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)       38 2023-05-26 22:17:44.984170 ducktables-0.1.2/setup.cfg
+-rw-rw-r--   0 mark      (4000) mark      (4000)      252 2023-05-26 22:16:08.000000 ducktables-0.1.2/setup.py
```

