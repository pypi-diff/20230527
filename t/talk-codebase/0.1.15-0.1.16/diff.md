# Comparing `tmp/talk_codebase-0.1.15.tar.gz` & `tmp/talk_codebase-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.15.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.16.tar", max compression
```

## Comparing `talk_codebase-0.1.15.tar` & `talk_codebase-0.1.16.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1237 2023-05-27 02:38:14.577253 talk_codebase-0.1.15/README.md
--rw-r--r--   0        0        0      787 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1960 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/talk_codebase/cli.py
--rw-r--r--   0        0        0      518 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/talk_codebase/consts.py
--rw-r--r--   0        0        0     1530 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/talk_codebase/llm.py
--rw-r--r--   0        0        0     1947 2023-05-27 02:38:14.581253 talk_codebase-0.1.15/talk_codebase/utils.py
--rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 talk_codebase-0.1.15/PKG-INFO
+-rw-r--r--   0        0        0     1237 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/README.md
+-rw-r--r--   0        0        0      811 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1960 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/talk_codebase/cli.py
+-rw-r--r--   0        0        0      518 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2149 2023-05-27 14:14:29.673279 talk_codebase-0.1.16/talk_codebase/llm.py
+-rw-r--r--   0        0        0     1947 2023-05-27 14:14:29.677279 talk_codebase-0.1.16/talk_codebase/utils.py
+-rw-r--r--   0        0        0     2099 1970-01-01 00:00:00.000000 talk_codebase-0.1.16/PKG-INFO
```

### Comparing `talk_codebase-0.1.15/README.md` & `talk_codebase-0.1.16/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.15/pyproject.toml` & `talk_codebase-0.1.16/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.15"
+version = "0.1.16"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
@@ -13,14 +13,15 @@
 fire = "^0.5.0"
 openai = "^0.27.7"
 tiktoken = "^0.4.0"
 faiss-cpu = "^1.7.4"
 halo = "^0.0.31"
 urllib3 = "1.26.6"
 gitpython = "^3.1.31"
+questionary = "^1.10.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
```

### Comparing `talk_codebase-0.1.15/talk_codebase/cli.py` & `talk_codebase-0.1.16/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.15/talk_codebase/consts.py` & `talk_codebase-0.1.16/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.15/talk_codebase/utils.py` & `talk_codebase-0.1.16/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.15/PKG-INFO` & `talk_codebase-0.1.16/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.15
+Version: 0.1.16
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: langchain (>=0.0.181,<0.0.182)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
+Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: urllib3 (==1.26.6)
 Description-Content-Type: text/markdown
 
 # talk-codebase is a powerful tool for chatting with your codebase
 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
```

