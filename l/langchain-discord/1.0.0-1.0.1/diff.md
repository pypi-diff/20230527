# Comparing `tmp/langchain_discord-1.0.0.tar.gz` & `tmp/langchain_discord-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_discord-1.0.0.tar", last modified: Sat May 27 18:29:40 2023, max compression
+gzip compressed data, was "langchain_discord-1.0.1.tar", last modified: Sat May 27 18:44:43 2023, max compression
```

## Comparing `langchain_discord-1.0.0.tar` & `langchain_discord-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 18:29:40.367060 langchain_discord-1.0.0/
--rw-r--r--   0 lennarddorst   (501) staff       (20)       42 2023-05-27 16:57:36.000000 langchain_discord-1.0.0/.gitignore
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1065 2023-05-25 16:34:10.000000 langchain_discord-1.0.0/LICENSE.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)     2602 2023-05-27 18:29:40.367280 langchain_discord-1.0.0/PKG-INFO
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1928 2023-05-27 18:25:36.000000 langchain_discord-1.0.0/README.md
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 18:29:40.365511 langchain_discord-1.0.0/langchain_discord/
--rw-r--r--   0 lennarddorst   (501) staff       (20)       22 2023-05-26 15:00:20.000000 langchain_discord-1.0.0/langchain_discord/__init__.py
--rw-r--r--   0 lennarddorst   (501) staff       (20)     2442 2023-05-27 18:15:55.000000 langchain_discord-1.0.0/langchain_discord/webhook.py
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 18:29:40.366881 langchain_discord-1.0.0/langchain_discord.egg-info/
--rw-r--r--   0 lennarddorst   (501) staff       (20)     2602 2023-05-27 18:29:40.000000 langchain_discord-1.0.0/langchain_discord.egg-info/PKG-INFO
--rw-r--r--   0 lennarddorst   (501) staff       (20)      354 2023-05-27 18:29:40.000000 langchain_discord-1.0.0/langchain_discord.egg-info/SOURCES.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)        1 2023-05-27 18:29:40.000000 langchain_discord-1.0.0/langchain_discord.egg-info/dependency_links.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)       17 2023-05-27 18:29:40.000000 langchain_discord-1.0.0/langchain_discord.egg-info/requires.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)       18 2023-05-27 18:29:40.000000 langchain_discord-1.0.0/langchain_discord.egg-info/top_level.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)      571 2023-05-27 17:06:27.000000 langchain_discord-1.0.0/main.py
--rw-r--r--   0 lennarddorst   (501) staff       (20)      478 2023-05-27 18:16:22.000000 langchain_discord-1.0.0/pyproject.toml
--rw-r--r--   0 lennarddorst   (501) staff       (20)       24 2023-05-25 19:47:54.000000 langchain_discord-1.0.0/requirements.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)       79 2023-05-27 18:29:40.367770 langchain_discord-1.0.0/setup.cfg
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1721 2023-05-27 18:16:11.000000 langchain_discord-1.0.0/setup.py
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 18:44:43.361354 langchain_discord-1.0.1/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       42 2023-05-27 16:57:36.000000 langchain_discord-1.0.1/.gitignore
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1065 2023-05-25 16:34:10.000000 langchain_discord-1.0.1/LICENSE.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     2602 2023-05-27 18:44:43.361538 langchain_discord-1.0.1/PKG-INFO
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1928 2023-05-27 18:25:36.000000 langchain_discord-1.0.1/README.md
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 18:44:43.360154 langchain_discord-1.0.1/langchain_discord/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       22 2023-05-26 15:00:20.000000 langchain_discord-1.0.1/langchain_discord/__init__.py
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     2376 2023-05-27 18:44:36.000000 langchain_discord-1.0.1/langchain_discord/webhook.py
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 18:44:43.361200 langchain_discord-1.0.1/langchain_discord.egg-info/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     2602 2023-05-27 18:44:43.000000 langchain_discord-1.0.1/langchain_discord.egg-info/PKG-INFO
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      354 2023-05-27 18:44:43.000000 langchain_discord-1.0.1/langchain_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)        1 2023-05-27 18:44:43.000000 langchain_discord-1.0.1/langchain_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       17 2023-05-27 18:44:43.000000 langchain_discord-1.0.1/langchain_discord.egg-info/requires.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       18 2023-05-27 18:44:43.000000 langchain_discord-1.0.1/langchain_discord.egg-info/top_level.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      571 2023-05-27 17:06:27.000000 langchain_discord-1.0.1/main.py
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      478 2023-05-27 18:44:22.000000 langchain_discord-1.0.1/pyproject.toml
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       24 2023-05-25 19:47:54.000000 langchain_discord-1.0.1/requirements.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       79 2023-05-27 18:44:43.361967 langchain_discord-1.0.1/setup.cfg
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1721 2023-05-27 18:44:18.000000 langchain_discord-1.0.1/setup.py
```

### Comparing `langchain_discord-1.0.0/LICENSE.txt` & `langchain_discord-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_discord-1.0.0/PKG-INFO` & `langchain_discord-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_discord
-Version: 1.0.0
+Version: 1.0.1
 Summary: A list of tools for LangChain to power Discord (Webhooks, etc.).
 Home-page: https://github.com/0w9/langchain-discord
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Lennard Dorst
 Author-email: Lennard Dorst <lennardsolana@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/0w9/langchain-discord
```

### Comparing `langchain_discord-1.0.0/README.md` & `langchain_discord-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_discord-1.0.0/langchain_discord/webhook.py` & `langchain_discord-1.0.1/langchain_discord/webhook.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Optional
-from langchain.callbacks.manager import CallbackManagerForToolRun
 from langchain.tools import BaseTool
 from pydantic import BaseModel, Field
 from typing import Optional, Type
 import requests, os
 from typing import Any, Dict
 from pydantic import BaseModel, Field, root_validator
 from langchain.output_parsers import StructuredOutputParser, ResponseSchema
```

### Comparing `langchain_discord-1.0.0/langchain_discord.egg-info/PKG-INFO` & `langchain_discord-1.0.1/langchain_discord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-discord
-Version: 1.0.0
+Version: 1.0.1
 Summary: A list of tools for LangChain to power Discord (Webhooks, etc.).
 Home-page: https://github.com/0w9/langchain-discord
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Lennard Dorst
 Author-email: Lennard Dorst <lennardsolana@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/0w9/langchain-discord
```

### Comparing `langchain_discord-1.0.0/main.py` & `langchain_discord-1.0.1/main.py`

 * *Files identical despite different names*

### Comparing `langchain_discord-1.0.0/setup.py` & `langchain_discord-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'langchain_discord',         # How you named your package folder (MyLib)
   packages = ['langchain_discord'],   # Chose the same as "name"
-  version = '1.0.0',      # Start with a small number and increase it with every change you make
+  version = '1.0.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This package offers some easy-to-use tools to integrate Discord into LangChain for agents.',   # Give a short description about your library
   author = 'Lennard Dorst',                   # Type in your name
   author_email = 'lennardsolana@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/0w9/langchain-discord',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['AI', 'LangChain', 'Discord'],   # Keywords that define your package best
```

