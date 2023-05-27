# Comparing `tmp/replicator-cli-0.0.1.tar.gz` & `tmp/replicator-cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicator-cli-0.0.1.tar", last modified: Sat May 27 10:29:28 2023, max compression
+gzip compressed data, was "replicator-cli-0.0.2.tar", last modified: Sat May 27 10:39:35 2023, max compression
```

## Comparing `replicator-cli-0.0.1.tar` & `replicator-cli-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 10:29:28.848762 replicator-cli-0.0.1/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2901 2023-05-27 10:29:28.848762 replicator-cli-0.0.1/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     1948 2023-05-27 10:00:30.000000 replicator-cli-0.0.1/README.md
--rwxrwxrwx   0 vitonsky  (1000) vitonsky  (1000)     2879 2023-05-27 09:41:41.000000 replicator-cli-0.0.1/app.py
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 10:29:28.848762 replicator-cli-0.0.1/replicator_cli.egg-info/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2901 2023-05-27 10:29:28.000000 replicator-cli-0.0.1/replicator_cli.egg-info/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      255 2023-05-27 10:29:28.000000 replicator-cli-0.0.1/replicator_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-05-27 10:29:28.000000 replicator-cli-0.0.1/replicator_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       58 2023-05-27 10:29:28.000000 replicator-cli-0.0.1/replicator_cli.egg-info/entry_points.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 10:29:28.000000 replicator-cli-0.0.1/replicator_cli.egg-info/requires.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       15 2023-05-27 10:29:28.000000 replicator-cli-0.0.1/replicator_cli.egg-info/top_level.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 10:29:28.848762 replicator-cli-0.0.1/setup.cfg
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      912 2023-05-27 10:28:45.000000 replicator-cli-0.0.1/setup.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 10:39:35.451398 replicator-cli-0.0.2/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 10:39:35.451398 replicator-cli-0.0.2/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2005 2023-05-27 10:31:08.000000 replicator-cli-0.0.2/README.md
+-rwxrwxrwx   0 vitonsky  (1000) vitonsky  (1000)     2879 2023-05-27 09:41:41.000000 replicator-cli-0.0.2/app.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 10:39:35.451398 replicator-cli-0.0.2/replicator_cli.egg-info/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      255 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       58 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/requires.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       15 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/top_level.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 10:39:35.451398 replicator-cli-0.0.2/setup.cfg
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      912 2023-05-27 10:39:33.000000 replicator-cli-0.0.2/setup.py
```

### Comparing `replicator-cli-0.0.1/PKG-INFO` & `replicator-cli-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: replicator-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Task runner for backups
 Home-page: https://github.com/vitonsky/replicator
 Author: Robert Vitonsky
 Author-email: rob@vitonsky.net
 License: MIT
 Description: Replicator is a task runner for backups.
         
         You can describe your tasks declarative with YAML file and run task files with CRON.
         
         Replicator supports notifications, it's useful for tasks that take a lot of time.
         
         ## Install
         
+        Install from pip `pip install replicator-cli`
+        
+        Or build:
         - Clone repository `git clone https://github.com/vitonsky/replicator.git`
         - Build package with run `make build`
         - Install package `pip install dist/replicator-0.0.1-py3-none-any.whl`
         
         ## Usage
         
         ```
```

### Comparing `replicator-cli-0.0.1/README.md` & `replicator-cli-0.0.2/replicator_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,86 @@
-Replicator is a task runner for backups.
-
-You can describe your tasks declarative with YAML file and run task files with CRON.
-
-Replicator supports notifications, it's useful for tasks that take a lot of time.
-
-## Install
-
-- Clone repository `git clone https://github.com/vitonsky/replicator.git`
-- Build package with run `make build`
-- Install package `pip install dist/replicator-0.0.1-py3-none-any.whl`
-
-## Usage
-
-```
-usage: replicator [-h] config
-
-Util to replicate backups from primary storage to a mirrors
-
-positional arguments:
-  config      Path to config file
-
-optional arguments:
-  -h, --help  show this help message and exit
-```
-
-To use util, first create task file.
-
-Example task file for a local device
-```yml
-tasks:
-    # Task may have name
-    - name: 'Copy files to backup disk'
-      run: rclone ./backups /path/to/local/mirror1
-
-    - name: 'Upload to S3'
-      run: rclone ./backups s3Replica:backups
-
-    - name: 'Replicate on server'
-      # Just run replicator on server with their own config and end locally
-      run: ssh replicator@backup-server 'nohup replicator ./backups.yml > ./replicator.log 2>&1 </dev/null &'
-```
-
-Example task file for backup server
-```yml
-# Notifications config
-notifications:
-    telegram:
-        # Define should notifications been sent
-        enabled: true
-        # Token for bot who will sent notifications
-        # How to: https://core.telegram.org/bots/tutorial#getting-ready
-        botToken: '123:token'
-        # User IDs to receive notifications
-        userIds:
-            - 123456
-
-# Replicate backup from main storage
-tasks:
-    - run: rclone s3Replica:backups s3Mirror1:backups
-    - run: rclone s3Replica:backups s3Mirror2:backups
-    - run: rclone s3Replica:backups s3Mirror3:backups
-```
-
-## TODO
-- [x] Support few entries for replication
-- [x] Provide commands to run, instead of paths
-- [x] Provide instructions to install as binary
-- [ ] Split the code
-- [ ] Add docker image
+Metadata-Version: 2.1
+Name: replicator-cli
+Version: 0.0.2
+Summary: Task runner for backups
+Home-page: https://github.com/vitonsky/replicator
+Author: Robert Vitonsky
+Author-email: rob@vitonsky.net
+License: MIT
+Description: Replicator is a task runner for backups.
+        
+        You can describe your tasks declarative with YAML file and run task files with CRON.
+        
+        Replicator supports notifications, it's useful for tasks that take a lot of time.
+        
+        ## Install
+        
+        Install from pip `pip install replicator-cli`
+        
+        Or build:
+        - Clone repository `git clone https://github.com/vitonsky/replicator.git`
+        - Build package with run `make build`
+        - Install package `pip install dist/replicator-0.0.1-py3-none-any.whl`
+        
+        ## Usage
+        
+        ```
+        usage: replicator [-h] config
+        
+        Util to replicate backups from primary storage to a mirrors
+        
+        positional arguments:
+          config      Path to config file
+        
+        optional arguments:
+          -h, --help  show this help message and exit
+        ```
+        
+        To use util, first create task file.
+        
+        Example task file for a local device
+        ```yml
+        tasks:
+            # Task may have name
+            - name: 'Copy files to backup disk'
+              run: rclone ./backups /path/to/local/mirror1
+        
+            - name: 'Upload to S3'
+              run: rclone ./backups s3Replica:backups
+        
+            - name: 'Replicate on server'
+              # Just run replicator on server with their own config and end locally
+              run: ssh replicator@backup-server 'nohup replicator ./backups.yml > ./replicator.log 2>&1 </dev/null &'
+        ```
+        
+        Example task file for backup server
+        ```yml
+        # Notifications config
+        notifications:
+            telegram:
+                # Define should notifications been sent
+                enabled: true
+                # Token for bot who will sent notifications
+                # How to: https://core.telegram.org/bots/tutorial#getting-ready
+                botToken: '123:token'
+                # User IDs to receive notifications
+                userIds:
+                    - 123456
+        
+        # Replicate backup from main storage
+        tasks:
+            - run: rclone s3Replica:backups s3Mirror1:backups
+            - run: rclone s3Replica:backups s3Mirror2:backups
+            - run: rclone s3Replica:backups s3Mirror3:backups
+        ```
+        
+        ## TODO
+        - [x] Support few entries for replication
+        - [x] Provide commands to run, instead of paths
+        - [x] Provide instructions to install as binary
+        - [ ] Split the code
+        - [ ] Add docker image
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
```

### Comparing `replicator-cli-0.0.1/app.py` & `replicator-cli-0.0.2/app.py`

 * *Files identical despite different names*

### Comparing `replicator-cli-0.0.1/setup.py` & `replicator-cli-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
     
 setup(
     name = 'replicator-cli',
-    version = '0.0.1',
+    version = '0.0.2',
     author = 'Robert Vitonsky',
     author_email = 'rob@vitonsky.net',
     license = 'MIT',
     description = 'Task runner for backups',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/vitonsky/replicator',
```

