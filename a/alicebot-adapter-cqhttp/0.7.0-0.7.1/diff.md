# Comparing `tmp/alicebot_adapter_cqhttp-0.7.0.tar.gz` & `tmp/alicebot_adapter_cqhttp-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot_adapter_cqhttp-0.7.0.tar", max compression
+gzip compressed data, was "alicebot_adapter_cqhttp-0.7.1.tar", max compression
```

## Comparing `alicebot_adapter_cqhttp-0.7.0.tar` & `alicebot_adapter_cqhttp-0.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      267 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/README.md
--rw-r--r--   0        0        0     9917 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/__init__.py
--rw-r--r--   0        0        0      875 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/config.py
--rw-r--r--   0        0        0    10223 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/event.py
--rw-r--r--   0        0        0      719 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/exceptions.py
--rw-r--r--   0        0        0     7571 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/message.py
--rw-r--r--   0        0        0     1081 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 alicebot_adapter_cqhttp-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      267 2023-05-27 15:02:19.823664 alicebot_adapter_cqhttp-0.7.1/README.md
+-rw-r--r--   0        0        0     9917 2023-05-27 15:02:19.823664 alicebot_adapter_cqhttp-0.7.1/alicebot/adapter/cqhttp/__init__.py
+-rw-r--r--   0        0        0      875 2023-05-27 15:02:19.823664 alicebot_adapter_cqhttp-0.7.1/alicebot/adapter/cqhttp/config.py
+-rw-r--r--   0        0        0    10223 2023-05-27 15:02:19.827664 alicebot_adapter_cqhttp-0.7.1/alicebot/adapter/cqhttp/event.py
+-rw-r--r--   0        0        0      719 2023-05-27 15:02:19.827664 alicebot_adapter_cqhttp-0.7.1/alicebot/adapter/cqhttp/exceptions.py
+-rw-r--r--   0        0        0     7571 2023-05-27 15:02:19.827664 alicebot_adapter_cqhttp-0.7.1/alicebot/adapter/cqhttp/message.py
+-rw-r--r--   0        0        0     1081 2023-05-27 15:02:19.827664 alicebot_adapter_cqhttp-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 alicebot_adapter_cqhttp-0.7.1/PKG-INFO
```

### Comparing `alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/__init__.py` & `alicebot_adapter_cqhttp-0.7.1/alicebot/adapter/cqhttp/__init__.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/config.py` & `alicebot_adapter_cqhttp-0.7.1/alicebot/adapter/cqhttp/config.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/event.py` & `alicebot_adapter_cqhttp-0.7.1/alicebot/adapter/cqhttp/event.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/exceptions.py` & `alicebot_adapter_cqhttp-0.7.1/alicebot/adapter/cqhttp/exceptions.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/message.py` & `alicebot_adapter_cqhttp-0.7.1/alicebot/adapter/cqhttp/message.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_cqhttp-0.7.0/pyproject.toml` & `alicebot_adapter_cqhttp-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alicebot-adapter-cqhttp"
-version = "0.7.0"
+version = "0.7.1"
 description = "OneBot(CQHTTP) adapter for AliceBot."
 license = "MIT"
 authors = ["st1020 <stone_1020@qq.com>"]
 readme = "README.md"
 homepage = "https://docs.alicebot.dev/"
 repository = "https://github.com/AliceBotProject/alicebot"
 documentation = "https://docs.alicebot.dev/"
@@ -20,15 +20,15 @@
     "Topic :: Communications :: Chat",
 ]
 packages = [{ include = "alicebot" }]
 exclude = ["alicebot/__init__.py", "alicebot/adapter/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-alicebot = "0.7.0"
+alicebot = "0.7.1"
 
 [tool.poetry.dev-dependencies]
 alicebot = { path = "../../", develop = true }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `alicebot_adapter_cqhttp-0.7.0/PKG-INFO` & `alicebot_adapter_cqhttp-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot-adapter-cqhttp
-Version: 0.7.0
+Version: 0.7.1
 Summary: OneBot(CQHTTP) adapter for AliceBot.
 Home-page: https://docs.alicebot.dev/
 License: MIT
 Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq
 Author: st1020
 Author-email: stone_1020@qq.com
 Requires-Python: >=3.8,<4.0
@@ -16,15 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
-Requires-Dist: alicebot (==0.7.0)
+Requires-Dist: alicebot (==0.7.1)
 Project-URL: Documentation, https://docs.alicebot.dev/
 Project-URL: Repository, https://github.com/AliceBotProject/alicebot
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/AliceBotProject/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: alicebot-adapter-cqhttp Version: 0.7.0 Summary:
+Metadata-Version: 2.1 Name: alicebot-adapter-cqhttp Version: 0.7.1 Summary:
 OneBot(CQHTTP) adapter for AliceBot. Home-page: https://docs.alicebot.dev/
 License: MIT Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq Author: st1020 Author-
 email: stone_1020@qq.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework ::
 Robot Framework Classifier: Framework :: Robot Framework :: Library Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Communications ::
-Chat Requires-Dist: alicebot (==0.7.0) Project-URL: Documentation, https://
+Chat Requires-Dist: alicebot (==0.7.1) Project-URL: Documentation, https://
 docs.alicebot.dev/ Project-URL: Repository, https://github.com/AliceBotProject/
 alicebot Description-Content-Type: text/markdown
        [logo] # AliceBot-Adapter-CQHTTP **OneBot(CQHTTP) åè®®éé**
```

