# Comparing `tmp/alicebot_adapter_dingtalk-0.6.2.tar.gz` & `tmp/alicebot_adapter_dingtalk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot_adapter_dingtalk-0.6.2.tar", max compression
+gzip compressed data, was "alicebot_adapter_dingtalk-0.7.0.tar", max compression
```

## Comparing `alicebot_adapter_dingtalk-0.6.2.tar` & `alicebot_adapter_dingtalk-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      260 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/README.md
--rw-r--r--   0        0        0     5287 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/__init__.py
--rw-r--r--   0        0        0      593 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/config.py
--rw-r--r--   0        0        0     2368 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/event.py
--rw-r--r--   0        0        0      315 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/exceptions.py
--rw-r--r--   0        0        0     3197 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/message.py
--rw-r--r--   0        0        0     1321 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1336 1970-01-01 00:00:00.000000 alicebot_adapter_dingtalk-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-05-27 14:25:34.118713 alicebot_adapter_dingtalk-0.7.0/README.md
+-rw-r--r--   0        0        0     5296 2023-05-27 14:25:34.118713 alicebot_adapter_dingtalk-0.7.0/alicebot/adapter/dingtalk/__init__.py
+-rw-r--r--   0        0        0      595 2023-05-27 14:25:34.118713 alicebot_adapter_dingtalk-0.7.0/alicebot/adapter/dingtalk/config.py
+-rw-r--r--   0        0        0     3023 2023-05-27 14:25:34.118713 alicebot_adapter_dingtalk-0.7.0/alicebot/adapter/dingtalk/event.py
+-rw-r--r--   0        0        0      315 2023-05-27 14:25:34.118713 alicebot_adapter_dingtalk-0.7.0/alicebot/adapter/dingtalk/exceptions.py
+-rw-r--r--   0        0        0     3436 2023-05-27 14:25:34.118713 alicebot_adapter_dingtalk-0.7.0/alicebot/adapter/dingtalk/message.py
+-rw-r--r--   0        0        0     1118 2023-05-27 14:25:34.118713 alicebot_adapter_dingtalk-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1288 1970-01-01 00:00:00.000000 alicebot_adapter_dingtalk-0.7.0/PKG-INFO
```

### Comparing `alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/__init__.py` & `alicebot_adapter_dingtalk-0.7.0/alicebot/adapter/dingtalk/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """DingTalk 协议适配器。
 
 本适配器适配了钉钉企业自建机器人协议。
-协议详情请参考: [钉钉开放平台](https://developers.dingtalk.com/document/robots/robot-overview) 。
+协议详情请参考: [钉钉开放平台](https://open.dingtalk.com/document/robots/robot-overview)。
 """
-import hmac
-import time
 import base64
 import hashlib
-from typing import Any, Dict, Union, Literal
+import hmac
+import time
+from typing import Any, Dict, Literal, Union
 
 import aiohttp
 from aiohttp import web
 
 from alicebot.adapter import Adapter
-from alicebot.log import logger, error_or_exception
+from alicebot.log import error_or_exception, logger
 
 from .config import Config
 from .event import DingTalkEvent
 from .exceptions import NetworkError
 from .message import DingTalkMessage
 
 __all__ = ["DingTalkAdapter"]
@@ -55,18 +55,18 @@
         await self.site.stop()
         await self.runner.cleanup()
 
     async def handler(self, request: web.Request):
         """处理 aiohttp 服务器的接收。
 
         Args:
-            request: aiohttp 服务器的 Request 对象。
+            request: aiohttp 服务器的 `Request` 对象。
         """
         if "timestamp" not in request.headers or "sign" not in request.headers:
-            logger.error(f"Illegal http header, incomplete http header")
+            logger.error("Illegal http header, incomplete http header")
         elif abs(int(request.headers["timestamp"]) - time.time() * 1000) > 3600000:
             logger.error(
                 f'Illegal http header, timestamp: {request.headers["timestamp"]}'
             )
         elif request.headers["sign"] != self.get_sign(request.headers["timestamp"]):
             logger.error(f'Illegal http header, sign: {request.headers["sign"]}')
         else:
@@ -89,31 +89,31 @@
             timestamp: 时间戳。
 
         Returns:
             签名。
         """
         hmac_code = hmac.new(
             self.config.app_secret.encode("utf-8"),
-            "{}\n{}".format(timestamp, self.config.app_secret).encode("utf-8"),
+            f"{timestamp}\n{self.config.app_secret}".encode(),
             digestmod=hashlib.sha256,
         ).digest()
         return base64.b64encode(hmac_code).decode("utf-8")
 
     async def send(
         self,
         webhook: str,
         conversation_type: Literal["1", "2"],
-        msg: Union[str, Dict, DingTalkMessage],
-        at: Union[None, Dict, DingTalkMessage] = None,
+        msg: Union[str, Dict[str, Any], DingTalkMessage],
+        at: Union[None, Dict[str, Any], DingTalkMessage] = None,
     ) -> Dict[str, Any]:
         """发送消息。
 
         Args:
             webhook: Webhook 网址。
-            conversation_type: 聊天类型，'1' 表示单聊，'2' 表示群聊。
+            conversation_type: 聊天类型，"1" 表示单聊，"2" 表示群聊。
             msg: 消息。
             at: At 对象，仅在群聊时生效，默认为空。
 
         Returns:
             钉钉服务器的响应。
 
         Raises:
@@ -154,9 +154,9 @@
             raise ValueError(
                 f'conversation_type must be "1" or "2" not {conversation_type}'
             )
 
         try:
             async with self.session.post(webhook, json=data) as resp:
                 return await resp.json()
-        except aiohttp.ClientError:
-            raise NetworkError
+        except aiohttp.ClientError as e:
+            raise NetworkError from e
```

### Comparing `alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/config.py` & `alicebot_adapter_dingtalk-0.7.0/alicebot/adapter/dingtalk/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """DingTalk 配置类，将在适配器被加载时被混入到机器人主配置中。
 
     Attributes:
         host: 本机域名。
         port: 监听的端口。
         url: 路径。
         api_timeout: 进行 API 调用时等待返回响应的超时时间。
-        app_secret: 机器人的 appSecret。
+        app_secret: 机器人的 `appSecret`。
     """
 
     __config_name__ = "dingtalk"
     host: str = "127.0.0.1"
     port: int = 8080
     url: str = "/dingtalk"
     api_timeout: int = 1000
```

### Comparing `alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/event.py` & `alicebot_adapter_dingtalk-0.7.0/alicebot/adapter/dingtalk/event.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 """DingTalk 适配器事件。"""
+from functools import cached_property
 import time
-from typing import TYPE_CHECKING, Any, Dict, List, Union, Literal, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional, Union
+from typing_extensions import Self
 
-from pydantic import Field, BaseModel, validator
+from pydantic import BaseModel, Field
 
-from alicebot.event import Event
+from alicebot.event import MessageEvent
 
-from .message import DingTalkMessage
 from .exceptions import WebhookExpiredError
+from .message import DingTalkMessage
 
 if TYPE_CHECKING:
-    from . import DingTalkAdapter
+    from . import DingTalkAdapter  # noqa: F401
 
 
 class UserInfo(BaseModel):
+    """用户信息"""
+
     dingtalkId: str
     staffId: Optional[str]
 
 
 class Text(BaseModel):
+    """文本消息"""
+
     content: str
 
 
-class DingTalkEvent(Event["DingTalkAdapter"]):
+class DingTalkEvent(MessageEvent["DingTalkAdapter", DingTalkMessage]):
     """DingTalk 事件基类"""
 
     type: Optional[str] = Field(alias="msgtype")
 
     msgtype: str
     msgId: str
     createAt: str
@@ -42,42 +48,60 @@
     chatbotCorpId: Optional[str]
     isInAtList: Optional[bool]
     senderStaffId: Optional[str]
     chatbotUserId: str
     atUsers: List[UserInfo]
     text: Text
 
-    message: Optional[DingTalkMessage]
-    response_msg: Union[None, str, Dict, DingTalkMessage] = None
-    response_at: Union[None, Dict, DingTalkMessage] = None
-
-    @validator("message", always=True)
-    def set_message(cls, v, values, **kwargs):  # type: ignore
-        return DingTalkMessage.text(values["text"].content)
+    response_msg: Union[None, str, Dict[str, Any], DingTalkMessage] = None
+    response_at: Union[None, Dict[str, Any], DingTalkMessage] = None
+
+    @cached_property
+    def message(self) -> DingTalkMessage:
+        """返回 message 字段。"""
+        return DingTalkMessage.text(self.text.content)
+
+    def get_plain_text(self) -> str:
+        """获取消息的纯文本内容。
+
+        Returns:
+            消息的纯文本内容。
+        """
+        return self.message.get_plain_text()
 
     async def reply(
         self,
-        msg: Union[str, Dict, DingTalkMessage],
-        at: Union[None, Dict, DingTalkMessage] = None,
+        message: Union[str, Dict[str, Any], DingTalkMessage],
+        at: Union[None, Dict[str, Any], DingTalkMessage] = None,
     ) -> Dict[str, Any]:
         """回复消息。
 
         Args:
-            msg: 回复消息的内容，可以是 str, Dict 或 DingTalkMessage。
-            at: 回复消息时 At 的对象，必须时 at 类型的 DingTalkMessage ，或者符合标准的 Dict。
+            message: 回复消息的内容，可以是 `str`, `Dict` 或 `DingTalkMessage`。
+            at: 回复消息时 At 的对象，必须时 at 类型的 `DingTalkMessage`，或者符合标准的 `Dict`。
 
         Returns:
             调用 Webhook 地址后钉钉服务器的响应。
 
         Raises:
             WebhookExpiredError: 当前事件的 Webhook 地址已经过期。
             ...: 同 `DingTalkAdapter.send()` 方法。
         """
         if self.sessionWebhookExpiredTime > time.time() * 1000:
             return await self.adapter.send(
                 webhook=self.sessionWebhook,
                 conversation_type=self.conversationType,
-                msg=msg,
+                msg=message,
                 at=at,
             )
-        else:
-            raise WebhookExpiredError
+        raise WebhookExpiredError
+
+    async def is_same_sender(self, other: Self) -> bool:
+        """判断自身和另一个事件是否是同一个发送者。
+
+        Args:
+            other: 另一个事件。
+
+        Returns:
+            是否是同一个发送者。
+        """
+        return self.senderId == other.senderId
```

### Comparing `alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/message.py` & `alicebot_adapter_dingtalk-0.7.0/alicebot/adapter/dingtalk/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,37 +2,45 @@
 from typing import Any, Dict, List, Optional
 
 from alicebot.message import MessageSegment
 
 __all__ = ["DingTalkMessage"]
 
 
-class DingTalkMessage(MessageSegment):
+class DingTalkMessage(MessageSegment):  # type: ignore
     """DingTalk 消息"""
 
     @property
     def _message_class(self) -> None:
         return None
 
     def __str__(self):
         if self.type == "text":
             return self.data["content"]
-        else:
-            return super().__str__()
+        return super().__str__()
+
+    def get_plain_text(self) -> str:
+        """获取消息中的纯文本部分。
+
+        Returns:
+            消息中的纯文本部分。
+        """
+        if self.type == "text":
+            return self.data["content"]
+        return ""
 
     def as_dict(self) -> Dict[str, Dict[str, Any]]:
         """返回符合钉钉消息标准的消息字段字典。
 
         Returns:
             符合钉钉消息标准的消息字段字典。
         """
         if self.type == "raw":
             return self.data
-        else:
-            return {self.type: self.data}
+        return {self.type: self.data}
 
     @classmethod
     def raw(cls, data: Dict[str, Any]) -> "DingTalkMessage":
         """DingTalk 原始消息"""
         return cls(type="raw", data=data)
 
     @classmethod
@@ -79,29 +87,29 @@
                 "singleURL": single_url,
                 "btnOrientation": btn_orientation,
             },
         )
 
     @classmethod
     def action_card_multi_btns(
-        cls, title: str, text: str, btns: list, btn_orientation: str = "0"
+        cls, title: str, text: str, btns: List[Any], btn_orientation: str = "0"
     ):
         """DingTalk 独立跳转 actionCard 消息"""
         return cls(
             type="actionCard",
             data={
                 "title": title,
                 "text": text,
                 "btns": btns,
                 "btnOrientation": btn_orientation,
             },
         )
 
     @classmethod
-    def feed_card(cls, links: list):
+    def feed_card(cls, links: List[Any]):
         """DingTalk feedCard 消息"""
         return cls(type="feedCard", data={"links": links})
 
     @classmethod
     def at(
         cls,
         at_mobiles: Optional[List[str]] = None,
```

### Comparing `alicebot_adapter_dingtalk-0.6.2/PKG-INFO` & `alicebot_adapter_dingtalk-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot-adapter-dingtalk
-Version: 0.6.2
+Version: 0.7.0
 Summary: DingTalk adapter for AliceBot.
 Home-page: https://docs.alicebot.dev/
 License: MIT
 Keywords: bot,chatbot,dingtalk
 Author: st1020
 Author-email: stone_1020@qq.com
 Requires-Python: >=3.8,<4.0
@@ -15,17 +15,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications :: Chat
-Requires-Dist: alicebot (==0.6.2)
+Requires-Dist: alicebot (==0.7.0)
 Project-URL: Documentation, https://docs.alicebot.dev/
 Project-URL: Repository, https://github.com/AliceBotProject/alicebot
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/AliceBotProject/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
```

#### html2text {}

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 2.1 Name: alicebot-adapter-dingtalk Version: 0.6.2 Summary:
+Metadata-Version: 2.1 Name: alicebot-adapter-dingtalk Version: 0.7.0 Summary:
 DingTalk adapter for AliceBot. Home-page: https://docs.alicebot.dev/ License:
 MIT Keywords: bot,chatbot,dingtalk Author: st1020 Author-email:
 stone_1020@qq.com Requires-Python: >=3.8,<4.0 Classifier: Development Status ::
 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework :: Robot
 Framework Classifier: Framework :: Robot Framework :: Library Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Classifier: Topic :: Communications :: Chat Requires-Dist: alicebot
-(==0.6.2) Project-URL: Documentation, https://docs.alicebot.dev/ Project-URL:
-Repository, https://github.com/AliceBotProject/alicebot Description-Content-
-Type: text/markdown
+Programming Language :: Python :: 3.11 Classifier: Topic :: Communications ::
+Chat Requires-Dist: alicebot (==0.7.0) Project-URL: Documentation, https://
+docs.alicebot.dev/ Project-URL: Repository, https://github.com/AliceBotProject/
+alicebot Description-Content-Type: text/markdown
            [logo] # AliceBot-Adapter-DingTalk **ééåè®®éé**
```

