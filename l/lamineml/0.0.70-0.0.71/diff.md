# Comparing `tmp/lamineml-0.0.70.tar.gz` & `tmp/lamineml-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.0.70.tar", last modified: Fri May 26 10:10:29 2023, max compression
+gzip compressed data, was "lamineml-0.0.71.tar", last modified: Fri May 26 15:26:11 2023, max compression
```

## Comparing `lamineml-0.0.70.tar` & `lamineml-0.0.71.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-26 10:10:29.368802 lamineml-0.0.70/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.70/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-26 10:10:29.368802 lamineml-0.0.70/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.70/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-05-18 14:20:16.000000 lamineml-0.0.70/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-26 10:10:29.368802 lamineml-0.0.70/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-26 10:10:29.368802 lamineml-0.0.70/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-26 10:10:29.368802 lamineml-0.0.70/src/lamine/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.70/src/lamine/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)     5442 2023-05-26 10:08:46.000000 lamineml-0.0.70/src/lamine/tools.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-26 10:10:29.368802 lamineml-0.0.70/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-26 10:10:29.000000 lamineml-0.0.70/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-26 10:10:29.000000 lamineml-0.0.70/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-26 10:10:29.000000 lamineml-0.0.70/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-26 10:10:29.000000 lamineml-0.0.70/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-26 15:26:11.559106 lamineml-0.0.71/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.71/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-26 15:26:11.563106 lamineml-0.0.71/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.71/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-05-18 14:20:16.000000 lamineml-0.0.71/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-26 15:26:11.563106 lamineml-0.0.71/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-26 15:26:11.559106 lamineml-0.0.71/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-26 15:26:11.559106 lamineml-0.0.71/src/lamine/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.71/src/lamine/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)     5550 2023-05-26 15:24:01.000000 lamineml-0.0.71/src/lamine/tools.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-26 15:26:11.559106 lamineml-0.0.71/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-26 15:26:11.000000 lamineml-0.0.71/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-26 15:26:11.000000 lamineml-0.0.71/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-26 15:26:11.000000 lamineml-0.0.71/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-26 15:26:11.000000 lamineml-0.0.71/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.0.70/PKG-INFO` & `lamineml-0.0.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.70
+Version: 0.0.71
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.0.70/README.md` & `lamineml-0.0.71/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.0.70/setup.cfg` & `lamineml-0.0.71/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.0.70
+version = 0.0.71
 author = Lamine ML
 author_email = lamineml128@gmail.com
 description = use this library in kivy android
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.0.70/src/lamine/tools.py` & `lamineml-0.0.71/src/lamine/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,22 @@
 view =autoclass("android.view.View")
 Ringtone=autoclass ("android.media.Ringtone")
 Ringm=autoclass("android.media.RingtoneManager")
 C= autoclass('android.media.AudioManager')
 Context = autoclass('android.content.Context')
 from android.runnable import run_on_ui_thread
 def mute_phone():
-    con = activity.getSystemService(Context.AUDIO_SERVICE)
-    C.adjustVolume(con.ADJUST_MUTE, 0)
+    x = cast("android.media.AudioManager", activity.getSystemService(Context.AUDIO_SERVICE))
+    x.adjustStreamVolume(C.STREAM_RING, C.ADJUST_MUTE, 0)
 
 def unmute_phone():
-    con = activity.getSystemService(Context.AUDIO_SERVICE)
-    C.adjustVolume(con.ADJUST_UNMUTE, 0)
+    x = cast("android.media.AudioManager", activity.getSystemService(Context.AUDIO_SERVICE))
+    x.adjustStreamVolume(C.STREAM_RING, C.ADJUST_UNMUTE, 0)
+
+
 def get_DefaultRingtone():
     d = Ringm.getActualDefaultRingtoneUri(activity, Ringm.TYPE_RINGTONE)
     d2 = Ringm.getRingtone(activity, d)
     d2.play()
 def remove_apps(pk):
     s=Intent()
     s.setAction(Intent.ACTION_DELETE)
```

### Comparing `lamineml-0.0.70/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.0.71/src/lamineml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.70
+Version: 0.0.71
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

