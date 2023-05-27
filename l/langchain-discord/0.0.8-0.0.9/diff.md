# Comparing `tmp/langchain_discord-0.0.8.tar.gz` & `tmp/langchain_discord-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_discord-0.0.8.tar", last modified: Sat May 27 15:22:32 2023, max compression
+gzip compressed data, was "langchain_discord-0.0.9.tar", last modified: Sat May 27 15:24:09 2023, max compression
```

## Comparing `langchain_discord-0.0.8.tar` & `langchain_discord-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:22:32.094710 langchain_discord-0.0.8/
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:22:32.092028 langchain_discord-0.0.8/.vscode/
--rw-r--r--   0 lennarddorst   (501) staff       (20)      237 2023-05-24 19:54:14.000000 langchain_discord-0.0.8/.vscode/settings.json
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1065 2023-05-25 16:34:10.000000 langchain_discord-0.0.8/LICENSE.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-27 15:22:32.094913 langchain_discord-0.0.8/PKG-INFO
--rw-r--r--   0 lennarddorst   (501) staff       (20)       65 2023-05-25 11:43:21.000000 langchain_discord-0.0.8/README.md
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:22:32.093373 langchain_discord-0.0.8/langchain_discord/
--rw-r--r--   0 lennarddorst   (501) staff       (20)       22 2023-05-26 15:00:20.000000 langchain_discord-0.0.8/langchain_discord/__init__.py
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1691 2023-05-27 15:22:19.000000 langchain_discord-0.0.8/langchain_discord/webhook.py
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:22:32.094538 langchain_discord-0.0.8/langchain_discord.egg-info/
--rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-27 15:22:31.000000 langchain_discord-0.0.8/langchain_discord.egg-info/PKG-INFO
--rw-r--r--   0 lennarddorst   (501) staff       (20)      357 2023-05-27 15:22:32.000000 langchain_discord-0.0.8/langchain_discord.egg-info/SOURCES.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)        1 2023-05-27 15:22:31.000000 langchain_discord-0.0.8/langchain_discord.egg-info/dependency_links.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)       17 2023-05-27 15:22:31.000000 langchain_discord-0.0.8/langchain_discord.egg-info/requires.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)       18 2023-05-27 15:22:31.000000 langchain_discord-0.0.8/langchain_discord.egg-info/top_level.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)      478 2023-05-27 15:22:28.000000 langchain_discord-0.0.8/pyproject.toml
--rw-r--r--   0 lennarddorst   (501) staff       (20)       24 2023-05-25 19:47:54.000000 langchain_discord-0.0.8/requirements.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)       79 2023-05-27 15:22:32.095377 langchain_discord-0.0.8/setup.cfg
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1721 2023-05-27 15:22:27.000000 langchain_discord-0.0.8/setup.py
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:24:09.280809 langchain_discord-0.0.9/
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:24:09.278506 langchain_discord-0.0.9/.vscode/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      237 2023-05-24 19:54:14.000000 langchain_discord-0.0.9/.vscode/settings.json
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1065 2023-05-25 16:34:10.000000 langchain_discord-0.0.9/LICENSE.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-27 15:24:09.281221 langchain_discord-0.0.9/PKG-INFO
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       65 2023-05-25 11:43:21.000000 langchain_discord-0.0.9/README.md
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:24:09.279528 langchain_discord-0.0.9/langchain_discord/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       22 2023-05-26 15:00:20.000000 langchain_discord-0.0.9/langchain_discord/__init__.py
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1684 2023-05-27 15:24:06.000000 langchain_discord-0.0.9/langchain_discord/webhook.py
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:24:09.280613 langchain_discord-0.0.9/langchain_discord.egg-info/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-27 15:24:09.000000 langchain_discord-0.0.9/langchain_discord.egg-info/PKG-INFO
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      357 2023-05-27 15:24:09.000000 langchain_discord-0.0.9/langchain_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)        1 2023-05-27 15:24:09.000000 langchain_discord-0.0.9/langchain_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       17 2023-05-27 15:24:09.000000 langchain_discord-0.0.9/langchain_discord.egg-info/requires.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       18 2023-05-27 15:24:09.000000 langchain_discord-0.0.9/langchain_discord.egg-info/top_level.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      478 2023-05-27 15:24:04.000000 langchain_discord-0.0.9/pyproject.toml
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       24 2023-05-25 19:47:54.000000 langchain_discord-0.0.9/requirements.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       79 2023-05-27 15:24:09.281910 langchain_discord-0.0.9/setup.cfg
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1721 2023-05-27 15:24:01.000000 langchain_discord-0.0.9/setup.py
```

### Comparing `langchain_discord-0.0.8/LICENSE.txt` & `langchain_discord-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_discord-0.0.8/PKG-INFO` & `langchain_discord-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_discord
-Version: 0.0.8
+Version: 0.0.9
 Summary: A list of tools for LangChain to power Discord (Webhooks, etc.).
 Home-page: https://github.com/0w9/langchain-discord
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Lennard Dorst
 Author-email: Lennard Dorst <lennardsolana@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/0w9/langchain-discord
```

### Comparing `langchain_discord-0.0.8/langchain_discord/webhook.py` & `langchain_discord-0.0.9/langchain_discord/webhook.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 from langchain.callbacks.manager import CallbackManagerForToolRun
-from langchain.tools import BaseTool, Field
+from langchain.tools import BaseTool
 from pydantic import BaseModel, Field
 import requests, os
 
 class DiscordWebhookInput(BaseModel):
     #webhook_url: str = Field()
     #webhook_username: str = Field()
     webhook_message: str = Field()
```

### Comparing `langchain_discord-0.0.8/langchain_discord.egg-info/PKG-INFO` & `langchain_discord-0.0.9/langchain_discord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-discord
-Version: 0.0.8
+Version: 0.0.9
 Summary: A list of tools for LangChain to power Discord (Webhooks, etc.).
 Home-page: https://github.com/0w9/langchain-discord
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Lennard Dorst
 Author-email: Lennard Dorst <lennardsolana@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/0w9/langchain-discord
```

### Comparing `langchain_discord-0.0.8/setup.py` & `langchain_discord-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'langchain_discord',         # How you named your package folder (MyLib)
   packages = ['langchain_discord'],   # Chose the same as "name"
-  version = '0.0.8',      # Start with a small number and increase it with every change you make
+  version = '0.0.9',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This package offers some easy-to-use tools to integrate Discord into LangChain for agents.',   # Give a short description about your library
   author = 'Lennard Dorst',                   # Type in your name
   author_email = 'lennardsolana@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/0w9/langchain-discord',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['AI', 'LangChain', 'Discord'],   # Keywords that define your package best
```

