# Comparing `tmp/alicebot_adapter_mirai-0.7.0.tar.gz` & `tmp/alicebot_adapter_mirai-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot_adapter_mirai-0.7.0.tar", max compression
+gzip compressed data, was "alicebot_adapter_mirai-0.7.1.tar", max compression
```

## Comparing `alicebot_adapter_mirai-0.7.0.tar` & `alicebot_adapter_mirai-0.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34522 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/LICENSE
--rw-r--r--   0        0        0      258 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/README.md
--rw-r--r--   0        0        0     9728 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/__init__.py
--rw-r--r--   0        0        0     1034 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/config.py
--rw-r--r--   0        0        0      119 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/__init__.py
--rw-r--r--   0        0        0      987 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/base.py
--rw-r--r--   0        0        0     1088 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/mate.py
--rw-r--r--   0        0        0     5390 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/message.py
--rw-r--r--   0        0        0     5659 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/notice.py
--rw-r--r--   0        0        0     4922 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/request.py
--rw-r--r--   0        0        0      659 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/exceptions.py
--rw-r--r--   0        0        0     5081 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/message.py
--rw-r--r--   0        0        0     1138 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 alicebot_adapter_mirai-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/LICENSE
+-rw-r--r--   0        0        0      258 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/README.md
+-rw-r--r--   0        0        0     9728 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/__init__.py
+-rw-r--r--   0        0        0     1034 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/config.py
+-rw-r--r--   0        0        0      119 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/event/__init__.py
+-rw-r--r--   0        0        0      987 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/event/base.py
+-rw-r--r--   0        0        0     1088 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/event/mate.py
+-rw-r--r--   0        0        0     5390 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/event/message.py
+-rw-r--r--   0        0        0     6064 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/event/notice.py
+-rw-r--r--   0        0        0     4922 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/event/request.py
+-rw-r--r--   0        0        0      659 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/exceptions.py
+-rw-r--r--   0        0        0     5081 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/message.py
+-rw-r--r--   0        0        0     1138 2023-05-27 15:02:19.827664 alicebot_adapter_mirai-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 alicebot_adapter_mirai-0.7.1/PKG-INFO
```

### Comparing `alicebot_adapter_mirai-0.7.0/LICENSE` & `alicebot_adapter_mirai-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/__init__.py` & `alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/__init__.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/config.py` & `alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/config.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/base.py` & `alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/event/base.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/mate.py` & `alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/event/mate.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/message.py` & `alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/event/message.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/notice.py` & `alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/event/notice.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pydantic import create_model
 
 from .base import (
     FriendInfo,
     GroupInfo,
     GroupMemberInfo,
     MiraiEvent,
+    OtherClientSender,
     Permission,
     Subject,
 )
 
 
 class NoticeEvent(MiraiEvent):
     """通知事件"""
@@ -263,7 +264,26 @@
 
 
 class MemberHonorChangeEvent(GroupMemberEvent):
     """群员称号改变"""
 
     type: Literal["MemberHonorChangeEvent"]
     action: Literal["achieve", "lose"]
+
+
+class OtherClinetEvent(NoticeEvent):
+    """其他客户端事件"""
+
+    client: OtherClientSender
+
+
+class OtherClientOnlineEvent(OtherClinetEvent):
+    """其他客户端上线"""
+
+    type: Literal["OtherClientOnlineEvent"]
+    kind: Optional[int]
+
+
+class OtherClientOfflineEvent(OtherClinetEvent):
+    """其他客户端下线"""
+
+    type: Literal["OtherClientOfflineEvent"]
```

### Comparing `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/request.py` & `alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/event/request.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/exceptions.py` & `alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/exceptions.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/message.py` & `alicebot_adapter_mirai-0.7.1/alicebot/adapter/mirai/message.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.7.0/pyproject.toml` & `alicebot_adapter_mirai-0.7.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alicebot-adapter-mirai"
-version = "0.7.0"
+version = "0.7.1"
 description = "Mirai adapter for AliceBot."
 license = "AGPL-3.0-or-later"
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
 
 [tool.ruff]
 extend = "../../pyproject.toml"
 ignore = ["N815"]
```

### Comparing `alicebot_adapter_mirai-0.7.0/PKG-INFO` & `alicebot_adapter_mirai-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot-adapter-mirai
-Version: 0.7.0
+Version: 0.7.1
 Summary: Mirai adapter for AliceBot.
 Home-page: https://docs.alicebot.dev/
 License: AGPL-3.0-or-later
 Keywords: bot,chatbot,qq,qqbot,mirai
 Author: st1020
 Author-email: stone_1020@qq.com
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,15 @@
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
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: alicebot-adapter-mirai Version: 0.7.0 Summary:
+Metadata-Version: 2.1 Name: alicebot-adapter-mirai Version: 0.7.1 Summary:
 Mirai adapter for AliceBot. Home-page: https://docs.alicebot.dev/ License:
 AGPL-3.0-or-later Keywords: bot,chatbot,qq,qqbot,mirai Author: st1020 Author-
 email: stone_1020@qq.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework ::
 Robot Framework Classifier: Framework :: Robot Framework :: Library Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 or later
 (AGPLv3+) Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Communications :: Chat Requires-Dist: alicebot (==0.7.0) Project-URL:
+Communications :: Chat Requires-Dist: alicebot (==0.7.1) Project-URL:
 Documentation, https://docs.alicebot.dev/ Project-URL: Repository, https://
 github.com/AliceBotProject/alicebot Description-Content-Type: text/markdown
             [logo] # AliceBot-Adapter-CQHTTP **Mirai åè®®éé**
```

