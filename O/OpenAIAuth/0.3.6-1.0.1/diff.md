# Comparing `tmp/OpenAIAuth-0.3.6.tar.gz` & `tmp/OpenAIAuth-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenAIAuth-0.3.6.tar", last modified: Fri Mar 31 11:50:15 2023, max compression
+gzip compressed data, was "OpenAIAuth-1.0.1.tar", last modified: Sat May 27 02:10:56 2023, max compression
```

## Comparing `OpenAIAuth-0.3.6.tar` & `OpenAIAuth-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:50:15.504293 OpenAIAuth-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-31 11:49:47.000000 OpenAIAuth-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-31 11:50:15.504293 OpenAIAuth-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-31 11:49:47.000000 OpenAIAuth-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 11:50:15.504293 OpenAIAuth-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-31 11:49:47.000000 OpenAIAuth-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:50:15.500293 OpenAIAuth-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:50:15.504293 OpenAIAuth-0.3.6/src/OpenAIAuth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-31 11:50:15.000000 OpenAIAuth-0.3.6/src/OpenAIAuth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-31 11:50:15.000000 OpenAIAuth-0.3.6/src/OpenAIAuth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:50:15.000000 OpenAIAuth-0.3.6/src/OpenAIAuth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 11:50:15.000000 OpenAIAuth-0.3.6/src/OpenAIAuth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-31 11:50:15.000000 OpenAIAuth-0.3.6/src/OpenAIAuth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-03-31 11:49:47.000000 OpenAIAuth-0.3.6/src/OpenAIAuth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:10:56.641596 OpenAIAuth-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-27 02:10:31.000000 OpenAIAuth-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-27 02:10:56.641596 OpenAIAuth-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-27 02:10:31.000000 OpenAIAuth-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:10:56.641596 OpenAIAuth-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-27 02:10:31.000000 OpenAIAuth-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:10:56.641596 OpenAIAuth-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:10:56.641596 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-27 02:10:56.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-27 02:10:56.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:10:56.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 02:10:56.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 02:10:56.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-05-27 02:10:31.000000 OpenAIAuth-1.0.1/src/OpenAIAuth.py
```

### Comparing `OpenAIAuth-0.3.6/LICENSE` & `OpenAIAuth-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenAIAuth-0.3.6/setup.py` & `OpenAIAuth-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="OpenAIAuth",
-    version="0.3.6",
+    version="1.0.1",
     license="MIT",
-    author="Rawand Ahmed Shaswar and Antonio Cheong",
+    author="pengzhile",
     author_email="acheong@student.dalat.org",
     description="OpenAI Authentication Reverse Engineered",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=["OpenAIAuth"],
     url="https://github.com/acheong08/OpenAIAuth",
     project_urls={"Bug Report": "https://github.com/acheong08/OpenAIAuth/issues/new"},
```

