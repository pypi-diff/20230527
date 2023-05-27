# Comparing `tmp/alicebot_adapter_cqhttp-0.6.2.tar.gz` & `tmp/alicebot_adapter_cqhttp-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot_adapter_cqhttp-0.6.2.tar", max compression
+gzip compressed data, was "alicebot_adapter_cqhttp-0.7.0.tar", max compression
```

## Comparing `alicebot_adapter_cqhttp-0.6.2.tar` & `alicebot_adapter_cqhttp-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      267 2023-04-25 11:14:36.277730 alicebot_adapter_cqhttp-0.6.2/README.md
--rw-r--r--   0        0        0     9890 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/__init__.py
--rw-r--r--   0        0        0      875 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/config.py
--rw-r--r--   0        0        0     9252 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/event.py
--rw-r--r--   0        0        0      706 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/exceptions.py
--rw-r--r--   0        0        0     7530 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/message.py
--rw-r--r--   0        0        0     1347 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1360 1970-01-01 00:00:00.000000 alicebot_adapter_cqhttp-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      267 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/README.md
+-rw-r--r--   0        0        0     9917 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/__init__.py
+-rw-r--r--   0        0        0      875 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/config.py
+-rw-r--r--   0        0        0    10223 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/event.py
+-rw-r--r--   0        0        0      719 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/exceptions.py
+-rw-r--r--   0        0        0     7571 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/message.py
+-rw-r--r--   0        0        0     1081 2023-05-27 14:25:34.118713 alicebot_adapter_cqhttp-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 alicebot_adapter_cqhttp-0.7.0/PKG-INFO
```

### Comparing `alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/__init__.py` & `alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """CQHTTP 协议适配器。
 
 本适配器适配了 OneBot v11 协议。
 协议详情请参考: [OneBot](https://github.com/howmanybots/onebot/blob/master/README.md) 。
 """
-import sys
-import json
-import time
 import asyncio
-import inspect
 from functools import partial
+import inspect
+import json
+import sys
+import time
 from typing import (
     TYPE_CHECKING,
     Any,
-    Dict,
-    Type,
-    Tuple,
-    Literal,
+    Awaitable,
     Callable,
     ClassVar,
+    Dict,
+    Literal,
     Optional,
-    Awaitable,
+    Tuple,
+    Type,
 )
 
 import aiohttp
 from aiohttp import web
 
-from alicebot.utils import DataclassEncoder
 from alicebot.adapter.utils import WebSocketAdapter
-from alicebot.log import logger, error_or_exception
+from alicebot.log import error_or_exception, logger
+from alicebot.utils import DataclassEncoder
 
 from . import event
 from .config import Config
+from .event import CQHTTPEvent, HeartbeatMetaEvent, LifecycleMetaEvent, MetaEvent
+from .exceptions import ActionFailed, ApiNotAvailable, ApiTimeout, NetworkError
 from .message import CQHTTPMessage
-from .exceptions import ApiTimeout, ActionFailed, NetworkError, ApiNotAvailable
-from .event import MetaEvent, CQHTTPEvent, HeartbeatMetaEvent, LifecycleMetaEvent
 
 if TYPE_CHECKING:
     from .message import T_CQMSG
 
 __all__ = ["CQHTTPAdapter"]
 
 T_EventModels = Dict[
@@ -76,15 +76,15 @@
         self.url = self.config.url
         self.reconnect_interval = self.config.reconnect_interval
         self._api_response_cond = asyncio.Condition()
         await super().startup()
 
     async def reverse_ws_connection_hook(self):
         """反向 WebSocket 连接建立时的钩子函数。"""
-        logger.info(f"WebSocket connected!")
+        logger.info("WebSocket connected!")
         if self.config.access_token:
             assert isinstance(self.websocket, web.WebSocketResponse)
             if (
                 self.websocket.headers.get("Authorization", "")
                 != f"Bearer {self.config.access_token}"
             ):
                 await self.websocket.close()
@@ -225,16 +225,16 @@
         try:
             await self.websocket.send_str(
                 json.dumps(
                     {"action": api, "params": params, "echo": api_echo},
                     cls=DataclassEncoder,
                 )
             )
-        except Exception:
-            raise NetworkError
+        except Exception as e:
+            raise NetworkError from e
 
         start_time = time.time()
         while not self.bot.should_exit.is_set():
             if time.time() - start_time > self.config.api_timeout:
                 break
             async with self._api_response_cond:
                 try:
@@ -249,37 +249,37 @@
                         raise ApiNotAvailable(resp=self._api_response)
                     if self._api_response.get("status") == "failed":
                         raise ActionFailed(resp=self._api_response)
                     return self._api_response.get("data")
 
         if not self.bot.should_exit.is_set():
             raise ApiTimeout
+        return None
 
     async def send(
         self, message_: "T_CQMSG", message_type: Literal["private", "group"], id_: int
     ) -> Any:
-        """发送消息，调用 send_private_msg 或 send_group_msg API 发送消息。
+        """发送消息，调用 `send_private_msg` 或 `send_group_msg` API 发送消息。
 
         Args:
-            message_: 消息内容，可以是 str, Mapping, Iterable[Mapping],
-                'CQHTTPMessageSegment', 'CQHTTPMessage'。
+            message_: 消息内容，可以是 `str`, `Mapping`, `Iterable[Mapping]`,
+                `CQHTTPMessageSegment`, `CQHTTPMessage。`
                 将使用 `CQHTTPMessage` 进行封装。
-            message_type: 消息类型。应该是 private 或者 group。
+            message_type: 消息类型。应该是 "private" 或者 "group"。
             id_: 发送对象的 ID ， QQ 号码或者群号码。
 
         Returns:
             API 响应。
 
         Raises:
-            TypeError: message_type 不是 'private' 或 'group'。
+            TypeError: `message_type` 不是 "private" 或 "group"。
             ...: 同 `call_api()` 方法。
         """
         if message_type == "private":
             return await self.send_private_msg(
                 user_id=id_, message=CQHTTPMessage(message_)
             )
-        elif message_type == "group":
+        if message_type == "group":
             return await self.send_group_msg(
                 group_id=id_, message=CQHTTPMessage(message_)
             )
-        else:
-            raise TypeError('message_type must be "private" or "group"')
+        raise TypeError('message_type must be "private" or "group"')
```

### Comparing `alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/config.py` & `alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/config.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/event.py` & `alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/event.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 """CQHTTP 适配器事件。"""
-import inspect
-from typing import TYPE_CHECKING, Any, Dict, Tuple, Literal, Optional
+from typing import TYPE_CHECKING, Any, Dict, Literal, Optional, Tuple
+from typing_extensions import Self
 
-from pydantic import Field, BaseModel
+from pydantic import BaseModel, Field
 from pydantic.fields import ModelField
-from pydantic.typing import is_literal_type, all_literal_values
+from pydantic.typing import all_literal_values, is_literal_type
 
 from alicebot.event import Event
+from alicebot.event import MessageEvent as BaseMessageEvent
 
 from .message import CQHTTPMessage
 
 if TYPE_CHECKING:
-    from . import CQHTTPAdapter
+    from . import CQHTTPAdapter  # noqa: F401
     from .message import T_CQMSG
 
 
 class Sender(BaseModel):
+    """发送人信息"""
+
     user_id: Optional[int]
     nickname: Optional[str]
     card: Optional[str]
     sex: Optional[Literal["male", "female", "unknown"]]
     age: Optional[int]
     area: Optional[str]
     level: Optional[str]
     role: Optional[str]
     title: Optional[str]
 
 
 class Anonymous(BaseModel):
+    """匿名信息"""
+
     id: int
     name: str
     flag: str
 
 
 class File(BaseModel):
+    """文件信息"""
+
     id: str
     name: str
     size: int
     busid: int
 
 
 class Status(BaseModel):
+    """状态信息"""
+
     online: bool
     good: bool
 
     class Config:
         extra = "allow"
 
 
@@ -64,16 +73,16 @@
     type: Optional[str] = Field(alias="post_type")
     time: int
     self_id: int
     post_type: str
 
     @property
     def to_me(self) -> bool:
-        """当前事件的 user_id 是否等于 self_id。"""
-        return getattr(self, "user_id") == self.self_id
+        """当前事件的 `user_id` 是否等于 `self_id`。"""
+        return getattr(self, "user_id", None) == self.self_id
 
     @classmethod
     def get_event_type(cls) -> Tuple[Optional[str], Optional[str], Optional[str]]:
         """获取事件类型。
 
         Returns:
             事件类型。
@@ -85,15 +94,15 @@
         detail_type_field = cls.__fields__.get(post_type + "_type", None)
         detail_type = detail_type_field and _get_literal_field(detail_type_field)
         sub_type_field = cls.__fields__.get("sub_type", None)
         sub_type = sub_type_field and _get_literal_field(sub_type_field)
         return (post_type, detail_type, sub_type)
 
 
-class MessageEvent(CQHTTPEvent):
+class MessageEvent(CQHTTPEvent, BaseMessageEvent["CQHTTPAdapter", CQHTTPMessage]):
     """消息事件"""
 
     __event__ = "message"
     post_type: Literal["message"]
     message_type: Literal["private", "group"]
     sub_type: str
     message_id: int
@@ -110,51 +119,78 @@
         """获取消息的纯文本内容。
 
         Returns:
             消息的纯文本内容。
         """
         return self.message.get_plain_text()
 
-    async def reply(self, msg: "T_CQMSG") -> Dict[str, Any]:
+    async def reply(self, message: "T_CQMSG") -> Dict[str, Any]:
         """回复消息。
 
         Args:
-            msg: 回复消息的内容，同 `call_api()` 方法。
+            message: 回复消息的内容，同 `call_api()` 方法。
 
         Returns:
             API 请求响应。
         """
         raise NotImplementedError
 
+    async def is_same_sender(self, other: Self) -> bool:
+        """判断自身和另一个事件是否是同一个发送者。
+
+        Args:
+            other: 另一个事件。
+
+        Returns:
+            是否是同一个发送者。
+        """
+        return self.sender.user_id == other.sender.user_id
+
 
 class PrivateMessageEvent(MessageEvent):
     """私聊消息"""
 
     __event__ = "message.private"
     message_type: Literal["private"]
     sub_type: Literal["friend", "group", "other"]
 
-    async def reply(self, msg: "T_CQMSG") -> Dict[str, Any]:
+    async def reply(self, message: "T_CQMSG") -> Dict[str, Any]:
+        """回复消息。
+
+        Args:
+            message: 回复消息的内容，同 `call_api()` 方法。
+
+        Returns:
+            API 请求响应。
+        """
         return await self.adapter.send_private_msg(
-            user_id=self.user_id, message=CQHTTPMessage(msg)
+            user_id=self.user_id, message=CQHTTPMessage(message)
         )
 
 
 class GroupMessageEvent(MessageEvent):
     """群消息"""
 
     __event__ = "message.group"
     message_type: Literal["group"]
     sub_type: Literal["normal", "anonymous", "notice"]
     group_id: int
     anonymous: Optional[Anonymous] = None
 
-    async def reply(self, msg: "T_CQMSG") -> Dict[str, Any]:
+    async def reply(self, message: "T_CQMSG") -> Dict[str, Any]:
+        """回复消息。
+
+        Args:
+            message: 回复消息的内容，同 `call_api()` 方法。
+
+        Returns:
+            API 请求响应。
+        """
         return await self.adapter.send_group_msg(
-            group_id=self.group_id, message=CQHTTPMessage(msg)
+            group_id=self.group_id, message=CQHTTPMessage(message)
         )
 
 
 class NoticeEvent(CQHTTPEvent):
     """通知事件"""
 
     __event__ = "notice"
@@ -324,14 +360,19 @@
             API 请求响应。
         """
         return await self.adapter.set_friend_add_request(
             flag=self.flag, approve=True, remark=remark
         )
 
     async def refuse(self) -> Dict[str, Any]:
+        """拒绝请求。
+
+        Returns:
+            API 请求响应。
+        """
         return await self.adapter.set_friend_add_request(flag=self.flag, approve=False)
 
 
 class GroupRequestEvent(RequestEvent):
     """加群请求／邀请"""
 
     __event__ = "request.group"
@@ -339,14 +380,19 @@
     sub_type: Literal["add", "invite"]
     group_id: int
     user_id: int
     comment: str
     flag: str
 
     async def approve(self) -> Dict[str, Any]:
+        """同意请求。
+
+        Returns:
+            API 请求响应。
+        """
         return await self.adapter.set_group_add_request(
             flag=self.flag, sub_type=self.sub_type, approve=True
         )
 
     async def refuse(self, reason: str = "") -> Dict[str, Any]:
         """拒绝请求。
 
@@ -380,14 +426,7 @@
 class HeartbeatMetaEvent(MetaEvent):
     """心跳"""
 
     __event__ = "meta_event.heartbeat"
     meta_event_type: Literal["heartbeat"]
     status: Status
     interval: int
-
-
-_cqhttp_events = {
-    model.__event__: model
-    for model in globals().values()
-    if inspect.isclass(model) and issubclass(model, CQHTTPEvent)
-}
```

### Comparing `alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/exceptions.py` & `alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     """网络异常。"""
 
 
 class ActionFailed(CQHTTPException):
     """API 请求成功响应，但响应表示 API 操作失败。"""
 
     def __init__(self, resp: Dict[str, Any]):
-        """
+        """初始化。
+
         Args:
             resp: 返回的响应。
         """
         self.resp = resp
 
 
 class ApiNotAvailable(ActionFailed):
```

### Comparing `alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/message.py` & `alicebot_adapter_cqhttp-0.7.0/alicebot/adapter/cqhttp/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """CQHTTP 适配器消息。"""
-from typing import Any, Type, Union, Literal, Mapping, Iterable, Optional
+from typing import Any, Iterable, Literal, Mapping, Optional, Type, Union
 
 from alicebot.message import Message, MessageSegment
 
 __all__ = ["T_CQMSG", "CQHTTPMessage", "CQHTTPMessageSegment", "escape"]
 
 T_CQMSG = Union[
     str,
@@ -34,15 +34,16 @@
 
     def __str__(self) -> str:
         if self.type == "text":
             return self.data.get("text", "")
         return self.get_cqcode()
 
     def get_cqcode(self) -> str:
-        """
+        """获取此消息字段的 CQ 码形式。
+
         Returns:
             此消息字段的 CQ 码形式。
         """
         if self.type == "text":
             return escape(self.data.get("text", ""), escape_comma=False)
 
         params = ",".join(
```

### Comparing `alicebot_adapter_cqhttp-0.6.2/pyproject.toml` & `alicebot_adapter_cqhttp-0.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alicebot-adapter-cqhttp"
-version = "0.6.2"
+version = "0.7.0"
 description = "OneBot(CQHTTP) adapter for AliceBot."
 license = "MIT"
 authors = ["st1020 <stone_1020@qq.com>"]
 readme = "README.md"
 homepage = "https://docs.alicebot.dev/"
 repository = "https://github.com/AliceBotProject/alicebot"
 documentation = "https://docs.alicebot.dev/"
@@ -20,28 +20,15 @@
     "Topic :: Communications :: Chat",
 ]
 packages = [{ include = "alicebot" }]
 exclude = ["alicebot/__init__.py", "alicebot/adapter/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-alicebot = "0.6.2"
+alicebot = "0.7.0"
 
 [tool.poetry.dev-dependencies]
 alicebot = { path = "../../", develop = true }
 
-[tool.pydantic-pycharm-plugin]
-ignore-init-method-arguments = true
-
-[tool.black]
-target-version = ["py38", "py39", "py310"]
-
-[tool.isort]
-profile = "black"
-length_sort = true
-skip_gitignore = true
-force_sort_within_sections = true
-src_paths = ["alicebot", "tests"]
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `alicebot_adapter_cqhttp-0.6.2/PKG-INFO` & `alicebot_adapter_cqhttp-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot-adapter-cqhttp
-Version: 0.6.2
+Version: 0.7.0
 Summary: OneBot(CQHTTP) adapter for AliceBot.
 Home-page: https://docs.alicebot.dev/
 License: MIT
 Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq
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
-Metadata-Version: 2.1 Name: alicebot-adapter-cqhttp Version: 0.6.2 Summary:
+Metadata-Version: 2.1 Name: alicebot-adapter-cqhttp Version: 0.7.0 Summary:
 OneBot(CQHTTP) adapter for AliceBot. Home-page: https://docs.alicebot.dev/
 License: MIT Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq Author: st1020 Author-
 email: stone_1020@qq.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework ::
 Robot Framework Classifier: Framework :: Robot Framework :: Library Classifier:
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
        [logo] # AliceBot-Adapter-CQHTTP **OneBot(CQHTTP) åè®®éé**
```

