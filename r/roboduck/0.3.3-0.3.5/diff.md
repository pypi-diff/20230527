# Comparing `tmp/roboduck-0.3.3.tar.gz` & `tmp/roboduck-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/roboduck-0.3.3.tar", last modified: Sat May 27 04:22:25 2023, max compression
+gzip compressed data, was "dist/roboduck-0.3.5.tar", last modified: Sat May 27 04:33:43 2023, max compression
```

## Comparing `roboduck-0.3.3.tar` & `roboduck-0.3.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/
--rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.3.3/MANIFEST.in
--rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-27 04:22:25.000000 roboduck-0.3.3/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)    10364 2023-05-27 04:22:10.000000 roboduck-0.3.3/README.md
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.3.3/requirements.txt
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck/
--rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-05-27 04:22:13.000000 roboduck-0.3.3/roboduck/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck/cli/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.3.3/roboduck/cli/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     4134 2023-05-17 05:54:18.000000 roboduck-0.3.3/roboduck/cli/cli.py
--rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.3.3/roboduck/config.py
--rw-r--r--   0 hmamin     (501) staff       (20)    20180 2023-05-26 05:12:05.000000 roboduck-0.3.3/roboduck/debug.py
--rw-r--r--   0 hmamin     (501) staff       (20)    10255 2023-05-22 05:58:53.000000 roboduck-0.3.3/roboduck/decorators.py
--rw-r--r--   0 hmamin     (501) staff       (20)    11284 2023-05-18 04:08:24.000000 roboduck-0.3.3/roboduck/errors.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.3.3/roboduck/ipy_utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck/langchain/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.3.3/roboduck/langchain/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.3.3/roboduck/langchain/callbacks.py
--rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.3.3/roboduck/langchain/chat.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.3.3/roboduck/langchain/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     6280 2023-05-19 05:20:48.000000 roboduck-0.3.3/roboduck/logging.py
--rw-r--r--   0 hmamin     (501) staff       (20)     6016 2023-05-25 04:05:13.000000 roboduck-0.3.3/roboduck/magic.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck/prompts/
--rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.3.3/roboduck/prompts/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck/prompts/chat/
--rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.3.3/roboduck/prompts/chat/__template__.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.3.3/roboduck/prompts/chat/debug.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.3.3/roboduck/prompts/chat/debug_full.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.3.3/roboduck/prompts/chat/debug_full_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.3.3/roboduck/prompts/chat/debug_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-15 05:03:45.000000 roboduck-0.3.3/roboduck/prompts/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1314 2023-05-16 04:49:53.000000 roboduck-0.3.3/roboduck/shell.py
--rw-r--r--   0 hmamin     (501) staff       (20)    14365 2023-05-16 04:13:23.000000 roboduck-0.3.3/roboduck/utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck.egg-info/
--rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-27 04:22:24.000000 roboduck-0.3.3/roboduck.egg-info/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)      861 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck.egg-info/SOURCES.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-05-27 04:22:24.000000 roboduck-0.3.3/roboduck.egg-info/dependency_links.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck.egg-info/entry_points.txt
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck.egg-info/requires.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-05-27 04:22:25.000000 roboduck-0.3.3/roboduck.egg-info/top_level.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-05-27 04:22:25.000000 roboduck-0.3.3/setup.cfg
--rw-r--r--   0 hmamin     (501) staff       (20)      848 2023-05-17 05:17:44.000000 roboduck-0.3.3/setup.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/
+-rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.3.5/MANIFEST.in
+-rw-r--r--   0 hmamin     (501) staff       (20)    10575 2023-05-27 04:33:43.000000 roboduck-0.3.5/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)    10346 2023-05-27 04:23:03.000000 roboduck-0.3.5/README.md
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.3.5/requirements.txt
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck/
+-rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-05-27 04:33:21.000000 roboduck-0.3.5/roboduck/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck/cli/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.3.5/roboduck/cli/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     4134 2023-05-17 05:54:18.000000 roboduck-0.3.5/roboduck/cli/cli.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.3.5/roboduck/config.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    20180 2023-05-26 05:12:05.000000 roboduck-0.3.5/roboduck/debug.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    10255 2023-05-22 05:58:53.000000 roboduck-0.3.5/roboduck/decorators.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    11284 2023-05-18 04:08:24.000000 roboduck-0.3.5/roboduck/errors.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.3.5/roboduck/ipy_utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck/langchain/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.3.5/roboduck/langchain/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.3.5/roboduck/langchain/callbacks.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.3.5/roboduck/langchain/chat.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.3.5/roboduck/langchain/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6280 2023-05-19 05:20:48.000000 roboduck-0.3.5/roboduck/logging.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6016 2023-05-25 04:05:13.000000 roboduck-0.3.5/roboduck/magic.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck/prompts/
+-rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.3.5/roboduck/prompts/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck/prompts/chat/
+-rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.3.5/roboduck/prompts/chat/__template__.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.3.5/roboduck/prompts/chat/debug.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.3.5/roboduck/prompts/chat/debug_full.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.3.5/roboduck/prompts/chat/debug_full_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.3.5/roboduck/prompts/chat/debug_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-15 05:03:45.000000 roboduck-0.3.5/roboduck/prompts/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1314 2023-05-16 04:49:53.000000 roboduck-0.3.5/roboduck/shell.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14365 2023-05-16 04:13:23.000000 roboduck-0.3.5/roboduck/utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:33:43.000000 roboduck-0.3.5/roboduck.egg-info/
+-rw-r--r--   0 hmamin     (501) staff       (20)    10575 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)      861 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/SOURCES.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/dependency_links.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/entry_points.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/requires.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-05-27 04:33:42.000000 roboduck-0.3.5/roboduck.egg-info/top_level.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-05-27 04:33:43.000000 roboduck-0.3.5/setup.cfg
+-rw-r--r--   0 hmamin     (501) staff       (20)     1181 2023-05-27 04:33:17.000000 roboduck-0.3.5/setup.py
```

### Comparing `roboduck-0.3.3/README.md` & `roboduck-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 Many AI-powered dev tools help you write boilerplate more quickly, but the hardest and most time-consuming part of programming is often the last mile. Roboduck's goal is to help you understand and fix those bugs. It essentially embeds an LLM (large language model) in the Python interpreter, providing drop-in natural language replacements for Python's standard approaches to:  
 - debugging  
 - error handling  
 - logging  
 
 ## Quickstart
 
-# TODO add gifs
-
-
 ### Install
 
 ```
 pip install roboduck
 ```
 
 ### API Key Setup
```

### Comparing `roboduck-0.3.3/roboduck/__init__.py` & `roboduck-0.3.5/roboduck/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from roboduck.debug import duck, DuckDB, CodeCompletionCache
 from roboduck.langchain.chat import Chat, DummyChatModel
 from roboduck.config import update_config, load_config, set_openai_api_key
 from roboduck.ipy_utils import is_colab
 from roboduck.utils import available_models
 
 
-__version__ = '0.3.3'
+__version__ = '0.3.5'
 set_openai_api_key()
 if is_colab():
     warnings.warn(
         'It looks like you\'re using Google Colab, which may make your '
         'roboduck experience slightly sub-optimal (e.g. typing can be a bit '
         'laggy).'
     )
```

### Comparing `roboduck-0.3.3/roboduck/cli/cli.py` & `roboduck-0.3.5/roboduck/cli/cli.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/config.py` & `roboduck-0.3.5/roboduck/config.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/debug.py` & `roboduck-0.3.5/roboduck/debug.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/decorators.py` & `roboduck-0.3.5/roboduck/decorators.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/errors.py` & `roboduck-0.3.5/roboduck/errors.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/ipy_utils.py` & `roboduck-0.3.5/roboduck/ipy_utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/langchain/callbacks.py` & `roboduck-0.3.5/roboduck/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/langchain/chat.py` & `roboduck-0.3.5/roboduck/langchain/chat.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/langchain/utils.py` & `roboduck-0.3.5/roboduck/langchain/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/logging.py` & `roboduck-0.3.5/roboduck/logging.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/magic.py` & `roboduck-0.3.5/roboduck/magic.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/prompts/chat/__template__.yaml` & `roboduck-0.3.5/roboduck/prompts/chat/__template__.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/prompts/chat/debug.yaml` & `roboduck-0.3.5/roboduck/prompts/chat/debug.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/prompts/chat/debug_full.yaml` & `roboduck-0.3.5/roboduck/prompts/chat/debug_full.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/prompts/chat/debug_full_stack_trace.yaml` & `roboduck-0.3.5/roboduck/prompts/chat/debug_full_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/prompts/chat/debug_stack_trace.yaml` & `roboduck-0.3.5/roboduck/prompts/chat/debug_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/prompts/utils.py` & `roboduck-0.3.5/roboduck/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/shell.py` & `roboduck-0.3.5/roboduck/shell.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck/utils.py` & `roboduck-0.3.5/roboduck/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/roboduck.egg-info/SOURCES.txt` & `roboduck-0.3.5/roboduck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.3/setup.py` & `roboduck-0.3.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,20 +13,31 @@
     with open(path, 'r') as f:
         for row in f:
             if not row.startswith('__version__'):
                 continue
             return row.split(' = ')[-1].strip('\n').strip("'")
 
 
+def load_file(name):
+    """Load contents of file in the same directory as setup.py and return it as
+    a string.
+    """
+    path = os.path.join(os.path.dirname(__file__), name)
+    with open(path, 'r') as f:
+        return f.read()
+
+
 setuptools.setup(
     name='roboduck',
     version=version(),
     author='Harrison Mamin',
     author_email='harrisonmamin@gmail.com',
     description='A natural language debugger.',
+    long_description=load_file('README.md'),
+    long_description_content_type='text/markdown',
     install_requires=requirements(),
     packages=setuptools.find_packages(),
     package_data={
         'roboduck': ['**/*.yaml']
     },
     entry_points={'console_scripts': ['duck=roboduck.cli.cli:run']},
     include_package_data=True
```

