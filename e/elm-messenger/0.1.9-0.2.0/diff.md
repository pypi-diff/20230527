# Comparing `tmp/elm-messenger-0.1.9.tar.gz` & `tmp/elm-messenger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.1.9.tar", last modified: Wed May 24 04:47:35 2023, max compression
+gzip compressed data, was "elm-messenger-0.2.0.tar", last modified: Sat May 27 13:26:01 2023, max compression
```

## Comparing `elm-messenger-0.1.9.tar` & `elm-messenger-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-24 04:47:35.067003 elm-messenger-0.1.9/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.9/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-24 04:47:35.067003 elm-messenger-0.1.9/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.9/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-24 04:47:35.067003 elm-messenger-0.1.9/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-24 04:47:35.000000 elm-messenger-0.1.9/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-24 04:47:35.067003 elm-messenger-0.1.9/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.9/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.9/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    17575 2023-05-24 04:45:46.000000 elm-messenger-0.1.9/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.1.9/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-24 04:47:35.067003 elm-messenger-0.1.9/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.9/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 13:26:01.041392 elm-messenger-0.2.0/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.0/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-27 13:26:01.041392 elm-messenger-0.2.0/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.2.0/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 13:26:01.038059 elm-messenger-0.2.0/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-27 13:26:01.000000 elm-messenger-0.2.0/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-27 13:26:01.038059 elm-messenger-0.2.0/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.0/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.0/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    18276 2023-05-27 13:25:04.000000 elm-messenger-0.2.0/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.0/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-27 13:26:01.041392 elm-messenger-0.2.0/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.0/setup.py
```

### Comparing `elm-messenger-0.1.9/messengercli/messenger.py` & `elm-messenger-0.2.0/messengercli/messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import typer
 import os
 import shutil
 import json
 from .updater import Updater
 
 app = typer.Typer(add_completion=False, help="Messenger CLI")
-API_VERSION = "0.1.9"
+API_VERSION = "0.2.0"
 
 
 class Messenger:
     config = None
 
     def __init__(self) -> None:
         """
@@ -43,24 +43,24 @@
             raise Exception("Scene already exists.")
         self.config["scenes"][scene] = []
         self.dump_config()
         os.mkdir(f"src/Scenes/{scene}")
 
         Updater(
             [
-                ".messenger/scene/Sample/Common.elm",
                 ".messenger/scene/Sample/Export.elm",
                 ".messenger/scene/Sample/Global.elm",
+                ".messenger/scene/Sample/Model.elm",
                 ".messenger/scene/Sample/LayerBase.elm",
                 ".messenger/scene/Sample/LayerInit.elm",
             ],
             [
-                f"src/Scenes/{scene}/Common.elm",
                 f"src/Scenes/{scene}/Export.elm",
                 f"src/Scenes/{scene}/Global.elm",
+                f"src/Scenes/{scene}/Model.elm",
                 f"src/Scenes/{scene}/LayerBase.elm",
                 f"src/Scenes/{scene}/LayerInit.elm",
             ],
         ).rep(scene)
 
         # Modify Scene
         with open("src/Lib/Scene/Base.elm", "r") as f:
@@ -140,26 +140,26 @@
         self.dump_config()
         os.mkdir(f"src/SceneProtos/{scene}")
         os.mkdir(f"src/SceneProtos/{scene}/GameComponent")
         os.mkdir(f"src/SceneProtos/{scene}/GameComponents")
 
         Updater(
             [
-                ".messenger/sceneproto/scene/Common.elm",
                 ".messenger/sceneproto/scene/Export.elm",
                 ".messenger/sceneproto/scene/Global.elm",
+                ".messenger/sceneproto/scene/Model.elm",
                 ".messenger/sceneproto/scene/LayerBase.elm",
                 ".messenger/sceneproto/scene/LayerInit.elm",
                 ".messenger/sceneproto/gamecomponent/Base.elm",
                 ".messenger/sceneproto/gamecomponent/Handler.elm",
             ],
             [
-                f"src/SceneProtos/{scene}/Common.elm",
                 f"src/SceneProtos/{scene}/Export.elm",
                 f"src/SceneProtos/{scene}/Global.elm",
+                f"src/SceneProtos/{scene}/Model.elm",
                 f"src/SceneProtos/{scene}/LayerBase.elm",
                 f"src/SceneProtos/{scene}/LayerInit.elm",
                 f"src/SceneProtos/{scene}/GameComponent/Base.elm",
                 f"src/SceneProtos/{scene}/GameComponent/Handler.elm",
             ],
         ).rep(scene)
 
@@ -216,16 +216,16 @@
                 [f"import SceneProtos.{sceneproto}.{l}.Export as {l}" for l in layers]
             )
         ).rep(
             "\n    | ".join([f"{l}Data {l}.Data" for l in layers])
         )
 
         Updater(
-            [".messenger/sceneproto/scene/Model.elm"],
-            [f"src/SceneProtos/{sceneproto}/Model.elm"],
+            [".messenger/sceneproto/scene/Common.elm"],
+            [f"src/SceneProtos/{sceneproto}/Common.elm"],
         ).rep(sceneproto).rep(
             "\n".join(
                 [
                     f"import SceneProtos.{sceneproto}.{l}.Export as {l}\nimport SceneProtos.{sceneproto}.{l}.Global as {l}G"
                     for l in layers
                 ]
             )
@@ -352,16 +352,16 @@
             [f"src/Scenes/{scene}/LayerSettings.elm"],
         ).rep(scene).rep(
             "\n".join([f"import Scenes.{scene}.{l}.Export as {l}" for l in layers])
         ).rep(
             "\n    | ".join([f"{l}Data {l}.Data" for l in layers])
         )
         Updater(
-            [".messenger/scene/Sample/Model.elm"],
-            [f"src/Scenes/{scene}/Model.elm"],
+            [".messenger/scene/Sample/Common.elm"],
+            [f"src/Scenes/{scene}/Common.elm"],
         ).rep(scene).rep(
             "\n".join(
                 [
                     f"import Scenes.{scene}.{l}.Export as {l}\nimport Scenes.{scene}.{l}.Global as {l}G"
                     for l in layers
                 ]
             )
@@ -428,14 +428,34 @@
     input(f"You are going to create a component named {name}, continue?")
     msg.add_component(name)
     msg.format()
     print("Done!")
 
 
 @app.command()
+def update(
+    scene=typer.Option(False, "--scene", "-s", help="Update scenes."),
+    scenelayer=typer.Option(None, "--scenelayer", "-sl", help="Update layers in that scene."),
+    sceneprotolayer=typer.Option(None, "--sceneprotolayer", "-spl", help="Update sceneproto layers in that sceneproto."),
+):
+    msg = Messenger()
+    input(
+        f"You are going to regenerate settings (including scenes, layers, sceneproto layers), continue?"
+    )
+    if scene:
+        msg.update_scenes()
+    if scenelayer is not None:
+        msg.update_layers(scenelayer)
+    if sceneprotolayer is not None:
+        msg.update_sceneproto_layers(sceneprotolayer)
+    msg.format()
+    print("Done!")
+
+
+@app.command()
 def scene(name: str):
     msg = Messenger()
     input(f"You are going to create a scene named {name}, continue?")
     msg.add_scene(name)
     msg.update_scenes()
     msg.format()
     print("Done!")
```

### Comparing `elm-messenger-0.1.9/messengercli/updater.py` & `elm-messenger-0.2.0/messengercli/updater.py`

 * *Files identical despite different names*

