# Comparing `tmp/seaplayer-0.5.4.dev1.tar.gz` & `tmp/seaplayer-0.5.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.5.4.dev1.tar", max compression
+gzip compressed data, was "seaplayer-0.5.4.dev2.tar", max compression
```

## Comparing `seaplayer-0.5.4.dev1.tar` & `seaplayer-0.5.4.dev2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.4.dev1/LICENSE
--rw-r--r--   0        0        0     1727 2023-05-27 09:50:47.975939 seaplayer-0.5.4.dev1/pyproject.toml
--rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.4.dev1/README.md
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev1/seaplayer/__init__.py
--rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev1/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev1/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev1/seaplayer/codecs/__init__.py
--rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.4.dev1/seaplayer/codecs/Any.py
--rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev1/seaplayer/codecs/FLAC.py
--rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.4.dev1/seaplayer/codecs/MIDI.py
--rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev1/seaplayer/codecs/MP3.py
--rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev1/seaplayer/codecs/OGG.py
--rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev1/seaplayer/codecs/WAV.py
--rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.4.dev1/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     6188 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev1/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.4.dev1/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev1/seaplayer/css/objects.css
--rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev1/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev1/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev1/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.4.dev1/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.4.dev1/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev1/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.4.dev1/seaplayer/objects/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev1/seaplayer/objects/Configurate.py
--rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.4.dev1/seaplayer/objects/DataOptions.py
--rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev1/seaplayer/objects/Image.py
--rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev1/seaplayer/objects/Input.py
--rw-r--r--   0        0        0     1287 2023-05-26 21:36:55.785380 seaplayer-0.5.4.dev1/seaplayer/objects/Log.py
--rw-r--r--   0        0        0     5562 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev1/seaplayer/objects/MusicList.py
--rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev1/seaplayer/objects/Notification.py
--rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev1/seaplayer/objects/ProgressBar.py
--rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev1/seaplayer/plug/__init__.py
--rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.4.dev1/seaplayer/plug/__main__.py
--rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.4.dev1/seaplayer/plug/cli/__init__.py
--rw-r--r--   0        0        0     5229 2023-05-26 22:12:49.607340 seaplayer-0.5.4.dev1/seaplayer/plug/cli/cli.py
--rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.4.dev1/seaplayer/plug/cli/exceptions.py
--rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.4.dev1/seaplayer/plug/cli/functions.py
--rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.4.dev1/seaplayer/plug/cli/vars.py
--rw-r--r--   0        0        0      817 2023-05-26 22:40:27.692911 seaplayer-0.5.4.dev1/seaplayer/plug/pluginbase.py
--rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.4.dev1/seaplayer/plug/pluginbase.pyi
--rw-r--r--   0        0        0     8688 2023-05-26 22:50:40.897429 seaplayer-0.5.4.dev1/seaplayer/plug/pluginloader.py
--rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.4.dev1/seaplayer/plug/pluginloader.pyi
--rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.4.dev1/seaplayer/screens/__init__.py
--rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.4.dev1/seaplayer/screens/Configurate.py
--rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.4.dev1/seaplayer/screens/Unknown.py
--rw-r--r--   0        0        0    19768 2023-05-27 09:45:04.264003 seaplayer-0.5.4.dev1/seaplayer/seaplayer.py
--rw-r--r--   0        0        0       91 2023-05-27 09:37:18.022755 seaplayer-0.5.4.dev1/seaplayer/types/__init__.py
--rw-r--r--   0        0        0     1587 2023-05-27 09:48:54.630300 seaplayer-0.5.4.dev1/seaplayer/types/Cache.py
--rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.4.dev1/seaplayer/types/Convert.py
--rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.4.dev1/seaplayer/types/MusicList.py
--rw-r--r--   0        0        0     1525 2023-05-27 09:50:35.690173 seaplayer-0.5.4.dev1/seaplayer/units.py
--rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 seaplayer-0.5.4.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.4.dev2/LICENSE
+-rw-r--r--   0        0        0     1652 2023-05-27 12:20:18.053841 seaplayer-0.5.4.dev2/pyproject.toml
+-rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.4.dev2/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev2/seaplayer/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev2/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev2/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev2/seaplayer/codecs/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.4.dev2/seaplayer/codecs/Any.py
+-rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev2/seaplayer/codecs/FLAC.py
+-rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.4.dev2/seaplayer/codecs/MIDI.py
+-rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev2/seaplayer/codecs/MP3.py
+-rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev2/seaplayer/codecs/OGG.py
+-rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev2/seaplayer/codecs/WAV.py
+-rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.4.dev2/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     6188 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev2/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.4.dev2/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev2/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev2/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev2/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev2/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.4.dev2/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.4.dev2/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev2/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.4.dev2/seaplayer/objects/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev2/seaplayer/objects/Configurate.py
+-rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.4.dev2/seaplayer/objects/DataOptions.py
+-rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev2/seaplayer/objects/Image.py
+-rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev2/seaplayer/objects/Input.py
+-rw-r--r--   0        0        0     1287 2023-05-26 21:36:55.785380 seaplayer-0.5.4.dev2/seaplayer/objects/Log.py
+-rw-r--r--   0        0        0     5562 2023-05-27 11:40:26.374121 seaplayer-0.5.4.dev2/seaplayer/objects/MusicList.py
+-rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev2/seaplayer/objects/Notification.py
+-rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev2/seaplayer/objects/ProgressBar.py
+-rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev2/seaplayer/plug/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.4.dev2/seaplayer/plug/__main__.py
+-rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.4.dev2/seaplayer/plug/cli/__init__.py
+-rw-r--r--   0        0        0     5259 2023-05-27 12:11:55.197047 seaplayer-0.5.4.dev2/seaplayer/plug/cli/cli.py
+-rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.4.dev2/seaplayer/plug/cli/exceptions.py
+-rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.4.dev2/seaplayer/plug/cli/functions.py
+-rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.4.dev2/seaplayer/plug/cli/vars.py
+-rw-r--r--   0        0        0      817 2023-05-26 22:40:27.692911 seaplayer-0.5.4.dev2/seaplayer/plug/pluginbase.py
+-rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.4.dev2/seaplayer/plug/pluginbase.pyi
+-rw-r--r--   0        0        0     8688 2023-05-26 22:50:40.897429 seaplayer-0.5.4.dev2/seaplayer/plug/pluginloader.py
+-rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.4.dev2/seaplayer/plug/pluginloader.pyi
+-rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.4.dev2/seaplayer/screens/__init__.py
+-rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.4.dev2/seaplayer/screens/Configurate.py
+-rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.4.dev2/seaplayer/screens/Unknown.py
+-rw-r--r--   0        0        0    19765 2023-05-27 12:08:26.337289 seaplayer-0.5.4.dev2/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0       91 2023-05-27 09:37:18.022755 seaplayer-0.5.4.dev2/seaplayer/types/__init__.py
+-rw-r--r--   0        0        0     1576 2023-05-27 12:03:27.045912 seaplayer-0.5.4.dev2/seaplayer/types/Cache.py
+-rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.4.dev2/seaplayer/types/Convert.py
+-rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.4.dev2/seaplayer/types/MusicList.py
+-rw-r--r--   0        0        0     1525 2023-05-27 12:13:15.760303 seaplayer-0.5.4.dev2/seaplayer/units.py
+-rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 seaplayer-0.5.4.dev2/PKG-INFO
```

### Comparing `seaplayer-0.5.4.dev1/LICENSE` & `seaplayer-0.5.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/pyproject.toml` & `seaplayer-0.5.4.dev2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.5.4.dev1"
+version = "0.5.4.dev2"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
@@ -15,16 +15,14 @@
     "Operating System :: MacOS",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 packages = [{ include = "seaplayer" }]
 include = [
-    "seaplayer/modules/__init__.py",
-    "seaplayer/modules/colorizer.py",
     "seaplayer/assets/image-not-found.png",
     "seaplayer/css/configurate.css",
     "seaplayer/css/objects.css",
     "seaplayer/css/seaplayer.css",
     "seaplayer/css/unknown.css"
 ]
 
@@ -34,24 +32,25 @@
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 pillow = "^9.5.0"
 aiofiles = "^23.1.0"
 rich = ">=13.3.5"
 mutagen = "1.45.1"
-textual = ">=0.25.0"
+textual = ">=0.26.0"
 playsoundsimple-py = "0.7.0"
 properties-py = "1.1.0"
 typing-inspect = "^0.8.0"
 ripix = ">=2.2.3"
 platformdirs = "^3.5.1"
 pydantic = "^1.10.7"
+click = "^8.1.3"
 poetry = {version = "^1.5.0", optional = true}
 pyinstaller = {version = "^5.11.0", optional = true}
-click = "^8.1.3"
+
 
 [tool.poetry.extras]
 build = ["poetry", "pyinstaller"]
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `seaplayer-0.5.4.dev1/README.md` & `seaplayer-0.5.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/assets/image-not-found.png` & `seaplayer-0.5.4.dev2/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/codecs/Any.py` & `seaplayer-0.5.4.dev2/seaplayer/codecs/Any.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/codecs/MIDI.py` & `seaplayer-0.5.4.dev2/seaplayer/codecs/MIDI.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/codecs/WAV.py` & `seaplayer-0.5.4.dev2/seaplayer/codecs/WAV.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/codeсbase.py` & `seaplayer-0.5.4.dev2/seaplayer/codeсbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/config.py` & `seaplayer-0.5.4.dev2/seaplayer/config.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/css/objects.css` & `seaplayer-0.5.4.dev2/seaplayer/css/objects.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/css/seaplayer.css` & `seaplayer-0.5.4.dev2/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/functions.py` & `seaplayer-0.5.4.dev2/seaplayer/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/modules/colorizer.py` & `seaplayer-0.5.4.dev2/seaplayer/modules/colorizer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/objects/Configurate.py` & `seaplayer-0.5.4.dev2/seaplayer/objects/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/objects/DataOptions.py` & `seaplayer-0.5.4.dev2/seaplayer/objects/DataOptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/objects/Image.py` & `seaplayer-0.5.4.dev2/seaplayer/objects/Image.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/objects/Input.py` & `seaplayer-0.5.4.dev2/seaplayer/objects/Input.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/objects/Log.py` & `seaplayer-0.5.4.dev2/seaplayer/objects/Log.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/objects/MusicList.py` & `seaplayer-0.5.4.dev2/seaplayer/objects/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/objects/Notification.py` & `seaplayer-0.5.4.dev2/seaplayer/objects/Notification.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/objects/ProgressBar.py` & `seaplayer-0.5.4.dev2/seaplayer/objects/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/plug/cli/cli.py` & `seaplayer-0.5.4.dev2/seaplayer/plug/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 
 # ! Commands
 @click.command("enable", help="Enabling plugin.")
 @click.argument("plugin_name_id")
 def enabling(plugin_name_id: str):
     if plugin_config.exists_plugin_by_name_id(plugin_name_id):
         plugin_config.enable_plugin_by_name_id(plugin_name_id)
-        console.print(f"[yellow]The {repr(plugin_name_id)} plug-in is [green]enabled[/green].[/yellow]")
+        console.print(f"[yellow]The [green]{repr(plugin_name_id)}[/green] plug-in is [green]enabled[/green].[/yellow]")
     else:
         raise_exception(console, PluginNotExistsError, plugin_name_id)
 
 @click.command("disable", help="Disabling plugin.")
 @click.argument("plugin_name_id")
 def disabling(plugin_name_id: str):
     if plugin_config.exists_plugin_by_name_id(plugin_name_id):
         plugin_config.disable_plugin_by_name_id(plugin_name_id)
-        console.print(f"[yellow]The {repr(plugin_name_id)} plug-in is [red]disabled[/red].[/yellow]")
+        console.print(f"[yellow]The [green]{repr(plugin_name_id)}[/green] plug-in is [red]disabled[/red].[/yellow]")
     else:
         raise_exception(console, PluginNotExistsError, plugin_name_id)
 
 @click.command("list", help="List of plugins.")
 def listing():
     if len(plugin_config.config.plugins_enable) > 0:
         for n, info in enumerate(get_plugins_info(), 1):
```

### Comparing `seaplayer-0.5.4.dev1/seaplayer/plug/cli/exceptions.py` & `seaplayer-0.5.4.dev2/seaplayer/plug/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/plug/cli/functions.py` & `seaplayer-0.5.4.dev2/seaplayer/plug/cli/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/plug/pluginbase.py` & `seaplayer-0.5.4.dev2/seaplayer/plug/pluginbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/plug/pluginbase.pyi` & `seaplayer-0.5.4.dev2/seaplayer/plug/pluginbase.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/plug/pluginloader.py` & `seaplayer-0.5.4.dev2/seaplayer/plug/pluginloader.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/plug/pluginloader.pyi` & `seaplayer-0.5.4.dev2/seaplayer/plug/pluginloader.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/screens/Configurate.py` & `seaplayer-0.5.4.dev2/seaplayer/screens/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/screens/Unknown.py` & `seaplayer-0.5.4.dev2/seaplayer/screens/Unknown.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/seaplayer.py` & `seaplayer-0.5.4.dev2/seaplayer/seaplayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,14 @@
     ENABLE_PLUGIN_SYSTEM,
     CACHE_DIRPATH
 )
 # > Plugin System Init
 if ENABLE_PLUGIN_SYSTEM:
     from .plug import PluginLoader
 
-# ! Initialize
-cache = Cacher(CACHE_DIRPATH)
-
 # ! Main Functions
 def build_bindings(config: SeaPlayerConfig):
     yield Binding(config.key_quit, "quit", "Quit")
     yield Binding("c,с", "push_screen('configurate')", "Configurate")
     if config.log_menu_enable:
         yield Binding("l,д", "app.toggle_class('.log-menu', '-hidden')", 'Logs')
     yield Binding(config.key_rewind_back, "minus_rewind", f"Rewind -{config.rewind_count_seconds} sec")
@@ -80,15 +77,16 @@
         os.path.join(CSS_LOCALDIR, "objects.css")
     ]
     SCREENS = {
         "unknown": Unknown(id="screen_unknown"),
         "configurate": Configurate(id="screen_configurate")
     }
     
-    # ! SeaPlayer Configuration
+    # ! SeaPlayer Configuration & Hanlders
+    cache = Cacher(CACHE_DIRPATH)
     config = SeaPlayerConfig(CONFIG_FILEPATH)
     max_volume_percent: float = config.max_volume_percent
     
     # ! Textual Keys Configuration
     BINDINGS = list(build_bindings(config))
     
     # ! Template Configuration
```

### Comparing `seaplayer-0.5.4.dev1/seaplayer/types/Convert.py` & `seaplayer-0.5.4.dev2/seaplayer/types/Convert.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/types/MusicList.py` & `seaplayer-0.5.4.dev2/seaplayer/types/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev1/seaplayer/units.py` & `seaplayer-0.5.4.dev2/seaplayer/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from platformdirs import user_config_dir
 # > Image Works
 from PIL.Image import Resampling
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.5.4.dev1"
+__version__ = "0.5.4.dev2"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
```

### Comparing `seaplayer-0.5.4.dev1/PKG-INFO` & `seaplayer-0.5.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.5.4.dev1
+Version: 0.5.4.dev2
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -27,15 +27,15 @@
 Requires-Dist: playsoundsimple-py (==0.7.0)
 Requires-Dist: poetry (>=1.5.0,<2.0.0) ; extra == "build"
 Requires-Dist: properties-py (==1.1.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyinstaller (>=5.11.0,<6.0.0) ; extra == "build"
 Requires-Dist: rich (>=13.3.5)
 Requires-Dist: ripix (>=2.2.3)
-Requires-Dist: textual (>=0.25.0)
+Requires-Dist: textual (>=0.26.0)
 Requires-Dist: typing-inspect (>=0.8.0,<0.9.0)
 Project-URL: Repository, https://github.com/romanin-rf/SeaPlayer
 Description-Content-Type: text/markdown
 
 <div id="header" align="center">
     <img src="https://github.com/romanin-rf/SeaPlayer/assets/60302782/937adcc4-f547-440c-8139-a5f15bffa157" alt="Icon" width="300">
 </div>
```

