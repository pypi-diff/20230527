# Comparing `tmp/replicator-cli-0.0.4.tar.gz` & `tmp/replicator-cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicator-cli-0.0.4.tar", last modified: Sat May 27 13:19:03 2023, max compression
+gzip compressed data, was "replicator-cli-0.0.5.tar", last modified: Sat May 27 13:44:36 2023, max compression
```

## Comparing `replicator-cli-0.0.4.tar` & `replicator-cli-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:19:03.585169 replicator-cli-0.0.4/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:19:03.585169 replicator-cli-0.0.4/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2005 2023-05-27 10:31:08.000000 replicator-cli-0.0.4/README.md
--rwxrwxrwx   0 vitonsky  (1000) vitonsky  (1000)     2766 2023-05-27 13:19:01.000000 replicator-cli-0.0.4/app.py
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:19:03.585169 replicator-cli-0.0.4/replicator_cli.egg-info/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      255 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       58 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/entry_points.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/requires.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       15 2023-05-27 13:19:03.000000 replicator-cli-0.0.4/replicator_cli.egg-info/top_level.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:19:03.585169 replicator-cli-0.0.4/setup.cfg
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      936 2023-05-27 13:10:13.000000 replicator-cli-0.0.4/setup.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:44:36.306747 replicator-cli-0.0.5/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:44:36.306747 replicator-cli-0.0.5/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2005 2023-05-27 10:31:08.000000 replicator-cli-0.0.5/README.md
+-rwxrwxrwx   0 vitonsky  (1000) vitonsky  (1000)     2772 2023-05-27 13:30:42.000000 replicator-cli-0.0.5/app.py
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       17 2023-05-27 13:42:14.000000 replicator-cli-0.0.5/meta.py
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      671 2023-05-27 13:01:13.000000 replicator-cli-0.0.5/notifier.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:44:36.306747 replicator-cli-0.0.5/replicator_cli.egg-info/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      275 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       58 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/requires.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       18 2023-05-27 13:44:36.000000 replicator-cli-0.0.5/replicator_cli.egg-info/top_level.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:44:36.306747 replicator-cli-0.0.5/setup.cfg
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      974 2023-05-27 13:37:07.000000 replicator-cli-0.0.5/setup.py
```

### Comparing `replicator-cli-0.0.4/PKG-INFO` & `replicator-cli-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicator-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: Task runner for backups
 Home-page: https://github.com/vitonsky/replicator
 Author: Robert Vitonsky
 Author-email: rob@vitonsky.net
 License: MIT
 Description: Replicator is a task runner for backups.
```

### Comparing `replicator-cli-0.0.4/README.md` & `replicator-cli-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `replicator-cli-0.0.4/app.py` & `replicator-cli-0.0.5/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
 import sys, subprocess
 import asyncio
 import yaml
 
 from notifier import TelegramNotifier
-
-version = '0.0.4'
+from meta import version
 
 reportLinesLimit = 20
 
 # TODO: create log file for each execution
 async def main():
     parser = argparse.ArgumentParser(
         description='Util to replicate backups from primary storage to a mirrors',
```

### Comparing `replicator-cli-0.0.4/replicator_cli.egg-info/PKG-INFO` & `replicator-cli-0.0.5/replicator_cli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicator-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: Task runner for backups
 Home-page: https://github.com/vitonsky/replicator
 Author: Robert Vitonsky
 Author-email: rob@vitonsky.net
 License: MIT
 Description: Replicator is a task runner for backups.
```

