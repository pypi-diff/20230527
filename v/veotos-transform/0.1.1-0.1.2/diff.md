# Comparing `tmp/veotos_transform-0.1.1.tar.gz` & `tmp/veotos_transform-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veotos_transform-0.1.1.tar", last modified: Fri May 26 23:40:42 2023, max compression
+gzip compressed data, was "veotos_transform-0.1.2.tar", last modified: Fri May 26 23:47:06 2023, max compression
```

## Comparing `veotos_transform-0.1.1.tar` & `veotos_transform-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 veotos    (1000) veotos    (1000)        0 2023-05-26 23:40:42.782617 veotos_transform-0.1.1/
--rw-rw-r--   0 veotos    (1000) veotos    (1000)       19 2023-05-26 20:09:35.000000 veotos_transform-0.1.1/MANIFEST.in
--rw-rw-r--   0 veotos    (1000) veotos    (1000)     8258 2023-05-26 23:40:42.778617 veotos_transform-0.1.1/PKG-INFO
--rw-rw-r--   0 veotos    (1000) veotos    (1000)     7857 2023-05-26 22:41:21.000000 veotos_transform-0.1.1/README.rst
--rw-rw-r--   0 veotos    (1000) veotos    (1000)       38 2023-05-26 23:40:42.782617 veotos_transform-0.1.1/setup.cfg
--rw-rw-r--   0 veotos    (1000) veotos    (1000)      864 2023-05-26 23:16:40.000000 veotos_transform-0.1.1/setup.py
-drwxrwxr-x   0 veotos    (1000) veotos    (1000)        0 2023-05-26 23:40:42.770617 veotos_transform-0.1.1/veotos_transform/
--rw-rw-r--   0 veotos    (1000) veotos    (1000)       40 2023-05-26 19:03:29.000000 veotos_transform-0.1.1/veotos_transform/__init__.py
--rw-rw-r--   0 veotos    (1000) veotos    (1000)      444 2023-05-26 22:27:24.000000 veotos_transform-0.1.1/veotos_transform/command_line.py
--rwxrwxr-x   0 veotos    (1000) veotos    (1000)     2727 2023-05-26 19:03:29.000000 veotos_transform-0.1.1/veotos_transform/obfuscations.py
-drwxrwxr-x   0 veotos    (1000) veotos    (1000)        0 2023-05-26 23:40:42.778617 veotos_transform-0.1.1/veotos_transform.egg-info/
--rw-rw-r--   0 veotos    (1000) veotos    (1000)     8258 2023-05-26 23:40:42.000000 veotos_transform-0.1.1/veotos_transform.egg-info/PKG-INFO
--rw-rw-r--   0 veotos    (1000) veotos    (1000)      407 2023-05-26 23:40:42.000000 veotos_transform-0.1.1/veotos_transform.egg-info/SOURCES.txt
--rw-rw-r--   0 veotos    (1000) veotos    (1000)        1 2023-05-26 23:40:42.000000 veotos_transform-0.1.1/veotos_transform.egg-info/dependency_links.txt
--rw-rw-r--   0 veotos    (1000) veotos    (1000)       72 2023-05-26 23:40:42.000000 veotos_transform-0.1.1/veotos_transform.egg-info/entry_points.txt
--rw-rw-r--   0 veotos    (1000) veotos    (1000)        1 2023-05-26 18:43:37.000000 veotos_transform-0.1.1/veotos_transform.egg-info/not-zip-safe
--rw-rw-r--   0 veotos    (1000) veotos    (1000)        6 2023-05-26 23:40:42.000000 veotos_transform-0.1.1/veotos_transform.egg-info/requires.txt
--rw-rw-r--   0 veotos    (1000) veotos    (1000)       17 2023-05-26 23:40:42.000000 veotos_transform-0.1.1/veotos_transform.egg-info/top_level.txt
+drwxrwxr-x   0 veotos    (1000) veotos    (1000)        0 2023-05-26 23:47:06.626607 veotos_transform-0.1.2/
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)       19 2023-05-26 20:09:35.000000 veotos_transform-0.1.2/MANIFEST.in
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)     8264 2023-05-26 23:47:06.626607 veotos_transform-0.1.2/PKG-INFO
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)     7857 2023-05-26 22:41:21.000000 veotos_transform-0.1.2/README.rst
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)       38 2023-05-26 23:47:06.626607 veotos_transform-0.1.2/setup.cfg
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)      870 2023-05-26 23:46:42.000000 veotos_transform-0.1.2/setup.py
+drwxrwxr-x   0 veotos    (1000) veotos    (1000)        0 2023-05-26 23:47:06.618607 veotos_transform-0.1.2/veotos_transform/
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)       40 2023-05-26 19:03:29.000000 veotos_transform-0.1.2/veotos_transform/__init__.py
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)      444 2023-05-26 22:27:24.000000 veotos_transform-0.1.2/veotos_transform/command_line.py
+-rwxrwxr-x   0 veotos    (1000) veotos    (1000)     2727 2023-05-26 19:03:29.000000 veotos_transform-0.1.2/veotos_transform/obfuscations.py
+drwxrwxr-x   0 veotos    (1000) veotos    (1000)        0 2023-05-26 23:47:06.626607 veotos_transform-0.1.2/veotos_transform.egg-info/
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)     8264 2023-05-26 23:47:06.000000 veotos_transform-0.1.2/veotos_transform.egg-info/PKG-INFO
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)      407 2023-05-26 23:47:06.000000 veotos_transform-0.1.2/veotos_transform.egg-info/SOURCES.txt
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)        1 2023-05-26 23:47:06.000000 veotos_transform-0.1.2/veotos_transform.egg-info/dependency_links.txt
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)       72 2023-05-26 23:47:06.000000 veotos_transform-0.1.2/veotos_transform.egg-info/entry_points.txt
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)        1 2023-05-26 18:43:37.000000 veotos_transform-0.1.2/veotos_transform.egg-info/not-zip-safe
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)        6 2023-05-26 23:47:06.000000 veotos_transform-0.1.2/veotos_transform.egg-info/requires.txt
+-rw-rw-r--   0 veotos    (1000) veotos    (1000)       17 2023-05-26 23:47:06.000000 veotos_transform-0.1.2/veotos_transform.egg-info/top_level.txt
```

### Comparing `veotos_transform-0.1.1/PKG-INFO` & `veotos_transform-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: veotos_transform
-Version: 0.1.1
+Version: 0.1.2
 Summary: Obfuscate text with next consonant or vowel
-Home-page: http://github.com/veotos/veotos_aoc
+Home-page: http://github.com/veotos/veotos-transform
 Author: veotos
 Author-email: veotos@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `veotos_transform-0.1.1/README.rst` & `veotos_transform-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `veotos_transform-0.1.1/veotos_transform/obfuscations.py` & `veotos_transform-0.1.2/veotos_transform/obfuscations.py`

 * *Files identical despite different names*

### Comparing `veotos_transform-0.1.1/veotos_transform.egg-info/PKG-INFO` & `veotos_transform-0.1.2/veotos_transform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: veotos-transform
-Version: 0.1.1
+Version: 0.1.2
 Summary: Obfuscate text with next consonant or vowel
-Home-page: http://github.com/veotos/veotos_aoc
+Home-page: http://github.com/veotos/veotos-transform
 Author: veotos
 Author-email: veotos@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

