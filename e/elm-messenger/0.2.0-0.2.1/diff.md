# Comparing `tmp/elm-messenger-0.2.0.tar.gz` & `tmp/elm-messenger-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.2.0.tar", last modified: Sat May 27 13:26:01 2023, max compression
+gzip compressed data, was "elm-messenger-0.2.1.tar", last modified: Sat May 27 16:00:29 2023, max compression
```

## Comparing `elm-messenger-0.2.0.tar` & `elm-messenger-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 13:26:01.041392 elm-messenger-0.2.0/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.0/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-27 13:26:01.041392 elm-messenger-0.2.0/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.2.0/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 13:26:01.038059 elm-messenger-0.2.0/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 13:26:01.038059 elm-messenger-0.2.0/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.0/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.0/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    18276 2023-05-27 13:25:04.000000 elm-messenger-0.2.0/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.0/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-27 13:26:01.041392 elm-messenger-0.2.0/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.0/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 16:00:29.127185 elm-messenger-0.2.1/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.1/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-27 16:00:29.127185 elm-messenger-0.2.1/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.2.1/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 16:00:29.123852 elm-messenger-0.2.1/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-27 16:00:29.000000 elm-messenger-0.2.1/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 16:00:29.123852 elm-messenger-0.2.1/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.1/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.1/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    18588 2023-05-27 15:53:54.000000 elm-messenger-0.2.1/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      771 2023-05-27 15:51:04.000000 elm-messenger-0.2.1/messengercli/patcher.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.1/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-05-27 16:00:29.127185 elm-messenger-0.2.1/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.1/setup.py
```

### Comparing `elm-messenger-0.2.0/messengercli/messenger.py` & `elm-messenger-0.2.1/messengercli/messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 """
 
 import typer
 import os
 import shutil
 import json
 from .updater import Updater
+from .patcher import patch
 
 app = typer.Typer(add_completion=False, help="Messenger CLI")
-API_VERSION = "0.2.0"
+API_VERSION = "0.2.1"
 
 
 class Messenger:
     config = None
 
     def __init__(self) -> None:
         """
         Check if `messager.json` exists and load it.
         """
         if os.path.exists("messenger.json"):
             with open("messenger.json", "r") as f:
                 self.config = json.load(f)
             if "version" not in self.config:
-                raise Exception("API version not found in the config file.")
+                raise Exception("Messenger API version not found in the config file.")
             if self.config["version"] != API_VERSION:
-                raise Exception(f"API version not matched. I'm using v{API_VERSION}.")
+                raise Exception(f"Messenger API version not matched. I'm using v{API_VERSION}. You can edit messenger.json manually to upgrade.")
         else:
             raise Exception(
                 "messenger.json not found. Are you in the project initialized by the Messenger? Try `messenger init <your-project-name>`."
             )
 
     def dump_config(self):
         with open("messenger.json", "w") as f:
@@ -387,24 +388,24 @@
 ):
     input(
         f"""Thanks for using Messenger v{API_VERSION}.
 See https://github.com/linsyking/Messenger.git for more information.
 Here is my plan:
 
 - Create a directory named {name}
-- Install the core Messenger liberary
+- Install the core Messenger library
 - Install the elm packages needed
 
 Press Enter to continue
 """
     )
     os.makedirs(name, exist_ok=True)
     os.chdir(name)
     os.system(f"git clone {template_repo} .messenger --depth=1")
-    shutil.copytree(".messenger/core/", "./src")
+    shutil.copytree(".messenger/src/", "./src")
     shutil.copytree(".messenger/public/", "./public")
     shutil.copy(".messenger/.gitignore", "./.gitignore")
     shutil.copy(".messenger/Makefile", "./Makefile")
     shutil.copy(".messenger/make", "./make")
     shutil.copy(".messenger/elm.json", "./elm.json")
 
     os.makedirs("src/Scenes", exist_ok=True)
@@ -519,9 +520,17 @@
         f"You are going to create a game component named {gc} under sceneproto {sceneproto}, continue?"
     )
     msg.add_gamecomponent(sceneproto, gc)
     msg.format()
     print("Done!")
 
 
+@app.command(help="Update Messenger core library")
+def updatelib():
+    msg = Messenger()
+    input(f"You are going to update the core library of Messenger, continue?")
+    patch()
+    msg.format()
+    print("Done!")
+
 if __name__ == "__main__":
     app()
```

### Comparing `elm-messenger-0.2.0/messengercli/updater.py` & `elm-messenger-0.2.1/messengercli/updater.py`

 * *Files identical despite different names*

