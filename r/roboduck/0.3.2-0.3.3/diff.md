# Comparing `tmp/roboduck-0.3.2.tar.gz` & `tmp/roboduck-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/roboduck-0.3.2.tar", last modified: Sat May 27 04:20:13 2023, max compression
+gzip compressed data, was "dist/roboduck-0.3.3.tar", last modified: Sat May 27 04:22:25 2023, max compression
```

## Comparing `roboduck-0.3.2.tar` & `roboduck-0.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:20:13.000000 roboduck-0.3.2/
--rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.3.2/MANIFEST.in
--rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-27 04:20:13.000000 roboduck-0.3.2/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)    10360 2023-05-27 04:19:37.000000 roboduck-0.3.2/README.md
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.3.2/requirements.txt
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck/
--rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-05-27 04:19:58.000000 roboduck-0.3.2/roboduck/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck/cli/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.3.2/roboduck/cli/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     4134 2023-05-17 05:54:18.000000 roboduck-0.3.2/roboduck/cli/cli.py
--rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.3.2/roboduck/config.py
--rw-r--r--   0 hmamin     (501) staff       (20)    20180 2023-05-26 05:12:05.000000 roboduck-0.3.2/roboduck/debug.py
--rw-r--r--   0 hmamin     (501) staff       (20)    10255 2023-05-22 05:58:53.000000 roboduck-0.3.2/roboduck/decorators.py
--rw-r--r--   0 hmamin     (501) staff       (20)    11284 2023-05-18 04:08:24.000000 roboduck-0.3.2/roboduck/errors.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.3.2/roboduck/ipy_utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck/langchain/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.3.2/roboduck/langchain/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.3.2/roboduck/langchain/callbacks.py
--rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.3.2/roboduck/langchain/chat.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.3.2/roboduck/langchain/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     6280 2023-05-19 05:20:48.000000 roboduck-0.3.2/roboduck/logging.py
--rw-r--r--   0 hmamin     (501) staff       (20)     6016 2023-05-25 04:05:13.000000 roboduck-0.3.2/roboduck/magic.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck/prompts/
--rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.3.2/roboduck/prompts/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck/prompts/chat/
--rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.3.2/roboduck/prompts/chat/__template__.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.3.2/roboduck/prompts/chat/debug.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.3.2/roboduck/prompts/chat/debug_full.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.3.2/roboduck/prompts/chat/debug_full_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.3.2/roboduck/prompts/chat/debug_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-15 05:03:45.000000 roboduck-0.3.2/roboduck/prompts/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1314 2023-05-16 04:49:53.000000 roboduck-0.3.2/roboduck/shell.py
--rw-r--r--   0 hmamin     (501) staff       (20)    14365 2023-05-16 04:13:23.000000 roboduck-0.3.2/roboduck/utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck.egg-info/
--rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck.egg-info/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)      861 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck.egg-info/SOURCES.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck.egg-info/dependency_links.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck.egg-info/entry_points.txt
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck.egg-info/requires.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-05-27 04:20:13.000000 roboduck-0.3.2/roboduck.egg-info/top_level.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-05-27 04:20:13.000000 roboduck-0.3.2/setup.cfg
--rw-r--r--   0 hmamin     (501) staff       (20)      848 2023-05-17 05:17:44.000000 roboduck-0.3.2/setup.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/
+-rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.3.3/MANIFEST.in
+-rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-27 04:22:25.000000 roboduck-0.3.3/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)    10364 2023-05-27 04:22:10.000000 roboduck-0.3.3/README.md
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.3.3/requirements.txt
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck/
+-rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-05-27 04:22:13.000000 roboduck-0.3.3/roboduck/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck/cli/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.3.3/roboduck/cli/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     4134 2023-05-17 05:54:18.000000 roboduck-0.3.3/roboduck/cli/cli.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.3.3/roboduck/config.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    20180 2023-05-26 05:12:05.000000 roboduck-0.3.3/roboduck/debug.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    10255 2023-05-22 05:58:53.000000 roboduck-0.3.3/roboduck/decorators.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    11284 2023-05-18 04:08:24.000000 roboduck-0.3.3/roboduck/errors.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.3.3/roboduck/ipy_utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck/langchain/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.3.3/roboduck/langchain/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.3.3/roboduck/langchain/callbacks.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.3.3/roboduck/langchain/chat.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.3.3/roboduck/langchain/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6280 2023-05-19 05:20:48.000000 roboduck-0.3.3/roboduck/logging.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6016 2023-05-25 04:05:13.000000 roboduck-0.3.3/roboduck/magic.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck/prompts/
+-rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.3.3/roboduck/prompts/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck/prompts/chat/
+-rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.3.3/roboduck/prompts/chat/__template__.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.3.3/roboduck/prompts/chat/debug.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.3.3/roboduck/prompts/chat/debug_full.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.3.3/roboduck/prompts/chat/debug_full_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.3.3/roboduck/prompts/chat/debug_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-15 05:03:45.000000 roboduck-0.3.3/roboduck/prompts/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1314 2023-05-16 04:49:53.000000 roboduck-0.3.3/roboduck/shell.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14365 2023-05-16 04:13:23.000000 roboduck-0.3.3/roboduck/utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck.egg-info/
+-rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-27 04:22:24.000000 roboduck-0.3.3/roboduck.egg-info/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)      861 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck.egg-info/SOURCES.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-05-27 04:22:24.000000 roboduck-0.3.3/roboduck.egg-info/dependency_links.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck.egg-info/entry_points.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck.egg-info/requires.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck.egg-info/top_level.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-05-27 04:22:25.000000 roboduck-0.3.3/setup.cfg
+-rw-r--r--   0 hmamin     (501) staff       (20)      848 2023-05-17 05:17:44.000000 roboduck-0.3.3/setup.py
```

### Comparing `roboduck-0.3.2/README.md` & `roboduck-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-<p align="center">
+<div align="center">
 <img src="https://raw.githubusercontent.com/hdmamin/roboduck/main/data/images/roboduck_blue_banner.png" alt="roboduck logo">
 <p></p>
 <a href="https://hdmamin.github.io/roboduck/"><img src="https://img.shields.io/badge/Documentation-Online-blue.svg" alt="Documentation"></a>
 <a href="https://badge.fury.io/py/roboduck"><img src="https://badge.fury.io/py/roboduck.svg" alt="PyPI version"></a>
 <a href="https://github.com/hdmamin/roboduck/actions/workflows/main.yml"><img src="https://github.com/hdmamin/roboduck/actions/workflows/main.yml/badge.svg" alt="Build Status"></a>
 <a href="https://colab.research.google.com/github/hdmamin/roboduck/blob/main/notebooks/quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"></a>
 <p></p>
-</p>
+</div>
 
 **rubber duck debugging**: a method of debugging code by articulating a problem in spoken or written natural language. The name is a reference to a story in the book The Pragmatic Programmer in which a programmer would carry around a rubber duck and debug their code by forcing themselves to explain it, line-by-line, to the duck. [[1](https://en.wikipedia.org/wiki/Rubber_duck_debugging)]
 
 **robo duck debugging**: a bit like rubber duck debugging, but the duck talks back.
 
 ## About
```

### Comparing `roboduck-0.3.2/roboduck/__init__.py` & `roboduck-0.3.3/roboduck/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from roboduck.debug import duck, DuckDB, CodeCompletionCache
 from roboduck.langchain.chat import Chat, DummyChatModel
 from roboduck.config import update_config, load_config, set_openai_api_key
 from roboduck.ipy_utils import is_colab
 from roboduck.utils import available_models
 
 
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 set_openai_api_key()
 if is_colab():
     warnings.warn(
         'It looks like you\'re using Google Colab, which may make your '
         'roboduck experience slightly sub-optimal (e.g. typing can be a bit '
         'laggy).'
     )
```

### Comparing `roboduck-0.3.2/roboduck/cli/cli.py` & `roboduck-0.3.3/roboduck/cli/cli.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/config.py` & `roboduck-0.3.3/roboduck/config.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/debug.py` & `roboduck-0.3.3/roboduck/debug.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/decorators.py` & `roboduck-0.3.3/roboduck/decorators.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/errors.py` & `roboduck-0.3.3/roboduck/errors.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/ipy_utils.py` & `roboduck-0.3.3/roboduck/ipy_utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/langchain/callbacks.py` & `roboduck-0.3.3/roboduck/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/langchain/chat.py` & `roboduck-0.3.3/roboduck/langchain/chat.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/langchain/utils.py` & `roboduck-0.3.3/roboduck/langchain/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/logging.py` & `roboduck-0.3.3/roboduck/logging.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/magic.py` & `roboduck-0.3.3/roboduck/magic.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/prompts/chat/__template__.yaml` & `roboduck-0.3.3/roboduck/prompts/chat/__template__.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/prompts/chat/debug.yaml` & `roboduck-0.3.3/roboduck/prompts/chat/debug.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/prompts/chat/debug_full.yaml` & `roboduck-0.3.3/roboduck/prompts/chat/debug_full.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/prompts/chat/debug_full_stack_trace.yaml` & `roboduck-0.3.3/roboduck/prompts/chat/debug_full_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/prompts/chat/debug_stack_trace.yaml` & `roboduck-0.3.3/roboduck/prompts/chat/debug_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/prompts/utils.py` & `roboduck-0.3.3/roboduck/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/shell.py` & `roboduck-0.3.3/roboduck/shell.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck/utils.py` & `roboduck-0.3.3/roboduck/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/roboduck.egg-info/SOURCES.txt` & `roboduck-0.3.3/roboduck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.2/setup.py` & `roboduck-0.3.3/setup.py`

 * *Files identical despite different names*

