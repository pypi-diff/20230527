# Comparing `tmp/roboduck-0.3.0.tar.gz` & `tmp/roboduck-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboduck-0.3.0.tar", last modified: Wed May 24 04:02:13 2023, max compression
+gzip compressed data, was "dist/roboduck-0.3.1.tar", last modified: Sat May 27 04:15:34 2023, max compression
```

## Comparing `roboduck-0.3.0.tar` & `roboduck-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.194975 roboduck-0.3.0/
--rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.3.0/MANIFEST.in
--rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-24 04:02:13.194007 roboduck-0.3.0/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)     5067 2023-04-24 03:54:00.000000 roboduck-0.3.0/README.md
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.3.0/requirements.txt
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.181743 roboduck-0.3.0/roboduck/
--rw-r--r--   0 hmamin     (501) staff       (20)      282 2023-05-24 04:01:58.000000 roboduck-0.3.0/roboduck/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.185418 roboduck-0.3.0/roboduck/cli/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.3.0/roboduck/cli/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     4134 2023-05-17 05:54:18.000000 roboduck-0.3.0/roboduck/cli/cli.py
--rw-r--r--   0 hmamin     (501) staff       (20)     6981 2023-05-16 03:52:42.000000 roboduck-0.3.0/roboduck/config.py
--rw-r--r--   0 hmamin     (501) staff       (20)    20177 2023-05-22 05:37:54.000000 roboduck-0.3.0/roboduck/debug.py
--rw-r--r--   0 hmamin     (501) staff       (20)    10255 2023-05-22 05:58:53.000000 roboduck-0.3.0/roboduck/decorators.py
--rw-r--r--   0 hmamin     (501) staff       (20)    11284 2023-05-18 04:08:24.000000 roboduck-0.3.0/roboduck/errors.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5326 2023-05-16 04:48:56.000000 roboduck-0.3.0/roboduck/ipy_utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.187955 roboduck-0.3.0/roboduck/langchain/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.3.0/roboduck/langchain/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.3.0/roboduck/langchain/callbacks.py
--rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.3.0/roboduck/langchain/chat.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.3.0/roboduck/langchain/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     6280 2023-05-19 05:20:48.000000 roboduck-0.3.0/roboduck/logging.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5783 2023-05-18 04:01:27.000000 roboduck-0.3.0/roboduck/magic.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.188840 roboduck-0.3.0/roboduck/prompts/
--rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.3.0/roboduck/prompts/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.193391 roboduck-0.3.0/roboduck/prompts/chat/
--rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.3.0/roboduck/prompts/chat/__template__.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2131 2023-04-17 04:48:07.000000 roboduck-0.3.0/roboduck/prompts/chat/debug.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2178 2023-04-17 04:48:07.000000 roboduck-0.3.0/roboduck/prompts/chat/debug_full.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2106 2023-04-17 04:48:07.000000 roboduck-0.3.0/roboduck/prompts/chat/debug_full_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2075 2023-04-17 04:48:07.000000 roboduck-0.3.0/roboduck/prompts/chat/debug_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-15 05:03:45.000000 roboduck-0.3.0/roboduck/prompts/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1314 2023-05-16 04:49:53.000000 roboduck-0.3.0/roboduck/shell.py
--rw-r--r--   0 hmamin     (501) staff       (20)    14365 2023-05-16 04:13:23.000000 roboduck-0.3.0/roboduck/utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-24 04:02:13.184405 roboduck-0.3.0/roboduck.egg-info/
--rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-24 04:02:12.000000 roboduck-0.3.0/roboduck.egg-info/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)      861 2023-05-24 04:02:13.000000 roboduck-0.3.0/roboduck.egg-info/SOURCES.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-05-24 04:02:12.000000 roboduck-0.3.0/roboduck.egg-info/dependency_links.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-05-24 04:02:12.000000 roboduck-0.3.0/roboduck.egg-info/entry_points.txt
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-05-24 04:02:12.000000 roboduck-0.3.0/roboduck.egg-info/requires.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-05-24 04:02:13.000000 roboduck-0.3.0/roboduck.egg-info/top_level.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-05-24 04:02:13.195156 roboduck-0.3.0/setup.cfg
--rw-r--r--   0 hmamin     (501) staff       (20)      848 2023-05-17 05:17:44.000000 roboduck-0.3.0/setup.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:15:34.000000 roboduck-0.3.1/
+-rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.3.1/MANIFEST.in
+-rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-27 04:15:34.000000 roboduck-0.3.1/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)    10364 2023-05-27 04:14:23.000000 roboduck-0.3.1/README.md
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.3.1/requirements.txt
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:15:34.000000 roboduck-0.3.1/roboduck/
+-rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-05-27 04:15:20.000000 roboduck-0.3.1/roboduck/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:15:34.000000 roboduck-0.3.1/roboduck/cli/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.3.1/roboduck/cli/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     4134 2023-05-17 05:54:18.000000 roboduck-0.3.1/roboduck/cli/cli.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.3.1/roboduck/config.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    20180 2023-05-26 05:12:05.000000 roboduck-0.3.1/roboduck/debug.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    10255 2023-05-22 05:58:53.000000 roboduck-0.3.1/roboduck/decorators.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    11284 2023-05-18 04:08:24.000000 roboduck-0.3.1/roboduck/errors.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.3.1/roboduck/ipy_utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:15:34.000000 roboduck-0.3.1/roboduck/langchain/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.3.1/roboduck/langchain/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.3.1/roboduck/langchain/callbacks.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.3.1/roboduck/langchain/chat.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.3.1/roboduck/langchain/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6280 2023-05-19 05:20:48.000000 roboduck-0.3.1/roboduck/logging.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6016 2023-05-25 04:05:13.000000 roboduck-0.3.1/roboduck/magic.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:15:34.000000 roboduck-0.3.1/roboduck/prompts/
+-rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.3.1/roboduck/prompts/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:15:34.000000 roboduck-0.3.1/roboduck/prompts/chat/
+-rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.3.1/roboduck/prompts/chat/__template__.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.3.1/roboduck/prompts/chat/debug.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.3.1/roboduck/prompts/chat/debug_full.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.3.1/roboduck/prompts/chat/debug_full_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.3.1/roboduck/prompts/chat/debug_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-15 05:03:45.000000 roboduck-0.3.1/roboduck/prompts/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1314 2023-05-16 04:49:53.000000 roboduck-0.3.1/roboduck/shell.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14365 2023-05-16 04:13:23.000000 roboduck-0.3.1/roboduck/utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-27 04:15:34.000000 roboduck-0.3.1/roboduck.egg-info/
+-rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-27 04:15:32.000000 roboduck-0.3.1/roboduck.egg-info/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)      861 2023-05-27 04:15:33.000000 roboduck-0.3.1/roboduck.egg-info/SOURCES.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-05-27 04:15:32.000000 roboduck-0.3.1/roboduck.egg-info/dependency_links.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-05-27 04:15:32.000000 roboduck-0.3.1/roboduck.egg-info/entry_points.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-05-27 04:15:33.000000 roboduck-0.3.1/roboduck.egg-info/requires.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-05-27 04:15:33.000000 roboduck-0.3.1/roboduck.egg-info/top_level.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-05-27 04:15:34.000000 roboduck-0.3.1/setup.cfg
+-rw-r--r--   0 hmamin     (501) staff       (20)      848 2023-05-17 05:17:44.000000 roboduck-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `roboduck-0.3.0/roboduck/cli/cli.py` & `roboduck-0.3.1/roboduck/cli/cli.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/roboduck/config.py` & `roboduck-0.3.1/roboduck/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -162,12 +162,20 @@
             msg = 'Openai api key must either be passed into this function ' \
                   f'or stored in {config_path} with field name ' \
                   f'{var_name.lower()}. No key found.'
             if strict:
                 raise RuntimeError(msg)
             else:
                 warnings.warn(msg + ' Not raising error because strict=False, '
-                              'but openai API will not be available.')
+                              'but openai API will not be available until you '
+                              'make key available via one of these methods.')
                 return
+    if not key.startswith('sk-'):
+        partially_redacted_key = key[:4] + '*'*max(0, len(key) - 4)
+        warnings.warn(
+            f'Your openai api key ({partially_redacted_key}) looks unusual. '
+            f'Are you sure it\'s correct? (Key is partially redacted in '
+            f'warning to err on the side of caution.)'
+        )
     os.environ[var_name] = key
     if update_config_:
         update_config(config_path, **{var_name.lower(): key})
```

### Comparing `roboduck-0.3.0/roboduck/debug.py` & `roboduck-0.3.1/roboduck/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 second to last line where you might normally call `breakpoint()`.
 
 ```
 from roboduck import duck
 
 def bubble_sort(nums):
     for i in range(len(nums)):
-        for j in range(len(nums)):
+        for j in range(len(nums) - 1):
             if nums[j] > nums[j + 1]:
                 nums[j + 1] = nums[j]
                 nums[j] = nums[j + 1]
                 duck()   # <--------------------------- instead of breakpoint()
     return nums
 
 nums = [3, 1, 9, 2, 1]
@@ -45,15 +45,15 @@
 
 @store_class_defaults(attr_filter=lambda x: x.startswith('last_'))
 class CodeCompletionCache:
     """Stores values related to the last completion from DuckDB in a way that
     a. our `duck` jupyter magic can access, and
     b. allows us to easily reset all defaults
 
-    The magic only needs to access it in insert mode (-i flag) to insert
+    The magic only needs to access it in Paste mode (-p flag) to insert
     the fixed code snippet into a new code cell.
     """
 
     # LLM full completion.
     last_completion = ''
     # LLM natural language explanation.
     last_explanation = ''
```

### Comparing `roboduck-0.3.0/roboduck/decorators.py` & `roboduck-0.3.1/roboduck/decorators.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/roboduck/errors.py` & `roboduck-0.3.1/roboduck/errors.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/roboduck/ipy_utils.py` & `roboduck-0.3.1/roboduck/ipy_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,8 +166,21 @@
 
     start_md5 = file_md5(file_path)
     display(Javascript('IPython.notebook.save_checkpoint();'))
     current_md5 = start_md5
 
     while start_md5 == current_md5:
         time.sleep(1)
-        current_md5 = file_md5(file_path)
+        current_md5 = file_md5(file_path)
+
+
+def is_colab(shell=None):
+    """Check if we're currently in google colab.
+
+    Parameters
+    ----------
+    shell : None or IPython.core.interactiveshell.InteractiveShell
+        Colab uses a custom shell class so we can use this to distinguish
+        between colab and jupyter.
+    """
+    shell = shell or get_ipython()
+    return 'google.colab' in str(type(shell))
```

### Comparing `roboduck-0.3.0/roboduck/langchain/callbacks.py` & `roboduck-0.3.1/roboduck/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/roboduck/langchain/chat.py` & `roboduck-0.3.1/roboduck/langchain/chat.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/roboduck/langchain/utils.py` & `roboduck-0.3.1/roboduck/langchain/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/roboduck/logging.py` & `roboduck-0.3.1/roboduck/logging.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/roboduck/magic.py` & `roboduck-0.3.1/roboduck/magic.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from IPython.core.magic import line_magic, magics_class, Magics
 from IPython.core.magic_arguments import argument, magic_arguments, \
     parse_argstring
 import sys
 import warnings
 
 from roboduck.debug import DuckDB, CodeCompletionCache
+from roboduck.ipy_utils import is_colab
 
 
 @magics_class
 class DebugMagic(Magics):
     """Enter a conversational debugging session after an error is thrown by a
     jupyter notebook code cell.
 
@@ -79,14 +80,17 @@
         change persist, at least until the user changes it again.
         """
         args = parse_argstring(self.duck, line)
         if args.prompt:
             warnings.warn('Support for custom prompts is somewhat limited - '
                           'your prompt must use the default parse_func '
                           '(roboduck.utils.parse_completion).')
+        if args.p and is_colab(self.shell):
+            warnings.warn('Paste mode is unavailable in google colab, which '
+                          'you appear to be using. Ignoring -p flag.')
         if args.i:
             old_cls = self.shell.debugger_cls
             if args.prompt:
                 new_cls = partial(DuckDB, prompt=args.prompt)
             else:
                 new_cls = DuckDB
             try:
```

### Comparing `roboduck-0.3.0/roboduck/prompts/chat/__template__.yaml` & `roboduck-0.3.1/roboduck/prompts/chat/__template__.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/roboduck/prompts/chat/debug.yaml` & `roboduck-0.3.1/roboduck/prompts/chat/debug_full.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 kwargs:
-    model_name: gpt-3.5-turbo
+    model_name: gpt-4
     max_tokens: 512
     temperature: 0.0
     top_p: 1.0
     frequency_penalty: 0.0
     presence_penalty: 0.0
     # Try to reduce probability of section titles - gpt3.5 sometimes ignores
     # those instructions. {section, Section}
@@ -14,31 +14,34 @@
       - QUESTION
       - section 3
 system: |-
   You are an incredibly effective AI programming assistant embedded in the Python interpreter. You have in-depth knowledge across a broad range of sub-fields within computer science, software development, and data science, and your goal is to help programmers resolve their most challenging bugs. Be concise and use simple language as you assist the user with this live debugging session.
 # First key defines default message type.
 user:
   contextful: |-
-    I'm debugging some code that is not working as expected and I need your help. First read my question, then examine the problematic code snippet and the current program state. Your response must have exactly two sections (1. natural language explanation, and 2. code) separated by an empty line. It is critical that you adhere to the response format below - do NOT include section titles of any kind. In section 1, use plain English to answer my question. If you don't know the answer, section 1 should instead list a few possible explanations or actions I could take in order to identify the issue. If it would contribute to a more helpful answer, use section 2 to provide a corrected version of the input code snippet (leave section 2 empty otherwise). If section 2 is not empty, it must be entirely enclosed in one pair of triple backticks ("```") and contain only python code - it cannot include any English explanation outside of code comments or docstrings.
+    I'm debugging some code in a {file_type}. It's not working as expected and I need your help. First read my question, then examine the problematic code snippet and the current program state. Your response must have exactly two sections (1. natural language explanation, and 2. code) separated by an empty line. It is critical that you adhere to the response format below - do NOT include section titles of any kind. In section 1, use plain English to answer my question. If you don't know the answer, section 1 should instead list a few possible explanations or actions I could take in order to identify the issue. If it would contribute to a more helpful answer, use section 2 to provide a corrected version of the input code snippet (leave section 2 empty otherwise). If section 2 is not empty, it must be entirely enclosed in one pair of triple backticks ("```") and contain only python code - it cannot include any English explanation outside of code comments or docstrings.
 
     QUESTION:
     {question}
 
+    FULL CODE:
+    {full_code}
+    
     CODE SNIPPET:
     {code}
 
     NEXT LINE TO EXECUTE:
     {next_line}
 
     LOCAL VARIABLES:
     {local_vars}
 
     GLOBAL VARIABLES:
     {global_vars}
-    
+
     RESPONSE FORMAT:
     {{ natural language answer }}
 
     ```
     {{ working python code }}
     ```
   contextless: |-
```

### Comparing `roboduck-0.3.0/roboduck/prompts/chat/debug_full.yaml` & `roboduck-0.3.1/roboduck/prompts/chat/debug.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 kwargs:
-    model_name: gpt-3.5-turbo
+    model_name: gpt-4
     max_tokens: 512
     temperature: 0.0
     top_p: 1.0
     frequency_penalty: 0.0
     presence_penalty: 0.0
     # Try to reduce probability of section titles - gpt3.5 sometimes ignores
     # those instructions. {section, Section}
@@ -14,34 +14,31 @@
       - QUESTION
       - section 3
 system: |-
   You are an incredibly effective AI programming assistant embedded in the Python interpreter. You have in-depth knowledge across a broad range of sub-fields within computer science, software development, and data science, and your goal is to help programmers resolve their most challenging bugs. Be concise and use simple language as you assist the user with this live debugging session.
 # First key defines default message type.
 user:
   contextful: |-
-    I'm debugging some code in a {file_type}. It's not working as expected and I need your help. First read my question, then examine the problematic code snippet and the current program state. Your response must have exactly two sections (1. natural language explanation, and 2. code) separated by an empty line. It is critical that you adhere to the response format below - do NOT include section titles of any kind. In section 1, use plain English to answer my question. If you don't know the answer, section 1 should instead list a few possible explanations or actions I could take in order to identify the issue. If it would contribute to a more helpful answer, use section 2 to provide a corrected version of the input code snippet (leave section 2 empty otherwise). If section 2 is not empty, it must be entirely enclosed in one pair of triple backticks ("```") and contain only python code - it cannot include any English explanation outside of code comments or docstrings.
+    I'm debugging some code that is not working as expected and I need your help. First read my question, then examine the problematic code snippet and the current program state. Your response must have exactly two sections (1. natural language explanation, and 2. code) separated by an empty line. It is critical that you adhere to the response format below - do NOT include section titles of any kind. In section 1, use plain English to answer my question. If you don't know the answer, section 1 should instead list a few possible explanations or actions I could take in order to identify the issue. If it would contribute to a more helpful answer, use section 2 to provide a corrected version of the input code snippet (leave section 2 empty otherwise). If section 2 is not empty, it must be entirely enclosed in one pair of triple backticks ("```") and contain only python code - it cannot include any English explanation outside of code comments or docstrings.
 
     QUESTION:
     {question}
 
-    FULL CODE:
-    {full_code}
-    
     CODE SNIPPET:
     {code}
 
     NEXT LINE TO EXECUTE:
     {next_line}
 
     LOCAL VARIABLES:
     {local_vars}
 
     GLOBAL VARIABLES:
     {global_vars}
-
+    
     RESPONSE FORMAT:
     {{ natural language answer }}
 
     ```
     {{ working python code }}
     ```
   contextless: |-
```

### Comparing `roboduck-0.3.0/roboduck/prompts/chat/debug_full_stack_trace.yaml` & `roboduck-0.3.1/roboduck/prompts/chat/debug_full_stack_trace.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 kwargs:
-    model_name: gpt-3.5-turbo
+    model_name: gpt-4
     max_tokens: 512
     temperature: 0.0
     top_p: 1.0
     frequency_penalty: 0.0
     presence_penalty: 0.0
     # Try to reduce probability of section titles - gpt3.5 sometimes ignores
     # those instructions. {section, Section}
```

### Comparing `roboduck-0.3.0/roboduck/prompts/chat/debug_stack_trace.yaml` & `roboduck-0.3.1/roboduck/prompts/chat/debug_stack_trace.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 kwargs:
-    model_name: gpt-3.5-turbo
+    model_name: gpt-4
     max_tokens: 512
     temperature: 0.0
     top_p: 1.0
     frequency_penalty: 0.0
     presence_penalty: 0.0
     # Try to reduce probability of section titles - gpt3.5 sometimes ignores
     # those instructions. {section, Section}
```

### Comparing `roboduck-0.3.0/roboduck/prompts/utils.py` & `roboduck-0.3.1/roboduck/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/roboduck/shell.py` & `roboduck-0.3.1/roboduck/shell.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/roboduck/utils.py` & `roboduck-0.3.1/roboduck/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/roboduck.egg-info/SOURCES.txt` & `roboduck-0.3.1/roboduck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboduck-0.3.0/setup.py` & `roboduck-0.3.1/setup.py`

 * *Files identical despite different names*

