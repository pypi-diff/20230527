# Comparing `tmp/comex-0.0.6.tar.gz` & `tmp/comex-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comex-0.0.6.tar", last modified: Sat May 27 08:23:57 2023, max compression
+gzip compressed data, was "comex-0.0.7.tar", last modified: Sat May 27 08:30:36 2023, max compression
```

## Comparing `comex-0.0.6.tar` & `comex-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:23:57.930000 comex-0.0.6/
--rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.6/LICENSE
--rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:23:57.940000 comex-0.0.6/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)     7489 2023-05-27 06:29:25.000000 comex-0.0.6/README.md
--rwxrwxrwx   0 noble      (501) staff       (20)     1009 2023-05-27 08:23:57.940000 comex-0.0.6/setup.cfg
--rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.6/setup.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:23:57.930000 comex-0.0.6/src/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:23:57.930000 comex-0.0.6/src/comex/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:22:22.000000 comex-0.0.6/src/comex/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)      109 2023-05-27 08:23:18.000000 comex-0.0.6/src/comex/__main__.py
--rwxrwxrwx   0 noble      (501) staff       (20)     3593 2023-05-27 08:15:21.000000 comex-0.0.6/src/comex/cli.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:23:57.930000 comex-0.0.6/src/comex.egg-info/
--rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:23:57.000000 comex-0.0.6/src/comex.egg-info/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)      297 2023-05-27 08:23:57.000000 comex-0.0.6/src/comex.egg-info/SOURCES.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-27 08:23:57.000000 comex-0.0.6/src/comex.egg-info/dependency_links.txt
--rwxrwxrwx   0 noble      (501) staff       (20)       28 2023-05-27 08:23:57.000000 comex-0.0.6/src/comex.egg-info/entry_points.txt
--rwxrwxrwx   0 noble      (501) staff       (20)      137 2023-05-27 08:23:57.000000 comex-0.0.6/src/comex.egg-info/requires.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-05-27 08:23:57.000000 comex-0.0.6/src/comex.egg-info/top_level.txt
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:30:36.820000 comex-0.0.7/
+-rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.7/LICENSE
+-rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:30:36.830000 comex-0.0.7/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)     7489 2023-05-27 06:29:25.000000 comex-0.0.7/README.md
+-rwxrwxrwx   0 noble      (501) staff       (20)     1021 2023-05-27 08:30:36.830000 comex-0.0.7/setup.cfg
+-rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.7/setup.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:30:36.820000 comex-0.0.7/src/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:30:36.820000 comex-0.0.7/src/comex/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:28:52.000000 comex-0.0.7/src/comex/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)      109 2023-05-27 08:28:48.000000 comex-0.0.7/src/comex/__main__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     3593 2023-05-27 08:15:21.000000 comex-0.0.7/src/comex/cli.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:30:36.820000 comex-0.0.7/src/comex.egg-info/
+-rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)      297 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/SOURCES.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/dependency_links.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/entry_points.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)      137 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/requires.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/top_level.txt
```

### Comparing `comex-0.0.6/LICENSE` & `comex-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `comex-0.0.6/PKG-INFO` & `comex-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `comex-0.0.6/README.md` & `comex-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `comex-0.0.6/setup.cfg` & `comex-0.0.7/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = comex
-version = 0.0.6
+version = 0.0.7
 description = Generate combined multi-code view graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/tree-sitter-codeviews
 license = Apache-2.0
 license_file = LICENSE
 classifiers = 
@@ -26,15 +26,15 @@
 python_requires = >=3.8
 package_dir = =src
 
 [options.packages.find]
 where = ./src
 
 [options.entry_points]
-pip = 
+console_scripts = 
 	comex=comex.cli:app
 
 [options.extras_require]
 dev = 
 	pytest
 	pytest-cov
 	tqdm
```

### Comparing `comex-0.0.6/src/comex/cli.py` & `comex-0.0.7/src/comex/cli.py`

 * *Files identical despite different names*

### Comparing `comex-0.0.6/src/comex.egg-info/PKG-INFO` & `comex-0.0.7/src/comex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

