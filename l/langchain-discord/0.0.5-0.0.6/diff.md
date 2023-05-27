# Comparing `tmp/langchain_discord-0.0.5.tar.gz` & `tmp/langchain_discord-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_discord-0.0.5.tar", last modified: Fri May 26 15:01:27 2023, max compression
+gzip compressed data, was "langchain_discord-0.0.6.tar", last modified: Sat May 27 15:14:08 2023, max compression
```

## Comparing `langchain_discord-0.0.5.tar` & `langchain_discord-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 15:01:27.144879 langchain_discord-0.0.5/
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 15:01:27.143570 langchain_discord-0.0.5/.vscode/
--rw-r--r--   0 lennarddorst   (501) staff       (20)      237 2023-05-24 19:54:14.000000 langchain_discord-0.0.5/.vscode/settings.json
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1065 2023-05-25 16:34:10.000000 langchain_discord-0.0.5/LICENSE.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-26 15:01:27.145059 langchain_discord-0.0.5/PKG-INFO
--rw-r--r--   0 lennarddorst   (501) staff       (20)       65 2023-05-25 11:43:21.000000 langchain_discord-0.0.5/README.md
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 15:01:27.143875 langchain_discord-0.0.5/langchain_discord/
--rw-r--r--   0 lennarddorst   (501) staff       (20)       22 2023-05-26 15:00:20.000000 langchain_discord-0.0.5/langchain_discord/__init__.py
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1689 2023-05-26 14:42:53.000000 langchain_discord-0.0.5/langchain_discord/webhook.py
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 15:01:27.144730 langchain_discord-0.0.5/langchain_discord.egg-info/
--rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-26 15:01:26.000000 langchain_discord-0.0.5/langchain_discord.egg-info/PKG-INFO
--rw-r--r--   0 lennarddorst   (501) staff       (20)      340 2023-05-26 15:01:27.000000 langchain_discord-0.0.5/langchain_discord.egg-info/SOURCES.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)        1 2023-05-26 15:01:26.000000 langchain_discord-0.0.5/langchain_discord.egg-info/dependency_links.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)       17 2023-05-26 15:01:26.000000 langchain_discord-0.0.5/langchain_discord.egg-info/requires.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)       18 2023-05-26 15:01:26.000000 langchain_discord-0.0.5/langchain_discord.egg-info/top_level.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)      478 2023-05-26 15:01:14.000000 langchain_discord-0.0.5/pyproject.toml
--rw-r--r--   0 lennarddorst   (501) staff       (20)       79 2023-05-26 15:01:27.145442 langchain_discord-0.0.5/setup.cfg
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1720 2023-05-26 15:01:11.000000 langchain_discord-0.0.5/setup.py
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:14:08.025943 langchain_discord-0.0.6/
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:14:08.023440 langchain_discord-0.0.6/.vscode/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      237 2023-05-24 19:54:14.000000 langchain_discord-0.0.6/.vscode/settings.json
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1065 2023-05-25 16:34:10.000000 langchain_discord-0.0.6/LICENSE.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-27 15:14:08.026181 langchain_discord-0.0.6/PKG-INFO
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       65 2023-05-25 11:43:21.000000 langchain_discord-0.0.6/README.md
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:14:08.024460 langchain_discord-0.0.6/langchain_discord/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       22 2023-05-26 15:00:20.000000 langchain_discord-0.0.6/langchain_discord/__init__.py
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1722 2023-05-27 15:13:48.000000 langchain_discord-0.0.6/langchain_discord/webhook.py
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-27 15:14:08.025757 langchain_discord-0.0.6/langchain_discord.egg-info/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-27 15:14:07.000000 langchain_discord-0.0.6/langchain_discord.egg-info/PKG-INFO
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      340 2023-05-27 15:14:08.000000 langchain_discord-0.0.6/langchain_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)        1 2023-05-27 15:14:07.000000 langchain_discord-0.0.6/langchain_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       17 2023-05-27 15:14:07.000000 langchain_discord-0.0.6/langchain_discord.egg-info/requires.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       18 2023-05-27 15:14:07.000000 langchain_discord-0.0.6/langchain_discord.egg-info/top_level.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      478 2023-05-27 15:14:01.000000 langchain_discord-0.0.6/pyproject.toml
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       79 2023-05-27 15:14:08.026681 langchain_discord-0.0.6/setup.cfg
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1720 2023-05-27 15:14:04.000000 langchain_discord-0.0.6/setup.py
```

### Comparing `langchain_discord-0.0.5/LICENSE.txt` & `langchain_discord-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_discord-0.0.5/PKG-INFO` & `langchain_discord-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_discord
-Version: 0.0.5
+Version: 0.0.6
 Summary: A list of tools for LangChain to power Discord (Webhooks, etc.).
 Home-page: https://github.com/0w9/langchain-discord
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Lennard Dorst
 Author-email: Lennard Dorst <lennardsolana@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/0w9/langchain-discord
```

### Comparing `langchain_discord-0.0.5/langchain_discord/webhook.py` & `langchain_discord-0.0.6/langchain_discord/webhook.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
                             "content": webhook_message, 
                             "username": WEBHOOK_USERNAME
                         }, 
                       headers={"Content-Type": "application/json"}
         )
 
         if(answer.status_code != 204 or answer.status_code != 200):
+            print(answer.json())
             raise Exception("Webhook message could not be sent! Please check your webhook URL and message and try again.")
         else:
             return "Webhook message sent successfully!"
 
     
     def _arun(self, webhook_message: str, webhook_url: str, webhook_username: str): raise NotImplementedError("This tool does not support async")
```

### Comparing `langchain_discord-0.0.5/langchain_discord.egg-info/PKG-INFO` & `langchain_discord-0.0.6/langchain_discord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-discord
-Version: 0.0.5
+Version: 0.0.6
 Summary: A list of tools for LangChain to power Discord (Webhooks, etc.).
 Home-page: https://github.com/0w9/langchain-discord
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Lennard Dorst
 Author-email: Lennard Dorst <lennardsolana@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/0w9/langchain-discord
```

### Comparing `langchain_discord-0.0.5/setup.py` & `langchain_discord-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'langchain_discord',         # How you named your package folder (MyLib)
   packages = ['langchain_discord'],   # Chose the same as "name"
-  version = '0.05',      # Start with a small number and increase it with every change you make
+  version = '0.06',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This package offers some easy-to-use tools to integrate Discord into LangChain for agents.',   # Give a short description about your library
   author = 'Lennard Dorst',                   # Type in your name
   author_email = 'lennardsolana@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/0w9/langchain-discord',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['AI', 'LangChain', 'Discord'],   # Keywords that define your package best
```

