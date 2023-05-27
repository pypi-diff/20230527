# Comparing `tmp/chatcmd-1.0.25.tar.gz` & `tmp/chatcmd-1.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.25.tar", last modified: Sat May 27 21:18:48 2023, max compression
+gzip compressed data, was "chatcmd-1.0.26.tar", last modified: Sat May 27 21:22:40 2023, max compression
```

## Comparing `chatcmd-1.0.25.tar` & `chatcmd-1.0.26.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:18:48.458632 chatcmd-1.0.25/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.25/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:18:48.458294 chatcmd-1.0.25/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 21:18:27.000000 chatcmd-1.0.25/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:18:48.455344 chatcmd-1.0.25/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.25/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-27 20:45:29.000000 chatcmd-1.0.25/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3464 2023-05-27 21:18:27.000000 chatcmd-1.0.25/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3754 2023-05-27 21:02:39.000000 chatcmd-1.0.25/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     2373 2023-05-27 21:05:11.000000 chatcmd-1.0.25/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2619 2023-05-27 21:18:14.000000 chatcmd-1.0.25/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:18:48.457800 chatcmd-1.0.25/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:18:48.000000 chatcmd-1.0.25/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 21:18:48.000000 chatcmd-1.0.25/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 21:18:48.000000 chatcmd-1.0.25/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 21:18:48.000000 chatcmd-1.0.25/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       44 2023-05-27 21:18:48.000000 chatcmd-1.0.25/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 21:18:48.000000 chatcmd-1.0.25/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1795 2023-05-27 21:18:27.000000 chatcmd-1.0.25/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 21:18:48.458715 chatcmd-1.0.25/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      556 2023-05-27 21:18:27.000000 chatcmd-1.0.25/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:22:40.616708 chatcmd-1.0.26/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.26/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:22:40.616457 chatcmd-1.0.26/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 21:22:25.000000 chatcmd-1.0.26/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:22:40.613981 chatcmd-1.0.26/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.26/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-27 20:45:29.000000 chatcmd-1.0.26/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3464 2023-05-27 21:22:25.000000 chatcmd-1.0.26/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3754 2023-05-27 21:02:39.000000 chatcmd-1.0.26/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     2373 2023-05-27 21:05:11.000000 chatcmd-1.0.26/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2628 2023-05-27 21:22:25.000000 chatcmd-1.0.26/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:22:40.616075 chatcmd-1.0.26/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:22:40.000000 chatcmd-1.0.26/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 21:22:40.000000 chatcmd-1.0.26/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 21:22:40.000000 chatcmd-1.0.26/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 21:22:40.000000 chatcmd-1.0.26/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       44 2023-05-27 21:22:40.000000 chatcmd-1.0.26/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 21:22:40.000000 chatcmd-1.0.26/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1795 2023-05-27 21:22:25.000000 chatcmd-1.0.26/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 21:22:40.616786 chatcmd-1.0.26/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      556 2023-05-27 21:22:25.000000 chatcmd-1.0.26/setup.py
```

### Comparing `chatcmd-1.0.25/LICENSE` & `chatcmd-1.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.25/PKG-INFO` & `chatcmd-1.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.25
+Version: 1.0.26
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -65,17 +65,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.25-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.26-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.25
+    Successfully installed chatcmd-1.0.26
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.25/README.md` & `chatcmd-1.0.26/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.25-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.26-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.25
+    Successfully installed chatcmd-1.0.26
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.25/chatcmd/api.py` & `chatcmd-1.0.26/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.25/chatcmd/chatcmd.py` & `chatcmd-1.0.26/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print(color_text('ChatCMD','green')+' 1.0.25')
+            print(color_text('ChatCMD','green')+' 1.0.26')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.25/chatcmd/commands.py` & `chatcmd-1.0.26/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.25/chatcmd/helpers.py` & `chatcmd-1.0.26/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.25/chatcmd/lookup.py` & `chatcmd-1.0.26/chatcmd/lookup.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 def lookup(prompt, api_key):
     try:
         if validate_api_key(api_key) is False:
             error_msg("Error 1009: API key is invalid or missing")
             exit()
 
         prompt = prompt
-        print(f"Looking up: {prompt}...\n")
+        print(color_text("Looking up...\n",'yellow')
 
         stop_keywords = ["###", "END", "stop", "Command:", "Syntax:", "Usage:","The command to install MySQL on Windows is:"]
         response = openai.Completion.create(
             engine='text-davinci-003',
             prompt=f"Please help me with a CLI command lookup, I only need the command without any extra information: Show me the command for {prompt}",
             max_tokens=70,
             n=1,
```

### Comparing `chatcmd-1.0.25/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.26/chatcmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.25
+Version: 1.0.26
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -65,17 +65,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.25-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.26-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.25
+    Successfully installed chatcmd-1.0.26
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.25/pyproject.toml` & `chatcmd-1.0.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "colorama >=0.4.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.25"
+version = "1.0.26"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.25/setup.py` & `chatcmd-1.0.26/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.25",
+    version="1.0.26",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

