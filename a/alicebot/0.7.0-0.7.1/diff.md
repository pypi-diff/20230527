# Comparing `tmp/alicebot-0.7.0.tar.gz` & `tmp/alicebot-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot-0.7.0.tar", max compression
+gzip compressed data, was "alicebot-0.7.1.tar", max compression
```

## Comparing `alicebot-0.7.0.tar` & `alicebot-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-05-27 14:25:34.114713 alicebot-0.7.0/LICENSE
--rw-r--r--   0        0        0     6021 2023-05-27 14:25:34.114713 alicebot-0.7.0/README.md
--rw-r--r--   0        0        0      728 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/__init__.py
--rw-r--r--   0        0        0     5330 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/adapter/__init__.py
--rw-r--r--   0        0        0     8621 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/adapter/utils.py
--rw-r--r--   0        0        0    38583 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/bot.py
--rw-r--r--   0        0        0     1879 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/config.py
--rw-r--r--   0        0        0     4319 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/dependencies.py
--rw-r--r--   0        0        0     4216 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/event.py
--rw-r--r--   0        0        0     1130 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/exceptions.py
--rw-r--r--   0        0        0      597 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/log.py
--rw-r--r--   0        0        0    15028 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/message.py
--rw-r--r--   0        0        0     4045 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/plugin.py
--rw-r--r--   0        0        0        0 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/py.typed
--rw-r--r--   0        0        0     1084 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/typing.py
--rw-r--r--   0        0        0     8052 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/utils.py
--rw-r--r--   0        0        0     4380 2023-05-27 14:25:34.122713 alicebot-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7408 1970-01-01 00:00:00.000000 alicebot-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-27 15:02:19.819664 alicebot-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6021 2023-05-27 15:02:19.819664 alicebot-0.7.1/README.md
+-rw-r--r--   0        0        0      728 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/__init__.py
+-rw-r--r--   0        0        0     5330 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/adapter/__init__.py
+-rw-r--r--   0        0        0     8621 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/adapter/utils.py
+-rw-r--r--   0        0        0    38583 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/bot.py
+-rw-r--r--   0        0        0     1879 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/config.py
+-rw-r--r--   0        0        0     4319 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/dependencies.py
+-rw-r--r--   0        0        0     4216 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/event.py
+-rw-r--r--   0        0        0     1130 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/exceptions.py
+-rw-r--r--   0        0        0      597 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/log.py
+-rw-r--r--   0        0        0    15028 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/message.py
+-rw-r--r--   0        0        0     4045 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/py.typed
+-rw-r--r--   0        0        0     1084 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/typing.py
+-rw-r--r--   0        0        0     8052 2023-05-27 15:02:19.819664 alicebot-0.7.1/alicebot/utils.py
+-rw-r--r--   0        0        0     4380 2023-05-27 15:02:19.827664 alicebot-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7408 1970-01-01 00:00:00.000000 alicebot-0.7.1/PKG-INFO
```

### Comparing `alicebot-0.7.0/LICENSE` & `alicebot-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/README.md` & `alicebot-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/__init__.py` & `alicebot-0.7.1/alicebot/__init__.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/adapter/__init__.py` & `alicebot-0.7.1/alicebot/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/adapter/utils.py` & `alicebot-0.7.1/alicebot/adapter/utils.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/bot.py` & `alicebot-0.7.1/alicebot/bot.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/config.py` & `alicebot-0.7.1/alicebot/config.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/dependencies.py` & `alicebot-0.7.1/alicebot/dependencies.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/event.py` & `alicebot-0.7.1/alicebot/event.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/exceptions.py` & `alicebot-0.7.1/alicebot/exceptions.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/log.py` & `alicebot-0.7.1/alicebot/log.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/message.py` & `alicebot-0.7.1/alicebot/message.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/plugin.py` & `alicebot-0.7.1/alicebot/plugin.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/typing.py` & `alicebot-0.7.1/alicebot/typing.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/alicebot/utils.py` & `alicebot-0.7.1/alicebot/utils.py`

 * *Files identical despite different names*

### Comparing `alicebot-0.7.0/pyproject.toml` & `alicebot-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alicebot"
-version = "0.7.0"
+version = "0.7.1"
 description = "A simply asynchronous python chatbot framework."
 license = "MIT"
 authors = ["st1020 <stone_1020@qq.com>"]
 readme = "README.md"
 homepage = "https://docs.alicebot.dev/"
 repository = "https://github.com/AliceBotProject/alicebot"
 documentation = "https://docs.alicebot.dev/"
```

### Comparing `alicebot-0.7.0/PKG-INFO` & `alicebot-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot
-Version: 0.7.0
+Version: 0.7.1
 Summary: A simply asynchronous python chatbot framework.
 Home-page: https://docs.alicebot.dev/
 License: MIT
 Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq
 Author: st1020
 Author-email: stone_1020@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alicebot Version: 0.7.0 Summary: A simply
+Metadata-Version: 2.1 Name: alicebot Version: 0.7.1 Summary: A simply
 asynchronous python chatbot framework. Home-page: https://docs.alicebot.dev/
 License: MIT Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq Author: st1020 Author-
 email: stone_1020@qq.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework ::
 Robot Framework Classifier: Framework :: Robot Framework :: Library Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

