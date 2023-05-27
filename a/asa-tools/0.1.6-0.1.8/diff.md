# Comparing `tmp/asa-tools-0.1.6.tar.gz` & `tmp/asa-tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asa-tools-0.1.6.tar", last modified: Wed May 17 00:14:03 2023, max compression
+gzip compressed data, was "asa-tools-0.1.8.tar", last modified: Wed May 17 00:22:20 2023, max compression
```

## Comparing `asa-tools-0.1.6.tar` & `asa-tools-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 00:14:03.243107 asa-tools-0.1.6/
--rw-rw-rw-   0        0        0     1060 2023-05-17 00:14:03.242109 asa-tools-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-05-15 12:48:02.000000 asa-tools-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 00:14:03.238121 asa-tools-0.1.6/asa_tools.egg-info/
--rw-rw-rw-   0        0        0     1060 2023-05-17 00:14:03.000000 asa-tools-0.1.6/asa_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-17 00:14:03.000000 asa-tools-0.1.6/asa_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 00:14:03.000000 asa-tools-0.1.6/asa_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-17 00:14:03.000000 asa-tools-0.1.6/asa_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-05-17 00:14:03.000000 asa-tools-0.1.6/asa_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       45 2023-05-17 00:14:03.000000 asa-tools-0.1.6/asa_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2683 2023-05-17 00:05:40.000000 asa-tools-0.1.6/copyallmp4.py
--rw-rw-rw-   0        0        0     1830 2023-05-09 06:15:06.000000 asa-tools-0.1.6/out_dutys.py
--rw-rw-rw-   0        0        0       42 2023-05-17 00:14:03.243107 asa-tools-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-05-17 00:13:43.000000 asa-tools-0.1.6/setup.py
--rw-rw-rw-   0        0        0     4725 2023-05-15 04:04:27.000000 asa-tools-0.1.6/spyderBili.py
--rw-rw-rw-   0        0        0     3431 2023-05-17 00:08:51.000000 asa-tools-0.1.6/turn2release.py
+drwxrwxrwx   0        0        0        0 2023-05-17 00:22:20.319099 asa-tools-0.1.8/
+-rw-rw-rw-   0        0        0     1060 2023-05-17 00:22:20.317104 asa-tools-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2023-05-15 12:48:02.000000 asa-tools-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 00:22:20.313115 asa-tools-0.1.8/asa_tools.egg-info/
+-rw-rw-rw-   0        0        0     1060 2023-05-17 00:22:20.000000 asa-tools-0.1.8/asa_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-05-17 00:22:20.000000 asa-tools-0.1.8/asa_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 00:22:20.000000 asa-tools-0.1.8/asa_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-17 00:22:20.000000 asa-tools-0.1.8/asa_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-17 00:22:20.000000 asa-tools-0.1.8/asa_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       45 2023-05-17 00:22:20.000000 asa-tools-0.1.8/asa_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2683 2023-05-17 00:05:40.000000 asa-tools-0.1.8/copyallmp4.py
+-rw-rw-rw-   0        0        0     1830 2023-05-09 06:15:06.000000 asa-tools-0.1.8/out_dutys.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 00:22:20.319099 asa-tools-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-05-17 00:22:07.000000 asa-tools-0.1.8/setup.py
+-rw-rw-rw-   0        0        0     4725 2023-05-15 04:04:27.000000 asa-tools-0.1.8/spyderBili.py
+-rw-rw-rw-   0        0        0     3431 2023-05-17 00:08:51.000000 asa-tools-0.1.8/turn2release.py
```

### Comparing `asa-tools-0.1.6/PKG-INFO` & `asa-tools-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asa-tools
-Version: 0.1.6
+Version: 0.1.8
 Summary: asa's personal toolbox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `asa-tools-0.1.6/README.md` & `asa-tools-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `asa-tools-0.1.6/asa_tools.egg-info/PKG-INFO` & `asa-tools-0.1.8/asa_tools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asa-tools
-Version: 0.1.6
+Version: 0.1.8
 Summary: asa's personal toolbox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `asa-tools-0.1.6/copyallmp4.py` & `asa-tools-0.1.8/copyallmp4.py`

 * *Files identical despite different names*

### Comparing `asa-tools-0.1.6/out_dutys.py` & `asa-tools-0.1.8/out_dutys.py`

 * *Files identical despite different names*

### Comparing `asa-tools-0.1.6/spyderBili.py` & `asa-tools-0.1.8/spyderBili.py`

 * *Files identical despite different names*

### Comparing `asa-tools-0.1.6/turn2release.py` & `asa-tools-0.1.8/turn2release.py`

 * *Files identical despite different names*

