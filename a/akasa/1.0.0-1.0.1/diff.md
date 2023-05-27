# Comparing `tmp/akasa-1.0.0.tar.gz` & `tmp/akasa-1.0.1.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akasa-1.0.0.tar", last modified: Sat May 27 20:22:02 2023, max compression
+gzip compressed data, was "akasa-1.0.1.linux-x86_64.tar", last modified: Sat May 27 20:23:52 2023, max compression
```

## Comparing `akasa-1.0.0.tar` & `akasa-1.0.1.linux-x86_64.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:22:02.401069 akasa-1.0.0/
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)    35149 2023-05-27 20:11:48.000000 akasa-1.0.0/LICENSE
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)     3730 2023-05-27 20:22:02.401069 akasa-1.0.0/PKG-INFO
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)     3497 2023-05-27 20:13:14.000000 akasa-1.0.0/README.md
-drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:22:02.397069 akasa-1.0.0/akasa/
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:09:48.000000 akasa-1.0.0/akasa/__init__.py
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:09:55.000000 akasa-1.0.0/akasa/module1.py
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:09:57.000000 akasa-1.0.0/akasa/module2.py
-drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:22:02.401069 akasa-1.0.0/akasa.egg-info/
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)     3730 2023-05-27 20:22:02.000000 akasa-1.0.0/akasa.egg-info/PKG-INFO
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)      194 2023-05-27 20:22:02.000000 akasa-1.0.0/akasa.egg-info/SOURCES.txt
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)        1 2023-05-27 20:22:02.000000 akasa-1.0.0/akasa.egg-info/dependency_links.txt
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)        6 2023-05-27 20:22:02.000000 akasa-1.0.0/akasa.egg-info/top_level.txt
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)       38 2023-05-27 20:22:02.401069 akasa-1.0.0/setup.cfg
--rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)      647 2023-05-27 20:19:59.000000 akasa-1.0.0/setup.py
+drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:23:52.697368 ./
+drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:23:52.697368 ./home/
+drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:23:52.697368 ./home/bijaydas/
+drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:23:52.697368 ./home/bijaydas/pyenvs/
+drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:23:52.697368 ./home/bijaydas/pyenvs/dev/
+drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:23:52.697368 ./home/bijaydas/pyenvs/dev/lib/
+drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:23:52.697368 ./home/bijaydas/pyenvs/dev/lib/python3.10/
+drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:23:52.769368 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/
+drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:23:52.697368 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa/
+-rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:09:48.000000 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa/__init__.py
+drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:23:52.701368 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa/__pycache__/
+-rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)      165 2023-05-27 20:23:52.697368 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)      164 2023-05-27 20:23:52.697368 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa/__pycache__/module1.cpython-310.pyc
+-rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)      164 2023-05-27 20:23:52.701368 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa/__pycache__/module2.cpython-310.pyc
+-rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:09:55.000000 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa/module1.py
+-rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:09:57.000000 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa/module2.py
+drwxrwxr-x   0 bijaydas  (1000) bijaydas  (1000)        0 2023-05-27 20:23:52.769368 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa-1.0.1-py3.10.egg-info/
+-rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)     3730 2023-05-27 20:23:52.733368 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa-1.0.1-py3.10.egg-info/PKG-INFO
+-rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)      194 2023-05-27 20:23:52.769368 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa-1.0.1-py3.10.egg-info/SOURCES.txt
+-rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)        1 2023-05-27 20:23:52.733368 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa-1.0.1-py3.10.egg-info/dependency_links.txt
+-rw-rw-r--   0 bijaydas  (1000) bijaydas  (1000)        6 2023-05-27 20:23:52.733368 ./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa-1.0.1-py3.10.egg-info/top_level.txt
```

### Comparing `akasa-1.0.0/PKG-INFO` & `./home/bijaydas/pyenvs/dev/lib/python3.10/site-packages/akasa-1.0.1-py3.10.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akasa
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is a cool package
 Author: Bijay Das
 Author-email: imbijaydas@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: akasa Version: 1.0.0 Summary: This is a cool
+Metadata-Version: 2.1 Name: akasa Version: 1.0.1 Summary: This is a cool
 package Author: Bijay Das Author-email: imbijaydas@gmail.com License: GNU
 GENERAL PUBLIC LICENSE Description-Content-Type: text/markdown License-File:
 LICENSE
   [https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/
           2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg]
       [Build_Status] [Total_Downloads] [Latest_Stable_Version] [License]
 ## About Laravel > **Note:** This repository contains the core code of the
```

