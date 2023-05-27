# Comparing `tmp/sciform-0.4.0.tar.gz` & `tmp/sciform-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciform-0.4.0.tar", last modified: Sat May 27 07:16:51 2023, max compression
+gzip compressed data, was "sciform-0.4.1.tar", last modified: Sat May 27 07:22:28 2023, max compression
```

## Comparing `sciform-0.4.0.tar` & `sciform-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 07:16:51.769379 sciform-0.4.0/
--rw-rw-rw-   0        0        0     1074 2023-05-26 03:30:56.000000 sciform-0.4.0/LICENSE
--rw-rw-rw-   0        0        0    30674 2023-05-27 07:16:51.769379 sciform-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    30306 2023-05-27 07:11:38.000000 sciform-0.4.0/README.md
--rw-rw-rw-   0        0        0      589 2023-05-27 07:16:40.000000 sciform-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 07:16:51.769379 sciform-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 07:16:51.751927 sciform-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 07:16:51.757917 sciform-0.4.0/src/sciform/
--rw-rw-rw-   0        0        0       84 2023-05-27 06:34:40.000000 sciform-0.4.0/src/sciform/__init__.py
--rw-rw-rw-   0        0        0     7672 2023-05-27 05:52:09.000000 sciform-0.4.0/src/sciform/format_spec.py
--rw-rw-rw-   0        0        0     6178 2023-05-26 23:20:43.000000 sciform-0.4.0/src/sciform/format_utils.py
--rw-rw-rw-   0        0        0     2373 2023-05-26 18:40:38.000000 sciform-0.4.0/src/sciform/grouping.py
--rw-rw-rw-   0        0        0     4090 2023-05-27 04:30:16.000000 sciform-0.4.0/src/sciform/modes.py
--rw-rw-rw-   0        0        0     1896 2023-05-27 06:26:43.000000 sciform-0.4.0/src/sciform/prefix.py
--rw-rw-rw-   0        0        0     6597 2023-05-27 06:34:06.000000 sciform-0.4.0/src/sciform/sfloat.py
--rw-rw-rw-   0        0        0     3592 2023-05-27 06:34:06.000000 sciform-0.4.0/src/sciform/unc_format.py
-drwxrwxrwx   0        0        0        0 2023-05-27 07:16:51.768376 sciform-0.4.0/src/sciform.egg-info/
--rw-rw-rw-   0        0        0    30674 2023-05-27 07:16:51.000000 sciform-0.4.0/src/sciform.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-05-27 07:16:51.000000 sciform-0.4.0/src/sciform.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 07:16:51.000000 sciform-0.4.0/src/sciform.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-27 07:16:51.000000 sciform-0.4.0/src/sciform.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 07:16:51.768376 sciform-0.4.0/tests/
--rw-rw-rw-   0        0        0    19550 2023-05-27 06:30:46.000000 sciform-0.4.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-27 07:22:28.773744 sciform-0.4.1/
+-rw-rw-rw-   0        0        0     1074 2023-05-26 03:30:56.000000 sciform-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0    30674 2023-05-27 07:22:28.773744 sciform-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    30306 2023-05-27 07:11:38.000000 sciform-0.4.1/README.md
+-rw-rw-rw-   0        0        0      589 2023-05-27 07:16:40.000000 sciform-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 07:22:28.773744 sciform-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 07:22:28.755622 sciform-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 07:22:28.761212 sciform-0.4.1/src/sciform/
+-rw-rw-rw-   0        0        0       84 2023-05-27 07:21:46.000000 sciform-0.4.1/src/sciform/__init__.py
+-rw-rw-rw-   0        0        0     7672 2023-05-27 05:52:09.000000 sciform-0.4.1/src/sciform/format_spec.py
+-rw-rw-rw-   0        0        0     6178 2023-05-26 23:20:43.000000 sciform-0.4.1/src/sciform/format_utils.py
+-rw-rw-rw-   0        0        0     2373 2023-05-26 18:40:38.000000 sciform-0.4.1/src/sciform/grouping.py
+-rw-rw-rw-   0        0        0     4090 2023-05-27 04:30:16.000000 sciform-0.4.1/src/sciform/modes.py
+-rw-rw-rw-   0        0        0     1896 2023-05-27 06:26:43.000000 sciform-0.4.1/src/sciform/prefix.py
+-rw-rw-rw-   0        0        0     6597 2023-05-27 06:34:06.000000 sciform-0.4.1/src/sciform/sfloat.py
+-rw-rw-rw-   0        0        0     3592 2023-05-27 06:34:06.000000 sciform-0.4.1/src/sciform/unc_format.py
+drwxrwxrwx   0        0        0        0 2023-05-27 07:22:28.771774 sciform-0.4.1/src/sciform.egg-info/
+-rw-rw-rw-   0        0        0    30674 2023-05-27 07:22:28.000000 sciform-0.4.1/src/sciform.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-05-27 07:22:28.000000 sciform-0.4.1/src/sciform.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 07:22:28.000000 sciform-0.4.1/src/sciform.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-27 07:22:28.000000 sciform-0.4.1/src/sciform.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 07:22:28.772766 sciform-0.4.1/tests/
+-rw-rw-rw-   0        0        0    19550 2023-05-27 06:30:46.000000 sciform-0.4.1/tests/test.py
```

### Comparing `sciform-0.4.0/LICENSE` & `sciform-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sciform-0.4.0/PKG-INFO` & `sciform-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciform
-Version: 0.4.0
+Version: 0.4.1
 Summary: A package for formatting floats into scientific formatted strings.
 Author-email: Justin Gerber <justin.gerber48@gmail.com>
 Project-URL: Homepage, https://github.com/jagerber48/sciform
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sciform-0.4.0/README.md` & `sciform-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sciform-0.4.0/pyproject.toml` & `sciform-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sciform-0.4.0/src/sciform/format_spec.py` & `sciform-0.4.1/src/sciform/format_spec.py`

 * *Files identical despite different names*

### Comparing `sciform-0.4.0/src/sciform/format_utils.py` & `sciform-0.4.1/src/sciform/format_utils.py`

 * *Files identical despite different names*

### Comparing `sciform-0.4.0/src/sciform/grouping.py` & `sciform-0.4.1/src/sciform/grouping.py`

 * *Files identical despite different names*

### Comparing `sciform-0.4.0/src/sciform/modes.py` & `sciform-0.4.1/src/sciform/modes.py`

 * *Files identical despite different names*

### Comparing `sciform-0.4.0/src/sciform/prefix.py` & `sciform-0.4.1/src/sciform/prefix.py`

 * *Files identical despite different names*

### Comparing `sciform-0.4.0/src/sciform/sfloat.py` & `sciform-0.4.1/src/sciform/sfloat.py`

 * *Files identical despite different names*

### Comparing `sciform-0.4.0/src/sciform/unc_format.py` & `sciform-0.4.1/src/sciform/unc_format.py`

 * *Files identical despite different names*

### Comparing `sciform-0.4.0/src/sciform.egg-info/PKG-INFO` & `sciform-0.4.1/src/sciform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciform
-Version: 0.4.0
+Version: 0.4.1
 Summary: A package for formatting floats into scientific formatted strings.
 Author-email: Justin Gerber <justin.gerber48@gmail.com>
 Project-URL: Homepage, https://github.com/jagerber48/sciform
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sciform-0.4.0/tests/test.py` & `sciform-0.4.1/tests/test.py`

 * *Files identical despite different names*

