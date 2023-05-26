# Comparing `tmp/seaplayer-0.5.3.dev1.tar.gz` & `tmp/seaplayer-0.5.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.5.3.dev1.tar", max compression
+gzip compressed data, was "seaplayer-0.5.3.dev2.tar", max compression
```

## Comparing `seaplayer-0.5.3.dev1.tar` & `seaplayer-0.5.3.dev2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.3.dev1/LICENSE
--rw-r--r--   0        0        0     1727 2023-05-26 20:39:52.670544 seaplayer-0.5.3.dev1/pyproject.toml
--rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.3.dev1/README.md
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev1/seaplayer/__init__.py
--rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev1/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev1/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev1/seaplayer/codecs/__init__.py
--rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.3.dev1/seaplayer/codecs/Any.py
--rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev1/seaplayer/codecs/FLAC.py
--rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.3.dev1/seaplayer/codecs/MIDI.py
--rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev1/seaplayer/codecs/MP3.py
--rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev1/seaplayer/codecs/OGG.py
--rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev1/seaplayer/codecs/WAV.py
--rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.3.dev1/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     6188 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev1/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.3.dev1/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev1/seaplayer/css/objects.css
--rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev1/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev1/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev1/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.3.dev1/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.3.dev1/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev1/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.3.dev1/seaplayer/objects/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev1/seaplayer/objects/Configurate.py
--rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.3.dev1/seaplayer/objects/DataOptions.py
--rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev1/seaplayer/objects/Image.py
--rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev1/seaplayer/objects/Input.py
--rw-r--r--   0        0        0     1236 2023-05-26 18:16:55.015726 seaplayer-0.5.3.dev1/seaplayer/objects/Log.py
--rw-r--r--   0        0        0     5562 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev1/seaplayer/objects/MusicList.py
--rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev1/seaplayer/objects/Notification.py
--rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev1/seaplayer/objects/ProgressBar.py
--rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev1/seaplayer/plug/__init__.py
--rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.3.dev1/seaplayer/plug/__main__.py
--rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.3.dev1/seaplayer/plug/cli/__init__.py
--rw-r--r--   0        0        0     4980 2023-05-26 20:35:00.054615 seaplayer-0.5.3.dev1/seaplayer/plug/cli/cli.py
--rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.3.dev1/seaplayer/plug/cli/exceptions.py
--rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.3.dev1/seaplayer/plug/cli/functions.py
--rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.3.dev1/seaplayer/plug/cli/vars.py
--rw-r--r--   0        0        0      817 2023-05-26 19:49:05.778773 seaplayer-0.5.3.dev1/seaplayer/plug/pluginbase.py
--rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.3.dev1/seaplayer/plug/pluginbase.pyi
--rw-r--r--   0        0        0     7967 2023-05-26 18:16:55.019724 seaplayer-0.5.3.dev1/seaplayer/plug/pluginloader.py
--rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.3.dev1/seaplayer/plug/pluginloader.pyi
--rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.3.dev1/seaplayer/screens/__init__.py
--rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.3.dev1/seaplayer/screens/Configurate.py
--rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.3.dev1/seaplayer/screens/Unknown.py
--rw-r--r--   0        0        0    19615 2023-05-26 18:16:55.021730 seaplayer-0.5.3.dev1/seaplayer/seaplayer.py
--rw-r--r--   0        0        0       64 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev1/seaplayer/types/__init__.py
--rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev1/seaplayer/types/Convert.py
--rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev1/seaplayer/types/MusicList.py
--rw-r--r--   0        0        0     1468 2023-05-26 20:40:03.758787 seaplayer-0.5.3.dev1/seaplayer/units.py
--rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 seaplayer-0.5.3.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.3.dev2/LICENSE
+-rw-r--r--   0        0        0     1727 2023-05-26 22:20:45.843959 seaplayer-0.5.3.dev2/pyproject.toml
+-rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.3.dev2/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev2/seaplayer/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev2/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev2/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev2/seaplayer/codecs/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.3.dev2/seaplayer/codecs/Any.py
+-rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev2/seaplayer/codecs/FLAC.py
+-rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.3.dev2/seaplayer/codecs/MIDI.py
+-rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev2/seaplayer/codecs/MP3.py
+-rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev2/seaplayer/codecs/OGG.py
+-rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev2/seaplayer/codecs/WAV.py
+-rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.3.dev2/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     6188 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev2/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.3.dev2/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev2/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev2/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev2/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev2/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.3.dev2/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.3.dev2/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev2/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.3.dev2/seaplayer/objects/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev2/seaplayer/objects/Configurate.py
+-rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.3.dev2/seaplayer/objects/DataOptions.py
+-rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev2/seaplayer/objects/Image.py
+-rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev2/seaplayer/objects/Input.py
+-rw-r--r--   0        0        0     1287 2023-05-26 21:36:55.785380 seaplayer-0.5.3.dev2/seaplayer/objects/Log.py
+-rw-r--r--   0        0        0     5562 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev2/seaplayer/objects/MusicList.py
+-rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev2/seaplayer/objects/Notification.py
+-rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev2/seaplayer/objects/ProgressBar.py
+-rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev2/seaplayer/plug/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.3.dev2/seaplayer/plug/__main__.py
+-rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.3.dev2/seaplayer/plug/cli/__init__.py
+-rw-r--r--   0        0        0     5229 2023-05-26 22:12:49.607340 seaplayer-0.5.3.dev2/seaplayer/plug/cli/cli.py
+-rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.3.dev2/seaplayer/plug/cli/exceptions.py
+-rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.3.dev2/seaplayer/plug/cli/functions.py
+-rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.3.dev2/seaplayer/plug/cli/vars.py
+-rw-r--r--   0        0        0      817 2023-05-26 19:49:05.778773 seaplayer-0.5.3.dev2/seaplayer/plug/pluginbase.py
+-rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.3.dev2/seaplayer/plug/pluginbase.pyi
+-rw-r--r--   0        0        0     8452 2023-05-26 22:01:23.658288 seaplayer-0.5.3.dev2/seaplayer/plug/pluginloader.py
+-rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.3.dev2/seaplayer/plug/pluginloader.pyi
+-rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.3.dev2/seaplayer/screens/__init__.py
+-rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.3.dev2/seaplayer/screens/Configurate.py
+-rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.3.dev2/seaplayer/screens/Unknown.py
+-rw-r--r--   0        0        0    19615 2023-05-26 18:16:55.021730 seaplayer-0.5.3.dev2/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0       64 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev2/seaplayer/types/__init__.py
+-rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev2/seaplayer/types/Convert.py
+-rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev2/seaplayer/types/MusicList.py
+-rw-r--r--   0        0        0     1468 2023-05-26 22:20:42.038959 seaplayer-0.5.3.dev2/seaplayer/units.py
+-rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 seaplayer-0.5.3.dev2/PKG-INFO
```

### Comparing `seaplayer-0.5.3.dev1/LICENSE` & `seaplayer-0.5.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/pyproject.toml` & `seaplayer-0.5.3.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.5.3.dev1"
+version = "0.5.3.dev2"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
```

### Comparing `seaplayer-0.5.3.dev1/README.md` & `seaplayer-0.5.3.dev2/README.md`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/assets/image-not-found.png` & `seaplayer-0.5.3.dev2/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/codecs/Any.py` & `seaplayer-0.5.3.dev2/seaplayer/codecs/Any.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/codecs/MIDI.py` & `seaplayer-0.5.3.dev2/seaplayer/codecs/MIDI.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/codecs/WAV.py` & `seaplayer-0.5.3.dev2/seaplayer/codecs/WAV.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/codeсbase.py` & `seaplayer-0.5.3.dev2/seaplayer/codeсbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/config.py` & `seaplayer-0.5.3.dev2/seaplayer/config.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/css/objects.css` & `seaplayer-0.5.3.dev2/seaplayer/css/objects.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/css/seaplayer.css` & `seaplayer-0.5.3.dev2/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/functions.py` & `seaplayer-0.5.3.dev2/seaplayer/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/modules/colorizer.py` & `seaplayer-0.5.3.dev2/seaplayer/modules/colorizer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/objects/Configurate.py` & `seaplayer-0.5.3.dev2/seaplayer/objects/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/objects/DataOptions.py` & `seaplayer-0.5.3.dev2/seaplayer/objects/DataOptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/objects/Image.py` & `seaplayer-0.5.3.dev2/seaplayer/objects/Image.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/objects/Input.py` & `seaplayer-0.5.3.dev2/seaplayer/objects/Input.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/objects/Log.py` & `seaplayer-0.5.3.dev2/seaplayer/objects/Log.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from textual.widgets import TextLog
+from rich.traceback import Traceback
 # > Typing
 from typing import TypeVar
 # > Local Import's
 from ..functions import rich_exception
 
 # ! Types
 RETURN = TypeVar('RETURN')
@@ -17,13 +18,14 @@
             kwargs["classes"] = kwargs["classes"] + " log-menu -hidden"
         else:
             kwargs["classes"] = "log-menu -hidden"
         
         super().__init__(**kwargs)
     
     def write_log(self, chap: str, msg: str, *, chap_color: str="green") -> None:
-        if self.enable_logging: self.write(f"[[{chap_color}]{chap.center(self.chap_max_width)}[/]]: {msg}", shrink=False)
+        if self.enable_logging:
+            self.write(f"[[{chap_color}]{chap.center(self.chap_max_width)}[/]]: {msg}", shrink=False)
     
     def info(self, msg: str) -> None: self.write_log("INFO", msg, chap_color="green")
     def error(self, msg: str) -> None: self.write_log("ERROR", msg, chap_color="red")
     def warn(self, msg: str) -> None: self.write_log("WARN", msg, chap_color="orange")
     def exception(self, e: Exception) -> None: self.write_log("ERROR", rich_exception(e), chap_color="red")
```

### Comparing `seaplayer-0.5.3.dev1/seaplayer/objects/MusicList.py` & `seaplayer-0.5.3.dev2/seaplayer/objects/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/objects/Notification.py` & `seaplayer-0.5.3.dev2/seaplayer/objects/Notification.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/objects/ProgressBar.py` & `seaplayer-0.5.3.dev2/seaplayer/objects/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/plug/cli/cli.py` & `seaplayer-0.5.3.dev2/seaplayer/plug/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,21 +103,28 @@
         else:
             raise_exception(console, IsPluginDirectoryError, dirpath)
     except:
         console.print_exception()
 
 @click.command("load", help="Load the plugin into the SeaPlayer plugins directory.")
 @click.argument("dirpath", type=click.Path(True, False))
-def loading(dirpath: str):
+@click.option(
+    "--rewrite", "-w", "rewrite",
+    help="Delete if it exists and overwrite.",
+    is_flag=True, default=False
+)
+def loading(dirpath: str, rewrite: bool):
     dirpath = os.path.abspath(dirpath)
     if is_plugin_dirpath(dirpath):
         with Live("[yellow]Loading...[/yellow]", console=console) as l:
+            to_path = os.path.join(PLUGINS_DIRPATH, os.path.basename(dirpath))
+            if rewrite: shutil.rmtree(to_path, ignore_errors=True)
             shutil.copytree(
                 dirpath,
-                os.path.join(PLUGINS_DIRPATH, os.path.basename(dirpath)),
+                to_path,
                 dirs_exist_ok=True
             )
             init_config()
             l.update("[yellow]Plugin [green]loaded[/green]![/yellow]", refresh=True)
     else:
         raise_exception(console, IsNotPluginDirectoryError, dirpath)
```

### Comparing `seaplayer-0.5.3.dev1/seaplayer/plug/cli/exceptions.py` & `seaplayer-0.5.3.dev2/seaplayer/plug/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/plug/cli/functions.py` & `seaplayer-0.5.3.dev2/seaplayer/plug/cli/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/plug/pluginbase.py` & `seaplayer-0.5.3.dev2/seaplayer/plug/pluginbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/plug/pluginbase.pyi` & `seaplayer-0.5.3.dev2/seaplayer/plug/pluginbase.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/plug/pluginloader.py` & `seaplayer-0.5.3.dev2/seaplayer/plug/pluginloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 import glob
 import asyncio
 from pathlib import Path
 from pydantic import BaseModel
 # > ImportLib
 from importlib.util import spec_from_file_location, module_from_spec
 # > Typing
@@ -24,18 +25,30 @@
 
 # ! Functions
 def get_module_info(path: str):
     if os.path.basename(path) == "__init__.py":
         return os.path.basename(os.path.dirname(path)), path
     return os.path.basename(path), path
 
-def load_module(path: str) -> PluginModuleType:
-    module_name, module_location = get_module_info(path)
-    module_spec = spec_from_file_location(module_name, module_location)
+def get_submodules_locations(init_path: str) -> List[str]:
+    return [ os.path.dirname(init_path) ]
+
+def load_module(init_path: str) -> PluginModuleType:
+    module_name, module_location = get_module_info(init_path)
+    module_spec = spec_from_file_location(
+        module_name,
+        module_location,
+        submodule_search_locations=get_submodules_locations(init_path)
+    )
     module = module_from_spec(module_spec)
+    
+    sys.modules[module_spec.name] = module 
+    # TODO: Temporary option as there is a risk of replacing existing modules
+    # TODO: Make an environment-module to surround all these modules for security
+    
     module_spec.loader.exec_module(module)
     return module
 
 def plugin_from_module(app, pl, info: PluginInfo, module: PluginModuleType) -> PluginBase:
     return module.plugin_main(app, pl, info)
 
 # ! Plugin Loader Config
@@ -87,29 +100,29 @@
         return False
     
     def disable_plugin(self, info: PluginInfo) -> None:
         self.config.plugins_enable[info.name_id] = False
         self.refresh()
     
     def disable_plugin_by_name_id(self, name_id: str) -> None:
-        self.config.plugins_enable[name_id] = True
+        self.config.plugins_enable[name_id] = False
         self.refresh()
     
     def enable_plugin(self, info: PluginInfo) -> None:
         self.config.plugins_enable[info.name_id] = True
         self.refresh()
     
     def enable_plugin_by_name_id(self, name_id: str) -> None:
         self.config.plugins_enable[name_id] = True
         self.refresh()
 
 # ! Plugin Loader Class
 class PluginLoader:
     __title__: str = "PluginLoader"
-    __version__: str = "0.1.2"
+    __version__: str = "0.1.3"
     __author__: str = "Romanin"
     __email__: str = "semina054@gmail.com"
 
     def __init__(
         self,
         app,
         plugins_dirpath: Optional[Union[str, Path]]=None,
@@ -178,17 +191,18 @@
                         plugin.on_init()
                     except:
                         self.app.info(f"Failed to do [green]`on_init`[/green] in: {plugin}")
                     
                     self.on_plugins.append(plugin)
                 else:
                     self.off_plugins.append(info)
-            except:
+            except Exception as e:
                 self.error_plugins.append( (info_path, init_path) )
                 self.app.info(f"Failed to load plugin: {repr( (info_path, init_path) )}")
+                raise e
         self.app.info(f"Plugins loaded ([green]ON [/green]) : {repr(self.on_plugins)}")
         self.app.info(f"Plugins loaded ([red]OFF[/red]) : {repr(self.off_plugins)}")
     
     def on_run(self) -> None:
         for i in self.on_plugins:
             try:
                 i.on_run()
```

### Comparing `seaplayer-0.5.3.dev1/seaplayer/plug/pluginloader.pyi` & `seaplayer-0.5.3.dev2/seaplayer/plug/pluginloader.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/screens/Configurate.py` & `seaplayer-0.5.3.dev2/seaplayer/screens/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/screens/Unknown.py` & `seaplayer-0.5.3.dev2/seaplayer/screens/Unknown.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/seaplayer.py` & `seaplayer-0.5.3.dev2/seaplayer/seaplayer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/types/Convert.py` & `seaplayer-0.5.3.dev2/seaplayer/types/Convert.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/types/MusicList.py` & `seaplayer-0.5.3.dev2/seaplayer/types/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.3.dev1/seaplayer/units.py` & `seaplayer-0.5.3.dev2/seaplayer/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from platformdirs import user_config_dir
 # > Image Works
 from PIL.Image import Resampling
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.5.3.dev1"
+__version__ = "0.5.3.dev2"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
```

### Comparing `seaplayer-0.5.3.dev1/PKG-INFO` & `seaplayer-0.5.3.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.5.3.dev1
+Version: 0.5.3.dev2
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
```

