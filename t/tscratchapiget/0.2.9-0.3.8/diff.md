# Comparing `tmp/tscratchapiget-0.2.9.tar.gz` & `tmp/tscratchapiget-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tscratchapiget-0.2.9.tar", last modified: Fri May 26 15:05:40 2023, max compression
+gzip compressed data, was "tscratchapiget-0.3.8.tar", last modified: Sat May 27 09:05:33 2023, max compression
```

## Comparing `tscratchapiget-0.2.9.tar` & `tscratchapiget-0.3.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 15:05:40.367826 tscratchapiget-0.2.9/
--rw-rw-rw-   0        0        0     1075 2023-05-21 08:00:32.000000 tscratchapiget-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     3627 2023-05-26 15:05:40.366821 tscratchapiget-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     1806 2023-05-26 14:21:43.000000 tscratchapiget-0.2.9/README.md
--rw-rw-rw-   0        0        0      639 2023-05-26 15:04:41.000000 tscratchapiget-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 15:05:40.368822 tscratchapiget-0.2.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 15:05:40.300447 tscratchapiget-0.2.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 15:05:40.335722 tscratchapiget-0.2.9/src/tscratchapiget/
--rw-rw-rw-   0        0        0        0 2023-05-21 04:30:30.000000 tscratchapiget-0.2.9/src/tscratchapiget/__init__.py
--rw-rw-rw-   0        0        0     2405 2023-05-26 14:21:43.000000 tscratchapiget-0.2.9/src/tscratchapiget/user.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:05:40.356739 tscratchapiget-0.2.9/src/tscratchapiget.egg-info/
--rw-rw-rw-   0        0        0     3627 2023-05-26 15:05:40.000000 tscratchapiget-0.2.9/src/tscratchapiget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-05-26 15:05:40.000000 tscratchapiget-0.2.9/src/tscratchapiget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 15:05:40.000000 tscratchapiget-0.2.9/src/tscratchapiget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-26 15:05:40.000000 tscratchapiget-0.2.9/src/tscratchapiget.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 15:05:40.364299 tscratchapiget-0.2.9/tests/
--rw-rw-rw-   0        0        0       71 2023-05-26 14:54:28.000000 tscratchapiget-0.2.9/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:05:33.237279 tscratchapiget-0.3.8/
+-rw-rw-rw-   0        0        0     1075 2023-05-21 08:00:32.000000 tscratchapiget-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0     4957 2023-05-27 09:05:33.234218 tscratchapiget-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3120 2023-05-27 08:59:31.000000 tscratchapiget-0.3.8/README.md
+-rw-rw-rw-   0        0        0      639 2023-05-27 08:59:31.000000 tscratchapiget-0.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 09:05:33.237879 tscratchapiget-0.3.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 09:05:33.123844 tscratchapiget-0.3.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 09:05:33.187005 tscratchapiget-0.3.8/src/tscratchapiget/
+-rw-rw-rw-   0        0        0        0 2023-05-21 04:30:30.000000 tscratchapiget-0.3.8/src/tscratchapiget/__init__.py
+-rw-rw-rw-   0        0        0     2303 2023-05-27 08:47:30.000000 tscratchapiget-0.3.8/src/tscratchapiget/project.py
+-rw-rw-rw-   0        0        0     2405 2023-05-26 14:21:43.000000 tscratchapiget-0.3.8/src/tscratchapiget/user.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:05:33.213857 tscratchapiget-0.3.8/src/tscratchapiget.egg-info/
+-rw-rw-rw-   0        0        0     4957 2023-05-27 09:05:33.000000 tscratchapiget-0.3.8/src/tscratchapiget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-27 09:05:33.000000 tscratchapiget-0.3.8/src/tscratchapiget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 09:05:33.000000 tscratchapiget-0.3.8/src/tscratchapiget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-27 09:05:33.000000 tscratchapiget-0.3.8/src/tscratchapiget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 09:05:33.224116 tscratchapiget-0.3.8/tests/
+-rw-rw-rw-   0        0        0       42 2023-05-27 08:47:30.000000 tscratchapiget-0.3.8/tests/test.py
```

### Comparing `tscratchapiget-0.2.9/LICENSE` & `tscratchapiget-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tscratchapiget-0.2.9/PKG-INFO` & `tscratchapiget-0.3.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tscratchapiget
-Version: 0.2.9
+Version: 0.3.8
 Summary: A library can get scratch api
 Author-email: Tony <tonyvu4913@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Scratch_Tony_14261
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,23 +31,38 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This project gets the scratch api. Everything in this project code by me (except some needed library). Big credit to TimMcCool(Scratcher) for example codes. (This project is not related to TimMcCool)<br>
-Install: `pip install tscratchapiget`
-Change log: https://github.com/Tony14261/tscratchapiget/blob/main/change.log
-
-**This can do**<br>
+Install: `pip install tscratchapiget`<br>
+Change log: https://github.com/Tony14261/tscratchapiget/blob/main/changelog.md<br>
+Report bugs or request new features here: https://github.com/Tony14261/tscratchapiget/issues<br>
+Contact me (Discord): Tony14261#2089<br>
+<br>
+**Functions**<br>
     **User features(v0.2.7)(Updated commands in v0.3.0)** (New commands are at the top):<br>
-        - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'
+        Note: Remeber to ```from tscratchapiget import user```<br>
+        - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'<br>
         - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```<br>
         - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```<br>
         - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'<br>
         - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'<br>
         - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```<br>
         - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```<br>
         - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```<br>
         - Get user country ```country(['user]')```     EX: ```user.country(['')```<br>
         - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```<br>
         - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```<br>
+        <br>
+    **Project features(v0.3.6)**<br>
+        Note: Remember to ```from tscratchapiget import project```<br>
+              ONLY FILL IN [PROJECT ID] NOT A FULL LINK<br>
+        - Get a project title ```title('[Project_ID]')```     EX: ```project.title('105500895')```<br>
+        - Get a project description ```description('[Project_ID]')```     EX: ```project.description('105500895')```<br>
+        - Get a project views ```views('[Project_ID]')```     EX: ```project.views('105500895')```<br>
+        - Get a project loves ```loves('[Project_ID]')```     EX: ```project.loves('105500895')```<br>
+        - Get a project favorites ```favorites('[Project_ID]')```    EX: ```project.favorites('105500895')```<br>
+        - Get a project remixes ```remixes('[Project_ID]')```     EX:   ```project.remixes('105500895')```<br>
+        - Get if a project exists ```exists('[Project_ID]')```     EX: ```project.exists('105500895')``` This check returns to your terminal<br>
+        - Open a project in a web browser ```open('[Project_ID]')```     EX: ```project.open('105500895')```<br>
```

### Comparing `tscratchapiget-0.2.9/pyproject.toml` & `tscratchapiget-0.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tscratchapiget"
-version = "0.2.9"
+version = "0.3.8"
 authors = [
   { name="Tony", email="tonyvu4913@gmail.com" },
 ]
 description = "A library can get scratch api"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `tscratchapiget-0.2.9/src/tscratchapiget/user.py` & `tscratchapiget-0.3.8/src/tscratchapiget/user.py`

 * *Files identical despite different names*

### Comparing `tscratchapiget-0.2.9/src/tscratchapiget.egg-info/PKG-INFO` & `tscratchapiget-0.3.8/src/tscratchapiget.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tscratchapiget
-Version: 0.2.9
+Version: 0.3.8
 Summary: A library can get scratch api
 Author-email: Tony <tonyvu4913@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Scratch_Tony_14261
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,23 +31,38 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This project gets the scratch api. Everything in this project code by me (except some needed library). Big credit to TimMcCool(Scratcher) for example codes. (This project is not related to TimMcCool)<br>
-Install: `pip install tscratchapiget`
-Change log: https://github.com/Tony14261/tscratchapiget/blob/main/change.log
-
-**This can do**<br>
+Install: `pip install tscratchapiget`<br>
+Change log: https://github.com/Tony14261/tscratchapiget/blob/main/changelog.md<br>
+Report bugs or request new features here: https://github.com/Tony14261/tscratchapiget/issues<br>
+Contact me (Discord): Tony14261#2089<br>
+<br>
+**Functions**<br>
     **User features(v0.2.7)(Updated commands in v0.3.0)** (New commands are at the top):<br>
-        - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'
+        Note: Remeber to ```from tscratchapiget import user```<br>
+        - Get if a username exists  ```exists([username])```     EX: ```user.exists('Scratch_Tony_14261')``` if yes: Return 'User exists'     if not: Return 'User does not exist'<br>
         - Get a user unread-message-count ```message_count('[user]')```     EX: ```user.message_count('TimMcCool')```<br>
         - Get a user id ```id('[user]')```     EX: ```user.id('griffpatch')```<br>
         - Get if a user is a scratchteam ```scratchteam('[user]')```     EX: ```user.scratchteam('ScratchCat')``` #Return 'True'<br>
         - Get user join date ```join('[user]')```     EX: ```user.join('Will_Wam')```#Return '2013-11-25T19:52:29.000Z'<br>
         - Get a user pfp(link) ```pfp_link('[user]')```     EX: ```user.pfp_link('Scratch_Tony_14261')```          +Bonus Feature: Open that pfp link in browser. Change that to ```pfp_link_open('[Username]')```<br>
         - Get user About-Me section ```aboutme('[user]')``` EX: ```user.aboutme('WazzoTV')```<br>
         - Get user What-I'm-Working-On section ```wiwo('[username]')```     EX: ```user.wiwo('ceebee')```<br>
         - Get user country ```country(['user]')```     EX: ```user.country(['')```<br>
         - Get user follower count ```followers('[user]')```     Ex: ```user.followers('sharkyshar')```<br>
         - Get user following count ```following('[user]')```     EX: ```user.followers('atomicmagicnumber')```<br>
+        <br>
+    **Project features(v0.3.6)**<br>
+        Note: Remember to ```from tscratchapiget import project```<br>
+              ONLY FILL IN [PROJECT ID] NOT A FULL LINK<br>
+        - Get a project title ```title('[Project_ID]')```     EX: ```project.title('105500895')```<br>
+        - Get a project description ```description('[Project_ID]')```     EX: ```project.description('105500895')```<br>
+        - Get a project views ```views('[Project_ID]')```     EX: ```project.views('105500895')```<br>
+        - Get a project loves ```loves('[Project_ID]')```     EX: ```project.loves('105500895')```<br>
+        - Get a project favorites ```favorites('[Project_ID]')```    EX: ```project.favorites('105500895')```<br>
+        - Get a project remixes ```remixes('[Project_ID]')```     EX:   ```project.remixes('105500895')```<br>
+        - Get if a project exists ```exists('[Project_ID]')```     EX: ```project.exists('105500895')``` This check returns to your terminal<br>
+        - Open a project in a web browser ```open('[Project_ID]')```     EX: ```project.open('105500895')```<br>
```

