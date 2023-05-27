# Comparing `tmp/nonebot-plugin-msgbuf-0.2.0.tar.gz` & `tmp/nonebot-plugin-msgbuf-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-msgbuf-0.2.0.tar", last modified: Wed May 17 07:32:53 2023, max compression
+gzip compressed data, was "nonebot-plugin-msgbuf-0.3.0.tar", last modified: Sat May 27 13:22:37 2023, max compression
```

## Comparing `nonebot-plugin-msgbuf-0.2.0.tar` & `nonebot-plugin-msgbuf-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:32:53.008829 nonebot-plugin-msgbuf-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-17 07:32:53.008829 nonebot-plugin-msgbuf-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:32:53.004829 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:32:53.008829 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-17 07:32:52.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-17 07:32:53.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:32:52.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 07:32:52.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 07:32:52.000000 nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-17 07:32:40.000000 nonebot-plugin-msgbuf-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:32:53.008829 nonebot-plugin-msgbuf-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:22:37.515633 nonebot-plugin-msgbuf-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-27 13:22:37.511633 nonebot-plugin-msgbuf-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:22:37.511633 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 13:22:37.511633 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-27 13:22:37.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-27 13:22:37.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 13:22:37.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-27 13:22:37.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 13:22:37.000000 nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-27 13:22:26.000000 nonebot-plugin-msgbuf-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 13:22:37.515633 nonebot-plugin-msgbuf-0.3.0/setup.cfg
```

### Comparing `nonebot-plugin-msgbuf-0.2.0/LICENSE` & `nonebot-plugin-msgbuf-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-msgbuf-0.2.0/PKG-INFO` & `nonebot-plugin-msgbuf-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-msgbuf
-Version: 0.2.0
+Version: 0.3.0
 Summary: 适用于 NoneBot2 插件的被动消息构造集成
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -47,14 +47,15 @@
 |  ❌  | 不支持，发送时自动转化为后备文本 |
 
 |                             适配器                             | 纯文本 | 图片 | 提及(@) | 回复 | 表情 | 语音 | 视频 | 文件 | 分享 | 地理位置 |
 | :------------------------------------------------------------: | :----: | :--: | :-----: | :--: | :--: | :--: | :--: | :--: | :--: | :------: |
 |                           OneBot V11                           |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ❌  |  ✅  |    ✅    |
 | OneBot V11 ([Go-CQHTTP](https://github.com/Mrs4s/go-cqhttp) 拓展) |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ✅  |  ✅  |    ✅    |
 |                           OneBot V12                           |   ✅   |  ✅  |   🟨   |  🟨  |  ❌  |  ✅  |  ✅  |  ✅  |  ❌  |    ✅    |
+|                            QQ 频道                            |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
 |                            未写明的                            |   ✅   |  ❌  |   ❌   |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
 
 ## 安装
 
 通过 `nb-cli`:
 
 ```console
@@ -179,16 +180,37 @@
 @ma.handle()
 async def test():
     await MsgBuf().image(Path("image.png")).text("Hello world!").send()
 ```
 
 ### 使用 Go-CQHTTP 拓展
 
+#### 发送文件
+
 ```python
 from nonebot_plugin_msgbuf import Specs
 from pathlib import Path
 
 @ma.handle()
 async def test():
     async with MsgBuf(specs=Specs.OB11_GOCQHTTP) as mb:
-        mb.image(Path("image.png")).text("Hello world!").file(Path("image.png"))
+        mb.file(Path("image.png"))
+```
+
+#### 发送合并转发
+
+```python
+from nonebot.adapters.onebot.v11 import Bot
+from nonebot_plugin_msgbuf import FwdBuf
+
+@ma.handle()
+async def test(bot: Bot):
+    async with FwdBuf(bot, ("group", 114514)) as fb:
+        async with fb.node(1919810, "homo") as n:
+            n.text("114514")
+            n.image("file://homo.jpg")
+        async with fb.node(1919810, "homo") as n:
+            async with n.node(1919810, "homo") as n1:
+                n1.text("homo")
+            async with n.node(1919810, "homo") as n1:
+                n1.text("1919810")
 ```
```

### Comparing `nonebot-plugin-msgbuf-0.2.0/README.md` & `nonebot-plugin-msgbuf-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 |  ❌  | 不支持，发送时自动转化为后备文本 |
 
 |                             适配器                             | 纯文本 | 图片 | 提及(@) | 回复 | 表情 | 语音 | 视频 | 文件 | 分享 | 地理位置 |
 | :------------------------------------------------------------: | :----: | :--: | :-----: | :--: | :--: | :--: | :--: | :--: | :--: | :------: |
 |                           OneBot V11                           |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ❌  |  ✅  |    ✅    |
 | OneBot V11 ([Go-CQHTTP](https://github.com/Mrs4s/go-cqhttp) 拓展) |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ✅  |  ✅  |    ✅    |
 |                           OneBot V12                           |   ✅   |  ✅  |   🟨   |  🟨  |  ❌  |  ✅  |  ✅  |  ✅  |  ❌  |    ✅    |
+|                            QQ 频道                            |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
 |                            未写明的                            |   ✅   |  ❌  |   ❌   |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
 
 ## 安装
 
 通过 `nb-cli`:
 
 ```console
@@ -167,16 +168,37 @@
 @ma.handle()
 async def test():
     await MsgBuf().image(Path("image.png")).text("Hello world!").send()
 ```
 
 ### 使用 Go-CQHTTP 拓展
 
+#### 发送文件
+
 ```python
 from nonebot_plugin_msgbuf import Specs
 from pathlib import Path
 
 @ma.handle()
 async def test():
     async with MsgBuf(specs=Specs.OB11_GOCQHTTP) as mb:
-        mb.image(Path("image.png")).text("Hello world!").file(Path("image.png"))
+        mb.file(Path("image.png"))
+```
+
+#### 发送合并转发
+
+```python
+from nonebot.adapters.onebot.v11 import Bot
+from nonebot_plugin_msgbuf import FwdBuf
+
+@ma.handle()
+async def test(bot: Bot):
+    async with FwdBuf(bot, ("group", 114514)) as fb:
+        async with fb.node(1919810, "homo") as n:
+            n.text("114514")
+            n.image("file://homo.jpg")
+        async with fb.node(1919810, "homo") as n:
+            async with n.node(1919810, "homo") as n1:
+                n1.text("homo")
+            async with n.node(1919810, "homo") as n1:
+                n1.text("1919810")
 ```
```

### Comparing `nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/__init__.py` & `nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 )
 from nonebot import logger, __version__ as nbver
 from nonebot.adapters import MessageSegment
 from nonebot.exception import ActionFailed
 from nonebot.matcher import current_bot, current_event
 from nonebot.plugin import PluginMetadata
 
+from .base import MsgBufManager
 from .models import (
-    Face,               File,               Image,              Location,
-    Mention,            Model,              Raw,                Reply,
-    Share,              SupportedFileData,  Text,               Video,
-    Voice
+    Face,       File,       Image,      Location,   Mention,    Model,
+    Raw,        Reply,      Share,      Text,       Video,      Voice
 )
-from .platforms import _BotT, _EventT, Specs, find_proxy
+from .platforms import _BotT, _EventT, ForwardBuffer, Specs, find_proxy
 
 _extra_meta_source = {
     "type": "library",
     "homepage": "https://github.com/NCBM/nonebot-plugin-msgbuf"
 }
 
 if (
@@ -39,15 +38,15 @@
     name="信鸽巴夫",
     description="适用于 NoneBot2 插件的被动消息构造集成",
     usage="无",
     **_extra_meta
 )
 
 
-class MessageBuffer(Generic[_BotT, _EventT]):
+class MessageBuffer(Generic[_BotT, _EventT], MsgBufManager):
     """消息构造器"""
 
     def __init__(
         self,
         bot: Optional[_BotT] = None,
         event: Optional[_EventT] = None,
         *,
@@ -57,15 +56,15 @@
     ) -> None:
         """
         初始化消息构造器
 
         - bot: 机器人对象
         - event: 响应事件
         - specs: 特殊规则
-        - send: 是否进行发送（需要异步上下文）
+        - send: 是否进行发送
         - send_incomplete: 是否在上下文内部出错后仍发送
         - retry: 重试次数
         - fallback: 后备（通常是纯文本）重试次数
         - cooldown: 重试冷却
         """
         if bot is None:
             bot = cast(_BotT, current_bot.get())
@@ -75,33 +74,17 @@
         self.msgbuf: Deque[Model] = deque()
         self.ifsend = send
         self.send_incomplete = send_incomplete
         self.retry = retry
         self.fallback = fallback
         self.cooldown = cooldown
 
-    def __enter__(self):
-        return self
-
     async def __aenter__(self):
         return self
 
-    def __exit__(
-        self,
-        exc_tp: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType]
-    ) -> Optional[bool]:
-        if exc_tb and not self.send_incomplete:
-            return False
-        if self.ifsend:
-            logger.warning("未使用异步上下文，无法发送消息！")
-        if exc_tb:
-            return False
-    
     async def __aexit__(
         self,
         exc_tp: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType]
     ) -> Optional[bool]:
         if (
@@ -109,42 +92,23 @@
             and (not exc_tb or self.send_incomplete)    # noerror or inc.
             and self.msgbuf                             # not empty
         ):
             await self.send()
         if exc_tb:
             return False
 
-    def __lshift__(self, __o: Model):
-        self.msgbuf.append(__o)
-        return self
-
-    def add(self, *m: Model):
-        """批量插入消息结构"""
-        self.msgbuf.extend(m)
-        return self
-    
     async def export(
         self, convert: bool = False
     ) -> Union[List[MessageSegment], List[Model], List[str]]:
         if convert:
             return await asyncio.gather(
                 *(self.proxy.convert(s) for s in self.msgbuf)
             )
         return list(self.msgbuf)
 
-    def revert(self, n: int = 1):
-        """
-        从末尾删除消息结构
-        
-        - n: 删除个数
-        """
-        for _ in range(n):
-            self.msgbuf.pop()
-        return self
-
     async def send(self, *, use_fallback: bool = False) -> List[Any]:
         """
         发送消息
 
         - use_fallback: 是否使用后备
         """
         try:
@@ -162,76 +126,24 @@
             elif self.fallback > 0:
                 logger.warning(f"消息发送失败，剩余 {self.fallback} 次重试（后备）。")
                 await asyncio.sleep(self.cooldown)
                 self.fallback -= 1
                 return await self.send(use_fallback=True)
             logger.error("消息发送失败！")
             raise
-    
+
     async def flush(self):
         """发送当前缓冲的消息并清空缓冲区"""
         res = await self.send()
         self.msgbuf.clear()
         return res
 
-    def text(self, text: str):
-        """追加普通文本"""
-        self.msgbuf.append(Text(text))
-        return self
-
-    def image(self, image: SupportedFileData):
-        """追加图片"""
-        self.msgbuf.append(Image(image))
-        return self
-
-    def mention(self, uid: Union[str, int]):
-        """追加提及 (At)"""
-        self.msgbuf.append(Mention(str(uid)))
-        return self
-
-    def reply(self, mid: Union[str, int]):
-        """追加回复"""
-        self.msgbuf.append(Reply(str(mid)))
-        return self
-
-    def face(self, fid: Union[str, int]):
-        """追加表情"""
-        self.msgbuf.append(Face(str(fid)))
-        return self
-
-    def voice(self, voice: SupportedFileData):
-        """追加语音"""
-        self.msgbuf.append(Voice(voice))
-        return self
-
-    def video(self, video: SupportedFileData):
-        """追加视频"""
-        self.msgbuf.append(Video(video))
-        return self
-
-    def file(self, file: SupportedFileData, name: str = ""):
-        """追加文件"""
-        self.msgbuf.append(File(file, name))
-        return self
-    
-    def share(self, url: str, title: str, content: str = "", image: str = ""):
-        """追加分享"""
-        self.msgbuf.append(Share(url, title, content, image))
-        return self
-    
-    def location(
-        self,
-        latitude: float, lontitude: float,
-        title: str = "", content: str = ""
-    ):
-        """追加地理位置"""
-        self.msgbuf.append(Location(latitude, lontitude, title, content))
-        return self
-
 
 MsgBuf = MessageBuffer
+FwdBuf = ForwardBuffer
 
 __all__ = (
     "Face",     "File",     "Image",    "Location", "Mention",  "Raw",
     "Reply",    "Share",    "Text",     "Video",    "Voice",
-    "MessageBuffer",        "MsgBuf",               "Specs"
+    "MessageBuffer",        "MsgBuf",               "Specs",
+    "ForwardBuffer",        "FwdBuf"
 )
```

### Comparing `nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf/models.py` & `nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     def alternative(self) -> str:
         return "[图片]"
 
 
 @dataclass
 class Mention(Body):
     user_id: str
+    domain: str = ""
 
     def alternative(self) -> str:
         return f"@{self.user_id} "
 
 
 @dataclass
 class Reply(Single):
```

### Comparing `nonebot-plugin-msgbuf-0.2.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO` & `nonebot-plugin-msgbuf-0.3.0/nonebot_plugin_msgbuf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-msgbuf
-Version: 0.2.0
+Version: 0.3.0
 Summary: 适用于 NoneBot2 插件的被动消息构造集成
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-msgbuf
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-msgbuf
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -47,14 +47,15 @@
 |  ❌  | 不支持，发送时自动转化为后备文本 |
 
 |                             适配器                             | 纯文本 | 图片 | 提及(@) | 回复 | 表情 | 语音 | 视频 | 文件 | 分享 | 地理位置 |
 | :------------------------------------------------------------: | :----: | :--: | :-----: | :--: | :--: | :--: | :--: | :--: | :--: | :------: |
 |                           OneBot V11                           |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ❌  |  ✅  |    ✅    |
 | OneBot V11 ([Go-CQHTTP](https://github.com/Mrs4s/go-cqhttp) 拓展) |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ✅  |  ✅  |  ✅  |  ✅  |    ✅    |
 |                           OneBot V12                           |   ✅   |  ✅  |   🟨   |  🟨  |  ❌  |  ✅  |  ✅  |  ✅  |  ❌  |    ✅    |
+|                            QQ 频道                            |   ✅   |  ✅  |   🟨   |  🟨  |  🟨  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
 |                            未写明的                            |   ✅   |  ❌  |   ❌   |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |  ❌  |    ❌    |
 
 ## 安装
 
 通过 `nb-cli`:
 
 ```console
@@ -179,16 +180,37 @@
 @ma.handle()
 async def test():
     await MsgBuf().image(Path("image.png")).text("Hello world!").send()
 ```
 
 ### 使用 Go-CQHTTP 拓展
 
+#### 发送文件
+
 ```python
 from nonebot_plugin_msgbuf import Specs
 from pathlib import Path
 
 @ma.handle()
 async def test():
     async with MsgBuf(specs=Specs.OB11_GOCQHTTP) as mb:
-        mb.image(Path("image.png")).text("Hello world!").file(Path("image.png"))
+        mb.file(Path("image.png"))
+```
+
+#### 发送合并转发
+
+```python
+from nonebot.adapters.onebot.v11 import Bot
+from nonebot_plugin_msgbuf import FwdBuf
+
+@ma.handle()
+async def test(bot: Bot):
+    async with FwdBuf(bot, ("group", 114514)) as fb:
+        async with fb.node(1919810, "homo") as n:
+            n.text("114514")
+            n.image("file://homo.jpg")
+        async with fb.node(1919810, "homo") as n:
+            async with n.node(1919810, "homo") as n1:
+                n1.text("homo")
+            async with n.node(1919810, "homo") as n1:
+                n1.text("1919810")
 ```
```

