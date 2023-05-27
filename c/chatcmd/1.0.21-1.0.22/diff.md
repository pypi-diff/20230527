# Comparing `tmp/chatcmd-1.0.21.tar.gz` & `tmp/chatcmd-1.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.21.tar", last modified: Sat May 27 21:00:23 2023, max compression
+gzip compressed data, was "chatcmd-1.0.22.tar", last modified: Sat May 27 21:06:35 2023, max compression
```

## Comparing `chatcmd-1.0.21.tar` & `chatcmd-1.0.22.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:00:23.694071 chatcmd-1.0.21/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.21/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:00:23.693776 chatcmd-1.0.21/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 21:00:10.000000 chatcmd-1.0.21/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:00:23.690731 chatcmd-1.0.21/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.21/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-27 20:45:29.000000 chatcmd-1.0.21/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3464 2023-05-27 21:00:10.000000 chatcmd-1.0.21/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3769 2023-05-27 20:45:29.000000 chatcmd-1.0.21/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     2442 2023-05-27 20:15:43.000000 chatcmd-1.0.21/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2594 2023-05-27 21:00:10.000000 chatcmd-1.0.21/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:00:23.693366 chatcmd-1.0.21/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:00:23.000000 chatcmd-1.0.21/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 21:00:23.000000 chatcmd-1.0.21/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 21:00:23.000000 chatcmd-1.0.21/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 21:00:23.000000 chatcmd-1.0.21/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       44 2023-05-27 21:00:23.000000 chatcmd-1.0.21/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 21:00:23.000000 chatcmd-1.0.21/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1795 2023-05-27 21:00:10.000000 chatcmd-1.0.21/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 21:00:23.694167 chatcmd-1.0.21/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      556 2023-05-27 21:00:10.000000 chatcmd-1.0.21/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:06:35.888098 chatcmd-1.0.22/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.22/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:06:35.887762 chatcmd-1.0.22/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 21:06:23.000000 chatcmd-1.0.22/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:06:35.884730 chatcmd-1.0.22/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.22/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-27 20:45:29.000000 chatcmd-1.0.22/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3464 2023-05-27 21:06:23.000000 chatcmd-1.0.22/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3754 2023-05-27 21:02:39.000000 chatcmd-1.0.22/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     2373 2023-05-27 21:05:11.000000 chatcmd-1.0.22/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2594 2023-05-27 21:06:23.000000 chatcmd-1.0.22/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:06:35.887270 chatcmd-1.0.22/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:06:35.000000 chatcmd-1.0.22/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 21:06:35.000000 chatcmd-1.0.22/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 21:06:35.000000 chatcmd-1.0.22/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 21:06:35.000000 chatcmd-1.0.22/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       44 2023-05-27 21:06:35.000000 chatcmd-1.0.22/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 21:06:35.000000 chatcmd-1.0.22/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1795 2023-05-27 21:06:23.000000 chatcmd-1.0.22/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 21:06:35.888198 chatcmd-1.0.22/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      556 2023-05-27 21:06:23.000000 chatcmd-1.0.22/setup.py
```

### Comparing `chatcmd-1.0.21/LICENSE` & `chatcmd-1.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.21/PKG-INFO` & `chatcmd-1.0.22/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.21
+Version: 1.0.22
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
-    Using cached chatcmd-1.0.21-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.22-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.21
+    Successfully installed chatcmd-1.0.22
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.21/README.md` & `chatcmd-1.0.22/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.21-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.22-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.21
+    Successfully installed chatcmd-1.0.22
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.21/chatcmd/api.py` & `chatcmd-1.0.22/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.21/chatcmd/chatcmd.py` & `chatcmd-1.0.22/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print(color_text('ChatCMD','green')+' 1.0.21')
+            print(color_text('ChatCMD','green')+' 1.0.22')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.21/chatcmd/commands.py` & `chatcmd-1.0.22/chatcmd/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,13 +94,13 @@
     size = file_size_bytes
     unit_index = 0
 
     while size >= 1024 and unit_index < len(units)-1:
         size /= 1024
         unit_index += 1
 
-    print(f"\nDB File size: \033[32m{size:.2f} {units[unit_index]}\033[0m\n")
+    print(f"\nDB File size: {size:.2f} {units[unit_index]}\n")
 
 def get_commands_count(conn, cursor):
     cursor.execute('SELECT COUNT(*) FROM history')
     count = cursor.fetchone()[0]
     return count
```

### Comparing `chatcmd-1.0.21/chatcmd/helpers.py` & `chatcmd-1.0.22/chatcmd/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,16 +38,14 @@
 
 def success_msg(text):
     print("\n"+color_text(text, 'green'))
 
 def error_msg(text):
     print("\n"+color_text(text, 'red'))
     exit()
-#     print("\n"+color_text(text.split('.')[0], 'red'))
-#     exit()
 
 def warning_msg(text):
     print("\n"+color_text(text, 'yellow'))
 
 def clear_input(input):
     input = re.sub('[^a-zA-Z0-9 -_=]', '', input.strip())
     return input
@@ -72,12 +70,12 @@
         if system == 'Darwin':  # macOS
             subprocess.run(['pbcopy'], input=text, encoding='utf-8')
         elif system == 'Linux':  # Linux
             subprocess.run(['xclip', '-selection', 'clipboard'], input=text, encoding='utf-8')
         elif system == 'Windows':  # Windows
             subprocess.run(['clip'], input=text, encoding='utf-8', shell=True)
     except Exception as e:
-        error_msg("Error 1018: Failed ot copy command. "+str(e))
+        error_msg("Error 1018: Failed to copy command. "+str(e))
 
 def get_line_number():
     frame = inspect.currentframe().f_back
     return frame.f_lineno
```

### Comparing `chatcmd-1.0.21/chatcmd/lookup.py` & `chatcmd-1.0.22/chatcmd/lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 def lookup(prompt, api_key):
     try:
         if validate_api_key(api_key) is False:
             error_msg("Error 1009: API key is invalid or missing")
             exit()
 
         prompt = prompt
-        print(color_text(f"Looking up:"+prompt+"...\n",'green'))
+        print(color_text("Looking up: "+prompt+"...\n",'green'))
 
         stop_keywords = ["###", "END", "stop", "Command:", "Syntax:", "Usage:"]
         response = openai.Completion.create(
             engine='text-davinci-003',
             prompt=f"Please help me with a CLI command lookup, I only need the command without any extra information: Show me the command for {prompt}",
             max_tokens=70,
             n=1,
```

### Comparing `chatcmd-1.0.21/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.22/chatcmd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.21
+Version: 1.0.22
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
-    Using cached chatcmd-1.0.21-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.22-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.21
+    Successfully installed chatcmd-1.0.22
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.21/pyproject.toml` & `chatcmd-1.0.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "colorama >=0.4.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.21"
+version = "1.0.22"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.21/setup.py` & `chatcmd-1.0.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.21",
+    version="1.0.22",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

