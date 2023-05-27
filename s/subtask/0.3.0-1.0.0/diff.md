# Comparing `tmp/Subtask-0.3.0.tar.gz` & `tmp/subtask-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subtask-0.3.0.tar", last modified: Thu Mar  9 14:25:47 2023, max compression
+gzip compressed data, was "subtask-1.0.0.tar", max compression
```

## Comparing `Subtask-0.3.0.tar` & `subtask-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:25:47.575073 Subtask-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-09 14:25:30.000000 Subtask-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-09 14:25:30.000000 Subtask-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-09 14:25:47.575073 Subtask-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-09 14:25:30.000000 Subtask-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:25:47.571073 Subtask-0.3.0/Subtask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-09 14:25:47.000000 Subtask-0.3.0/Subtask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-09 14:25:47.000000 Subtask-0.3.0/Subtask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 14:25:47.000000 Subtask-0.3.0/Subtask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-09 14:25:47.000000 Subtask-0.3.0/Subtask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-09 14:25:30.000000 Subtask-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-09 14:25:47.575073 Subtask-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:25:47.571073 Subtask-0.3.0/subtask/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-09 14:25:30.000000 Subtask-0.3.0/subtask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-03-09 14:25:30.000000 Subtask-0.3.0/subtask/__subtask.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 14:25:30.000000 Subtask-0.3.0/subtask/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:25:47.575073 Subtask-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-09 14:25:30.000000 Subtask-0.3.0/tests/test_subtask.py
+-rw-r--r--   0        0        0     1073 2023-05-27 11:47:52.018372 subtask-1.0.0/LICENSE
+-rw-r--r--   0        0        0      576 2023-05-27 11:47:52.018372 subtask-1.0.0/README.md
+-rw-r--r--   0        0        0     1302 2023-05-27 11:47:52.018372 subtask-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      200 2023-05-27 11:47:52.018372 subtask-1.0.0/subtask/__init__.py
+-rw-r--r--   0        0        0     4842 2023-05-27 11:47:52.018372 subtask-1.0.0/subtask/__subtask.py
+-rw-r--r--   0        0        0        0 2023-05-27 11:47:52.018372 subtask-1.0.0/subtask/py.typed
+-rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 subtask-1.0.0/PKG-INFO
```

### Comparing `Subtask-0.3.0/LICENSE` & `subtask-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Subtask-0.3.0/PKG-INFO` & `subtask-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
-Name: Subtask
-Version: 0.3.0
-Summary: "A simple wrapper around `subprocess.Popen` to reduce the painfulness of running multiple processes concurrently."
-Home-page: https://github.com/MiguelGuthridge/Subtask
+Name: subtask
+Version: 1.0.0
+Summary: A simple wrapper around `subprocess.Popen` to reduce the painfulness of running multiple processes concurrently.
+Home-page: https://github.com/MiguelGuthridge/subtask
+License: MIT
+Keywords: popen,task,process,subprocess,subtask
 Author: Miguel Guthridge
 Author-email: hdsq@outlook.com.au
-Project-URL: Online Documentation, https://github.com/MiguelGuthridge/Subtask
-Project-URL: Bug Tracker, https://github.com/MiguelGuthridge/Subtask/issues
-Keywords: subprocess
-Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Other Environment
-Classifier: Framework :: Pytest
-Requires-Python: >=3.9.1
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
+Project-URL: Bug Tracker, https://github.com/MiguelGuthridge/subtask/issues
+Project-URL: Documentation, https://github.com/MiguelGuthridge/subtask
+Project-URL: Online Documentation, https://github.com/MiguelGuthridge/subtask
+Project-URL: Repository, https://github.com/MiguelGuthridge/subtask
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Subtask
 
 A simple wrapper around `subprocess.Popen` to reduce the painfulness of running
 multiple processes concurrently.
 
 ```py
@@ -35,7 +40,8 @@
 Subtask makes it easy to keep track of many concurrent subprocesses. It makes
 it much easier to capture outputs and give inputs to these processes.
 
 ## What is Subtask not for?
 
 Subtask is designed for simplicity. It should not be used if you want high
 performance, or to chain outputs for many files together.
+
```

### Comparing `Subtask-0.3.0/README.md` & `subtask-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `Subtask-0.3.0/subtask/__subtask.py` & `subtask-1.0.0/subtask/__subtask.py`

 * *Files identical despite different names*

