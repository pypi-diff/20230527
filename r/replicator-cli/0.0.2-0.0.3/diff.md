# Comparing `tmp/replicator-cli-0.0.2.tar.gz` & `tmp/replicator-cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicator-cli-0.0.2.tar", last modified: Sat May 27 10:39:35 2023, max compression
+gzip compressed data, was "replicator-cli-0.0.3.tar", last modified: Sat May 27 13:05:05 2023, max compression
```

## Comparing `replicator-cli-0.0.2.tar` & `replicator-cli-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 10:39:35.451398 replicator-cli-0.0.2/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 10:39:35.451398 replicator-cli-0.0.2/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2005 2023-05-27 10:31:08.000000 replicator-cli-0.0.2/README.md
--rwxrwxrwx   0 vitonsky  (1000) vitonsky  (1000)     2879 2023-05-27 09:41:41.000000 replicator-cli-0.0.2/app.py
-drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 10:39:35.451398 replicator-cli-0.0.2/replicator_cli.egg-info/
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/PKG-INFO
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      255 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       58 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/entry_points.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/requires.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       15 2023-05-27 10:39:35.000000 replicator-cli-0.0.2/replicator_cli.egg-info/top_level.txt
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 10:39:35.451398 replicator-cli-0.0.2/setup.cfg
--rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      912 2023-05-27 10:39:33.000000 replicator-cli-0.0.2/setup.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:05:05.444111 replicator-cli-0.0.3/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:05:05.440111 replicator-cli-0.0.3/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2005 2023-05-27 10:31:08.000000 replicator-cli-0.0.3/README.md
+-rwxrwxrwx   0 vitonsky  (1000) vitonsky  (1000)     2649 2023-05-27 13:01:13.000000 replicator-cli-0.0.3/app.py
+drwxrwxr-x   0 vitonsky  (1000) vitonsky  (1000)        0 2023-05-27 13:05:05.440111 replicator-cli-0.0.3/replicator_cli.egg-info/
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)     2982 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      255 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)        1 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       58 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/requires.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       15 2023-05-27 13:05:05.000000 replicator-cli-0.0.3/replicator_cli.egg-info/top_level.txt
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)       38 2023-05-27 13:05:05.444111 replicator-cli-0.0.3/setup.cfg
+-rw-rw-r--   0 vitonsky  (1000) vitonsky  (1000)      912 2023-05-27 13:00:39.000000 replicator-cli-0.0.3/setup.py
```

### Comparing `replicator-cli-0.0.2/PKG-INFO` & `replicator-cli-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicator-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Task runner for backups
 Home-page: https://github.com/vitonsky/replicator
 Author: Robert Vitonsky
 Author-email: rob@vitonsky.net
 License: MIT
 Description: Replicator is a task runner for backups.
```

### Comparing `replicator-cli-0.0.2/README.md` & `replicator-cli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `replicator-cli-0.0.2/app.py` & `replicator-cli-0.0.3/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import argparse
 import sys, subprocess
 import asyncio
-import telegram
 import yaml
 
+from notifier import TelegramNotifier
+
 reportLinesLimit = 20
 
 # TODO: create log file for each execution
 async def main():
     parser = argparse.ArgumentParser(
         description='Util to replicate backups from primary storage to a mirrors')
 
     parser.add_argument('config', help="Path to config file")
 
     args = parser.parse_args()
 
     config = yaml.load(open(args.config), Loader=yaml.Loader)
 
-    # Configure bot
-    bot = None
+    # Configure notifier
+    notifier = None
     if ('notifications' in config):
-        bot = telegram.Bot(config['notifications']['telegram']['botToken'])
-        async with bot:
-            print(await bot.get_me())
+        token = config['notifications']['telegram']['botToken']
+        users = config['notifications']['telegram']['userIds']
+
+        notifier = TelegramNotifier(token, users)
 
+    # Run tasks
     for task in config['tasks']:
         taskName = task['name'] if 'name' in task else task['run']
 
         print(f'Run command "{taskName}"', flush=True)
 
         # Run command
         # TODO: add timeout to stop process
@@ -52,28 +55,25 @@
             outLines.append(line)
         replicationProcess.stdout.close()
         replicationProcess.wait()
 
         isRunSuccessful = replicationProcess.returncode == 0
 
         # Notify result
-        if bot is not None:
+        if notifier is not None:
             notifications = config['notifications']
-            isNotificationsEnabled = 'enabled' in notifications and notifications['enabled'] == True
             notificationPrefix = '*' + notifications['prefix'] + '*: ' if 'prefix' in notifications else ''
 
-            if isNotificationsEnabled:
-                async with bot:
-                    for userId in config['notifications']['telegram']['userIds']:
-                        if isRunSuccessful:
-                            await bot.send_message(text=notificationPrefix + f'Task "{taskName}" final successful', chat_id=userId, parse_mode='MarkdownV2')
-                        else:
-                            # add last few lines to explain context
-                            lastLog= ''.join(outLines)
-                            await bot.send_message(text=notificationPrefix + f'⚠️ Task "{taskName}" are failed\n\n```\n...\n{lastLog}\n```', chat_id=userId, parse_mode='MarkdownV2')
+            escapedTaskName = notifier.escapeText(taskName)
+            if isRunSuccessful:
+                await notifier.notify(notificationPrefix + f'Task "{escapedTaskName}" final successful')
+            else:
+                # add last few lines to explain context
+                lastLog = notifier.escapeText(''.join(outLines))
+                await notifier.notify(notificationPrefix + f'⚠️ Task "{escapedTaskName}" are failed\n\n```\n...\n{lastLog}\n```')
 
         # Stop the program for fails
         if not isRunSuccessful:
             exit(replicationProcess.returncode)
 
 
 def cli():
```

### Comparing `replicator-cli-0.0.2/replicator_cli.egg-info/PKG-INFO` & `replicator-cli-0.0.3/replicator_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicator-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Task runner for backups
 Home-page: https://github.com/vitonsky/replicator
 Author: Robert Vitonsky
 Author-email: rob@vitonsky.net
 License: MIT
 Description: Replicator is a task runner for backups.
```

### Comparing `replicator-cli-0.0.2/setup.py` & `replicator-cli-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
     
 setup(
     name = 'replicator-cli',
-    version = '0.0.2',
+    version = '0.0.3',
     author = 'Robert Vitonsky',
     author_email = 'rob@vitonsky.net',
     license = 'MIT',
     description = 'Task runner for backups',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/vitonsky/replicator',
```

