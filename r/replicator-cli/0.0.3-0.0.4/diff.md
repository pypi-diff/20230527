# Comparing `tmp/replicator-cli-0.0.3.tar.gz` & `tmp/replicator-cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicator-cli-0.0.3.tar", last modified: Sat May 27 13:05:05 2023, max compression
+gzip compressed data, was "replicator-cli-0.0.4.tar", last modified: Sat May 27 13:19:03 2023, max compression
```

## Comparing `replicator-cli-0.0.3.tar` & `replicator-cli-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:05:05.444111 replicator-cli-0.0.3/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:05:05.440111 replicator-cli-0.0.3/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2005 2023-05-27 10:31:08.000000 replicator-cli-0.0.3/README.md
--rwxrwxrwx   0 vitonsky  (1000) vitonsky  (1000)     2649 2023-05-27 13:01:13.000000 replicator-cli-0.0.3/app.py
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:05:05.440111 replicator-cli-0.0.3/replicator_cli.egg-info/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      255 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       58 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/entry_points.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/requires.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       15 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/top_level.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:05:05.444111 replicator-cli-0.0.3/setup.cfg
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      912 2023-05-27 13:00:39.000000 replicator-cli-0.0.3/setup.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:19:03.585169 replicator-cli-0.0.4/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:19:03.585169 replicator-cli-0.0.4/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2005 2023-05-27 10:31:08.000000 replicator-cli-0.0.4/README.md
+-rwxrwxrwx   0 vitonsky  (1000) vitonsky  (1000)     2766 2023-05-27 13:19:01.000000 replicator-cli-0.0.4/app.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:19:03.585169 replicator-cli-0.0.4/replicator_cli.egg-info/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      255 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       58 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/requires.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       15 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/top_level.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:19:03.585169 replicator-cli-0.0.4/setup.cfg
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      936 2023-05-27 13:10:13.000000 replicator-cli-0.0.4/setup.py
```

### Comparing `replicator-cli-0.0.3/PKG-INFO` & `replicator-cli-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicator-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: Task runner for backups
 Home-page: https://github.com/vitonsky/replicator
 Author: Robert Vitonsky
 Author-email: rob@vitonsky.net
 License: MIT
 Description: Replicator is a task runner for backups.
```

### Comparing `replicator-cli-0.0.3/README.md` & `replicator-cli-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `replicator-cli-0.0.3/app.py` & `replicator-cli-0.0.4/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import argparse
 import sys, subprocess
 import asyncio
 import yaml
 
 from notifier import TelegramNotifier
 
+version = '0.0.4'
+
 reportLinesLimit = 20
 
 # TODO: create log file for each execution
 async def main():
     parser = argparse.ArgumentParser(
-        description='Util to replicate backups from primary storage to a mirrors')
+        description='Util to replicate backups from primary storage to a mirrors',
+    )
+    parser.add_argument('--version', '-v', action='version', version='%(prog)s ' + version)
 
     parser.add_argument('config', help="Path to config file")
 
     args = parser.parse_args()
 
     config = yaml.load(open(args.config), Loader=yaml.Loader)
```

### Comparing `replicator-cli-0.0.3/replicator_cli.egg-info/PKG-INFO` & `replicator-cli-0.0.4/replicator_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicator-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: Task runner for backups
 Home-page: https://github.com/vitonsky/replicator
 Author: Robert Vitonsky
 Author-email: rob@vitonsky.net
 License: MIT
 Description: Replicator is a task runner for backups.
```

