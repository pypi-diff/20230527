# Comparing `tmp/comex-0.0.7.tar.gz` & `tmp/comex-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comex-0.0.7.tar", last modified: Sat May 27 08:30:36 2023, max compression
+gzip compressed data, was "comex-0.0.8.tar", last modified: Sat May 27 08:39:56 2023, max compression
```

## Comparing `comex-0.0.7.tar` & `comex-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:30:36.820000 comex-0.0.7/
--rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.7/LICENSE
--rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:30:36.830000 comex-0.0.7/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)     7489 2023-05-27 06:29:25.000000 comex-0.0.7/README.md
--rwxrwxrwx   0 noble      (501) staff       (20)     1021 2023-05-27 08:30:36.830000 comex-0.0.7/setup.cfg
--rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.7/setup.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:30:36.820000 comex-0.0.7/src/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:30:36.820000 comex-0.0.7/src/comex/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:28:52.000000 comex-0.0.7/src/comex/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)      109 2023-05-27 08:28:48.000000 comex-0.0.7/src/comex/__main__.py
--rwxrwxrwx   0 noble      (501) staff       (20)     3593 2023-05-27 08:15:21.000000 comex-0.0.7/src/comex/cli.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:30:36.820000 comex-0.0.7/src/comex.egg-info/
--rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)      297 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/SOURCES.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/dependency_links.txt
--rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/entry_points.txt
--rwxrwxrwx   0 noble      (501) staff       (20)      137 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/requires.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-05-27 08:30:36.000000 comex-0.0.7/src/comex.egg-info/top_level.txt
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:39:56.030000 comex-0.0.8/
+-rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.0.8/LICENSE
+-rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:39:56.040000 comex-0.0.8/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)     7489 2023-05-27 06:29:25.000000 comex-0.0.8/README.md
+-rwxrwxrwx   0 noble      (501) staff       (20)     1036 2023-05-27 08:39:56.040000 comex-0.0.8/setup.cfg
+-rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.0.8/setup.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:39:56.030000 comex-0.0.8/src/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:39:56.030000 comex-0.0.8/src/comex/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:28:52.000000 comex-0.0.8/src/comex/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)      109 2023-05-27 08:28:48.000000 comex-0.0.8/src/comex/__main__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     3588 2023-05-27 08:34:37.000000 comex-0.0.8/src/comex/cli.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:39:56.030000 comex-0.0.8/src/comex.egg-info/
+-rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:39:55.000000 comex-0.0.8/src/comex.egg-info/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)      297 2023-05-27 08:39:56.000000 comex-0.0.8/src/comex.egg-info/SOURCES.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-27 08:39:55.000000 comex-0.0.8/src/comex.egg-info/dependency_links.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-27 08:39:55.000000 comex-0.0.8/src/comex.egg-info/entry_points.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)      151 2023-05-27 08:39:55.000000 comex-0.0.8/src/comex.egg-info/requires.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-05-27 08:39:55.000000 comex-0.0.8/src/comex.egg-info/top_level.txt
```

### Comparing `comex-0.0.7/LICENSE` & `comex-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `comex-0.0.7/PKG-INFO` & `comex-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.7
+Version: 0.0.8
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `comex-0.0.7/README.md` & `comex-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `comex-0.0.7/setup.cfg` & `comex-0.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = comex
-version = 0.0.7
+version = 0.0.8
 description = Generate combined multi-code view graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/tree-sitter-codeviews
 license = Apache-2.0
 license_file = LICENSE
 classifiers = 
@@ -19,14 +19,15 @@
 packages = find:
 install_requires = 
 	networkx==2.6.3
 	tree-sitter==0.20.1
 	deepdiff==5.8.1
 	pydot==1.4.1
 	typer==0.4.1
+	loguru==0.6.0
 python_requires = >=3.8
 package_dir = =src
 
 [options.packages.find]
 where = ./src
 
 [options.entry_points]
```

### Comparing `comex-0.0.7/src/comex/cli.py` & `comex-0.0.8/src/comex/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 from pathlib import Path
 from typing import Optional
 
 import typer
 from loguru import logger
 
-from comex.codeviews.combined_graph.combined_driver import CombinedDriver
+from .codeviews.combined_graph.combined_driver import CombinedDriver
 
 app = typer.Typer()
 
 
 @app.callback(invoke_without_command=True)
 def main(
         lang: str = typer.Option(..., help="java, cs"),
```

### Comparing `comex-0.0.7/src/comex.egg-info/PKG-INFO` & `comex-0.0.8/src/comex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.0.7
+Version: 0.0.8
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

