# Comparing `tmp/chatcmd-1.0.16.tar.gz` & `tmp/chatcmd-1.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.16.tar", last modified: Thu May 18 21:30:17 2023, max compression
+gzip compressed data, was "chatcmd-1.0.17.tar", last modified: Sat May 27 20:24:04 2023, max compression
```

## Comparing `chatcmd-1.0.16.tar` & `chatcmd-1.0.17.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-18 21:30:17.453202 chatcmd-1.0.16/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.16/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5488 2023-05-18 21:30:17.452904 chatcmd-1.0.16/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-18 21:29:40.000000 chatcmd-1.0.16/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-18 21:30:17.450266 chatcmd-1.0.16/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.16/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-14 22:57:58.000000 chatcmd-1.0.16/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3525 2023-05-18 21:29:40.000000 chatcmd-1.0.16/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3770 2023-05-15 21:19:30.000000 chatcmd-1.0.16/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     2783 2023-05-15 19:10:56.000000 chatcmd-1.0.16/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2602 2023-05-15 19:07:09.000000 chatcmd-1.0.16/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-18 21:30:17.452490 chatcmd-1.0.16/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5488 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       28 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1653 2023-05-18 21:29:40.000000 chatcmd-1.0.16/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-18 21:30:17.453286 chatcmd-1.0.16/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      537 2023-05-18 21:29:40.000000 chatcmd-1.0.16/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 20:24:04.817388 chatcmd-1.0.17/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.17/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5488 2023-05-27 20:24:04.816950 chatcmd-1.0.17/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 20:22:11.000000 chatcmd-1.0.17/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 20:24:04.813670 chatcmd-1.0.17/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.17/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1759 2023-05-27 20:01:41.000000 chatcmd-1.0.17/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3461 2023-05-27 20:22:11.000000 chatcmd-1.0.17/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3769 2023-05-27 20:01:41.000000 chatcmd-1.0.17/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     2442 2023-05-27 20:15:43.000000 chatcmd-1.0.17/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2601 2023-05-27 20:01:15.000000 chatcmd-1.0.17/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 20:24:04.816219 chatcmd-1.0.17/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5488 2023-05-27 20:24:04.000000 chatcmd-1.0.17/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 20:24:04.000000 chatcmd-1.0.17/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 20:24:04.000000 chatcmd-1.0.17/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 20:24:04.000000 chatcmd-1.0.17/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       28 2023-05-27 20:24:04.000000 chatcmd-1.0.17/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 20:24:04.000000 chatcmd-1.0.17/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1653 2023-05-27 20:22:11.000000 chatcmd-1.0.17/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 20:24:04.817571 chatcmd-1.0.17/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      537 2023-05-27 20:22:11.000000 chatcmd-1.0.17/setup.py
```

### Comparing `chatcmd-1.0.16/LICENSE` & `chatcmd-1.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.16/PKG-INFO` & `chatcmd-1.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.16
+Version: 1.0.17
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -63,17 +63,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.16-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.17-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.16
+    Successfully installed chatcmd-1.0.17
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.16/README.md` & `chatcmd-1.0.17/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.16-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.17-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.16
+    Successfully installed chatcmd-1.0.17
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.16/chatcmd/api.py` & `chatcmd-1.0.17/chatcmd/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sqlite3
-from .helpers import *
+from helpers import *
 
 def get_api_key(conn, cursor):
     try:
         cursor.execute('CREATE TABLE IF NOT EXISTS config (id INTEGER PRIMARY KEY, api_key TEXT)')
         conn.commit()
 
         cursor.execute('INSERT OR IGNORE INTO config (id, api_key) VALUES(?,?)', [1,None])
```

### Comparing `chatcmd-1.0.16/chatcmd/chatcmd.py` & `chatcmd-1.0.17/chatcmd/chatcmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/env python
 """
-\033[32m
      ######  ##     ##    ###    ########  ######  ##     ## ########
     ##    ## ##     ##   ## ##      ##    ##    ## ###   ### ##     ##
     ##       ##     ##  ##   ##     ##    ##       #### #### ##     ##
     ##       ######### ##     ##    ##    ##       ## ### ## ##     ##
     ##       ##     ## #########    ##    ##       ##     ## ##     ##
     ##    ## ##     ## ##     ##    ##    ##    ## ##     ## ##     ##
      ######  ##     ## ##     ##    ##     ######  ##     ## ########
    --------------------------------------------------------------------
                 AI-driven CLI command lookup using ChatGPT
           Boost Your Productivity, Say Goodbye to Manual Searches
    --------------------------------------------------------------------
-\033[37m               Developed By: Naif Alshaye | https://naif.io\033[0m
+               Developed By: Naif Alshaye | https://naif.io
 
-\033[33mUsage:\033[0m
-    \033[32mchatcmd\033[0m [options]
+Usage:
+    chatcmd [options]
 
-\033[33mOptions:\033[0m
+Options:
   -k, --set-key                     set or update ChatGPT API key.
   -o, --get-key                     display ChatGPT API key.
   -g, --get-cmd                     display the last command.
   -G, --get-last=<value>            display the last [number] of commands.
   -d, --delete-cmd                  delete the last command.
   -D, --delete-last-cmd=<value>     delete the last [number] of commands.
   -t, --cmd-total                   display the total number of commands.
@@ -30,17 +29,17 @@
   -h, --help                        display this screen.
   -v, --version                     display ChatCMD version.
   -i, --library-info                display library information.
 """
 
 import sqlite3
 from docopt import docopt
-from .helpers import *
-from .lookup import *
-from .api import *
+from helpers import *
+from lookup import *
+from api import *
 
 def main():
     try:
         args = docopt(__doc__)
         try:
             BASE_DIR = os.path.dirname(os.path.dirname(__file__))
             db_path = os.path.join(BASE_DIR, "chatcmd/db.sqlite")
@@ -53,15 +52,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD \033[32m1.0.16\033[0m')
+            print(color_text('ChatCMD','green')+' 1.0.17')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.16/chatcmd/commands.py` & `chatcmd-1.0.17/chatcmd/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sqlite3
 import datetime
-from .helpers import *
+from helpers import *
 
 
 def add_cmd(conn, cursor, prompt, command):
     try:
         cursor.execute('CREATE TABLE IF NOT EXISTS history (id INTEGER PRIMARY KEY, prompt TEXT, command TEXT, created_at DATETIME)')
         conn.commit()
```

### Comparing `chatcmd-1.0.16/chatcmd/helpers.py` & `chatcmd-1.0.17/chatcmd/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 import re
 import inspect
 import platform
 import subprocess
 import sys
-
-RESET = '\033[0m'
+import colorama
+from colorama import Fore, Back, Style
 
 def library_info():
     print(
     "----------------------------------------------------------------\n"
-    "  \033[32mLibrary Name:\033[0m \033[33mChatCMD\033[0m\n"
-    "  \033[32mLibrary Source [PyPi]:\033[0m https://pypi.org/naifalshaye/chatcmd\n"
-    "  \033[32mLibrary Source [Github]:\033[0m https://github.com/naifalshaye/chatcmd\n"
-    "  \033[32mDocumentation:\033[0m https://github.com/naifalshaye/chatcmd#readme\n"
-    "  \033[32mBug Tracker:\033[0m https://github.com/naifalshaye/chatcmd/issues\n"
-    "  \033[32mPublished Date:\033[0m 2023-05-15\n"
-    "  \033[32mLicense:\033[0m MIT\n"
-    "  \033[32mAuthor:\033[0m Naif Alshaye\n"
-    "  \033[32mAuthor Email:\033[0m naif@naif.io\n"
-    "  \033[32mAuthor Website:\033[0m https://naif.io\n"
+    "  Library Name: ChatCMD\n"
+    "  Library Source [PyPi]: https://pypi.org/naifalshaye/chatcmd\n"
+    "  Library Source [Github]: https://github.com/naifalshaye/chatcmd\n"
+    "  Documentation: https://github.com/naifalshaye/chatcmd#readme\n"
+    "  Bug Tracker: https://github.com/naifalshaye/chatcmd/issues\n"
+    "  Published Date: 2023-05-15\n"
+    "  License: MIT\n"
+    "  Author: Naif Alshaye\n"
+    "  Author Email: naif@naif.io\n"
+    "  Author Website: https://naif.io\n"
     "----------------------------------------------------------------"
     )
 
 def color_text(text, color):
     colors = {
-        'red': '\033[31m',
-        'green': '\033[32m',
-        'yellow': '\033[33m',
-        'blue': '\033[34m',
-        'magenta': '\033[35m',
-        'cyan': '\033[36m',
-        'white': '\033[97m',
-        'black': "\033[0;30m",
-        'light_gray': "\033[37m",
-        'dark_gray': "\033[1;30m",
-        'light_white': "\033[37m",
-        'bold': "\033[1m",
-        'italic': "\033[3m",
-        'underline': "\033[4m",
-        'end': "\033[0m",
+        'red': Fore.RED,
+        'green': Fore.GREEN,
+        'yellow': Fore.YELLOW,
+        'blue': Fore.BLUE,
+        'magenta':Fore.MAGENTA,
+        'cyan': Fore.CYAN,
+        'white':Fore.WHITE,
+        'black':Fore.BLACK,
     }
-    return f"{colors[color]}{text}{RESET}"
+
+    return f"{colors[color]}{text}" + Style.RESET_ALL
 
 def success_msg(text):
     print("\n"+color_text(text, 'green'))
 
 def error_msg(text):
     print("\n"+color_text(text, 'red'))
     exit()
```

### Comparing `chatcmd-1.0.16/chatcmd/lookup.py` & `chatcmd-1.0.17/chatcmd/lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .commands import *
+from commands import *
 import openai
 
 def prompt(conn, cursor, api_key):
     print("""
 
      ######  ##     ##    ###    ########  ######  ##     ## ########
     ##    ## ##     ##   ## ##      ##    ##    ## ###   ### ##     ##
```

### Comparing `chatcmd-1.0.16/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.17/chatcmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.16
+Version: 1.0.17
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -63,17 +63,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.16-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.17-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.16
+    Successfully installed chatcmd-1.0.17
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.16/pyproject.toml` & `chatcmd-1.0.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 65",
     "wheel >= 0.38",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.16"
+version = "1.0.17"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.16/setup.py` & `chatcmd-1.0.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.16",
+    version="1.0.17",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

