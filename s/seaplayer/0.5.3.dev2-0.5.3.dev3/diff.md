# Comparing `tmp/seaplayer-0.5.3.dev2.tar.gz` & `tmp/seaplayer-0.5.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.5.3.dev2.tar", max compression
+gzip compressed data, was "seaplayer-0.5.3.dev3.tar", max compression
```

## Comparing `seaplayer-0.5.3.dev2.tar` & `seaplayer-0.5.3.dev3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.3.dev2/LICENSE
--rw-r--r--   0        0        0     1727 2023-05-26 22:20:45.843959 seaplayer-0.5.3.dev2/pyproject.toml
--rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.3.dev2/README.md
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev2/seaplayer/__init__.py
--rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev2/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev2/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev2/seaplayer/codecs/__init__.py
--rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.3.dev2/seaplayer/codecs/Any.py
--rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev2/seaplayer/codecs/FLAC.py
--rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.3.dev2/seaplayer/codecs/MIDI.py
--rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev2/seaplayer/codecs/MP3.py
--rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev2/seaplayer/codecs/OGG.py
--rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev2/seaplayer/codecs/WAV.py
--rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.3.dev2/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     6188 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev2/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.3.dev2/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev2/seaplayer/css/objects.css
--rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev2/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev2/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev2/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.3.dev2/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.3.dev2/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev2/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.3.dev2/seaplayer/objects/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev2/seaplayer/objects/Configurate.py
--rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.3.dev2/seaplayer/objects/DataOptions.py
--rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev2/seaplayer/objects/Image.py
--rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev2/seaplayer/objects/Input.py
--rw-r--r--   0        0        0     1287 2023-05-26 21:36:55.785380 seaplayer-0.5.3.dev2/seaplayer/objects/Log.py
--rw-r--r--   0        0        0     5562 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev2/seaplayer/objects/MusicList.py
--rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev2/seaplayer/objects/Notification.py
--rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev2/seaplayer/objects/ProgressBar.py
--rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev2/seaplayer/plug/__init__.py
--rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.3.dev2/seaplayer/plug/__main__.py
--rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.3.dev2/seaplayer/plug/cli/__init__.py
--rw-r--r--   0        0        0     5229 2023-05-26 22:12:49.607340 seaplayer-0.5.3.dev2/seaplayer/plug/cli/cli.py
--rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.3.dev2/seaplayer/plug/cli/exceptions.py
--rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.3.dev2/seaplayer/plug/cli/functions.py
--rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.3.dev2/seaplayer/plug/cli/vars.py
--rw-r--r--   0        0        0      817 2023-05-26 19:49:05.778773 seaplayer-0.5.3.dev2/seaplayer/plug/pluginbase.py
--rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.3.dev2/seaplayer/plug/pluginbase.pyi
--rw-r--r--   0        0        0     8452 2023-05-26 22:01:23.658288 seaplayer-0.5.3.dev2/seaplayer/plug/pluginloader.py
--rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.3.dev2/seaplayer/plug/pluginloader.pyi
--rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.3.dev2/seaplayer/screens/__init__.py
--rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.3.dev2/seaplayer/screens/Configurate.py
--rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.3.dev2/seaplayer/screens/Unknown.py
--rw-r--r--   0        0        0    19615 2023-05-26 18:16:55.021730 seaplayer-0.5.3.dev2/seaplayer/seaplayer.py
--rw-r--r--   0        0        0       64 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev2/seaplayer/types/__init__.py
--rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev2/seaplayer/types/Convert.py
--rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev2/seaplayer/types/MusicList.py
--rw-r--r--   0        0        0     1468 2023-05-26 22:20:42.038959 seaplayer-0.5.3.dev2/seaplayer/units.py
--rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 seaplayer-0.5.3.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.3.dev3/LICENSE
+-rw-r--r--   0        0        0     1727 2023-05-26 22:55:41.298774 seaplayer-0.5.3.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.3.dev3/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev3/seaplayer/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev3/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev3/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev3/seaplayer/codecs/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.3.dev3/seaplayer/codecs/Any.py
+-rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev3/seaplayer/codecs/FLAC.py
+-rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.3.dev3/seaplayer/codecs/MIDI.py
+-rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev3/seaplayer/codecs/MP3.py
+-rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev3/seaplayer/codecs/OGG.py
+-rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev3/seaplayer/codecs/WAV.py
+-rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.3.dev3/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     6188 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev3/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.3.dev3/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev3/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev3/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev3/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev3/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.3.dev3/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.3.dev3/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev3/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.3.dev3/seaplayer/objects/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev3/seaplayer/objects/Configurate.py
+-rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.3.dev3/seaplayer/objects/DataOptions.py
+-rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev3/seaplayer/objects/Image.py
+-rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev3/seaplayer/objects/Input.py
+-rw-r--r--   0        0        0     1287 2023-05-26 21:36:55.785380 seaplayer-0.5.3.dev3/seaplayer/objects/Log.py
+-rw-r--r--   0        0        0     5562 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev3/seaplayer/objects/MusicList.py
+-rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev3/seaplayer/objects/Notification.py
+-rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev3/seaplayer/objects/ProgressBar.py
+-rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev3/seaplayer/plug/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.3.dev3/seaplayer/plug/__main__.py
+-rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.3.dev3/seaplayer/plug/cli/__init__.py
+-rw-r--r--   0        0        0     5229 2023-05-26 22:12:49.607340 seaplayer-0.5.3.dev3/seaplayer/plug/cli/cli.py
+-rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.3.dev3/seaplayer/plug/cli/exceptions.py
+-rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.3.dev3/seaplayer/plug/cli/functions.py
+-rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.3.dev3/seaplayer/plug/cli/vars.py
+-rw-r--r--   0        0        0      817 2023-05-26 22:40:27.692911 seaplayer-0.5.3.dev3/seaplayer/plug/pluginbase.py
+-rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.3.dev3/seaplayer/plug/pluginbase.pyi
+-rw-r--r--   0        0        0     8688 2023-05-26 22:50:40.897429 seaplayer-0.5.3.dev3/seaplayer/plug/pluginloader.py
+-rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.3.dev3/seaplayer/plug/pluginloader.pyi
+-rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.3.dev3/seaplayer/screens/__init__.py
+-rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.3.dev3/seaplayer/screens/Configurate.py
+-rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.3.dev3/seaplayer/screens/Unknown.py
+-rw-r--r--   0        0        0    19615 2023-05-26 18:16:55.021730 seaplayer-0.5.3.dev3/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0       64 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev3/seaplayer/types/__init__.py
+-rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev3/seaplayer/types/Convert.py
+-rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev3/seaplayer/types/MusicList.py
+-rw-r--r--   0        0        0     1468 2023-05-26 22:55:45.428073 seaplayer-0.5.3.dev3/seaplayer/units.py
+-rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 seaplayer-0.5.3.dev3/PKG-INFO
```

### Comparing `seaplayer-0.5.3.dev2/LICENSE` & `seaplayer-0.5.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/pyproject.toml` & `seaplayer-0.5.3.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.5.3.dev2"
+version = "0.5.3.dev3"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
```

### Comparing `seaplayer-0.5.3.dev2/README.md` & `seaplayer-0.5.3.dev3/README.md`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/assets/image-not-found.png` & `seaplayer-0.5.3.dev3/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/codecs/Any.py` & `seaplayer-0.5.3.dev3/seaplayer/codecs/Any.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/codecs/MIDI.py` & `seaplayer-0.5.3.dev3/seaplayer/codecs/MIDI.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/codecs/WAV.py` & `seaplayer-0.5.3.dev3/seaplayer/codecs/WAV.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/codeсbase.py` & `seaplayer-0.5.3.dev3/seaplayer/codeсbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/config.py` & `seaplayer-0.5.3.dev3/seaplayer/config.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/css/objects.css` & `seaplayer-0.5.3.dev3/seaplayer/css/objects.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/css/seaplayer.css` & `seaplayer-0.5.3.dev3/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/functions.py` & `seaplayer-0.5.3.dev3/seaplayer/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/modules/colorizer.py` & `seaplayer-0.5.3.dev3/seaplayer/modules/colorizer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/objects/Configurate.py` & `seaplayer-0.5.3.dev3/seaplayer/objects/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/objects/DataOptions.py` & `seaplayer-0.5.3.dev3/seaplayer/objects/DataOptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/objects/Image.py` & `seaplayer-0.5.3.dev3/seaplayer/objects/Image.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/objects/Input.py` & `seaplayer-0.5.3.dev3/seaplayer/objects/Input.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/objects/Log.py` & `seaplayer-0.5.3.dev3/seaplayer/objects/Log.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/objects/MusicList.py` & `seaplayer-0.5.3.dev3/seaplayer/objects/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/objects/Notification.py` & `seaplayer-0.5.3.dev3/seaplayer/objects/Notification.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/objects/ProgressBar.py` & `seaplayer-0.5.3.dev3/seaplayer/objects/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/plug/cli/cli.py` & `seaplayer-0.5.3.dev3/seaplayer/plug/cli/cli.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/plug/cli/exceptions.py` & `seaplayer-0.5.3.dev3/seaplayer/plug/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/plug/cli/functions.py` & `seaplayer-0.5.3.dev3/seaplayer/plug/cli/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/plug/pluginbase.py` & `seaplayer-0.5.3.dev3/seaplayer/plug/pluginbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/plug/pluginbase.pyi` & `seaplayer-0.5.3.dev3/seaplayer/plug/pluginbase.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/plug/pluginloader.py` & `seaplayer-0.5.3.dev3/seaplayer/plug/pluginloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,16 +171,17 @@
     
     @staticmethod
     def load_plugin_info(path: str) -> PluginInfo: return PluginInfo.parse_file(path)
     
     def on_init(self) -> None:
         self.app.info(f"{self.__title__} v{self.__version__} from {self.__author__} ({self.__email__})")
         plugins_paths = list(self.search_plugins_paths())
-        self.app.info(f"Found plugin paths   : {repr(plugins_paths)}")
+        self.app.info(f"Found plugins        : {repr([os.path.basename(os.path.dirname(i[0])) for i in plugins_paths])}")
         for info_path, init_path in plugins_paths:
+            info = None
             try:
                 info = self.load_plugin_info(info_path)
 
                 if not self.config.exists_plugin(info):
                     self.config.add_plugin(info)
                 
                 if self.config.is_enable_plugin(info):
@@ -193,15 +194,18 @@
                         self.app.info(f"Failed to do [green]`on_init`[/green] in: {plugin}")
                     
                     self.on_plugins.append(plugin)
                 else:
                     self.off_plugins.append(info)
             except Exception as e:
                 self.error_plugins.append( (info_path, init_path) )
-                self.app.info(f"Failed to load plugin: {repr( (info_path, init_path) )}")
+                if info is not None:
+                    self.app.info(f"Failed to load plugin: {repr(info)}")
+                else:
+                    self.app.info(f"Failed to load plugin: {repr(os.path.basename(os.path.dirname(info_path)))}")
                 raise e
         self.app.info(f"Plugins loaded ([green]ON [/green]) : {repr(self.on_plugins)}")
         self.app.info(f"Plugins loaded ([red]OFF[/red]) : {repr(self.off_plugins)}")
     
     def on_run(self) -> None:
         for i in self.on_plugins:
             try:
```

### Comparing `seaplayer-0.5.3.dev2/seaplayer/plug/pluginloader.pyi` & `seaplayer-0.5.3.dev3/seaplayer/plug/pluginloader.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/screens/Configurate.py` & `seaplayer-0.5.3.dev3/seaplayer/screens/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/screens/Unknown.py` & `seaplayer-0.5.3.dev3/seaplayer/screens/Unknown.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/seaplayer.py` & `seaplayer-0.5.3.dev3/seaplayer/seaplayer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/types/Convert.py` & `seaplayer-0.5.3.dev3/seaplayer/types/Convert.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/types/MusicList.py` & `seaplayer-0.5.3.dev3/seaplayer/types/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev2/seaplayer/units.py` & `seaplayer-0.5.3.dev3/seaplayer/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from platformdirs import user_config_dir
 # > Image Works
 from PIL.Image import Resampling
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.5.3.dev2"
+__version__ = "0.5.3.dev3"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
```

### Comparing `seaplayer-0.5.3.dev2/PKG-INFO` & `seaplayer-0.5.3.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.5.3.dev2
+Version: 0.5.3.dev3
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
```

