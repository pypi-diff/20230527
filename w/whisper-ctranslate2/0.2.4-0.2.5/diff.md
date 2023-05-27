# Comparing `tmp/whisper-ctranslate2-0.2.4.tar.gz` & `tmp/whisper-ctranslate2-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.2.4.tar", last modified: Thu May  4 05:18:32 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.2.5.tar", last modified: Sat May 27 11:31:40 2023, max compression
```

## Comparing `whisper-ctranslate2-0.2.4.tar` & `whisper-ctranslate2-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-04 05:18:32.939876 whisper-ctranslate2-0.2.4/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.2.4/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-05-04 05:18:32.939876 whisper-ctranslate2-0.2.4/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-04-25 18:49:27.000000 whisper-ctranslate2-0.2.4/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-05-04 05:18:32.939876 whisper-ctranslate2-0.2.4/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1501 2023-04-27 15:43:27.000000 whisper-ctranslate2-0.2.4/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-04 05:18:32.935876 whisper-ctranslate2-0.2.4/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-04 05:18:32.939876 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5154 2023-05-03 14:33:47.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6275 2023-05-01 06:35:27.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-05-03 14:00:51.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    17511 2023-05-03 17:29:49.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10279 2023-05-03 17:29:49.000000 whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-04 05:18:32.939876 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-05-04 05:18:32.000000 whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-27 11:31:40.077345 whisper-ctranslate2-0.2.5/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-05-27 11:31:40.077345 whisper-ctranslate2-0.2.5/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-05-27 11:31:40.077345 whisper-ctranslate2-0.2.5/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1501 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-27 11:31:40.073345 whisper-ctranslate2-0.2.5/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-27 11:31:40.073345 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5154 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6275 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    17511 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10359 2023-05-27 10:54:49.000000 whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-27 11:31:40.077345 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-05-27 11:31:39.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-05-27 11:31:40.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-27 11:31:39.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2023-05-27 11:31:39.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-05-27 11:31:39.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-05-27 11:31:39.000000 whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.2.4/LICENSE` & `whisper-ctranslate2-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.4/PKG-INFO` & `whisper-ctranslate2-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.4
+Version: 0.2.5
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `whisper-ctranslate2-0.2.4/README.md` & `whisper-ctranslate2-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.4/setup.py` & `whisper-ctranslate2-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/live.py` & `whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/live.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.4/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.2.5/src/whisper_ctranslate2/writers.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,19 @@
                             timing["word"] = "\n" + timing["word"]
                         line_len = len(timing["word"].strip())
                     subtitle.append(timing)
                     last = timing["start"]
             if len(subtitle) > 0:
                 yield subtitle
 
-        if "words" in result["segments"][0] and result["segments"][0]["words"]:
+        if (
+            len(result["segments"]) > 0
+            and "words" in result["segments"][0]
+            and result["segments"][0]["words"]
+        ):
             for subtitle in iterate_subtitles():
                 subtitle_start = self.format_timestamp(subtitle[0]["start"])
                 subtitle_end = self.format_timestamp(subtitle[-1]["end"])
                 subtitle_text = "".join([word["word"] for word in subtitle])
                 if highlight_words:
                     last = subtitle_start
                     all_words = [timing["word"] for timing in subtitle]
```

### Comparing `whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.4
+Version: 0.2.5
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `whisper-ctranslate2-0.2.4/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.2.5/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

