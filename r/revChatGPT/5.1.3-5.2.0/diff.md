# Comparing `tmp/revChatGPT-5.1.3.tar.gz` & `tmp/revChatGPT-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-5.1.3.tar", last modified: Fri May 26 01:10:59 2023, max compression
+gzip compressed data, was "revChatGPT-5.2.0.tar", last modified: Sat May 27 02:23:18 2023, max compression
```

## Comparing `revChatGPT-5.1.3.tar` & `revChatGPT-5.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    50929 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.678747 revChatGPT-5.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    50788 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 02:23:18.000000 revChatGPT-5.2.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:23:18.682747 revChatGPT-5.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-27 02:22:41.000000 revChatGPT-5.2.0/tests/test_recipient.py
```

### Comparing `revChatGPT-5.1.3/LICENSE` & `revChatGPT-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.3/PKG-INFO` & `revChatGPT-5.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.1.3
+Version: 5.2.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -64,26 +64,23 @@
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
 
-> _Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`_
 > Not supported for Google/Microsoft accounts.
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
-
-> Please this!
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
```

### Comparing `revChatGPT-5.1.3/README.md` & `revChatGPT-5.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,23 @@
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
 
-> _Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`_
 > Not supported for Google/Microsoft accounts.
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
-
-> Please this!
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
```

### Comparing `revChatGPT-5.1.3/setup.py` & `revChatGPT-5.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="5.1.3",
+    version="5.2.0",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
@@ -25,15 +25,15 @@
     author_email="acheong@student.dalat.org",
     license="GNU General Public License v2.0",
     packages=find_namespace_packages("src"),
     package_dir={"": "src"},
     py_modules=["revChatGPT"],
     package_data={"": ["*.json"]},
     install_requires=[
-        "OpenAIAuth==0.3.6",
+        "OpenAIAuth>=1.0.2",
         "requests[socks]",
         "httpx[socks]",
         "async_tio",
         "prompt-toolkit",
         "tiktoken>=0.3.0",
         "openai",
     ],
```

### Comparing `revChatGPT-5.1.3/src/revChatGPT/V1.py` & `revChatGPT-5.2.0/src/revChatGPT/V1.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 from typing import AsyncGenerator
 from typing import Generator
 from typing import NoReturn
 
 import httpx
 import requests
 from httpx import AsyncClient
-from OpenAIAuth import Authenticator
-from OpenAIAuth import Error as AuthError
+from OpenAIAuth import Auth0 as Authenticator
 
 from . import __version__
 from . import typings as t
 from .recipient import PythonRecipient
 from .recipient import Recipient
 from .recipient import RecipientManager
 from .utils import create_completer
@@ -191,17 +190,16 @@
             self.set_access_token(self.config["access_token"])
         elif "email" not in self.config or "password" not in self.config:
             error = t.AuthenticationError("Insufficient login details provided!")
             raise error
         if "access_token" not in self.config:
             try:
                 self.login()
-            except AuthError as error:
-                print(error.details)
-                print(error.status_code)
+            except Exception as error:
+                print(error)
                 raise error
 
     @logger(is_timed=False)
     def set_access_token(self, access_token: str) -> None:
         """Set access token in request header and self.config, then cache it to file.
 
         Args:
@@ -313,28 +311,26 @@
         except (FileNotFoundError, json.decoder.JSONDecodeError):
             cached = {}
         return cached
 
     @logger(is_timed=True)
     def login(self) -> None:
         """Login to OpenAI by email and password"""
-        if self.config.get("email") and self.config.get("password"):
+        if not self.config.get("email") and not self.config.get("password"):
             log.error("Insufficient login details provided!")
             error = t.AuthenticationError("Insufficient login details provided!")
             raise error
         auth = Authenticator(
-            email_address=self.config.get("email"),
+            email=self.config.get("email"),
             password=self.config.get("password"),
             proxy=self.config.get("proxy"),
         )
         log.debug("Using authenticator to get access token")
-        auth.begin()
-        auth.get_access_token()
 
-        self.set_access_token(auth.access_token)
+        self.set_access_token(auth.auth())
 
     @logger(is_timed=True)
     def __send_request(
         self,
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
```

### Comparing `revChatGPT-5.1.3/src/revChatGPT/V3.py` & `revChatGPT-5.2.0/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.3/src/revChatGPT/__init__.py` & `revChatGPT-5.2.0/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.3/src/revChatGPT/__main__.py` & `revChatGPT-5.2.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.3/src/revChatGPT/config/enable_internet.json` & `revChatGPT-5.2.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.3/src/revChatGPT/recipient.py` & `revChatGPT-5.2.0/src/revChatGPT/recipient.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.3/src/revChatGPT/typings.py` & `revChatGPT-5.2.0/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.3/src/revChatGPT/utils.py` & `revChatGPT-5.2.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.3/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-5.2.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.1.3
+Version: 5.2.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -64,26 +64,23 @@
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
 
-> _Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`_
 > Not supported for Google/Microsoft accounts.
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
-
-> Please this!
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
```

### Comparing `revChatGPT-5.1.3/tests/test_recipient.py` & `revChatGPT-5.2.0/tests/test_recipient.py`

 * *Files identical despite different names*

