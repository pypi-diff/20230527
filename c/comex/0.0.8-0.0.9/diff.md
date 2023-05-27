# Comparing `tmp/comex-0.0.8.tar.gz` & `tmp/comex-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comex-0.0.8.tar", last modified: Sat May 27 08:39:56 2023, max compression
+gzip compressed data, was "comex-0.0.9.tar", last modified: Sat May 27 08:50:21 2023, max compression
```

## Comparing `comex-0.0.8.tar` & `comex-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,58 @@
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:39:56.030000 comex-0.0.8/
--rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.8/LICENSE
--rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:39:56.040000 comex-0.0.8/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)     7489 2023-05-27 06:29:25.000000 comex-0.0.8/README.md
--rwxrwxrwx   0 noble      (501) staff       (20)     1036 2023-05-27 08:39:56.040000 comex-0.0.8/setup.cfg
--rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.8/setup.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:39:56.030000 comex-0.0.8/src/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:39:56.030000 comex-0.0.8/src/comex/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:28:52.000000 comex-0.0.8/src/comex/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)      109 2023-05-27 08:28:48.000000 comex-0.0.8/src/comex/__main__.py
--rwxrwxrwx   0 noble      (501) staff       (20)     3588 2023-05-27 08:34:37.000000 comex-0.0.8/src/comex/cli.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:39:56.030000 comex-0.0.8/src/comex.egg-info/
--rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:39:55.000000 comex-0.0.8/src/comex.egg-info/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)      297 2023-05-27 08:39:56.000000 comex-0.0.8/src/comex.egg-info/SOURCES.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-27 08:39:55.000000 comex-0.0.8/src/comex.egg-info/dependency_links.txt
--rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-27 08:39:55.000000 comex-0.0.8/src/comex.egg-info/entry_points.txt
--rwxrwxrwx   0 noble      (501) staff       (20)      151 2023-05-27 08:39:55.000000 comex-0.0.8/src/comex.egg-info/requires.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-05-27 08:39:55.000000 comex-0.0.8/src/comex.egg-info/top_level.txt
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/
+-rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.9/LICENSE
+-rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:50:21.400000 comex-0.0.9/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)     7489 2023-05-27 06:29:25.000000 comex-0.0.9/README.md
+-rwxrwxrwx   0 noble      (501) staff       (20)     1036 2023-05-27 08:50:21.410000 comex-0.0.9/setup.cfg
+-rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.9/setup.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/comex/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:28:52.000000 comex-0.0.9/src/comex/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)      109 2023-05-27 08:28:48.000000 comex-0.0.9/src/comex/__main__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     3588 2023-05-27 08:34:37.000000 comex-0.0.9/src/comex/cli.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/comex/codeviews/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/comex/codeviews/AST/
+-rwxrwxrwx   0 noble      (501) staff       (20)     4196 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/codeviews/AST/AST.py
+-rwxrwxrwx   0 noble      (501) staff       (20)      968 2023-05-27 08:37:58.000000 comex-0.0.9/src/comex/codeviews/AST/AST_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/codeviews/AST/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/comex/codeviews/CFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1426 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/codeviews/CFG/CFG.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    51528 2023-05-27 08:37:07.000000 comex-0.0.9/src/comex/codeviews/CFG/CFG_csharp.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1300 2023-05-27 08:37:31.000000 comex-0.0.9/src/comex/codeviews/CFG/CFG_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    78323 2023-05-27 08:37:41.000000 comex-0.0.9/src/comex/codeviews/CFG/CFG_java.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/codeviews/CFG/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/comex/codeviews/CST/
+-rwxrwxrwx   0 noble      (501) staff       (20)     2540 2023-05-27 08:36:43.000000 comex-0.0.9/src/comex/codeviews/CST/CST_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/codeviews/CST/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/comex/codeviews/DFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1246 2023-05-27 08:38:26.000000 comex-0.0.9/src/comex/codeviews/DFG/DFG_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/codeviews/DFG/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/comex/codeviews/SDFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     4535 2023-05-27 08:38:37.000000 comex-0.0.9/src/comex/codeviews/SDFG/SDFG.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    32117 2023-05-27 08:38:51.000000 comex-0.0.9/src/comex/codeviews/SDFG/SDFG_csharp.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    61608 2023-05-27 08:38:58.000000 comex-0.0.9/src/comex/codeviews/SDFG/SDFG_java.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/codeviews/SDFG/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/codeviews/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/comex/codeviews/combined_graph/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/codeviews/combined_graph/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     9551 2023-05-27 08:36:32.000000 comex-0.0.9/src/comex/codeviews/combined_graph/combined_driver.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/comex/tree_parser/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:49:05.000000 comex-0.0.9/src/comex/tree_parser/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     8617 2023-05-27 08:35:50.000000 comex-0.0.9/src/comex/tree_parser/cs_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     6152 2023-05-27 08:04:01.000000 comex-0.0.9/src/comex/tree_parser/custom_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    10057 2023-05-27 08:35:58.000000 comex-0.0.9/src/comex/tree_parser/java_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1819 2023-05-27 08:36:07.000000 comex-0.0.9/src/comex/tree_parser/parser_driver.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/comex/utils/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1763 2023-05-09 07:00:15.000000 comex-0.0.9/src/comex/utils/DFG_utils.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:48:37.000000 comex-0.0.9/src/comex/utils/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    19424 2023-05-24 03:11:00.000000 comex-0.0.9/src/comex/utils/cs_nodes.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    25191 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/utils/java_nodes.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1083 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/utils/postprocessor.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     2418 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/utils/preprocessor.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     2055 2023-05-09 06:59:54.000000 comex-0.0.9/src/comex/utils/src_parser.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:50:21.380000 comex-0.0.9/src/comex.egg-info/
+-rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:50:21.000000 comex-0.0.9/src/comex.egg-info/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)     1404 2023-05-27 08:50:21.000000 comex-0.0.9/src/comex.egg-info/SOURCES.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-27 08:50:21.000000 comex-0.0.9/src/comex.egg-info/dependency_links.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-27 08:50:21.000000 comex-0.0.9/src/comex.egg-info/entry_points.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)      151 2023-05-27 08:50:21.000000 comex-0.0.9/src/comex.egg-info/requires.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-05-27 08:50:21.000000 comex-0.0.9/src/comex.egg-info/top_level.txt
```

### Comparing `comex-0.0.8/LICENSE` & `comex-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `comex-0.0.8/PKG-INFO` & `comex-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `comex-0.0.8/README.md` & `comex-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `comex-0.0.8/setup.cfg` & `comex-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = comex
-version = 0.0.8
+version = 0.0.9
 description = Generate combined multi-code view graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/tree-sitter-codeviews
 license = Apache-2.0
 license_file = LICENSE
 classifiers =
```

### Comparing `comex-0.0.8/src/comex/cli.py` & `comex-0.0.9/src/comex/cli.py`

 * *Files identical despite different names*

### Comparing `comex-0.0.8/src/comex.egg-info/PKG-INFO` & `comex-0.0.9/src/comex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

