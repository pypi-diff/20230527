# Comparing `tmp/alicebot_adapter_mirai-0.6.2.tar.gz` & `tmp/alicebot_adapter_mirai-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot_adapter_mirai-0.6.2.tar", max compression
+gzip compressed data, was "alicebot_adapter_mirai-0.7.0.tar", max compression
```

## Comparing `alicebot_adapter_mirai-0.6.2.tar` & `alicebot_adapter_mirai-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34522 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/LICENSE
--rw-r--r--   0        0        0      258 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/README.md
--rw-r--r--   0        0        0     9718 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/__init__.py
--rw-r--r--   0        0        0     1032 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/config.py
--rw-r--r--   0        0        0      119 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/__init__.py
--rw-r--r--   0        0        0      825 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/base.py
--rw-r--r--   0        0        0     1042 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/mate.py
--rw-r--r--   0        0        0     3650 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/message.py
--rw-r--r--   0        0        0     5492 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/notice.py
--rw-r--r--   0        0        0     4264 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/request.py
--rw-r--r--   0        0        0      647 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/exceptions.py
--rw-r--r--   0        0        0     4425 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/message.py
--rw-r--r--   0        0        0     1341 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 alicebot_adapter_mirai-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/LICENSE
+-rw-r--r--   0        0        0      258 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/README.md
+-rw-r--r--   0        0        0     9728 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/__init__.py
+-rw-r--r--   0        0        0     1034 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/config.py
+-rw-r--r--   0        0        0      119 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/__init__.py
+-rw-r--r--   0        0        0      987 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/base.py
+-rw-r--r--   0        0        0     1088 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/mate.py
+-rw-r--r--   0        0        0     5390 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/message.py
+-rw-r--r--   0        0        0     5659 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/notice.py
+-rw-r--r--   0        0        0     4922 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/request.py
+-rw-r--r--   0        0        0      659 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/exceptions.py
+-rw-r--r--   0        0        0     5081 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/message.py
+-rw-r--r--   0        0        0     1138 2023-05-27 14:25:34.122713 alicebot_adapter_mirai-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 alicebot_adapter_mirai-0.7.0/PKG-INFO
```

### Comparing `alicebot_adapter_mirai-0.6.2/LICENSE` & `alicebot_adapter_mirai-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/__init__.py` & `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """Mirai 协议适配器。
 
 本适配器适配了 mirai-api-http 协议，仅支持 mirai-api-http 2.3.0 及以上版本。
 本适配器支持 mirai-api-http 的 Websocket Adapter 模式和 Reverse Websocket Adapter 模式。
 协议详情请参考: [mirai-api-http](https://github.com/project-mirai/mirai-api-http) 。
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
-    Literal,
+    Awaitable,
     Callable,
     ClassVar,
+    Dict,
+    Literal,
     Optional,
-    Awaitable,
+    Type,
 )
 
 import aiohttp
 
-from alicebot.utils import DataclassEncoder
 from alicebot.adapter.utils import WebSocketAdapter
-from alicebot.log import logger, error_or_exception
+from alicebot.log import error_or_exception, logger
+from alicebot.utils import DataclassEncoder
 
 from . import event
 from .config import Config
+from .event import BotEvent, CommandExecutedEvent, MateEvent, MiraiEvent
+from .exceptions import ActionFailed, ApiTimeout, NetworkError
 from .message import MiraiMessage
-from .exceptions import ApiTimeout, ActionFailed, NetworkError
-from .event import BotEvent, MateEvent, MiraiEvent, CommandExecutedEvent
 
 if TYPE_CHECKING:
     from .message import T_MiraiMSG
 
 __all__ = ["MiraiAdapter"]
 
 
@@ -55,14 +55,15 @@
         for name, model in inspect.getmembers(event, inspect.isclass)
         if issubclass(model, MiraiEvent)
     }
 
     _api_response: Dict[str, Any]
     _api_response_cond: asyncio.Condition
     _sync_id: int = 0
+    _verify_identity_task: "asyncio.Task[None]"
 
     def __getattr__(self, item: str) -> Callable[..., Awaitable[Any]]:
         return partial(self.call_api, item)
 
     async def startup(self):
         """初始化适配器。"""
         self.adapter_type = self.config.adapter_type
@@ -71,16 +72,16 @@
         self.url = self.config.url
         self.reconnect_interval = self.config.reconnect_interval
         self._api_response_cond = asyncio.Condition()
         await super().startup()
 
     async def reverse_ws_connection_hook(self):
         """反向 WebSocket 连接建立时的钩子函数。"""
-        logger.info(f"WebSocket connected!")
-        asyncio.create_task(self.verify_identity())
+        logger.info("WebSocket connected!")
+        self._verify_identity_task = asyncio.create_task(self.verify_identity())
 
     async def websocket_connect(self):
         """创建正向 WebSocket 连接。"""
         assert self.session is not None
         logger.info("Trying to verify identity and create connection...")
         async with self.session.ws_connect(
             f"ws://{self.host}:{self.port}/all?"
@@ -98,15 +99,15 @@
                 error_or_exception(
                     "WebSocket message parsing error, not json:",
                     e,
                     self.bot.config.bot.log.verbose_exception,
                 )
                 return
 
-            if msg_dict.get("syncId") == "":
+            if not msg_dict.get("syncId", None):
                 if msg_dict.get("data", {}).get("code") == 0:
                     logger.info(
                         f"Verify success! "
                         f"Session key: {msg_dict.get('data').get('session')}"
                     )
                 else:
                     logger.warning(
@@ -166,28 +167,26 @@
         """验证身份，创建与 Mirai-api-http 的连接。"""
         while not self.bot.should_exit.is_set():
             await asyncio.sleep(self.reconnect_interval)
             try:
                 logger.info("Trying to verify identity and create connection...")
                 await self.call_api(
                     "verify",
-                    **{
-                        "verifyKey": self.config.verify_key,
-                        "sessionKey": None,
-                        "qq": self.config.qq,
-                    },
+                    verifyKey=self.config.verify_key,
+                    sessionKey=None,
+                    qq=self.config.qq,
                 )
             except ActionFailed as e:
                 logger.warning(f"Verify failed with code {e.code}, retrying...")
             else:
                 logger.info("Verify success!")
                 return
 
     async def call_api(
-        self, command: str, sub_command: Optional[str] = None, **content: Dict[str, Any]
+        self, command: str, sub_command: Optional[str] = None, **content: Any
     ) -> Any:
         """调用 Mirai API ，协程会等待直到获得 API 响应。
 
         Args:
             command: 命令字。
             sub_command: 子命令字。
             **content: 请求内容。
@@ -210,16 +209,16 @@
                         "command": command,
                         "subCommand": sub_command,
                         "content": content,
                     },
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
@@ -243,31 +242,30 @@
         message_type: Literal["private", "friend", "group"],
         target: int,
         quote: Optional[int] = None,
     ) -> Any:
         """调用 Mirai API 发送消息。
 
         Args:
-            message_: 消息内容，可以是 str, Mapping, Iterable[Mapping],
-                'MiraiMessageSegment', 'MiraiMessage'。
+            message_: 消息内容，可以是 `str`, `Mapping`, `Iterable[Mapping]`,
+                `MiraiMessageSegment`, `MiraiMessage`。
                 将使用 `MiraiMessage` 进行封装。
-            message_type: 消息类型。应该是 private, friend 或者 group。其中 private 和 friend 相同。
+            message_type: 消息类型。应该是 "private", "friend" 或者 "group"。其中 "private" 和 "friend" 相同。
             target: 发送对象的 ID ， QQ 号码或者群号码。
-            quote: 引用的消息的 messageId。默认为 `None` ，不引用任何消息。
+            quote: 引用的消息的 `messageId`。默认为 `None`，不引用任何消息。
 
         Returns:
             API 响应。
 
         Raises:
             TypeError: message_type 非法。
             ...: 同 `call_api()` 方法。
         """
         if message_type == "private" or message_type == "friend":
             return await self.sendFriendMessage(
                 target=target, messageChain=MiraiMessage(message_), quote=quote
             )
-        elif message_type == "group":
+        if message_type == "group":
             return await self.sendGroupMessage(
                 target=target, messageChain=MiraiMessage(message_), quote=quote
             )
-        else:
-            raise TypeError('message_type must be "private", "friend" or "group"')
+        raise TypeError('message_type must be "private", "friend" or "group"')
```

### Comparing `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/config.py` & `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Attributes:
         adapter_type: 适配器类型，需要和协议端配置相同。
         host: 本机域名。
         port: 监听的端口。
         url: WebSocket 路径，需要和协议端配置相同。
         reconnect_interval: 重连等待时间。
         api_timeout: 进行 API 调用时等待返回响应的超时时间。
-        verify_key: 建立连接时的认证密钥，需要和 mirai-api-http 配置中的 verifyKey 相同，如果关闭验证则留空。
+        verify_key: 建立连接时的认证密钥，需要和 mirai-api-http 配置中的 `verifyKey` 相同，如果关闭验证则留空。
         qq: 机器人的 QQ 号码，必须指定。
     """
 
     __config_name__ = "mirai"
     adapter_type: Literal["ws", "reverse-ws"] = "ws"
     host: str = "127.0.0.1"
     port: int = 8080
```

### Comparing `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/mate.py` & `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/mate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+"""默认不会被传播的特殊事件。"""
 from typing import Any, List, Literal, Optional
 
-from .base import FriendInfo, MiraiEvent, GroupMemberInfo
+from .base import FriendInfo, GroupMemberInfo, MiraiEvent
 
 
 class MateEvent(MiraiEvent):
     """默认不会被传播的特殊事件"""
 
 
 class BotEvent(MateEvent):
```

### Comparing `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/message.py` & `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/message.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,129 +1,189 @@
-from typing import TYPE_CHECKING, Any, Dict, Literal
+"""消息事件。"""
+from typing import TYPE_CHECKING, Any, Dict, Literal, Union
+from typing_extensions import Self
+
+from alicebot.event import MessageEvent as BaseMessageEvent
 
 from ..message import MiraiMessage
-from .base import FriendInfo, MiraiEvent, GroupMemberInfo, OtherClientSender
+from .base import FriendInfo, GroupMemberInfo, MiraiEvent, OtherClientSender
 
 if TYPE_CHECKING:
+    from .. import MiraiAdapter  # noqa: F401
     from ..message import T_MiraiMSG
 
 
-class MessageEvent(MiraiEvent):
+class MessageEvent(MiraiEvent, BaseMessageEvent["MiraiAdapter", MiraiMessage]):
     """消息事件"""
 
+    sender: Union[FriendInfo, GroupMemberInfo, OtherClientSender]
     messageChain: MiraiMessage
 
     @property
-    def message(self):
+    def message(self) -> MiraiMessage:
+        """与 messageChain 相同。"""
         return self.messageChain
 
     def __repr__(self) -> str:
         return f'Event<{self.type}>: "{self.messageChain}"'
 
     def get_plain_text(self) -> str:
-        """
+        """获取消息的纯文本内容。
+
         Returns:
             消息的纯文本内容。
         """
         return self.messageChain.get_plain_text()
 
-    async def reply(self, msg: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
+    async def reply(self, message: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
         """回复消息。
 
         Args:
-            msg: 回复消息的内容，同 `call_api()` 方法。
+            message: 回复消息的内容，同 `call_api()` 方法。
             quote: 引用消息，默认为 `False`。
 
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
+        return self.sender.id == other.sender.id
+
 
 class FriendMessage(MessageEvent):
     """好友消息"""
 
     type: Literal["FriendMessage"]
     sender: FriendInfo
 
-    async def reply(self, msg: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
+    async def reply(self, message: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
+        """回复消息。
+
+        Args:
+            message: 回复消息的内容，同 `call_api()` 方法。
+            quote: 引用消息，默认为 `False`。
+
+        Returns:
+            API 请求响应。
+        """
         if quote:
             return await self.adapter.send(
-                msg,
+                message,
                 message_type="friend",
                 target=self.sender.id,
-                quote=self.messageChain[0].id,  # type: ignore
-            )
-        else:
-            return await self.adapter.send(
-                msg, message_type="friend", target=self.sender.id
+                quote=self.messageChain[0]["id"],
             )
+        return await self.adapter.send(
+            message, message_type="friend", target=self.sender.id
+        )
 
 
 class GroupMessage(MessageEvent):
     """群消息"""
 
     type: Literal["GroupMessage"]
     sender: GroupMemberInfo
 
-    async def reply(self, msg: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
+    async def reply(self, message: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
+        """回复消息。
+
+        Args:
+            message: 回复消息的内容，同 `call_api()` 方法。
+            quote: 引用消息，默认为 `False`。
+
+        Returns:
+            API 请求响应。
+        """
         if quote:
             return await self.adapter.send(
-                msg,
+                message,
                 message_type="group",
                 target=self.sender.group.id,
-                quote=self.messageChain[0].id,  # type: ignore
-            )
-        else:
-            return await self.adapter.send(
-                msg, message_type="group", target=self.sender.group.id
+                quote=self.messageChain[0]["id"],
             )
+        return await self.adapter.send(
+            message, message_type="group", target=self.sender.group.id
+        )
 
 
 class TempMessage(MessageEvent):
     """群临时消息"""
 
     type: Literal["TempMessage"]
     sender: GroupMemberInfo
 
-    async def reply(self, msg: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
+    async def reply(self, message: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
+        """回复消息。
+
+        Args:
+            message: 回复消息的内容，同 `call_api()` 方法。
+            quote: 引用消息，默认为 `False`。
+
+        Returns:
+            API 请求响应。
+        """
         if quote:
             return await self.adapter.sendTempMessage(
                 qq=self.sender.id,
                 group=self.sender.group.id,
-                messageChain=msg,
-                quote=self.messageChain[0].id,  # type: ignore
-            )
-        else:
-            return await self.adapter.sendTempMessage(
-                qq=self.sender.id, group=self.sender.group.id, messageChain=msg
+                messageChain=message,
+                quote=self.messageChain[0]["id"],
             )
+        return await self.adapter.sendTempMessage(
+            qq=self.sender.id, group=self.sender.group.id, messageChain=message
+        )
 
 
 class StrangerMessage(MessageEvent):
     """陌生人消息"""
 
     type: Literal["StrangerMessage"]
     sender: FriendInfo
 
-    async def reply(self, msg: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
+    async def reply(self, message: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
+        """回复消息。
+
+        Args:
+            message: 回复消息的内容，同 `call_api()` 方法。
+            quote: 引用消息，默认为 `False`。
+
+        Returns:
+            API 请求响应。
+        """
         if quote:
             return await self.adapter.send(
-                msg,
+                message,
                 message_type="friend",
                 target=self.sender.id,
-                quote=self.messageChain[0].id,  # type: ignore
-            )
-        else:
-            return await self.adapter.send(
-                msg, message_type="friend", target=self.sender.id
+                quote=self.messageChain[0]["id"],
             )
+        return await self.adapter.send(
+            message, message_type="friend", target=self.sender.id
+        )
 
 
 class OtherClientMessage(MessageEvent):
     """其他客户端消息"""
 
     type: Literal["OtherClientMessage"]
     sender: OtherClientSender
 
-    async def reply(self, msg: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
+    async def reply(self, message: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
+        """回复消息。
+
+        Args:
+            message: 回复消息的内容，同 `call_api()` 方法。
+            quote: 引用消息，默认为 `False`。
+
+        Returns:
+            API 请求响应。
+        """
         raise NotImplementedError
```

### Comparing `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/notice.py` & `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/notice.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+"""通知事件。"""
 from typing import Literal, Optional
 
 from pydantic import create_model
 
 from .base import (
-    Subject,
-    GroupInfo,
     FriendInfo,
+    GroupInfo,
+    GroupMemberInfo,
     MiraiEvent,
     Permission,
-    GroupMemberInfo,
+    Subject,
 )
 
 
 class NoticeEvent(MiraiEvent):
     """通知事件"""
 
 
@@ -111,14 +112,21 @@
 class BotLeaveEventKick(GroupBotEvent):
     """Bot 被踢出一个群"""
 
     type: Literal["BotLeaveEventKick"]
     group: GroupInfo
 
 
+class BotLeaveEventDisband(GroupBotEvent):
+    """Bot 所在的群被解散"""
+
+    type: Literal["BotLeaveEventDisband"]
+    group: GroupInfo
+
+
 class GroupNoticeEvent(GroupEvent):
     """其他群事件"""
 
 
 class GroupRecallEvent(GroupNoticeEvent):
     """群消息撤回"""
```

### Comparing `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/request.py` & `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/event/request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""申请事件。"""
 from typing import Any, Dict, Literal
 
 from .base import MiraiEvent
 
 
 class RequestEvent(MiraiEvent):
     """申请事件"""
@@ -36,14 +37,22 @@
     eventId: int
     fromId: int
     groupId: int
     nick: str
     message: str
 
     async def approve(self, message: str = "") -> Dict[str, Any]:
+        """同意请求。
+
+        Args:
+            message: 回复的信息，默认为空。
+
+        Returns:
+            API 请求响应。
+        """
         return await self.adapter.resp_newFriendRequestEvent(
             eventId=self.eventId,
             fromId=self.fromId,
             groupId=self.groupId,
             operate=0,
             message=message,
         )
@@ -77,14 +86,22 @@
     fromId: int
     groupId: int
     groupName: str
     nick: str
     message: str
 
     async def approve(self, message: str = "") -> Dict[str, Any]:
+        """同意请求。
+
+        Args:
+            message: 回复的信息，默认为空。
+
+        Returns:
+            API 请求响应。
+        """
         return await self.adapter.resp_memberJoinRequestEvent(
             eventId=self.eventId,
             fromId=self.fromId,
             groupId=self.groupId,
             operate=0,
             message=message,
         )
@@ -138,23 +155,39 @@
     fromId: int
     groupId: int
     groupName: str
     nick: str
     message: str
 
     async def approve(self, message: str = "") -> Dict[str, Any]:
+        """同意请求。
+
+        Args:
+            message: 回复的信息，默认为空。
+
+        Returns:
+            API 请求响应。
+        """
         return await self.adapter.resp_botInvitedJoinGroupRequestEvent(
             eventId=self.eventId,
             fromId=self.fromId,
             groupId=self.groupId,
             operate=0,
             message=message,
         )
 
     async def refuse(self, message: str = "") -> Dict[str, Any]:
+        """拒绝请求。
+
+        Args:
+            message: 回复的信息，默认为空。
+
+        Returns:
+            API 请求响应。
+        """
         return await self.adapter.resp_botInvitedJoinGroupRequestEvent(
             eventId=self.eventId,
             fromId=self.fromId,
             groupId=self.groupId,
             operate=1,
             message=message,
         )
```

### Comparing `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/exceptions.py` & `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Mirai 适配器异常。
-"""
+"""Mirai 适配器异常。"""
 from typing import Any, Dict
 
 from alicebot.exceptions import AdapterException
 
 
 class MiraiException(AdapterException):
     """Mirai 异常基类。"""
@@ -13,15 +12,16 @@
     """网络异常。"""
 
 
 class ActionFailed(MiraiException):
     """API 请求成功响应，但响应表示 API 操作失败。"""
 
     def __init__(self, code: int, resp: Dict[str, Any]):
-        """
+        """初始化。
+
         Args:
             code: 错误代码。
             resp: 返回的响应。
         """
         self.code = code
         self.resp = resp
```

### Comparing `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/message.py` & `alicebot_adapter_mirai-0.7.0/alicebot/adapter/mirai/message.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,168 +1,196 @@
 """Mirai 适配器消息。"""
 import json
-from typing import Any, Dict, List, Type, Union, Mapping, Iterable, Optional
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Type, Union
 
-from alicebot.utils import DataclassEncoder
 from alicebot.message import Message, MessageSegment
+from alicebot.utils import DataclassEncoder
 
 __all__ = ["T_MiraiMSG", "MiraiMessage", "MiraiMessageSegment"]
 
 T_MiraiMSG = Union[
     str,
     Mapping[str, Any],
     Iterable[Mapping[str, Any]],
     "MiraiMessageSegment",
     "MiraiMessage",
 ]
 
 
 class MiraiMessage(Message["MiraiMessageSegment"]):
+    """Mirai 消息"""
+
     @property
     def _message_segment_class(self) -> Type["MiraiMessageSegment"]:
         return MiraiMessageSegment
 
     def _str_to_message_segment(self, msg: str) -> "MiraiMessageSegment":
         return self._message_segment_class.plain(msg)
 
     def as_message_chain(self) -> List[Dict[str, Any]]:
         """返回符合 Mirai-api-http 标准的 messageChain 数组。
 
         Returns:
             messageChain 数组。
         """
-        return list(map(lambda x: x.as_dict(), self))
+        return [x.as_dict() for x in self]
 
 
 class MiraiMessageSegment(MessageSegment["MiraiMessage"]):
+    """Mirai 消息段"""
+
     def __init__(self, type: str, **data: Any):
+        """初始化。
+
+        Args:
+            type: 消息类型。
+            **data: 消息内容。
+        """
         super().__init__(
             type=type, data={k: v for k, v in data.items() if v is not None}
         )
 
     @property
     def _message_class(self) -> Type["MiraiMessage"]:
         return MiraiMessage
 
     def __str__(self) -> str:
+        if self.type == "Source":
+            return ""
         if self.type == "Plain":
             return self.data.get("text", "")
         return json.dumps(self, cls=DataclassEncoder)
 
     def as_dict(self) -> Dict[str, Any]:
         """返回符合 Mirai-api-http 标准的消息字段字典。
 
         Returns:
             符合 Mirai-api-http 标准的消息字段字典。
         """
         return {"type": self.type, **self.data}
 
     def is_text(self) -> bool:
-        """
+        """是否是纯文本消息字段。
+
         Returns:
             是否是纯文本消息字段。
         """
         return self.type == "Plain"
 
     @classmethod
     def source(cls, id_: int, time: int):
+        """Source 消息"""
         return cls(type="Source", id=id_, time=time)
 
     @classmethod
     def quote(
         cls,
         id_: int,
         group_id: int,
         sender_id: int,
         target_id: int,
         origin: MiraiMessage,
     ):
+        """Quote 消息"""
         return cls(
             type="Quote",
             id=id_,
             groupId=group_id,
             senderId=sender_id,
             targetId=target_id,
             origin=origin.as_message_chain(),
         )
 
     @classmethod
     def at(cls, target: int):
+        """At 消息"""
         return cls(type="At", target=target)
 
     @classmethod
     def at_all(cls):
+        """AtAll 消息"""
         return cls(type="AtAll")
 
     @classmethod
     def face(cls, face_id: Optional[int] = None, name: Optional[str] = None):
+        """Face 消息"""
         return cls(type="Face", faceId=face_id, name=name)
 
     @classmethod
     def plain(cls, text: str):
+        """Plain 消息"""
         return cls(type="Plain", text=text)
 
     @classmethod
     def image(
         cls,
         image_id: Optional[str] = None,
         url: Optional[str] = None,
         path: Optional[str] = None,
     ):
+        """Image 消息"""
         return cls(type="Image", imageId=image_id, url=url, path=path)
 
     @classmethod
     def flash_image(
         cls,
         image_id: Optional[str] = None,
         url: Optional[str] = None,
         path: Optional[str] = None,
     ):
+        """FlashImage 消息"""
         return cls(type="FlashImage", imageId=image_id, url=url, path=path)
 
     @classmethod
     def voice(
         cls,
         voice_id: Optional[str] = None,
         url: Optional[str] = None,
         path: Optional[str] = None,
     ):
+        """Voice 消息"""
         return cls(type="Voice", imageId=voice_id, url=url, path=path)
 
     @classmethod
     def xml(cls, xml: str):
+        """Xml 消息"""
         return cls(type="Xml", xml=xml)
 
     @classmethod
     def json(cls, json_: str):
+        """Json 消息"""
         return cls(type="Json", json=json_)
 
     @classmethod
     def app(cls, content: str):
+        """App 消息"""
         return cls(type="App", content=content)
 
     @classmethod
     def poke(cls, name: str):
+        """Poke 消息"""
         return cls(type="Poke", name=name)
 
     @classmethod
     def dice(cls, value: int):
+        """Dice 消息"""
         return cls(type="Dice", value=value)
 
     @classmethod
     def music_share(
         cls,
         kind: str,
         title: str,
         summary: str,
         jump_url: str,
         picture_url: str,
         music_url: str,
         brief: str,
     ):
+        """MusicShare 消息"""
         return cls(
             type="MusicShare",
             kind=kind,
             title=title,
             summary=summary,
             jumpUrl=jump_url,
             pictureUrl=picture_url,
```

### Comparing `alicebot_adapter_mirai-0.6.2/pyproject.toml` & `alicebot_adapter_mirai-0.7.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alicebot-adapter-mirai"
-version = "0.6.2"
+version = "0.7.0"
 description = "Mirai adapter for AliceBot."
 license = "AGPL-3.0-or-later"
 authors = ["st1020 <stone_1020@qq.com>"]
 readme = "README.md"
 homepage = "https://docs.alicebot.dev/"
 repository = "https://github.com/AliceBotProject/alicebot"
 documentation = "https://docs.alicebot.dev/"
@@ -20,28 +20,19 @@
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
+[tool.ruff]
+extend = "../../pyproject.toml"
+ignore = ["N815"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `alicebot_adapter_mirai-0.6.2/PKG-INFO` & `alicebot_adapter_mirai-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot-adapter-mirai
-Version: 0.6.2
+Version: 0.7.0
 Summary: Mirai adapter for AliceBot.
 Home-page: https://docs.alicebot.dev/
 License: AGPL-3.0-or-later
 Keywords: bot,chatbot,qq,qqbot,mirai
 Author: st1020
 Author-email: stone_1020@qq.com
 Requires-Python: >=3.8,<4.0
@@ -16,17 +16,16 @@
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
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: alicebot-adapter-mirai Version: 0.6.2 Summary:
+Metadata-Version: 2.1 Name: alicebot-adapter-mirai Version: 0.7.0 Summary:
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
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3 Classifier: Topic :: Communications :: Chat Requires-
-Dist: alicebot (==0.6.2) Project-URL: Documentation, https://docs.alicebot.dev/
-Project-URL: Repository, https://github.com/AliceBotProject/alicebot
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Communications :: Chat Requires-Dist: alicebot (==0.7.0) Project-URL:
+Documentation, https://docs.alicebot.dev/ Project-URL: Repository, https://
+github.com/AliceBotProject/alicebot Description-Content-Type: text/markdown
             [logo] # AliceBot-Adapter-CQHTTP **Mirai åè®®éé**
```

