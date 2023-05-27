# Comparing `tmp/cq23-1.3.0.tar.gz` & `tmp/cq23-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-1.3.0.tar", last modified: Fri May 26 07:31:31 2023, max compression
+gzip compressed data, was "cq23-1.4.0.tar", last modified: Sat May 27 04:34:11 2023, max compression
```

## Comparing `cq23-1.3.0.tar` & `cq23-1.4.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:31.601729 cq23-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-26 07:31:31.601729 cq23-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 07:31:20.000000 cq23-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 07:31:20.000000 cq23-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-26 07:31:31.601729 cq23-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:31.593729 cq23-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:31.593729 cq23-1.3.0/src/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:20.000000 cq23-1.3.0/src/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-26 07:31:20.000000 cq23-1.3.0/src/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:31.593729 cq23-1.3.0/src/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:20.000000 cq23-1.3.0/src/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-26 07:31:20.000000 cq23-1.3.0/src/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:31.597729 cq23-1.3.0/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-26 07:31:31.000000 cq23-1.3.0/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-26 07:31:31.000000 cq23-1.3.0/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:31:31.000000 cq23-1.3.0/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 07:31:31.000000 cq23-1.3.0/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 07:31:31.000000 cq23-1.3.0/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 07:31:31.000000 cq23-1.3.0/src/cq23.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:31.597729 cq23-1.3.0/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:20.000000 cq23-1.3.0/src/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-26 07:31:20.000000 cq23-1.3.0/src/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-26 07:31:20.000000 cq23-1.3.0/src/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:31.597729 cq23-1.3.0/src/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:20.000000 cq23-1.3.0/src/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-26 07:31:20.000000 cq23-1.3.0/src/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-26 07:31:20.000000 cq23-1.3.0/src/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-26 07:31:20.000000 cq23-1.3.0/src/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:31.597729 cq23-1.3.0/src/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:31:20.000000 cq23-1.3.0/src/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-26 07:31:20.000000 cq23-1.3.0/src/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.879390 cq23-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-27 04:34:11.879390 cq23-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-27 04:34:03.000000 cq23-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-27 04:34:03.000000 cq23-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-27 04:34:11.879390 cq23-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-27 04:34:03.000000 cq23-1.4.0/src/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-27 04:34:03.000000 cq23-1.4.0/src/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-27 04:34:11.000000 cq23-1.4.0/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-27 04:34:03.000000 cq23-1.4.0/src/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-27 04:34:03.000000 cq23-1.4.0/src/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.875390 cq23-1.4.0/src/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-27 04:34:03.000000 cq23-1.4.0/src/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.879390 cq23-1.4.0/src/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-27 04:34:03.000000 cq23-1.4.0/src/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-27 04:34:03.000000 cq23-1.4.0/src/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-27 04:34:03.000000 cq23-1.4.0/src/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:11.879390 cq23-1.4.0/src/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 04:34:03.000000 cq23-1.4.0/src/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-27 04:34:03.000000 cq23-1.4.0/src/zip/command.py
```

### Comparing `cq23-1.3.0/PKG-INFO` & `cq23-1.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.3.0
+Version: 1.4.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
@@ -14,7 +14,15 @@
 Description-Content-Type: text/markdown
 
 # CLI Utilities for CodeQuest 23
 
 ```shell
 pip install cq23
 ```
+
+```shell
+cq23 run
+cq23 run map=<map name>
+cq23 zip
+cq23 check
+cq23 cleanup
+```
```

### Comparing `cq23-1.3.0/setup.cfg` & `cq23-1.4.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 1.3.0
+version = 1.4.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-1.3.0/src/check/command.py` & `cq23-1.4.0/src/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.3.0/src/cleanup/command.py` & `cq23-1.4.0/src/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.3.0/src/cq23.egg-info/PKG-INFO` & `cq23-1.4.0/src/cq23.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 1.3.0
+Version: 1.4.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
@@ -14,7 +14,15 @@
 Description-Content-Type: text/markdown
 
 # CLI Utilities for CodeQuest 23
 
 ```shell
 pip install cq23
 ```
+
+```shell
+cq23 run
+cq23 run map=<map name>
+cq23 zip
+cq23 check
+cq23 cleanup
+```
```

### Comparing `cq23-1.3.0/src/cq23.egg-info/SOURCES.txt` & `cq23-1.4.0/src/cq23.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -10,13 +10,15 @@
 src/cq23.egg-info/dependency_links.txt
 src/cq23.egg-info/entry_points.txt
 src/cq23.egg-info/requires.txt
 src/cq23.egg-info/top_level.txt
 src/main/__init__.py
 src/main/command.py
 src/main/utils.py
+src/new_client/__init__.py
+src/new_client/command.py
 src/run_game/__init__.py
 src/run_game/command.py
 src/run_game/docker_tools.py
 src/run_game/gcs.py
 src/zip/__init__.py
 src/zip/command.py
```

### Comparing `cq23-1.3.0/src/main/command.py` & `cq23-1.4.0/src/main/command.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import sys
 
 from check.command import check
 from cleanup.command import cleanup
+from new_client.command import new_client
 from run_game.command import run_game
 from zip.command import zip
 
 from .utils import restore_cwd
 
 
 def help_message():
     message = (
         "Available commands:\n\n"
+        + "> cq23 new python my_bot\n"
         + "> cq23 run\n"
         + "> cq23 run map=<map name>\n"
         + "> cq23 zip\n"
         + "> cq23 check\n"
         + "> cq23 cleanup\n\n"
         + "If you need help with the competition, post a message in Discord or email us at info@codequest.club."
     )
@@ -22,14 +24,15 @@
 
 
 @restore_cwd
 def route_command():
     command_args = sys.argv[1:]
 
     first_arg_mapping = {
+        "new": new_client,
         "run": run_game,
         "cleanup": cleanup,
         "zip": zip,
         "check": check,
     }
 
     if not command_args or command_args[0].lower() not in first_arg_mapping.keys():
```

### Comparing `cq23-1.3.0/src/run_game/command.py` & `cq23-1.4.0/src/run_game/command.py`

 * *Files identical despite different names*

### Comparing `cq23-1.3.0/src/run_game/docker_tools.py` & `cq23-1.4.0/src/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-1.3.0/src/run_game/gcs.py` & `cq23-1.4.0/src/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-1.3.0/src/zip/command.py` & `cq23-1.4.0/src/zip/command.py`

 * *Files identical despite different names*

