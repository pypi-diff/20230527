# Comparing `tmp/chatcmd-1.0.18.tar.gz` & `tmp/chatcmd-1.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.18.tar", last modified: Sat May 27 20:42:19 2023, max compression
+gzip compressed data, was "chatcmd-1.0.19.tar", last modified: Sat May 27 20:47:46 2023, max compression
```

## Comparing `chatcmd-1.0.18.tar` & `chatcmd-1.0.19.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 20:42:19.587129 chatcmd-1.0.18/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.18/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 20:42:19.586608 chatcmd-1.0.18/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 20:37:44.000000 chatcmd-1.0.18/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 20:42:19.583340 chatcmd-1.0.18/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.18/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1759 2023-05-27 20:01:41.000000 chatcmd-1.0.18/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3461 2023-05-27 20:37:44.000000 chatcmd-1.0.18/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3768 2023-05-27 20:35:35.000000 chatcmd-1.0.18/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     2442 2023-05-27 20:15:43.000000 chatcmd-1.0.18/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2601 2023-05-27 20:01:15.000000 chatcmd-1.0.18/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 20:42:19.586029 chatcmd-1.0.18/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 20:42:19.000000 chatcmd-1.0.18/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 20:42:19.000000 chatcmd-1.0.18/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 20:42:19.000000 chatcmd-1.0.18/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 20:42:19.000000 chatcmd-1.0.18/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       44 2023-05-27 20:42:19.000000 chatcmd-1.0.18/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 20:42:19.000000 chatcmd-1.0.18/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1795 2023-05-27 20:42:09.000000 chatcmd-1.0.18/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 20:42:19.587278 chatcmd-1.0.18/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      556 2023-05-27 20:37:44.000000 chatcmd-1.0.18/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 20:47:46.152341 chatcmd-1.0.19/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.19/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 20:47:46.151847 chatcmd-1.0.19/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 20:47:17.000000 chatcmd-1.0.19/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 20:47:46.148792 chatcmd-1.0.19/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.19/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-27 20:45:29.000000 chatcmd-1.0.19/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3464 2023-05-27 20:47:17.000000 chatcmd-1.0.19/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3769 2023-05-27 20:45:29.000000 chatcmd-1.0.19/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     2442 2023-05-27 20:15:43.000000 chatcmd-1.0.19/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2602 2023-05-27 20:45:29.000000 chatcmd-1.0.19/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 20:47:46.151383 chatcmd-1.0.19/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 20:47:46.000000 chatcmd-1.0.19/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 20:47:46.000000 chatcmd-1.0.19/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 20:47:46.000000 chatcmd-1.0.19/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 20:47:46.000000 chatcmd-1.0.19/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       44 2023-05-27 20:47:46.000000 chatcmd-1.0.19/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 20:47:46.000000 chatcmd-1.0.19/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1795 2023-05-27 20:46:39.000000 chatcmd-1.0.19/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 20:47:46.152496 chatcmd-1.0.19/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      556 2023-05-27 20:47:17.000000 chatcmd-1.0.19/setup.py
```

### Comparing `chatcmd-1.0.18/LICENSE` & `chatcmd-1.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.18/PKG-INFO` & `chatcmd-1.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.18
+Version: 1.0.19
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
-    Using cached chatcmd-1.0.18-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.19-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.18
+    Successfully installed chatcmd-1.0.19
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.18/README.md` & `chatcmd-1.0.19/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.18-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.19-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.18
+    Successfully installed chatcmd-1.0.19
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.18/chatcmd/api.py` & `chatcmd-1.0.19/chatcmd/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sqlite3
-from helpers import *
+from .helpers import *
 
 def get_api_key(conn, cursor):
     try:
         cursor.execute('CREATE TABLE IF NOT EXISTS config (id INTEGER PRIMARY KEY, api_key TEXT)')
         conn.commit()
 
         cursor.execute('INSERT OR IGNORE INTO config (id, api_key) VALUES(?,?)', [1,None])
```

### Comparing `chatcmd-1.0.18/chatcmd/chatcmd.py` & `chatcmd-1.0.19/chatcmd/chatcmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
   -h, --help                        display this screen.
   -v, --version                     display ChatCMD version.
   -i, --library-info                display library information.
 """
 
 import sqlite3
 from docopt import docopt
-from helpers import *
-from lookup import *
-from api import *
+from .helpers import *
+from .lookup import *
+from .api import *
 
 def main():
     try:
         args = docopt(__doc__)
         try:
             BASE_DIR = os.path.dirname(os.path.dirname(__file__))
             db_path = os.path.join(BASE_DIR, "chatcmd/db.sqlite")
@@ -52,15 +52,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print(color_text('ChatCMD','green')+' 1.0.18')
+            print(color_text('ChatCMD','green')+' 1.0.19')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.18/chatcmd/commands.py` & `chatcmd-1.0.19/chatcmd/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sqlite3
 import datetime
-from helpers import *
+from .helpers import *
 
 def add_cmd(conn, cursor, prompt, command):
     try:
         cursor.execute('CREATE TABLE IF NOT EXISTS history (id INTEGER PRIMARY KEY, prompt TEXT, command TEXT, created_at DATETIME)')
         conn.commit()
 
         cursor.execute("INSERT INTO history (prompt,command,created_at) VALUES(?,?,?)", (prompt, command, datetime.datetime.now()))
```

### Comparing `chatcmd-1.0.18/chatcmd/helpers.py` & `chatcmd-1.0.19/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.18/chatcmd/lookup.py` & `chatcmd-1.0.19/chatcmd/lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from commands import *
+from .commands import *
 import openai
 
 def prompt(conn, cursor, api_key):
     print("""
 
      ######  ##     ##    ###    ########  ######  ##     ## ########
     ##    ## ##     ##   ## ##      ##    ##    ## ###   ### ##     ##
```

### Comparing `chatcmd-1.0.18/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.19/chatcmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.18
+Version: 1.0.19
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
-    Using cached chatcmd-1.0.18-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.19-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.18
+    Successfully installed chatcmd-1.0.19
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.18/pyproject.toml` & `chatcmd-1.0.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "colorama >=0.4.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.18"
+version = "1.0.19"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.18/setup.py` & `chatcmd-1.0.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.18",
+    version="1.0.19",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

