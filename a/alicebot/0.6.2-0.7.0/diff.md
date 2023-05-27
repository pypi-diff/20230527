# Comparing `tmp/alicebot-0.6.2.tar.gz` & `tmp/alicebot-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot-0.6.2.tar", max compression
+gzip compressed data, was "alicebot-0.7.0.tar", max compression
```

## Comparing `alicebot-0.6.2.tar` & `alicebot-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-04-25 11:14:36.273730 alicebot-0.6.2/LICENSE
--rw-r--r--   0        0        0     6110 2023-04-25 11:14:36.273730 alicebot-0.6.2/README.md
--rw-r--r--   0        0        0      656 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/__init__.py
--rw-r--r--   0        0        0     4498 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/adapter/__init__.py
--rw-r--r--   0        0        0     8043 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/adapter/utils.py
--rw-r--r--   0        0        0    34806 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/bot.py
--rw-r--r--   0        0        0     1877 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/config.py
--rw-r--r--   0        0        0     1851 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/event.py
--rw-r--r--   0        0        0     1116 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/exceptions.py
--rw-r--r--   0        0        0      432 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/log.py
--rw-r--r--   0        0        0    14120 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/message.py
--rw-r--r--   0        0        0     3568 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/plugin.py
--rw-r--r--   0        0        0        0 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/py.typed
--rw-r--r--   0        0        0     1034 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/typing.py
--rw-r--r--   0        0        0     5457 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/utils.py
--rw-r--r--   0        0        0     2680 2023-04-25 11:14:36.281730 alicebot-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     7545 1970-01-01 00:00:00.000000 alicebot-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-27 14:25:34.114713 alicebot-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6021 2023-05-27 14:25:34.114713 alicebot-0.7.0/README.md
+-rw-r--r--   0        0        0      728 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/__init__.py
+-rw-r--r--   0        0        0     5330 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/adapter/__init__.py
+-rw-r--r--   0        0        0     8621 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/adapter/utils.py
+-rw-r--r--   0        0        0    38583 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/bot.py
+-rw-r--r--   0        0        0     1879 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/config.py
+-rw-r--r--   0        0        0     4319 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/dependencies.py
+-rw-r--r--   0        0        0     4216 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/event.py
+-rw-r--r--   0        0        0     1130 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/exceptions.py
+-rw-r--r--   0        0        0      597 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/log.py
+-rw-r--r--   0        0        0    15028 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/message.py
+-rw-r--r--   0        0        0     4045 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/py.typed
+-rw-r--r--   0        0        0     1084 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/typing.py
+-rw-r--r--   0        0        0     8052 2023-05-27 14:25:34.114713 alicebot-0.7.0/alicebot/utils.py
+-rw-r--r--   0        0        0     4380 2023-05-27 14:25:34.122713 alicebot-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7408 1970-01-01 00:00:00.000000 alicebot-0.7.0/PKG-INFO
```

### Comparing `alicebot-0.6.2/LICENSE` & `alicebot-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alicebot-0.6.2/README.md` & `alicebot-0.7.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -40,86 +40,85 @@
 
 AliceBot 是一个简单的 Python 异步多后端机器人框架，支持多种协议适配，可以轻松地编写易于学习和使用的插件来拓展其功能。
 
 本项目受到了 [NoneBot](https://github.com/nonebot/nonebot2/) 项目的启发，您可以在 [对比](#对比) 小节中查看这两个项目的异同，以便您选择更适合自己的机器人框架。
 
 ## 特点
 
-AliceBot 使用了非常灵活且易于使用的插件编写方式，您只需要编写两个方法即可实现一个功能强大的插件。
-
-AliceBot 的适配协议并不与任何一种库或网络协议绑定，您可以自由选择或编写适合您的适配器。
+- **简单**：AliceBot 使用了非常灵活且易于使用的插件编写方式，您只需要编写两个方法即可实现一个功能强大的插件。
+- **灵活**：AliceBot 的适配协议并不与任何一种库或网络协议绑定，您可以自由选择或编写适合您的适配器。
+- **高效**：AliceBot 基于 Python 的异步 I/O，轻松处理大量请求。较少的封装，在保持易用的同时追求最好的性能。
 
 目前 AliceBot 官方维护了以下协议适配：
 
-- [OneBot (CQHTTP) 协议](https://github.com/botuniverse/onebot) （支持QQ等）[ws](https://github.com/botuniverse/onebot-11/blob/master/communication/ws.md) 和 [ws-reverse](https://github.com/botuniverse/onebot-11/blob/master/communication/ws-reverse.md) 连接方式
+- [OneBot (CQHTTP) 协议](https://github.com/botuniverse/onebot) （支持 QQ 等）[ws](https://github.com/botuniverse/onebot-11/blob/master/communication/ws.md) 和 [ws-reverse](https://github.com/botuniverse/onebot-11/blob/master/communication/ws-reverse.md) 连接方式
 - [mirai-api-http 协议](https://github.com/project-mirai/mirai-api-http) 2.0+ [ws](https://github.com/project-mirai/mirai-api-http/blob/master/docs/adapter/WebsocketAdapter.md) 和 [reverse-ws](https://github.com/project-mirai/mirai-api-http/blob/master/docs/adapter/ReverseWebsocketAdapter.md) 连接方式
 - [钉钉](https://developers.dingtalk.com/document/robots/robot-overview) 企业机器人的 outgoing （回调）连接方式
 
 更多协议正在适配中 ...
 
+更多信息：[简介 - AliceBot 文档](https://docs.alicebot.dev/guide/)
+
 ## 即刻开始
 
 1. 安装：
 
    ```bash
    pip install alicebot[all]
    ```
 
 2. 第一个 AliceBot 项目：
 
    ```python
    from alicebot import Bot
-   
+
    bot = Bot()
    bot.load_adapters("alicebot.adapter.cqhttp")
-   
+
    bot.run()
    ```
 
 3. 第一个 AliceBot 插件：
 
    ```python
    from alicebot import Plugin
-   
-   
+
+
    class Echo(Plugin):
        async def handle(self) -> None:
            await self.event.reply(self.event.message.replace("echo ", ""))
-   
+
        async def rule(self) -> bool:
            if self.event.adapter.name != "cqhttp":
                return False
            if self.event.type != "message":
                return False
            return self.event.message.startswith("echo ")
    ```
 
 更多信息请参阅 AliceBot [文档](https://docs.alicebot.dev/)。
 
 ## 对比
 
-本项目受到了 [NoneBot](https://github.com/nonebot/nonebot2/) 项目的启发，以下简单介绍两者的异同。
+本项目受到了 [NoneBot](https://github.com/nonebot/nonebot2) 项目的启发，以下简单介绍两者的异同。
 
 相同点：
 
 - 两者都是使用 Python 编写的，使用了协程异步的高性能机器人框架。
 - 两者都支持多种协议。
 - 两者都会对机器人收到的事件进行解析和处理，并按优先级分发给插件（事件响应器）来完成具体的功能。
 - 两者都基于 MIT 协议开源，这意味着您可以在遵循协议的前提下任意使用本项目。
 
 不同点：
 
 - 总的来说，NoneBot 是一个较为全面的机器人框架，而 AliceBot 是一个小巧简洁的机器人框架，它不包含一些复杂的高级特性，但更加灵活且易于学习。
-- NoneBot 在实现上与 WebSocket 通讯协议深度绑定，它需要一个支持 ASGI 服务器协议的驱动框架，而 AliceBot 并不与任何协议绑定，它甚至可以用来驱动您的树莓派智能音箱。当然，如果您只需要一个支持常见网络聊天工具的机器人框架的话，它们并没有什么区别。
-- NoneBot 提供了很多预设规则和权限控制机制，而 AliceBot 则没有提供，由于插件编写方式的不同，AliceBot 选择给您最大的自由，您需要自行编写插件在何时运行的方法（`rule()` 方法），这在绝大部份情况下并不会造成您编写更多的代码或是影响插件的可读性，自行实现也不会非常困难，但如果您真的需要这些高级功能又不想自己实现的话，NoneBot 提供了更好的选择。
+- AliceBot 的插件编写风格和 NoneBot 不同，相对而言，AliceBot 更加注重于易于入门和“渐进式框架”，这意味着 AliceBot 大部分的功能都是可选的，您只需要了解很少的知识即可开始使用，随着项目规模的扩大和复杂性的增加，您可以继续深入需要的特性，而不需要一开始就掌握全部的特性。“它是一个可以与你共同成长、适应你不同需求的框架。”
+- NoneBot 在实现上与 HTTP / WebSocket 通讯协议深度绑定，它需要一个支持 ASGI 服务器协议的“驱动器”，而 AliceBot 并不与任何协议绑定，它甚至可以用来驱动您的树莓派智能音箱。当然，如果您只需要一个支持常见网络聊天工具的机器人框架的话，它们并没有什么区别。
 - NoneBot 拥有相对庞大的用户基数和社区规模，也拥有数量众多的插件，而 AliceBot 则是一个新生项目，这意味着如果您使用 NoneBot 您可能会更加容易找到已经编写完毕的您感兴趣的插件，并且您当您遇到问题时也能够更快地查找到相关资料或者获得解答。
-- NoneBot 相对较为庞大，封装相对较多，完全学习理解需要一定时间，而 AliceBot 小巧简洁，封装较少，很容易掌握。
 
 总而言之，两者有着各自的特点，您可以根据需要选用。
 
-作者就是在使用 NoneBot 时觉得插件编写不是很易用，于是萌发了编写一个新的机器人框架的想法，AliceBot 就这样诞生了。
-
 ## 许可证
 
 AliceBot 采用 MIT 许可证开放源代码。
 
 本项目的图标由 迷糊小梦神 绘制，作为本项目的一部分，使用与本项目相同的许可证开放使用。
```

#### html2text {}

```diff
@@ -3,64 +3,60 @@
                                   [qq-group]
                    ææ¡£ Â· æå Â· API_åè Â· ç¤ºä¾
 ## ç®ä» AliceBot æ¯ä¸ä¸ªç®åç Python
 å¼æ­¥å¤åç«¯æºå¨äººæ¡æ¶ï¼æ¯æå¤ç§åè®®ééï¼å¯ä»¥è½»æ¾å°ç¼åæäºå­¦ä¹ åä½¿ç¨çæä»¶æ¥æå±å¶åè½ã
 æ¬é¡¹ç®åå°äº [NoneBot](https://github.com/nonebot/nonebot2/
 ) é¡¹ç®çå¯åï¼æ¨å¯ä»¥å¨ [å¯¹æ¯](#å¯¹æ¯)
 å°èä¸­æ¥çè¿ä¸¤ä¸ªé¡¹ç®çå¼åï¼ä»¥ä¾¿æ¨éæ©æ´éåèªå·±çæºå¨äººæ¡æ¶ã
-## ç¹ç¹ AliceBot
+## ç¹ç¹ - **ç®å**ï¼AliceBot
 ä½¿ç¨äºéå¸¸çµæ´»ä¸æäºä½¿ç¨çæä»¶ç¼åæ¹å¼ï¼æ¨åªéè¦ç¼åä¸¤ä¸ªæ¹æ³å³å¯å®ç°ä¸ä¸ªåè½å¼ºå¤§çæä»¶ã
-AliceBot
+- **çµæ´»**ï¼AliceBot
 çééåè®®å¹¶ä¸ä¸ä»»ä½ä¸ç§åºæç½ç»åè®®ç»å®ï¼æ¨å¯ä»¥èªç±éæ©æç¼åéåæ¨çééå¨ã
+- **é«æ**ï¼AliceBot åºäº Python çå¼æ­¥ I/
+Oï¼è½»æ¾å¤çå¤§éè¯·æ±ãè¾å°çå°è£ï¼å¨ä¿ææç¨çåæ¶è¿½æ±æå¥½çæ§è½ã
 ç®å AliceBot å®æ¹ç»´æ¤äºä»¥ä¸åè®®ééï¼ - [OneBot (CQHTTP) åè®®]
-(https://github.com/botuniverse/onebot) ï¼æ¯æQQç­ï¼[ws](https://
+(https://github.com/botuniverse/onebot) ï¼æ¯æ QQ ç­ï¼[ws](https://
 github.com/botuniverse/onebot-11/blob/master/communication/ws.md) å [ws-
 reverse](https://github.com/botuniverse/onebot-11/blob/master/communication/ws-
 reverse.md) è¿æ¥æ¹å¼ - [mirai-api-http åè®®](https://github.com/project-
 mirai/mirai-api-http) 2.0+ [ws](https://github.com/project-mirai/mirai-api-
 http/blob/master/docs/adapter/WebsocketAdapter.md) å [reverse-ws](https://
 github.com/project-mirai/mirai-api-http/blob/master/docs/adapter/
 ReverseWebsocketAdapter.md) è¿æ¥æ¹å¼ - [éé](https://
 developers.dingtalk.com/document/robots/robot-overview) ä¼ä¸æºå¨äººç
-outgoing ï¼åè°ï¼è¿æ¥æ¹å¼ æ´å¤åè®®æ­£å¨ééä¸­ ... ##
+outgoing ï¼åè°ï¼è¿æ¥æ¹å¼ æ´å¤åè®®æ­£å¨ééä¸­ ...
+æ´å¤ä¿¡æ¯ï¼[ç®ä» - AliceBot ææ¡£](https://docs.alicebot.dev/guide/) ##
 å³å»å¼å§ 1. å®è£ï¼ ```bash pip install alicebot[all] ``` 2. ç¬¬ä¸ä¸ª
 AliceBot é¡¹ç®ï¼ ```python from alicebot import Bot bot = Bot()
 bot.load_adapters("alicebot.adapter.cqhttp") bot.run() ``` 3. ç¬¬ä¸ä¸ª
 AliceBot æä»¶ï¼ ```python from alicebot import Plugin class Echo(Plugin):
 async def handle(self) -> None: await self.event.reply
 (self.event.message.replace("echo ", "")) async def rule(self) -> bool: if
 self.event.adapter.name != "cqhttp": return False if self.event.type !=
 "message": return False return self.event.message.startswith("echo ") ```
 æ´å¤ä¿¡æ¯è¯·åé AliceBot [ææ¡£](https://docs.alicebot.dev/)ã ##
-å¯¹æ¯ æ¬é¡¹ç®åå°äº [NoneBot](https://github.com/nonebot/nonebot2/
-) é¡¹ç®çå¯åï¼ä»¥ä¸ç®åä»ç»ä¸¤èçå¼åã ç¸åç¹ï¼ -
+å¯¹æ¯ æ¬é¡¹ç®åå°äº [NoneBot](https://github.com/nonebot/nonebot2)
+é¡¹ç®çå¯åï¼ä»¥ä¸ç®åä»ç»ä¸¤èçå¼åã ç¸åç¹ï¼ -
 ä¸¤èé½æ¯ä½¿ç¨ Python
 ç¼åçï¼ä½¿ç¨äºåç¨å¼æ­¥çé«æ§è½æºå¨äººæ¡æ¶ã -
 ä¸¤èé½æ¯æå¤ç§åè®®ã -
 ä¸¤èé½ä¼å¯¹æºå¨äººæ¶å°çäºä»¶è¿è¡è§£æåå¤çï¼å¹¶æä¼åçº§ååç»æä»¶ï¼äºä»¶ååºå¨ï¼æ¥å®æå·ä½çåè½ã
 - ä¸¤èé½åºäº MIT
 åè®®å¼æºï¼è¿æå³çæ¨å¯ä»¥å¨éµå¾ªåè®®çåæä¸ä»»æä½¿ç¨æ¬é¡¹ç®ã
 ä¸åç¹ï¼ - æ»çæ¥è¯´ï¼NoneBot
 æ¯ä¸ä¸ªè¾ä¸ºå¨é¢çæºå¨äººæ¡æ¶ï¼è AliceBot
 æ¯ä¸ä¸ªå°å·§ç®æ´çæºå¨äººæ¡æ¶ï¼å®ä¸åå«ä¸äºå¤æçé«çº§ç¹æ§ï¼ä½æ´å çµæ´»ä¸æäºå­¦ä¹ ã
-- NoneBot å¨å®ç°ä¸ä¸ WebSocket
+- AliceBot çæä»¶ç¼åé£æ ¼å NoneBot ä¸åï¼ç¸å¯¹èè¨ï¼AliceBot
+æ´å æ³¨éäºæäºå¥é¨åâæ¸è¿å¼æ¡æ¶âï¼è¿æå³ç AliceBot
+å¤§é¨åçåè½é½æ¯å¯éçï¼æ¨åªéè¦äºè§£å¾å°çç¥è¯å³å¯å¼å§ä½¿ç¨ï¼éçé¡¹ç®è§æ¨¡çæ©å¤§åå¤ææ§çå¢å ï¼æ¨å¯ä»¥ç»§ç»­æ·±å¥éè¦çç¹æ§ï¼èä¸éè¦ä¸å¼å§å°±ææ¡å¨é¨çç¹æ§ãâå®æ¯ä¸ä¸ªå¯ä»¥ä¸ä½ å±åæé¿ãéåºä½ ä¸åéæ±çæ¡æ¶ãâ
+- NoneBot å¨å®ç°ä¸ä¸ HTTP / WebSocket
 éè®¯åè®®æ·±åº¦ç»å®ï¼å®éè¦ä¸ä¸ªæ¯æ ASGI
-æå¡å¨åè®®çé©±å¨æ¡æ¶ï¼è AliceBot
+æå¡å¨åè®®çâé©±å¨å¨âï¼è AliceBot
 å¹¶ä¸ä¸ä»»ä½åè®®ç»å®ï¼å®çè³å¯ä»¥ç¨æ¥é©±å¨æ¨çæ èæ´¾æºè½é³ç®±ãå½ç¶ï¼å¦ææ¨åªéè¦ä¸ä¸ªæ¯æå¸¸è§ç½ç»èå¤©å·¥å·çæºå¨äººæ¡æ¶çè¯ï¼å®ä»¬å¹¶æ²¡æä»ä¹åºå«ã
-- NoneBot æä¾äºå¾å¤é¢è®¾è§ååæéæ§å¶æºå¶ï¼è AliceBot
-åæ²¡ææä¾ï¼ç±äºæä»¶ç¼åæ¹å¼çä¸åï¼AliceBot
-éæ©ç»æ¨æå¤§çèªç±ï¼æ¨éè¦èªè¡ç¼åæä»¶å¨ä½æ¶è¿è¡çæ¹æ³ï¼`rule
-()`
-æ¹æ³ï¼ï¼è¿å¨ç»å¤§é¨ä»½æåµä¸å¹¶ä¸ä¼é ææ¨ç¼åæ´å¤çä»£ç ææ¯å½±åæä»¶çå¯è¯»æ§ï¼èªè¡å®ç°ä¹ä¸ä¼éå¸¸å°é¾ï¼ä½å¦ææ¨ççéè¦è¿äºé«çº§åè½åä¸æ³èªå·±å®ç°çè¯ï¼NoneBot
-æä¾äºæ´å¥½çéæ©ã - NoneBot
+- NoneBot
 æ¥æç¸å¯¹åºå¤§çç¨æ·åºæ°åç¤¾åºè§æ¨¡ï¼ä¹æ¥ææ°éä¼å¤çæä»¶ï¼è
 AliceBot åæ¯ä¸ä¸ªæ°çé¡¹ç®ï¼è¿æå³çå¦ææ¨ä½¿ç¨ NoneBot
 æ¨å¯è½ä¼æ´å å®¹ææ¾å°å·²ç»ç¼åå®æ¯çæ¨æå´è¶£çæä»¶ï¼å¹¶ä¸æ¨å½æ¨éå°é®é¢æ¶ä¹è½å¤æ´å¿«å°æ¥æ¾å°ç¸å³èµææèè·å¾è§£ç­ã
-- NoneBot
-ç¸å¯¹è¾ä¸ºåºå¤§ï¼å°è£ç¸å¯¹è¾å¤ï¼å®å¨å­¦ä¹ çè§£éè¦ä¸å®æ¶é´ï¼è
-AliceBot å°å·§ç®æ´ï¼å°è£è¾å°ï¼å¾å®¹æææ¡ã
-æ»èè¨ä¹ï¼ä¸¤èæçåèªçç¹ç¹ï¼æ¨å¯ä»¥æ ¹æ®éè¦éç¨ã
-ä½èå°±æ¯å¨ä½¿ç¨ NoneBot
-æ¶è§å¾æä»¶ç¼åä¸æ¯å¾æç¨ï¼äºæ¯èåäºç¼åä¸ä¸ªæ°çæºå¨äººæ¡æ¶çæ³æ³ï¼AliceBot
-å°±è¿æ ·è¯çäºã ## è®¸å¯è¯ AliceBot éç¨ MIT
-è®¸å¯è¯å¼æ¾æºä»£ç ã æ¬é¡¹ç®çå¾æ ç± è¿·ç³å°æ¢¦ç¥
+æ»èè¨ä¹ï¼ä¸¤èæçåèªçç¹ç¹ï¼æ¨å¯ä»¥æ ¹æ®éè¦éç¨ã ##
+è®¸å¯è¯ AliceBot éç¨ MIT è®¸å¯è¯å¼æ¾æºä»£ç ã æ¬é¡¹ç®çå¾æ ç±
+è¿·ç³å°æ¢¦ç¥
 ç»å¶ï¼ä½ä¸ºæ¬é¡¹ç®çä¸é¨åï¼ä½¿ç¨ä¸æ¬é¡¹ç®ç¸åçè®¸å¯è¯å¼æ¾ä½¿ç¨ã
```

### Comparing `alicebot-0.6.2/alicebot/__init__.py` & `alicebot-0.7.0/alicebot/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """AliceBot
+
 简单的 Python 异步多后端机器人框架
 
 本模块从子模块导入了以下内容：
 - `Bot` => [`alicebot.bot.Bot`](./bot#Bot)
 - `Event` => [`alicebot.event.Event`](./event#Event)
 - `Plugin` => [`alicebot.plugin.Plugin`](./plugin#Plugin)
 - `Adapter` => [`alicebot.adapter.Adapter`](./adapter/#Adapter)
 - `ConfigModel` => [`alicebot.config.ConfigModel`](./config#ConfigModel)
+- `Depends` => [`alicebot.dependencies.Depends`](./dependencies#Depends)
 """
-from alicebot.bot import Bot  # type: ignore
-from alicebot.event import Event  # type: ignore
-from alicebot.plugin import Plugin  # type: ignore
-from alicebot.adapter import Adapter  # type: ignore
-from alicebot.config import ConfigModel  # type: ignore
+# pyright: reportUnusedImport=false
+from alicebot.adapter import Adapter
+from alicebot.bot import Bot
+from alicebot.config import ConfigModel
+from alicebot.dependencies import Depends
+from alicebot.event import Event
+from alicebot.plugin import Plugin
```

### Comparing `alicebot-0.6.2/alicebot/adapter/__init__.py` & `alicebot-0.7.0/alicebot/adapter/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,78 @@
 """AliceBot 协议适配器。
 
 所有协议适配器都必须继承自 `Adapter` 基类。
 """
-import os
 from abc import ABC, abstractmethod
+import os
 from typing import (
     TYPE_CHECKING,
     Any,
-    Type,
-    Union,
-    Generic,
+    Awaitable,
     Callable,
+    Generic,
     Optional,
-    Awaitable,
+    Type,
+    TypeVar,
+    Union,
     final,
+    overload,
 )
 
 from alicebot.log import error_or_exception
-from alicebot.typing import T_Event, T_Config
-from alicebot.utils import wrap_get_func, is_config_class
+from alicebot.typing import T_Config, T_Event
+from alicebot.utils import is_config_class
 
 if TYPE_CHECKING:
     from alicebot.bot import Bot
     from alicebot.event import Event
 
 __all__ = ["Adapter"]
 
 if os.getenv("ALICEBOT_DEV") == "1":
     # 当处于开发环境时，使用 pkg_resources 风格的命名空间包
     __import__("pkg_resources").declare_namespace(__name__)
 
 
+_T_Event = TypeVar("_T_Event", bound="Event[Any]")
+
+
 class Adapter(Generic[T_Event, T_Config], ABC):
     """协议适配器基类。
 
     Attributes:
         name: 适配器的名称。
         bot: 当前的机器人对象。
     """
 
     name: str
     bot: "Bot"
-    Config: Type[T_Config] = type(None)  # type: ignore
+    Config: Type[T_Config]
 
     def __init__(self, bot: "Bot"):
+        """初始化。
+
+        Args:
+            bot: 当前机器人对象。
+        """
         if not hasattr(self, "name"):
             self.name = self.__class__.__name__
         self.bot: "Bot" = bot
         self.handle_event = self.bot.handle_event
 
     @property
     def config(self) -> T_Config:
         """适配器配置。"""
-        if is_config_class(self.Config):
-            return getattr(self.bot.config.adapter, self.Config.__config_name__, None)  # type: ignore
+        config_class = getattr(self, "Config", None)
+        if is_config_class(config_class):
+            return getattr(
+                self.bot.config.adapter,
+                config_class.__config_name__,
+                None,
+            )  # type: ignore
         return None  # type: ignore
 
     @final
     async def safe_run(self):
         """附带有异常处理地安全运行适配器。"""
         try:
             await self.run()
@@ -65,75 +80,89 @@
             error_or_exception(
                 f"Run adapter {self.__class__.__name__} failed:",
                 e,
                 self.bot.config.bot.log.verbose_exception,
             )
 
     @abstractmethod
-    async def run(self):
+    async def run(self) -> None:
         """适配器运行方法，适配器开发者必须实现该方法。
 
         适配器运行过程中保持保持运行，当此方法结束后， AliceBot 不会自动重新启动适配器。
         """
         raise NotImplementedError
 
     async def startup(self):
         """在适配器开始运行前运行的方法，用于初始化适配器。
 
         AliceBot 依次运行并等待所有适配器的 `startup()` 方法，待运行完毕后再创建 `run()` 任务。
         """
-        pass
 
     async def shutdown(self):
         """在适配器结束运行时运行的方法，用于安全地关闭适配器。
 
         AliceBot 在接收到系统的结束信号后依次运行并等待所有适配器的 `shutdown()` 方法。
         当强制退出时此方法可能未被执行。
         """
-        pass
 
-    async def send(self, *args: Any, **kwargs: Any):
+    async def send(self, *args: Any, **kwargs: Any) -> Any:
         """发送消息，需要适配器开发者实现。"""
         raise NotImplementedError
 
-    @final
+    @overload
     async def get(
         self,
-        func: Optional[Callable[["Event"], Union[bool, Awaitable[bool]]]] = None,
+        func: Optional[Callable[[T_Event], Union[bool, Awaitable[bool]]]] = None,
         *,
+        event_type: None = None,
         max_try_times: Optional[int] = None,
         timeout: Optional[Union[int, float]] = None,
     ) -> T_Event:
+        ...
+
+    @overload
+    async def get(
+        self,
+        func: Optional[Callable[[_T_Event], Union[bool, Awaitable[bool]]]] = None,
+        *,
+        event_type: Type[_T_Event],
+        max_try_times: Optional[int] = None,
+        timeout: Optional[Union[int, float]] = None,
+    ) -> _T_Event:
+        ...
+
+    @final
+    async def get(
+        self,
+        func: Optional[Callable[[T_Event], Union[bool, Awaitable[bool]]]] = None,
+        *,
+        event_type: Optional[Union[Type[T_Event], Type[_T_Event]]] = None,
+        max_try_times: Optional[int] = None,
+        timeout: Optional[Union[int, float]] = None,
+    ) -> Union[T_Event, _T_Event]:
         """获取满足指定条件的的事件，协程会等待直到适配器接收到满足条件的事件、超过最大事件数或超时。
 
-        类似 Bot 类的 get() 方法，但是隐含了判断产生 event 的适配器是本适配器。
+        类似 `Bot` 类的 `get()` 方法，但是隐含了判断产生事件的适配器是本适配器。
+        等效于 `Bot` 类的 `get()` 方法传入 adapter_type 为本适配器类型。
 
         Args:
             func: 协程或者函数，函数会被自动包装为协程执行。
                 要求接受一个事件作为参数，返回布尔值。
                 当协程返回 `True` 时返回当前事件。
                 当为 `None` 时相当于输入对于任何事件均返回真的协程，即返回适配器接收到的下一个事件。
+            event_type: 当指定时，只接受指定类型的事件，先于 func 条件生效。默认为 `None`。
             max_try_times: 最大事件数。
             timeout: 超时时间。
 
         Returns:
             返回满足 func 条件的事件。
 
         Raises:
             GetEventTimeout: 超过最大事件数或超时。
         """
-
-        def func_wrapper(
-            _func: Callable[["Event"], Awaitable[bool]]
-        ) -> Callable[["Event"], Awaitable[bool]]:
-            async def _wrapper(_event: "Event") -> bool:
-                if _event.adapter is not self:
-                    return False
-                return await _func(_event)
-
-            return _wrapper
-
         return await self.bot.get(
-            func_wrapper(wrap_get_func(func)),
+            func,
+            event_type=event_type,
+            adapter_type=type(self),
             max_try_times=max_try_times,
             timeout=timeout,
-        )  # type: ignore
+        )
```

### Comparing `alicebot-0.6.2/alicebot/adapter/utils.py` & `alicebot-0.7.0/alicebot/adapter/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,140 +1,152 @@
 """适配器实用工具。
 
 这里定义了一些在编写适配器时常用的基类，适配器开发者可以直接继承自这里的类或者用作参考。
 """
-import asyncio
 from abc import ABCMeta, abstractmethod
-from typing import Union, Literal, Optional
+import asyncio
+from typing import Literal, Optional, Union
 
 import aiohttp
 from aiohttp import web
 
 from alicebot.adapter import Adapter
-from alicebot.typing import T_Event, T_Config
-from alicebot.log import logger, error_or_exception
+from alicebot.log import error_or_exception, logger
+from alicebot.typing import T_Config, T_Event
 
 
 class PollingAdapter(Adapter[T_Event, T_Config], metaclass=ABCMeta):
     """轮询式适配器示例。"""
 
     delay: float = 0.1
     create_task: bool = False
+    _on_tick_task: Optional["asyncio.Task[None]"] = None
 
     async def run(self):
+        """运行适配器。"""
         while not self.bot.should_exit.is_set():
             await asyncio.sleep(self.delay)
             if self.create_task:
-                asyncio.create_task(self.on_tick())
+                self._on_tick_task = asyncio.create_task(self.on_tick())
             else:
                 await self.on_tick()
 
     @abstractmethod
     async def on_tick(self):
-        pass
+        """当轮询发生。"""
 
 
 class HttpClientAdapter(PollingAdapter[T_Event, T_Config], metaclass=ABCMeta):
     """HTTP 客户端适配器示例。"""
 
     session: aiohttp.ClientSession
 
     async def startup(self):
+        """初始化适配器。"""
         self.session = aiohttp.ClientSession()
 
     @abstractmethod
     async def on_tick(self):
-        pass
+        """当轮询发生。"""
 
     async def shutdown(self):
+        """关闭并清理连接。"""
         await self.session.close()
 
 
 class WebSocketClientAdapter(Adapter[T_Event, T_Config], metaclass=ABCMeta):
     """WebSocket 客户端适配器示例。"""
 
     url: str
 
     async def run(self):
+        """运行适配器。"""
         async with aiohttp.ClientSession() as session:
             async with session.ws_connect(self.url) as ws:
                 msg: aiohttp.WSMessage
                 async for msg in ws:
                     if self.bot.should_exit.is_set():
                         break
                     if msg.type == aiohttp.WSMsgType.ERROR:
                         break
                     await self.handle_response(msg)
 
     @abstractmethod
     async def handle_response(self, msg: aiohttp.WSMessage):
-        pass
+        """处理响应。"""
 
 
 class HttpServerAdapter(Adapter[T_Event, T_Config], metaclass=ABCMeta):
     """HTTP 服务端适配器示例。"""
 
     app: web.Application
     runner: web.AppRunner
     site: web.TCPSite
     host: str
     port: int
     get_url: str
     post_url: str
 
     async def startup(self):
+        """初始化适配器。"""
         self.app = web.Application()
         self.app.add_routes(
             [
                 web.get(self.get_url, self.handle_response),
                 web.post(self.post_url, self.handle_response),
             ]
         )
 
     async def run(self):
+        """运行适配器。"""
         self.runner = web.AppRunner(self.app)
         await self.runner.setup()
         self.site = web.TCPSite(self.runner, self.host, self.port)
         await self.site.start()
 
     async def shutdown(self):
+        """关闭并清理连接。"""
         await self.runner.cleanup()
 
     @abstractmethod
     async def handle_response(self, request: web.Request) -> web.StreamResponse:
-        pass
+        """处理响应。"""
 
 
 class WebSocketServerAdapter(Adapter[T_Event, T_Config], metaclass=ABCMeta):
     """WebSocket 服务端适配器示例。"""
 
     app: web.Application
     runner: web.AppRunner
     site: web.TCPSite
     websocket: web.WebSocketResponse
     host: str
     port: int
     url: str
 
     async def startup(self):
+        """初始化适配器。"""
         self.app = web.Application()
         self.app.add_routes([web.get(self.url, self.handle_response)])
 
     async def run(self):
+        """运行适配器。"""
         self.runner = web.AppRunner(self.app)
         await self.runner.setup()
         self.site = web.TCPSite(self.runner, self.host, self.port)
         await self.site.start()
 
     async def shutdown(self):
+        """关闭并清理连接。"""
         await self.websocket.close()
         await self.site.stop()
         await self.runner.cleanup()
 
     async def handle_response(self, request: web.Request) -> web.WebSocketResponse:
+        """处理 WebSocket。"""
         ws = web.WebSocketResponse()
         await ws.prepare(request)
         self.websocket = ws
 
         msg: aiohttp.WSMessage
         async for msg in ws:
             if msg.type == aiohttp.WSMsgType.TEXT:
@@ -142,15 +154,15 @@
             elif msg.type == aiohttp.WSMsgType.ERROR:
                 break
 
         return ws
 
     @abstractmethod
     async def handle_ws_response(self, msg: aiohttp.WSMessage):
-        pass
+        """处理 WebSocket 响应。"""
 
 
 class WebSocketAdapter(Adapter[T_Event, T_Config], metaclass=ABCMeta):
     """WebSocket 适配器示例。
 
     同时支持 WebSocket 客户端和服务端。
     """
@@ -230,15 +242,15 @@
         await self.websocket.prepare(request)
         await self.reverse_ws_connection_hook()
         await self.handle_websocket()
         return self.websocket
 
     async def reverse_ws_connection_hook(self):
         """反向 WebSocket 连接建立时的钩子函数。"""
-        logger.info(f"WebSocket connected!")
+        logger.info("WebSocket connected!")
 
     async def websocket_connect(self):
         """创建正向 WebSocket 连接。"""
         assert self.session is not None
         logger.info("Tying to connect to WebSocket server...")
         async with self.session.ws_connect(
             f"ws://{self.host}:{self.port}{self.url}"
@@ -252,10 +264,10 @@
         async for msg in self.websocket:
             msg: aiohttp.WSMessage
             await self.handle_websocket_msg(msg)
         if not self.bot.should_exit.is_set():
             logger.warning("WebSocket connection closed!")
 
     @abstractmethod
-    async def handle_websocket_msg(self, msg: aiohttp.WSMessage):
+    async def handle_websocket_msg(self, msg: aiohttp.WSMessage) -> None:
         """处理 WebSocket 消息。"""
         raise NotImplementedError
```

### Comparing `alicebot-0.6.2/alicebot/bot.py` & `alicebot-0.7.0/alicebot/bot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 """AliceBot 机器人对象。
 
 AliceBot 的基础模块，每一个 AliceBot 机器人即是一个 `Bot` 实例。
 """
-import os
-import sys
-import json
-import time
-import signal
 import asyncio
+from collections import defaultdict
+from contextlib import AsyncExitStack
+from itertools import chain
+import json
+import os
+from pathlib import Path
 import pkgutil
+import signal
+import sys
 import threading
-from pathlib import Path
-from itertools import chain
-from collections import defaultdict
-from typing import Any, Dict, List, Type, Union, Callable, Optional, Awaitable
+import time
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Set,
+    Type,
+    Union,
+    overload,
+)
 
 from pydantic import ValidationError, create_model
 
-from alicebot.event import Event
 from alicebot.adapter import Adapter
-from alicebot.plugin import Plugin, PluginLoadType
-from alicebot.log import logger, error_or_exception
-from alicebot.typing import T_Adapter, T_BotHook, T_EventHook, T_AdapterHook
-from alicebot.config import MainConfig, ConfigModel, PluginConfig, AdapterConfig
+from alicebot.config import AdapterConfig, ConfigModel, MainConfig, PluginConfig
+from alicebot.dependencies import solve_dependencies
+from alicebot.event import Event
 from alicebot.exceptions import (
-    SkipException,
-    StopException,
     GetEventTimeout,
     LoadModuleError,
+    SkipException,
+    StopException,
 )
+from alicebot.log import error_or_exception, logger
+from alicebot.plugin import Plugin, PluginLoadType
+from alicebot.typing import T_Adapter, T_AdapterHook, T_BotHook, T_Event, T_EventHook
 from alicebot.utils import (
     ModulePathFinder,
+    get_classes_from_module_name,
+    is_config_class,
     samefile,
     wrap_get_func,
-    is_config_class,
-    get_classes_from_module_name,
 )
 
 try:
     import tomllib  # type: ignore
 except ModuleNotFoundError:
     import tomli as tomllib  # type: ignore
 
@@ -49,49 +62,54 @@
     signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
     signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
 )
 
 
 class Bot:
     """AliceBot 机器人对象，定义了机器人的基本方法。
-        读取并储存配置 `Config`，加载适配器 `Adapter` 和插件 `Plugin`，并进行事件分发。
+
+    读取并储存配置 `Config`，加载适配器 `Adapter` 和插件 `Plugin`，并进行事件分发。
 
     Attributes:
         config: 机器人配置。
         should_exit: 机器人是否应该进入准备退出状态。
         adapters: 当前已经加载的适配器的列表。
         plugins_priority_dict: 插件优先级字典。
         plugin_state: 插件状态。
         global_state: 全局状态。
     """
 
     config: MainConfig
     should_exit: asyncio.Event
-    adapters: List[Adapter]
-    plugins_priority_dict: Dict[int, List[Type[Plugin]]]
+    adapters: List[Adapter[Any, Any]]
+    plugins_priority_dict: Dict[int, List[Type[Plugin[Any, Any, Any]]]]
     plugin_state: Dict[str, Any]
     global_state: Dict[Any, Any]
 
     _condition: asyncio.Condition  # 用于处理 get 的 Condition
-    _current_event: Event  # 当前待处理的 Event
+    _current_event: Event[Any]  # 当前待处理的 Event
 
     _restart_flag: bool  # 重新启动标志
     _module_path_finder: ModulePathFinder  # 用于查找 plugins 的模块元路径查找器
     _raw_config_dict: Dict[str, Any]  # 原始配置字典
+    _adapter_tasks: Set["asyncio.Task[None]"]  # 适配器任务集合，用于保持对适配器任务的引用
+    _handle_event_tasks: Set["asyncio.Task[None]"]  # 事件处理任务，用于保持对适配器任务的引用
 
     # 以下属性不会在重启时清除
     _config_file: Optional[str]  # 配置文件
     _config_dict: Optional[Dict[str, Any]]  # 配置字典
     _hot_reload: bool  # 热重载
 
     _extend_plugins: List[
-        Union[Type[Plugin], str, Path]
+        Union[Type[Plugin[Any, Any, Any]], str, Path]
     ]  # 使用 load_plugins() 方法程序化加载的插件列表
     _extend_plugin_dirs: List[Path]  # 使用 load_plugins_from_dirs() 方法程序化加载的插件路径列表
-    _extend_adapters: List[Union[Type[Adapter], str]]  # 使用 load_adapter() 方法程序化加载的适配器列表
+    _extend_adapters: List[
+        Union[Type[Adapter[Any, Any]], str]
+    ]  # 使用 load_adapter() 方法程序化加载的适配器列表
     _bot_run_hooks: List[T_BotHook]
     _bot_exit_hooks: List[T_BotHook]
     _adapter_startup_hooks: List[T_AdapterHook]
     _adapter_run_hooks: List[T_AdapterHook]
     _adapter_shutdown_hooks: List[T_AdapterHook]
     _event_preprocessor_hooks: List[T_EventHook]
     _event_postprocessor_hooks: List[T_EventHook]
@@ -103,29 +121,31 @@
         config_dict: Optional[Dict[str, Any]] = None,
         hot_reload: bool = False,
     ):
         """初始化 AliceBot ，读取配置文件，创建配置，加载适配器和插件。
 
         Args:
             config_file: 配置文件，如不指定则使用默认的 `config.toml`。
-                若指定为 None ，则不加载配置文件。
-            config_dict: 配置字典，默认为 None。
-                若指定字典，则会忽略 config_file 配置，不再读取配置文件。
+                若指定为 `None`，则不加载配置文件。
+            config_dict: 配置字典，默认为 `None。`
+                若指定字典，则会忽略 `config_file` 配置，不再读取配置文件。
             hot_reload: 热重载。
                 启用后将自动检查 `plugin_dir` 中的插件文件更新，并在更新时自动重新加载。
         """
         self.config = MainConfig()
         self.plugins_priority_dict = defaultdict(list)
         self.plugin_state = defaultdict(lambda: type(None)())
         self.global_state = {}
 
         self.adapters = []
         self._restart_flag = False
         self._module_path_finder = ModulePathFinder()
         self._raw_config_dict = {}
+        self._adapter_tasks = set()
+        self._handle_event_tasks = set()
 
         self._config_file = config_file
         self._config_dict = config_dict
         self._hot_reload = hot_reload
 
         self._extend_plugins = []
         self._extend_plugin_dirs = []
@@ -137,15 +157,15 @@
         self._adapter_shutdown_hooks = []
         self._event_preprocessor_hooks = []
         self._event_postprocessor_hooks = []
 
         sys.meta_path.insert(0, self._module_path_finder)
 
     @property
-    def plugins(self) -> List[Type[Plugin]]:
+    def plugins(self) -> List[Type[Plugin[Any, Any, Any]]]:
         """当前已经加载的插件的列表。"""
         return list(chain(*self.plugins_priority_dict.values()))
 
     def run(self):
         """运行 AliceBot ，监听并拦截系统退出信号，更新机器人配置。"""
         self._restart_flag = True
         while self._restart_flag:
@@ -210,35 +230,41 @@
                         e,
                         self.config.bot.log.verbose_exception,
                     )
 
             for _adapter in self.adapters:
                 for _hook_func in self._adapter_run_hooks:
                     await _hook_func(_adapter)
-                asyncio.create_task(_adapter.safe_run())
+                _adapter_task = asyncio.create_task(_adapter.safe_run())
+                self._adapter_tasks.add(_adapter_task)
+                _adapter_task.add_done_callback(self._adapter_tasks.discard)
 
             await self.should_exit.wait()
 
             if hot_reload_task is not None:
                 await hot_reload_task
         finally:
             for _adapter in self.adapters:
                 for _hook_func in self._adapter_shutdown_hooks:
                     await _hook_func(_adapter)
                 await _adapter.shutdown()
+
+            while self._adapter_tasks:
+                await asyncio.sleep(0)
+
             for _hook_func in self._bot_exit_hooks:
                 await _hook_func(self)
 
             self.adapters.clear()
             self.plugins_priority_dict.clear()
             self._module_path_finder.path.clear()
 
-    def _remove_plugin_by_path(self, file: str) -> List[Type[Plugin]]:
+    def _remove_plugin_by_path(self, file: str) -> List[Type[Plugin[Any, Any, Any]]]:
         """根据路径删除已加载的插件。"""
-        removed_plugins: List[Type[Plugin]] = []
+        removed_plugins: List[Type[Plugin[Any, Any, Any]]] = []
         for plugins in self.plugins_priority_dict.values():
             _removed_plugins = list(
                 filter(
                     lambda x: x.__plugin_load_type__ != PluginLoadType.CLASS
                     and x.__plugin_file_path__ is not None
                     and samefile(x.__plugin_file_path__, file),
                     plugins,
@@ -262,23 +288,23 @@
                 'Hot reload needs to install "watchfiles", '
                 'try "pip install watchfiles"'
             )
             return
 
         logger.info("Hot reload is working!")
         async for changes in awatch(
-            *map(
-                lambda x: x.resolve(),
-                set(self._extend_plugin_dirs)
+            *(
+                x.resolve()
+                for x in set(self._extend_plugin_dirs)
                 .union(self.config.bot.plugin_dirs)
                 .union(
                     {Path(self._config_file)}
                     if self._config_dict is None and self._config_file is not None
                     else set()
-                ),
+                )
             ),
             stop_event=self.should_exit,
         ):
             # 按照 Change.deleted, Change.modified, Change.added 的顺序处理
             # 以确保发生重命名时先处理删除再处理新增
             for change_type, file in sorted(changes, key=lambda x: x[0], reverse=True):
                 # 更改配置文件
@@ -297,55 +323,57 @@
                         self.restart()
                     continue
 
                 # 更改插件文件夹
                 if change_type == Change.deleted:
                     # 针对删除操作特殊处理
                     if not file.endswith(".py"):
-                        file = os.path.join(file, "__init__.py")
+                        file = os.path.join(file, "__init__.py")  # noqa: PLW2901
                 else:
                     if os.path.isdir(file) and os.path.isfile(
                         os.path.join(file, "__init__.py")
                     ):
                         # 当新增一个目录，且此目录中包含 __init__.py 文件
                         # 说明此时发生的是添加一个 Python 包，则视为添加了此包的 __init__.py 文件
-                        file = os.path.join(file, "__init__.py")
+                        file = os.path.join(file, "__init__.py")  # noqa: PLW2901
                     if not (os.path.isfile(file) and file.endswith(".py")):
                         continue
 
                 if change_type == Change.added:
-                    logger.info(f"Hot reload: added file: {file}")
+                    logger.info(f"Hot reload: Added file: {file}")
                     self._load_plugins(Path(file), plugin_load_type=PluginLoadType.DIR)
                     self._update_config()
                     continue
-                elif change_type == Change.deleted:
+                elif change_type == Change.deleted:  # noqa: RET507
                     logger.info(f"Hot reload: Deleted file: {file}")
                     self._remove_plugin_by_path(file)
                     self._update_config()
                 elif change_type == Change.modified:
                     logger.info(f"Hot reload: Modified file: {file}")
                     self._remove_plugin_by_path(file)
                     self._load_plugins(Path(file), plugin_load_type=PluginLoadType.DIR)
                     self._update_config()
 
     def _update_config(self):
         """更新 config ，合并入来自 Plugin 和 Adapter 的 Config。"""
 
         def update_config(
-            source: List, name: str, base: Type[ConfigModel]
+            source: Union[List[Type[Plugin[Any, Any, Any]]], List[Adapter[Any, Any]]],
+            name: str,
+            base: Type[ConfigModel],
         ) -> ConfigModel:
             config_update_dict = {}
             for i in source:
                 config_class = getattr(i, "Config", None)
                 if is_config_class(config_class):
                     try:
                         default_value = config_class()
                     except ValidationError:
                         default_value = ...
-                    config_update_dict[getattr(config_class, "__config_name__")] = (
+                    config_update_dict[config_class.__config_name__] = (
                         config_class,
                         default_value,
                     )
             return create_model(name, **config_update_dict, __base__=base)(
                 **self._raw_config_dict
             )
 
@@ -398,124 +426,176 @@
         self.plugins_priority_dict.clear()
         self._load_plugins(*self.config.bot.plugins)
         self._load_plugins_from_dirs(*self.config.bot.plugin_dirs)
         self._load_plugins(*self._extend_plugins)
         self._load_plugins_from_dirs(*self._extend_plugin_dirs)
         self._update_config()
 
-    def _handle_exit(self, *args: Any):
+    def _handle_exit(self, *args: Any):  # noqa: ARG002
         """当机器人收到退出信号时，根据情况进行处理。"""
         logger.info("Stopping AliceBot...")
         if self.should_exit.is_set():
             logger.warning("Force Exit AliceBot...")
             sys.exit()
         else:
             self.should_exit.set()
 
     async def handle_event(
         self,
-        current_event: Event,
+        current_event: Event[Any],
         *,
         handle_get: bool = True,
         show_log: bool = True,
     ):
         """被适配器对象调用，根据优先级分发事件给所有插件，并处理插件的 `stop` 、 `skip` 等信号。
 
         此方法不应该被用户手动调用。
 
         Args:
             current_event: 当前待处理的 `Event`。
-            handle_get: 当前事件是否可以被 get 方法捕获，默认为 True。
-            show_log: 是否在日志中显示，默认为 True。
+            handle_get: 当前事件是否可以被 get 方法捕获，默认为 `True`。
+            show_log: 是否在日志中显示，默认为 `True`。
         """
         if show_log:
             logger.info(
                 f"Adapter {current_event.adapter.name} received: {current_event!r}"
             )
 
         if handle_get:
-            asyncio.create_task(self._handle_event())
+            _handle_event_task = asyncio.create_task(self._handle_event())
+            self._handle_event_tasks.add(_handle_event_task)
+            _handle_event_task.add_done_callback(self._handle_event_tasks.discard)
             await asyncio.sleep(0)
             async with self._condition:
                 self._current_event = current_event
                 self._condition.notify_all()
         else:
-            asyncio.create_task(self._handle_event(current_event))
+            _handle_event_task = asyncio.create_task(self._handle_event(current_event))
+            self._handle_event_tasks.add(_handle_event_task)
+            _handle_event_task.add_done_callback(self._handle_event_tasks.discard)
 
-    async def _handle_event(self, current_event: Optional[Event] = None):
+    async def _handle_event(self, current_event: Optional[Event[Any]] = None):
         if current_event is None:
             async with self._condition:
                 await self._condition.wait()
                 current_event = self._current_event
             if current_event.__handled__:
                 return
 
         for _hook_func in self._event_preprocessor_hooks:
             await _hook_func(current_event)
 
         for plugin_priority in sorted(self.plugins_priority_dict.keys()):
-            try:
-                logger.debug(
-                    f"Checking for matching plugins with priority {plugin_priority!r}"
-                )
-                stop = False
-                for _plugin in self.plugins_priority_dict[plugin_priority]:
-                    try:
-                        _plugin = _plugin(current_event)
+            logger.debug(
+                f"Checking for matching plugins with priority {plugin_priority!r}"
+            )
+            stop = False
+            for _plugin in self.plugins_priority_dict[plugin_priority]:
+                try:
+                    async with AsyncExitStack() as stack:
+                        _plugin = await solve_dependencies(
+                            _plugin,
+                            use_cache=True,
+                            stack=stack,
+                            dependency_cache={
+                                Bot: self,
+                                Event: current_event,
+                            },
+                        )
+                        if _plugin.name not in self.plugin_state and hasattr(
+                            _plugin, "__init_state__"
+                        ):
+                            plugin_state = _plugin.__init_state__()
+                            if plugin_state is not None:
+                                self.plugin_state[_plugin.name] = plugin_state
                         if await _plugin.rule():
                             logger.info(f"Event will be handled by {_plugin!r}")
                             try:
                                 await _plugin.handle()
                             finally:
                                 if _plugin.block:
                                     stop = True
-                    except SkipException:
-                        # 插件要求跳过自身继续当前事件传播
-                        continue
-                    except StopException:
-                        # 插件要求停止当前事件传播
-                        stop = True
-                    except Exception as e:
-                        error_or_exception(
-                            f'Exception in plugin "{_plugin}":',
-                            e,
-                            self.config.bot.log.verbose_exception,
-                        )
-                if stop:
-                    break
-            except Exception as e:
-                error_or_exception(
-                    f"Exception in handling event {current_event!r}:",
-                    e,
-                    self.config.bot.log.verbose_exception,
-                )
+                except SkipException:
+                    # 插件要求跳过自身继续当前事件传播
+                    continue
+                except StopException:
+                    # 插件要求停止当前事件传播
+                    stop = True
+                except Exception as e:
+                    error_or_exception(
+                        f'Exception in plugin "{_plugin}":',
+                        e,
+                        self.config.bot.log.verbose_exception,
+                    )
+            if stop:
+                break
 
         for _hook_func in self._event_postprocessor_hooks:
             await _hook_func(current_event)
 
         logger.info("Event Finished")
 
+    @overload
     async def get(
         self,
-        func: Optional[Callable[[Event], Union[bool, Awaitable[bool]]]] = None,
+        func: Optional[Callable[[Event[Any]], Union[bool, Awaitable[bool]]]] = None,
         *,
+        event_type: None = None,
+        adapter_type: None = None,
         max_try_times: Optional[int] = None,
         timeout: Optional[Union[int, float]] = None,
-    ) -> Event:
+    ) -> Event[Any]:
+        ...
+
+    @overload
+    async def get(
+        self,
+        func: Optional[Callable[[T_Event], Union[bool, Awaitable[bool]]]] = None,
+        *,
+        event_type: None = None,
+        adapter_type: Type[Adapter[T_Event, Any]],
+        max_try_times: Optional[int] = None,
+        timeout: Optional[Union[int, float]] = None,
+    ) -> T_Event:
+        ...
+
+    @overload
+    async def get(
+        self,
+        func: Optional[Callable[[T_Event], Union[bool, Awaitable[bool]]]] = None,
+        *,
+        event_type: Type[T_Event],
+        adapter_type: Optional[Type[T_Adapter]] = None,
+        max_try_times: Optional[int] = None,
+        timeout: Optional[Union[int, float]] = None,
+    ) -> T_Event:
+        ...
+
+    async def get(
+        self,
+        func: Optional[Callable[[Event[Any]], Union[bool, Awaitable[bool]]]] = None,
+        *,
+        event_type: Optional[Type[Event[Any]]] = None,
+        adapter_type: Optional[Type[Adapter[Any, Any]]] = None,
+        max_try_times: Optional[int] = None,
+        timeout: Optional[Union[int, float]] = None,
+    ) -> Event[Any]:
         """获取满足指定条件的的事件，协程会等待直到适配器接收到满足条件的事件、超过最大事件数或超时。
 
         Args:
             func: 协程或者函数，函数会被自动包装为协程执行。
                 要求接受一个事件作为参数，返回布尔值。当协程返回 `True` 时返回当前事件。
                 当为 `None` 时相当于输入对于任何事件均返回真的协程，即返回适配器接收到的下一个事件。
+            event_type: 当指定时，只接受指定类型的事件，先于 func 条件生效。默认为 `None`。
+            adapter_type: 当指定时，只接受指定适配器产生的事件，先于 func 条件生效。默认为 `None`。
             max_try_times: 最大事件数。
             timeout: 超时时间。
 
         Returns:
-            返回满足 func 条件的事件。
+            返回满足 `func` 条件的事件。
 
         Raises:
             GetEventTimeout: 超过最大事件数或超时。
         """
         _func = wrap_get_func(func)
 
         try_times = 0
@@ -534,26 +614,36 @@
                         await asyncio.wait_for(
                             self._condition.wait(),
                             timeout=start_time + timeout - time.time(),
                         )
                     except asyncio.TimeoutError:
                         break
 
-                if not self._current_event.__handled__:
-                    if await _func(self._current_event):
-                        self._current_event.__handled__ = True
-                        return self._current_event
+                if (
+                    not self._current_event.__handled__
+                    and (
+                        event_type is None
+                        or isinstance(self._current_event, event_type)
+                    )
+                    and (
+                        adapter_type is None
+                        or isinstance(self._current_event.adapter, adapter_type)
+                    )
+                    and await _func(self._current_event)
+                ):
+                    self._current_event.__handled__ = True
+                    return self._current_event
 
                 try_times += 1
 
         raise GetEventTimeout
 
     def _load_plugin_class(
         self,
-        plugin_class: Type[Plugin],
+        plugin_class: Type[Plugin[Any, Any, Any]],
         plugin_load_type: PluginLoadType,
         plugin_file_path: Optional[str],
     ):
         """加载插件类。"""
         priority = getattr(plugin_class, "priority", None)
         if type(priority) is int and priority >= 0:
             for _plugin in self.plugins:
@@ -595,27 +685,27 @@
                     plugin_class,
                     plugin_load_type,
                     module.__file__,
                 )
 
     def _load_plugins(
         self,
-        *plugins: Union[Type[Plugin], str, Path],
+        *plugins: Union[Type[Plugin[Any, Any, Any]], str, Path],
         plugin_load_type: Optional[PluginLoadType] = None,
     ):
         """加载插件。
 
         Args:
             *plugins: 插件类、插件模块名称或者插件模块文件路径。类型可以是 `Type[Plugin]`, `str` 或 `pathlib.Path`。
                 如果为 `Type[Plugin]` 类型时，将作为插件类进行加载。
                 如果为 `str` 类型时，将作为插件模块名称进行加载，格式和 Python `import` 语句相同。
                     例如：`path.of.plugin`。
                 如果为 `pathlib.Path` 类型时，将作为插件模块文件路径进行加载。
                     例如：`pathlib.Path("path/of/plugin")`。
-            plugin_load_type: 插件加载类型，如果为 None 则自动判断，否则使用指定的类型。
+            plugin_load_type: 插件加载类型，如果为 `None` 则自动判断，否则使用指定的类型。
         """
         for plugin_ in plugins:
             if isinstance(plugin_, type):
                 if issubclass(plugin_, Plugin):
                     self._load_plugin_class(
                         plugin_, plugin_load_type or PluginLoadType.CLASS, None
                     )
@@ -660,19 +750,20 @@
                         plugin_module_name, plugin_load_type or PluginLoadType.FILE
                     )
                 else:
                     logger.error(f'The plugin path "{plugin_}" must be a file')
             else:
                 logger.error(f"Type error: {plugin_} can not be loaded as plugin")
 
-    def load_plugins(self, *plugins: Union[Type[Plugin], str, Path]):
+    def load_plugins(self, *plugins: Union[Type[Plugin[Any, Any, Any]], str, Path]):
         """加载插件。
 
         Args:
-            *plugins: 插件类、插件模块名称或者插件模块文件路径。类型可以是 `Type[Plugin]`, `str` 或 `pathlib.Path`。
+            *plugins: 插件类、插件模块名称或者插件模块文件路径。
+                类型可以是 `Type[Plugin]`, `str` 或 `pathlib.Path`。
                 如果为 `Type[Plugin]` 类型时，将作为插件类进行加载。
                 如果为 `str` 类型时，将作为插件模块名称进行加载，格式和 Python `import` 语句相同。
                     例如：`path.of.plugin`。
                 如果为 `pathlib.Path` 类型时，将作为插件模块文件路径进行加载。
                     例如：`pathlib.Path("path/of/plugin")`。
         """
         self._extend_plugins.extend(plugins)
@@ -681,15 +772,15 @@
     def _load_plugins_from_dirs(self, *dirs: Path):
         """从目录中加载插件，以 `_` 开头的模块中的插件不会被导入。路径可以是相对路径或绝对路径。
 
         Args:
             *dirs: 储存包含插件的模块的模块路径。
                 例如：`pathlib.Path("path/of/plugins/")` 。
         """
-        dir_list = list(map(lambda x: str(x.resolve()), dirs))
+        dir_list = [str(x.resolve()) for x in dirs]
         logger.info(f'Loading plugins from dirs "{", ".join(map(str, dir_list))}"')
         self._module_path_finder.path.extend(dir_list)
         for module_info in pkgutil.iter_modules(dir_list):
             if not module_info.name.startswith("_"):
                 self._load_plugins_from_module_name(
                     module_info.name, PluginLoadType.DIR
                 )
@@ -700,15 +791,15 @@
         Args:
             *dirs: 储存包含插件的模块的模块路径。
                 例如：`pathlib.Path("path/of/plugins/")` 。
         """
         self._extend_plugin_dirs.extend(dirs)
         self._load_plugins_from_dirs(*dirs)
 
-    def _load_adapters(self, *adapters: Union[Type[Adapter], str]):
+    def _load_adapters(self, *adapters: Union[Type[Adapter[Any, Any]], str]):
         """加载适配器。
 
         Args:
             *adapters: 适配器类或适配器名称，类型可以是 `Type[Adapter]` 或 `str`。
                 如果为 `Type[Adapter]` 类型时，将作为适配器类进行加载。
                 如果为 `str` 类型时，将作为适配器模块名称进行加载，格式和 Python `import` 语句相同。
                     例如：`path.of.adapter`。
@@ -725,15 +816,15 @@
                         )
                 elif isinstance(adapter_, str):
                     adapter_classes = get_classes_from_module_name(adapter_, Adapter)
                     if not adapter_classes:
                         raise LoadModuleError(
                             f"Can not find Adapter class in the {adapter_} module"
                         )
-                    elif len(adapter_classes) > 1:
+                    if len(adapter_classes) > 1:
                         raise LoadModuleError(
                             f"More then one Adapter class in the {adapter_} module"
                         )
                     adapter_object = adapter_classes[0][0](self)  # type: ignore
                 else:
                     raise LoadModuleError(
                         f"Type error: {adapter_} can not be loaded as adapter"
@@ -747,29 +838,37 @@
             else:
                 self.adapters.append(adapter_object)
                 logger.info(
                     f'Succeeded to load adapter "{adapter_object.__class__.__name__}" '
                     f'from "{adapter_}"'
                 )
 
-    def load_adapters(self, *adapters: Union[Type[Adapter], str]):
+    def load_adapters(self, *adapters: Union[Type[Adapter[Any, Any]], str]):
         """加载适配器。
 
         Args:
             *adapters: 适配器类或适配器名称，类型可以是 `Type[Adapter]` 或 `str`。
                 如果为 `Type[Adapter]` 类型时，将作为适配器类进行加载。
                 如果为 `str` 类型时，将作为适配器模块名称进行加载，格式和 Python `import` 语句相同。
                     例如：`path.of.adapter`。
         """
         self._extend_adapters.extend(adapters)
         return self._load_adapters(*adapters)
 
+    @overload
+    def get_adapter(self, adapter: str) -> Adapter[Any, Any]:
+        ...
+
+    @overload
+    def get_adapter(self, adapter: Type[T_Adapter]) -> T_Adapter:
+        ...
+
     def get_adapter(
         self, adapter: Union[str, Type[T_Adapter]]
-    ) -> Union[Adapter, T_Adapter]:
+    ) -> Union[Adapter[Any, Any], T_Adapter]:
         """按照名称或适配器类获取已经加载的适配器。
 
         Args:
             adapter: 适配器名称或适配器类。
 
         Returns:
             获取到的适配器对象。
@@ -781,15 +880,15 @@
             if isinstance(adapter, str):
                 if _adapter.name == adapter:
                     return _adapter
             elif isinstance(_adapter, adapter):
                 return _adapter
         raise LookupError(f'Can not find adapter named "{adapter}"')
 
-    def get_plugin(self, name: str) -> Type[Plugin]:
+    def get_plugin(self, name: str) -> Type[Plugin[Any, Any, Any]]:
         """按照名称获取已经加载的插件类。
 
         Args:
             name: 插件名称
 
         Returns:
             获取到的插件类。
```

### Comparing `alicebot-0.6.2/alicebot/config.py` & `alicebot-0.7.0/alicebot/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """AliceBot 配置。
 
 AliceBot 使用 [pydantic](https://pydantic-docs.helpmanual.io/) 来读取配置。
 """
 from typing import Set, Union
 
-from pydantic import Extra, Field, BaseModel, DirectoryPath
+from pydantic import BaseModel, DirectoryPath, Extra, Field
 
 __all__ = [
     "ConfigModel",
     "LogConfig",
     "BotConfig",
     "PluginConfig",
     "AdapterConfig",
@@ -30,15 +30,15 @@
 
 
 class LogConfig(ConfigModel):
     """AliceBot 日志相关设置。
 
     Attributes:
         level: 日志级别。
-        verbose_exception: 详细的异常记录，设置为 True 时会在日志中添加异常的 Traceback。
+        verbose_exception: 详细的异常记录，设置为 `True` 时会在日志中添加异常的 Traceback。
     """
 
     level: Union[str, int] = "DEBUG"
     verbose_exception: bool = False
 
 
 class BotConfig(ConfigModel):
```

### Comparing `alicebot-0.6.2/alicebot/exceptions.py` & `alicebot-0.7.0/alicebot/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """跳过当前插件继续当前事件传播。"""
 
 
 class StopException(EventException):
     """停止当前事件传播。"""
 
 
-class AliceBotException(Exception):
+class AliceBotException(Exception):  # noqa: N818
     """所有 AliceBot 发生的异常的基类。"""
 
 
 class GetEventTimeout(AliceBotException):
     """当 get 方法超时使被抛出。"""
```

### Comparing `alicebot-0.6.2/alicebot/message.py` & `alicebot-0.7.0/alicebot/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,131 +1,142 @@
 """AliceBot 消息。
 
 实现了常用的基本消息 `Message` 和消息字段 `MessageSegment` 模型供适配器使用。
 适配器开发者可以根据需要实现此模块中消息类的子类或定义与此不同的消息类型，但建议若可行的话应尽量使用此模块中消息类的子类。
 """
-import dataclasses
 from copy import copy, deepcopy
-from typing_extensions import Self
-from dataclasses import field, dataclass
+import dataclasses
+from dataclasses import dataclass, field
 from typing import (
     Any,
     Dict,
-    List,
-    Type,
-    Union,
     Generic,
-    Mapping,
-    TypeVar,
     Iterable,
     Iterator,
+    List,
+    Mapping,
     Optional,
     SupportsIndex,
+    Type,
+    TypeVar,
+    Union,
+    overload,
 )
+from typing_extensions import Self
 
 __all__ = ["T_Message", "T_MessageSegment", "T_MS", "Message", "MessageSegment"]
 
-T_Message = TypeVar("T_Message", bound="Message")
-T_MessageSegment = TypeVar("T_MessageSegment", bound="MessageSegment")
+T_Message = TypeVar("T_Message", bound="Message[Any]")
+T_MessageSegment = TypeVar("T_MessageSegment", bound="MessageSegment[Any]")
 
 # 可以转化为 MessageSegment 的类型
 T_MS = Union[T_MessageSegment, str, Mapping[str, Any]]
 
 
 class Message(List[T_MessageSegment]):
     """消息。
 
     本类是 `List` 的子类，并重写了 `__init__()` 方法，
-    可以直接处理 str, Mapping, Iterable[Mapping], MessageSegment, Message。
-    其中 str 的支持需要适配器开发者重写 `_str_to_message_segment()` 方法实现。
-    本类重写了 `+` 和 `+=` 运算符，可以直接和 Message, MessageSegment 等类型的对象执行取和运算。
-    若开发者实现了 MessageSegment 的子类则需要重写 `_message_segment_class()` 方法，
-    并在 MessageSegment 的子类中重写 `_message_class()` 方法。
+    可以直接处理 `str`, `Mapping`, `Iterable[Mapping]`, `MessageSegment`, `Message`。
+    其中 `str` 的支持需要适配器开发者重写 `_str_to_message_segment()` 方法实现。
+    本类重写了 `+` 和 `+=` 运算符，可以直接和 `Message`, `MessageSegment` 等类型的对象执行取和运算。
+    若开发者实现了 `MessageSegment` 的子类则需要重写 `_message_segment_class()` 方法，
+    并在 `MessageSegment` 的子类中重写 `_message_class()` 方法。
     """
 
     def __init__(
         self,
-        message: Union[Self, T_MS, Iterable[T_MS]] = None,
-        *args: Any,
-        **kwargs: Any,
+        message: Union[
+            Self, T_MS[T_MessageSegment], Iterable[T_MS[T_MessageSegment]], None
+        ] = None,
     ):
-        super().__init__(*args, **kwargs)
+        """初始化。
+
+        Args:
+            message: 可以被转化为消息的数据。
+            *args: 其他参数。
+        """
+        if message is None:
+            return
         if isinstance(message, self.__class__):
             self.extend(message)  # type: ignore
         else:
             self.extend(self._construct(message))
 
     @property
     def _message_segment_class(self) -> Type[T_MessageSegment]:
-        """若开发者实现了 MessageSegment 的子类则需要重写此方法。
+        """若开发者实现了 `MessageSegment` 的子类则需要重写此方法。
 
         Returns:
-            MessageSegment 类。
+            `MessageSegment` 类。
         """
         return MessageSegment  # type: ignore
 
     @classmethod
     def __get_validators__(cls):
-        """pydantic 自定义校验器。"""
+        """Pydantic 自定义校验器。"""
         yield cls._validate
 
     @classmethod
     def _validate(cls, value: Mapping[str, Any]):
         return cls(value)
 
     def _construct(
-        self, msg: Union[T_MS, Iterable[T_MS]]
+        self, msg: Union[T_MS[T_MessageSegment], Iterable[T_MS[T_MessageSegment]]]
     ) -> Iterator[T_MessageSegment]:
-        """用于将 str, Mapping, Iterable[Mapping] 等类型转换为 MessageSegment。
-        用于 pydantic 数据解析和方便用户使用。
+        """用于 Pydantic 数据解析和方便用户使用。
+
+        用于将 `str`, `Mapping`, `Iterable[Mapping]` 等类型转换为 `MessageSegment。`
 
         Args:
-            msg: 要解析为 MessageSegment 的数据。
+            msg: 要解析为 `MessageSegment` 的数据。
 
         Returns:
-            MessageSegment 生成器。
+            `MessageSegment` 生成器。
         """
         if isinstance(msg, self._message_segment_class):
             yield msg
         elif isinstance(msg, Mapping):
             yield self._mapping_to_message_segment(msg)  # type: ignore
         elif isinstance(msg, str):
             yield self._str_to_message_segment(msg)
         else:
             for seg in msg:
                 for i in self._construct(seg):
                     yield i
 
     def _mapping_to_message_segment(self, msg: Mapping[str, Any]) -> T_MessageSegment:
-        """用于将 Mapping 转换为 MessageSegment ，如有需要，子类可重写此方法以更改对 Mapping 的默认行为。
+        """用于将 `Mapping` 转换为 `MessageSegment`。
+
+        如有需要，子类可重写此方法以更改对 `Mapping` 的默认行为。
 
         Args:
-            msg: 要解析为 MessageSegment 的数据。
+            msg: 要解析为 `MessageSegment` 的数据。
 
         Returns:
-            由 Mapping 转换的 MessageSegment。
+            由 Mapping 转换的 `MessageSegment`。
         """
         return self._message_segment_class(**msg)
 
     def _str_to_message_segment(self, msg: str) -> T_MessageSegment:
-        """用于将 str 转换为 MessageSegment ，子类应重写此方法以支持 str 及支持新的消息字段类。
+        """用于将 `str` 转换为 `MessageSegment`，子类应重写此方法以支持 `str` 及支持新的消息字段类。
 
         Args:
-            msg: 要解析为 MessageSegment 的数据。
+            msg: 要解析为 `MessageSegment` 的数据。
 
         Returns:
-            由 str 转换的 MessageSegment。
+            由 `str` 转换的 `MessageSegment`。
         """
         raise NotImplementedError
 
     def __repr__(self) -> str:
-        return "Message:[{}]".format(",".join(map(lambda x: repr(x), self)))
+        return "Message:[{}]".format(",".join(map(repr, self)))
 
     def __str__(self) -> str:
-        return "".join(map(lambda x: str(x), self))
+        return "".join(map(str, self))
 
     def __contains__(self, item: object) -> bool:
         if isinstance(item, str):
             return item in str(self)
         return super().__contains__(item)
 
     def __add__(
@@ -151,23 +162,23 @@
             raise TypeError(
                 f"unsupported operand type(s) for +: '{type(self)}' and '{type(other)}'"
             )
         return self
 
     def is_text(self) -> bool:
         """是否是纯文本消息。"""
-        return all(map(lambda x: x.is_text(), self))
+        return all(x.is_text() for x in self)
 
     def get_plain_text(self) -> str:
         """获取消息中的纯文本部分。
 
         Returns:
             消息中的纯文本部分。
         """
-        return "".join(map(lambda x: str(x), filter(lambda x: x.is_text(), self)))
+        return "".join(map(str, filter(lambda x: x.is_text(), self)))
 
     def copy(self) -> Self:
         """返回自身的浅复制。
 
         Returns:
             自身的浅复制。
         """
@@ -185,29 +196,29 @@
         self,
         prefix: Union[str, T_MessageSegment],
         start: Optional[SupportsIndex] = None,
         end: Optional[SupportsIndex] = None,
     ) -> bool:
         """实现类似字符串的 `startswith()` 方法。
 
-        当 `prefix` 类型是 str 时，会将自身转换为 str 类型，再调用 str 类型的 `startswith()` 方法。
-        当 `prefix` 类型是 MessageSegment 时，`start` 和 `end` 参数将不其作用，
+        当 `prefix` 类型是 `str` 时，会将自身转换为 `str` 类型，再调用 `str` 类型的 `startswith()` 方法。
+        当 `prefix` 类型是 `MessageSegment` 时，`start` 和 `end` 参数将不其作用，
             会判断列表的第一个消息字段是否和 `prefix` 相等。
 
         Args:
             prefix: 前缀。
             start: 开始检查位置。
             end: 停止检查位置。
 
         Returns:
             检查结果。
-        """
+        """  # noqa: D402
         if isinstance(prefix, str):
             return str(self).startswith(prefix, start, end)
-        elif isinstance(prefix, self._message_segment_class):
+        if isinstance(prefix, self._message_segment_class):
             if len(self) == 0:
                 return False
             return self[0] == prefix
         raise TypeError(
             f"first arg must be str or {self._message_segment_class}, not {type(prefix)}"
         )
 
@@ -215,61 +226,71 @@
         self,
         suffix: Union[str, T_MessageSegment],
         start: Optional[SupportsIndex] = None,
         end: Optional[SupportsIndex] = None,
     ) -> bool:
         """实现类似字符串的 `endswith()` 方法。
 
-        当 `suffix` 类型是 str 时，会将自身转换为 str 类型，再调用 str 类型的 `endswith()` 方法。
+        当 `suffix` 类型是 `str` 时，会将自身转换为 `str` 类型，再调用 `str` 类型的 `endswith()` 方法。
         当 `suffix` 类型是 MessageSegment 时，`start` 和 `end` 参数将不其作用，
             会判断列表的最后一个消息字段是否和 `suffix` 相等。
 
         Args:
             suffix: 后缀。
             start: 开始检查位置。
             end: 停止检查位置。
 
         Returns:
             检查结果。
-        """
+        """  # noqa: D402
         if isinstance(suffix, str):
             return str(self).endswith(suffix, start, end)
-        elif isinstance(suffix, self._message_segment_class):
+        if isinstance(suffix, self._message_segment_class):
             if len(self) == 0:
                 return False
             return self[-1] == suffix
         raise TypeError(
             f"first arg must be str or {self._message_segment_class}, not {type(suffix)}"
         )
 
+    @overload
+    def replace(self, old: str, new: str, count: int = -1) -> Self:
+        ...
+
+    @overload
+    def replace(
+        self, old: T_MessageSegment, new: Optional[T_MessageSegment], count: int = -1
+    ) -> Self:
+        ...
+
     def replace(
         self,
         old: Union[str, T_MessageSegment],
         new: Optional[Union[str, T_MessageSegment]],
         count: int = -1,
     ) -> Self:
         """实现类似字符串的 `replace()` 方法。
 
-        当 `old` 为 str 类型时，`new` 也必须是 str ，本方法将仅对 `is_text()` 为 True 的消息字段进行处理。
-        当 `old` 为 MessageSegment 类型时，`new` 可以是 MessageSegment 或 None ，本方法将对所有消息字段进行处理，
-            并替换符合条件的消息字段。None 表示删除匹配到的消息字段。
+        当 `old` 为 `str` 类型时，`new` 也必须是 `str`，本方法将仅对 `is_text()` 为 `True` 的消息字段进行处理。
+        当 `old` 为 MessageSegment 类型时，`new` 可以是 `MessageSegment` 或 `None`，本方法将对所有消息字段进行处理，
+            并替换符合条件的消息字段。`None` 表示删除匹配到的消息字段。
 
         Args:
             old: 被匹配的字符串或消息字段。
             new: 被替换为的字符串或消息字段。
             count: 替换的次数。
 
         Returns:
             替换后的消息对象。
-        """
+        """  # noqa: D402
         if type(old) is str:
             if type(new) is not str:
                 raise TypeError("when type of old is str, type of new must be str.")
             return self._replace_str(old, new, count)
-        elif isinstance(old, self._message_segment_class):
+        if isinstance(old, self._message_segment_class):
             if not (isinstance(new, self._message_segment_class) or new is None):
                 raise TypeError(
                     "when type of old is MessageSegment, "
                     "type of new must be MessageSegment or None."
                 )
             temp_msg = self.deepcopy()
             for index, item in enumerate(temp_msg):
@@ -277,22 +298,21 @@
                     break
                 if item == old:
                     temp_msg[index] = new  # type: ignore
                     count -= 1
             if new is None:
                 temp_msg = self.__class__(filter(lambda x: x is not None, self))  # type: ignore
             return temp_msg
-        else:
-            raise TypeError("type of old must be str or MessageSegment")
+        raise TypeError("type of old must be str or MessageSegment")
 
     def _replace_str(self, old: str, new: str, count: int = -1) -> Self:
         """实现类似字符串的 `replace()` 方法。
 
-        本方法将被 `replace()` 方法调用以处理 str 类型的替换，
-        默认将 MessageSegment 对象的 data['text'] 视为存放纯文本的位置。
+        本方法将被 `replace()` 方法调用以处理 `str` 类型的替换，
+        默认将 `MessageSegment` 对象的 `data['text']` 视为存放纯文本的位置。
         适配器开发者可自行重写此方法以适配其他情况。
 
         Args:
             old: 被匹配的字符串或消息字段。
             new: 被替换为的字符串或消息字段。
             count: 替换的次数。
 
@@ -317,39 +337,39 @@
 
 
 @dataclass
 class MessageSegment(Mapping[str, Any], Generic[T_Message]):
     """消息字段。
 
     本类实现了所有映射类型的方法，这些方法全部是对 `data` 属性的操作。
-    本类重写了 `+` 和 `+=` 运算符，可以直接和 Message, MessageSegment 等类型的对象执行取和运算，返回 Message 对象。
-    若开发者实现了 Message 和 MessageSegment 的子类则需要重写 `_message_class()` 方法。
+    本类重写了 `+` 和 `+=` 运算符，可以直接和 `Message`, `MessageSegment` 等类型的对象执行取和运算，返回 `Message` 对象。
+    若开发者实现了 `Message` 和 `MessageSegment` 的子类则需要重写 `_message_class()` 方法。
 
     Attributes:
         type: 消息字段类型。
         data: 消息字段内容。
     """
 
     type: str
     data: Dict[str, Any] = field(default_factory=dict)
 
     @property
     def _message_class(self) -> Type[T_Message]:
-        """若开发者实现了 Message 和 MessageSegment 的子类则需要重写此方法。
+        """若开发者实现了 `Message` 和 `MessageSegment` 的子类则需要重写此方法。
 
         Returns:
-            Message 类。
+            `Message` 类。
         """
         return Message  # type: ignore
 
     def as_dict(self) -> Dict[str, Any]:
-        """将当前对象解析为 Dict 对象，开发者可重写本方法以适配特殊的解析方式。
+        """将当前对象解析为 `dict` 对象，开发者可重写本方法以适配特殊的解析方式。
 
         Returns:
-            Dict 对象。
+            `dict` 对象。
         """
         return dataclasses.asdict(self)
 
     def __str__(self) -> str:
         return str(self.data)
 
     def __repr__(self) -> str:
@@ -363,15 +383,15 @@
 
     def __delitem__(self, key: str):
         del self.data[key]
 
     def __len__(self) -> int:
         return len(self.data)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[str]:
         yield from self.data.__iter__()
 
     def __contains__(self, key: object) -> bool:
         return key in self.data
 
     def __eq__(self, other: Self) -> bool:
         return self.type == other.type and self.data == other.data
@@ -382,27 +402,32 @@
     def __add__(self, other: Any) -> T_Message:
         return self._message_class(self) + other
 
     def __radd__(self, other: Any) -> T_Message:
         return self._message_class(other) + self
 
     def get(self, key: str, default: Any = None):
+        """如果 `key` 存在于 `data` 字典中则返回 `key` 的值，否则返回 `default`。"""
         return self.data.get(key, default)
 
     def keys(self):
+        """返回由 `data` 字典键组成的一个新视图。"""
         return self.data.keys()
 
     def values(self):
+        """返回由 `data` 字典值组成的一个新视图。"""
         return self.data.values()
 
     def items(self):
+        """返回由 `data` 字典项 (`(键, 值)` 对) 组成的一个新视图。"""
         return self.data.items()
 
     def is_text(self) -> bool:
-        """
+        """是否是纯文本消息字段。
+
         Returns:
             是否是纯文本消息字段。
         """
         return self.type == "text"
 
     def copy(self) -> Self:
         """返回自身的浅复制。
@@ -415,8 +440,7 @@
     def deepcopy(self) -> Self:
         """返回自身的深复制。
 
         Returns:
             自身的深复制。
         """
         return deepcopy(self)
-        return deepcopy(self)
```

### Comparing `alicebot-0.6.2/alicebot/plugin.py` & `alicebot-0.7.0/alicebot/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 """AliceBot 插件。
 
 所有 AliceBot 插件的基类。所有用户编写的插件必须继承自 `Plugin` 类。
 """
-from enum import Enum
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Type, Generic, NoReturn, Optional, final
+from enum import Enum
+from typing import (
+    TYPE_CHECKING,
+    ClassVar,
+    Generic,
+    NoReturn,
+    Optional,
+    Type,
+    cast,
+    final,
+)
 
-from alicebot.utils import is_config_class
-from alicebot.typing import T_Event, T_State, T_Config
+from alicebot.dependencies import Depends
+from alicebot.event import Event
 from alicebot.exceptions import SkipException, StopException
+from alicebot.typing import T_Config, T_Event, T_State
+from alicebot.utils import is_config_class
 
 if TYPE_CHECKING:
     from alicebot.bot import Bot
 
 __all__ = ["Plugin", "PluginLoadType"]
 
 
@@ -27,44 +38,48 @@
 
 class Plugin(ABC, Generic[T_Event, T_State, T_Config]):
     """所有 AliceBot 插件的基类。
 
     Attributes:
         event: 当前正在被此插件处理的事件。
         priority: 插件的优先级，数字越小表示优先级越高，默认为 0。
-        block: 插件执行结束后是否阻止事件的传播。True 表示阻止。
+        block: 插件执行结束后是否阻止事件的传播。`True` 表示阻止。
         __plugin_load_type__: 插件加载类型，由 AliceBot 自动设置，反映了此插件是如何被加载的。
         __plugin_file_path__: 当插件加载类型为 `PluginLoadType.CLASS` 时为 `None`，
             否则为定义插件在的 Python 模块的位置。
     """
 
-    event: T_Event
-    priority: int = 0
-    block: bool = False
-    Config: Type[T_Config] = type(None)  # type: ignore
-
-    __plugin_load_type__: PluginLoadType
-    __plugin_file_path__: Optional[str]
-
-    @final
-    def __init__(self, event: T_Event):
-        self.event = event
-
-        if not hasattr(self, "priority"):
-            self.priority = 0
-        if not hasattr(self, "block"):
-            self.block = False
+    event: T_Event = cast(T_Event, Depends(Event))
 
-        self.get = self.bot.get
+    priority: ClassVar[int] = 0
+    block: ClassVar[bool] = False
 
-        self.__post_init__()
+    # 不能使用 ClassVar 因为 PEP 526 不允许这样做
+    Config: Type[T_Config]
 
-    def __post_init__(self):
-        """用于初始化后处理，被 `__init__()` 方法调用。"""
-        pass
+    __plugin_load_type__: ClassVar[PluginLoadType]
+    __plugin_file_path__: ClassVar[Optional[str]]
+
+    if TYPE_CHECKING:
+
+        def __init_state__(self) -> T_State:
+            """初始化插件状态。"""
+            ...
+
+    def __init_subclass__(
+        cls,
+        /,
+        config: Optional[Type[T_Config]] = None,
+        init_state: Optional[T_State] = None,
+    ) -> None:
+        super().__init_subclass__()
+        if not hasattr(cls, "Config") and config is not None:
+            cls.Config = config
+        if init_state is not None:
+            cls.__init_state__ = lambda self: init_state  # noqa: ARG005
 
     @final
     @property
     def name(self) -> str:
         """插件类名称。"""
         return self.__class__.__name__
 
@@ -74,27 +89,32 @@
         """机器人对象。"""
         return self.event.adapter.bot
 
     @final
     @property
     def config(self) -> T_Config:
         """插件配置。"""
-        if is_config_class(self.Config):
-            return getattr(self.bot.config.plugin, self.Config.__config_name__, None)  # type: ignore
+        config_class = getattr(self, "Config", None)
+        if is_config_class(config_class):
+            return getattr(
+                self.bot.config.plugin,
+                config_class.__config_name__,
+                None,
+            )  # type: ignore
         return None  # type: ignore
 
     @final
     def stop(self) -> NoReturn:
         """停止当前事件传播。"""
-        raise StopException()
+        raise StopException
 
     @final
     def skip(self) -> NoReturn:
         """跳过自身继续当前事件传播。"""
-        raise SkipException()
+        raise SkipException
 
     @final
     @property
     def state(self) -> T_State:
         """插件状态。"""
         return self.bot.plugin_state[self.name]
```

### Comparing `alicebot-0.6.2/PKG-INFO` & `alicebot-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot
-Version: 0.6.2
+Version: 0.7.0
 Summary: A simply asynchronous python chatbot framework.
 Home-page: https://docs.alicebot.dev/
 License: MIT
 Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq
 Author: st1020
 Author-email: stone_1020@qq.com
 Requires-Python: >=3.8,<4.0
@@ -15,15 +15,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications :: Chat
 Provides-Extra: all
 Provides-Extra: apscheduler
 Provides-Extra: cqhttp
 Provides-Extra: dingtalk
 Provides-Extra: hot-reload
 Provides-Extra: mirai
@@ -78,87 +77,86 @@
 
 AliceBot 是一个简单的 Python 异步多后端机器人框架，支持多种协议适配，可以轻松地编写易于学习和使用的插件来拓展其功能。
 
 本项目受到了 [NoneBot](https://github.com/nonebot/nonebot2/) 项目的启发，您可以在 [对比](#对比) 小节中查看这两个项目的异同，以便您选择更适合自己的机器人框架。
 
 ## 特点
 
-AliceBot 使用了非常灵活且易于使用的插件编写方式，您只需要编写两个方法即可实现一个功能强大的插件。
-
-AliceBot 的适配协议并不与任何一种库或网络协议绑定，您可以自由选择或编写适合您的适配器。
+- **简单**：AliceBot 使用了非常灵活且易于使用的插件编写方式，您只需要编写两个方法即可实现一个功能强大的插件。
+- **灵活**：AliceBot 的适配协议并不与任何一种库或网络协议绑定，您可以自由选择或编写适合您的适配器。
+- **高效**：AliceBot 基于 Python 的异步 I/O，轻松处理大量请求。较少的封装，在保持易用的同时追求最好的性能。
 
 目前 AliceBot 官方维护了以下协议适配：
 
-- [OneBot (CQHTTP) 协议](https://github.com/botuniverse/onebot) （支持QQ等）[ws](https://github.com/botuniverse/onebot-11/blob/master/communication/ws.md) 和 [ws-reverse](https://github.com/botuniverse/onebot-11/blob/master/communication/ws-reverse.md) 连接方式
+- [OneBot (CQHTTP) 协议](https://github.com/botuniverse/onebot) （支持 QQ 等）[ws](https://github.com/botuniverse/onebot-11/blob/master/communication/ws.md) 和 [ws-reverse](https://github.com/botuniverse/onebot-11/blob/master/communication/ws-reverse.md) 连接方式
 - [mirai-api-http 协议](https://github.com/project-mirai/mirai-api-http) 2.0+ [ws](https://github.com/project-mirai/mirai-api-http/blob/master/docs/adapter/WebsocketAdapter.md) 和 [reverse-ws](https://github.com/project-mirai/mirai-api-http/blob/master/docs/adapter/ReverseWebsocketAdapter.md) 连接方式
 - [钉钉](https://developers.dingtalk.com/document/robots/robot-overview) 企业机器人的 outgoing （回调）连接方式
 
 更多协议正在适配中 ...
 
+更多信息：[简介 - AliceBot 文档](https://docs.alicebot.dev/guide/)
+
 ## 即刻开始
 
 1. 安装：
 
    ```bash
    pip install alicebot[all]
    ```
 
 2. 第一个 AliceBot 项目：
 
    ```python
    from alicebot import Bot
-   
+
    bot = Bot()
    bot.load_adapters("alicebot.adapter.cqhttp")
-   
+
    bot.run()
    ```
 
 3. 第一个 AliceBot 插件：
 
    ```python
    from alicebot import Plugin
-   
-   
+
+
    class Echo(Plugin):
        async def handle(self) -> None:
            await self.event.reply(self.event.message.replace("echo ", ""))
-   
+
        async def rule(self) -> bool:
            if self.event.adapter.name != "cqhttp":
                return False
            if self.event.type != "message":
                return False
            return self.event.message.startswith("echo ")
    ```
 
 更多信息请参阅 AliceBot [文档](https://docs.alicebot.dev/)。
 
 ## 对比
 
-本项目受到了 [NoneBot](https://github.com/nonebot/nonebot2/) 项目的启发，以下简单介绍两者的异同。
+本项目受到了 [NoneBot](https://github.com/nonebot/nonebot2) 项目的启发，以下简单介绍两者的异同。
 
 相同点：
 
 - 两者都是使用 Python 编写的，使用了协程异步的高性能机器人框架。
 - 两者都支持多种协议。
 - 两者都会对机器人收到的事件进行解析和处理，并按优先级分发给插件（事件响应器）来完成具体的功能。
 - 两者都基于 MIT 协议开源，这意味着您可以在遵循协议的前提下任意使用本项目。
 
 不同点：
 
 - 总的来说，NoneBot 是一个较为全面的机器人框架，而 AliceBot 是一个小巧简洁的机器人框架，它不包含一些复杂的高级特性，但更加灵活且易于学习。
-- NoneBot 在实现上与 WebSocket 通讯协议深度绑定，它需要一个支持 ASGI 服务器协议的驱动框架，而 AliceBot 并不与任何协议绑定，它甚至可以用来驱动您的树莓派智能音箱。当然，如果您只需要一个支持常见网络聊天工具的机器人框架的话，它们并没有什么区别。
-- NoneBot 提供了很多预设规则和权限控制机制，而 AliceBot 则没有提供，由于插件编写方式的不同，AliceBot 选择给您最大的自由，您需要自行编写插件在何时运行的方法（`rule()` 方法），这在绝大部份情况下并不会造成您编写更多的代码或是影响插件的可读性，自行实现也不会非常困难，但如果您真的需要这些高级功能又不想自己实现的话，NoneBot 提供了更好的选择。
+- AliceBot 的插件编写风格和 NoneBot 不同，相对而言，AliceBot 更加注重于易于入门和“渐进式框架”，这意味着 AliceBot 大部分的功能都是可选的，您只需要了解很少的知识即可开始使用，随着项目规模的扩大和复杂性的增加，您可以继续深入需要的特性，而不需要一开始就掌握全部的特性。“它是一个可以与你共同成长、适应你不同需求的框架。”
+- NoneBot 在实现上与 HTTP / WebSocket 通讯协议深度绑定，它需要一个支持 ASGI 服务器协议的“驱动器”，而 AliceBot 并不与任何协议绑定，它甚至可以用来驱动您的树莓派智能音箱。当然，如果您只需要一个支持常见网络聊天工具的机器人框架的话，它们并没有什么区别。
 - NoneBot 拥有相对庞大的用户基数和社区规模，也拥有数量众多的插件，而 AliceBot 则是一个新生项目，这意味着如果您使用 NoneBot 您可能会更加容易找到已经编写完毕的您感兴趣的插件，并且您当您遇到问题时也能够更快地查找到相关资料或者获得解答。
-- NoneBot 相对较为庞大，封装相对较多，完全学习理解需要一定时间，而 AliceBot 小巧简洁，封装较少，很容易掌握。
 
 总而言之，两者有着各自的特点，您可以根据需要选用。
 
-作者就是在使用 NoneBot 时觉得插件编写不是很易用，于是萌发了编写一个新的机器人框架的想法，AliceBot 就这样诞生了。
-
 ## 许可证
 
 AliceBot 采用 MIT 许可证开放源代码。
 
 本项目的图标由 迷糊小梦神 绘制，作为本项目的一部分，使用与本项目相同的许可证开放使用。
```

#### html2text {}

```diff
@@ -1,85 +1,81 @@
-Metadata-Version: 2.1 Name: alicebot Version: 0.6.2 Summary: A simply
+Metadata-Version: 2.1 Name: alicebot Version: 0.7.0 Summary: A simply
 asynchronous python chatbot framework. Home-page: https://docs.alicebot.dev/
 License: MIT Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq Author: st1020 Author-
 email: stone_1020@qq.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework ::
 Robot Framework Classifier: Framework :: Robot Framework :: Library Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Classifier: Topic :: Communications :: Chat Provides-Extra: all
-Provides-Extra: apscheduler Provides-Extra: cqhttp Provides-Extra: dingtalk
-Provides-Extra: hot-reload Provides-Extra: mirai Requires-Dist: aiohttp
-(>=3.8.0,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: pydantic
-(>=1.10.0,<2.0.0) Requires-Dist: tomli (>=2.0.0,<3.0.0) ; python_version <
-"3.11" Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Project-URL:
-Documentation, https://docs.alicebot.dev/ Project-URL: Repository, https://
-github.com/AliceBotProject/alicebot Description-Content-Type: text/markdown
+Programming Language :: Python :: 3.11 Classifier: Topic :: Communications ::
+Chat Provides-Extra: all Provides-Extra: apscheduler Provides-Extra: cqhttp
+Provides-Extra: dingtalk Provides-Extra: hot-reload Provides-Extra: mirai
+Requires-Dist: aiohttp (>=3.8.0,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist: tomli (>=2.0.0,<3.0.0)
+; python_version < "3.11" Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Project-URL: Documentation, https://docs.alicebot.dev/ Project-URL: Repository,
+https://github.com/AliceBotProject/alicebot Description-Content-Type: text/
+markdown
      [logo] # AliceBot **ç®åç Python å¼æ­¥å¤åç«¯æºå¨äººæ¡æ¶**
                        [license] [pypi] [pypi] [github]
                                   [qq-group]
                    ææ¡£ Â· æå Â· API_åè Â· ç¤ºä¾
 ## ç®ä» AliceBot æ¯ä¸ä¸ªç®åç Python
 å¼æ­¥å¤åç«¯æºå¨äººæ¡æ¶ï¼æ¯æå¤ç§åè®®ééï¼å¯ä»¥è½»æ¾å°ç¼åæäºå­¦ä¹ åä½¿ç¨çæä»¶æ¥æå±å¶åè½ã
 æ¬é¡¹ç®åå°äº [NoneBot](https://github.com/nonebot/nonebot2/
 ) é¡¹ç®çå¯åï¼æ¨å¯ä»¥å¨ [å¯¹æ¯](#å¯¹æ¯)
 å°èä¸­æ¥çè¿ä¸¤ä¸ªé¡¹ç®çå¼åï¼ä»¥ä¾¿æ¨éæ©æ´éåèªå·±çæºå¨äººæ¡æ¶ã
-## ç¹ç¹ AliceBot
+## ç¹ç¹ - **ç®å**ï¼AliceBot
 ä½¿ç¨äºéå¸¸çµæ´»ä¸æäºä½¿ç¨çæä»¶ç¼åæ¹å¼ï¼æ¨åªéè¦ç¼åä¸¤ä¸ªæ¹æ³å³å¯å®ç°ä¸ä¸ªåè½å¼ºå¤§çæä»¶ã
-AliceBot
+- **çµæ´»**ï¼AliceBot
 çééåè®®å¹¶ä¸ä¸ä»»ä½ä¸ç§åºæç½ç»åè®®ç»å®ï¼æ¨å¯ä»¥èªç±éæ©æç¼åéåæ¨çééå¨ã
+- **é«æ**ï¼AliceBot åºäº Python çå¼æ­¥ I/
+Oï¼è½»æ¾å¤çå¤§éè¯·æ±ãè¾å°çå°è£ï¼å¨ä¿ææç¨çåæ¶è¿½æ±æå¥½çæ§è½ã
 ç®å AliceBot å®æ¹ç»´æ¤äºä»¥ä¸åè®®ééï¼ - [OneBot (CQHTTP) åè®®]
-(https://github.com/botuniverse/onebot) ï¼æ¯æQQç­ï¼[ws](https://
+(https://github.com/botuniverse/onebot) ï¼æ¯æ QQ ç­ï¼[ws](https://
 github.com/botuniverse/onebot-11/blob/master/communication/ws.md) å [ws-
 reverse](https://github.com/botuniverse/onebot-11/blob/master/communication/ws-
 reverse.md) è¿æ¥æ¹å¼ - [mirai-api-http åè®®](https://github.com/project-
 mirai/mirai-api-http) 2.0+ [ws](https://github.com/project-mirai/mirai-api-
 http/blob/master/docs/adapter/WebsocketAdapter.md) å [reverse-ws](https://
 github.com/project-mirai/mirai-api-http/blob/master/docs/adapter/
 ReverseWebsocketAdapter.md) è¿æ¥æ¹å¼ - [éé](https://
 developers.dingtalk.com/document/robots/robot-overview) ä¼ä¸æºå¨äººç
-outgoing ï¼åè°ï¼è¿æ¥æ¹å¼ æ´å¤åè®®æ­£å¨ééä¸­ ... ##
+outgoing ï¼åè°ï¼è¿æ¥æ¹å¼ æ´å¤åè®®æ­£å¨ééä¸­ ...
+æ´å¤ä¿¡æ¯ï¼[ç®ä» - AliceBot ææ¡£](https://docs.alicebot.dev/guide/) ##
 å³å»å¼å§ 1. å®è£ï¼ ```bash pip install alicebot[all] ``` 2. ç¬¬ä¸ä¸ª
 AliceBot é¡¹ç®ï¼ ```python from alicebot import Bot bot = Bot()
 bot.load_adapters("alicebot.adapter.cqhttp") bot.run() ``` 3. ç¬¬ä¸ä¸ª
 AliceBot æä»¶ï¼ ```python from alicebot import Plugin class Echo(Plugin):
 async def handle(self) -> None: await self.event.reply
 (self.event.message.replace("echo ", "")) async def rule(self) -> bool: if
 self.event.adapter.name != "cqhttp": return False if self.event.type !=
 "message": return False return self.event.message.startswith("echo ") ```
 æ´å¤ä¿¡æ¯è¯·åé AliceBot [ææ¡£](https://docs.alicebot.dev/)ã ##
-å¯¹æ¯ æ¬é¡¹ç®åå°äº [NoneBot](https://github.com/nonebot/nonebot2/
-) é¡¹ç®çå¯åï¼ä»¥ä¸ç®åä»ç»ä¸¤èçå¼åã ç¸åç¹ï¼ -
+å¯¹æ¯ æ¬é¡¹ç®åå°äº [NoneBot](https://github.com/nonebot/nonebot2)
+é¡¹ç®çå¯åï¼ä»¥ä¸ç®åä»ç»ä¸¤èçå¼åã ç¸åç¹ï¼ -
 ä¸¤èé½æ¯ä½¿ç¨ Python
 ç¼åçï¼ä½¿ç¨äºåç¨å¼æ­¥çé«æ§è½æºå¨äººæ¡æ¶ã -
 ä¸¤èé½æ¯æå¤ç§åè®®ã -
 ä¸¤èé½ä¼å¯¹æºå¨äººæ¶å°çäºä»¶è¿è¡è§£æåå¤çï¼å¹¶æä¼åçº§ååç»æä»¶ï¼äºä»¶ååºå¨ï¼æ¥å®æå·ä½çåè½ã
 - ä¸¤èé½åºäº MIT
 åè®®å¼æºï¼è¿æå³çæ¨å¯ä»¥å¨éµå¾ªåè®®çåæä¸ä»»æä½¿ç¨æ¬é¡¹ç®ã
 ä¸åç¹ï¼ - æ»çæ¥è¯´ï¼NoneBot
 æ¯ä¸ä¸ªè¾ä¸ºå¨é¢çæºå¨äººæ¡æ¶ï¼è AliceBot
 æ¯ä¸ä¸ªå°å·§ç®æ´çæºå¨äººæ¡æ¶ï¼å®ä¸åå«ä¸äºå¤æçé«çº§ç¹æ§ï¼ä½æ´å çµæ´»ä¸æäºå­¦ä¹ ã
-- NoneBot å¨å®ç°ä¸ä¸ WebSocket
+- AliceBot çæä»¶ç¼åé£æ ¼å NoneBot ä¸åï¼ç¸å¯¹èè¨ï¼AliceBot
+æ´å æ³¨éäºæäºå¥é¨åâæ¸è¿å¼æ¡æ¶âï¼è¿æå³ç AliceBot
+å¤§é¨åçåè½é½æ¯å¯éçï¼æ¨åªéè¦äºè§£å¾å°çç¥è¯å³å¯å¼å§ä½¿ç¨ï¼éçé¡¹ç®è§æ¨¡çæ©å¤§åå¤ææ§çå¢å ï¼æ¨å¯ä»¥ç»§ç»­æ·±å¥éè¦çç¹æ§ï¼èä¸éè¦ä¸å¼å§å°±ææ¡å¨é¨çç¹æ§ãâå®æ¯ä¸ä¸ªå¯ä»¥ä¸ä½ å±åæé¿ãéåºä½ ä¸åéæ±çæ¡æ¶ãâ
+- NoneBot å¨å®ç°ä¸ä¸ HTTP / WebSocket
 éè®¯åè®®æ·±åº¦ç»å®ï¼å®éè¦ä¸ä¸ªæ¯æ ASGI
-æå¡å¨åè®®çé©±å¨æ¡æ¶ï¼è AliceBot
+æå¡å¨åè®®çâé©±å¨å¨âï¼è AliceBot
 å¹¶ä¸ä¸ä»»ä½åè®®ç»å®ï¼å®çè³å¯ä»¥ç¨æ¥é©±å¨æ¨çæ èæ´¾æºè½é³ç®±ãå½ç¶ï¼å¦ææ¨åªéè¦ä¸ä¸ªæ¯æå¸¸è§ç½ç»èå¤©å·¥å·çæºå¨äººæ¡æ¶çè¯ï¼å®ä»¬å¹¶æ²¡æä»ä¹åºå«ã
-- NoneBot æä¾äºå¾å¤é¢è®¾è§ååæéæ§å¶æºå¶ï¼è AliceBot
-åæ²¡ææä¾ï¼ç±äºæä»¶ç¼åæ¹å¼çä¸åï¼AliceBot
-éæ©ç»æ¨æå¤§çèªç±ï¼æ¨éè¦èªè¡ç¼åæä»¶å¨ä½æ¶è¿è¡çæ¹æ³ï¼`rule
-()`
-æ¹æ³ï¼ï¼è¿å¨ç»å¤§é¨ä»½æåµä¸å¹¶ä¸ä¼é ææ¨ç¼åæ´å¤çä»£ç ææ¯å½±åæä»¶çå¯è¯»æ§ï¼èªè¡å®ç°ä¹ä¸ä¼éå¸¸å°é¾ï¼ä½å¦ææ¨ççéè¦è¿äºé«çº§åè½åä¸æ³èªå·±å®ç°çè¯ï¼NoneBot
-æä¾äºæ´å¥½çéæ©ã - NoneBot
+- NoneBot
 æ¥æç¸å¯¹åºå¤§çç¨æ·åºæ°åç¤¾åºè§æ¨¡ï¼ä¹æ¥ææ°éä¼å¤çæä»¶ï¼è
 AliceBot åæ¯ä¸ä¸ªæ°çé¡¹ç®ï¼è¿æå³çå¦ææ¨ä½¿ç¨ NoneBot
 æ¨å¯è½ä¼æ´å å®¹ææ¾å°å·²ç»ç¼åå®æ¯çæ¨æå´è¶£çæä»¶ï¼å¹¶ä¸æ¨å½æ¨éå°é®é¢æ¶ä¹è½å¤æ´å¿«å°æ¥æ¾å°ç¸å³èµææèè·å¾è§£ç­ã
-- NoneBot
-ç¸å¯¹è¾ä¸ºåºå¤§ï¼å°è£ç¸å¯¹è¾å¤ï¼å®å¨å­¦ä¹ çè§£éè¦ä¸å®æ¶é´ï¼è
-AliceBot å°å·§ç®æ´ï¼å°è£è¾å°ï¼å¾å®¹æææ¡ã
-æ»èè¨ä¹ï¼ä¸¤èæçåèªçç¹ç¹ï¼æ¨å¯ä»¥æ ¹æ®éè¦éç¨ã
-ä½èå°±æ¯å¨ä½¿ç¨ NoneBot
-æ¶è§å¾æä»¶ç¼åä¸æ¯å¾æç¨ï¼äºæ¯èåäºç¼åä¸ä¸ªæ°çæºå¨äººæ¡æ¶çæ³æ³ï¼AliceBot
-å°±è¿æ ·è¯çäºã ## è®¸å¯è¯ AliceBot éç¨ MIT
-è®¸å¯è¯å¼æ¾æºä»£ç ã æ¬é¡¹ç®çå¾æ ç± è¿·ç³å°æ¢¦ç¥
+æ»èè¨ä¹ï¼ä¸¤èæçåèªçç¹ç¹ï¼æ¨å¯ä»¥æ ¹æ®éè¦éç¨ã ##
+è®¸å¯è¯ AliceBot éç¨ MIT è®¸å¯è¯å¼æ¾æºä»£ç ã æ¬é¡¹ç®çå¾æ ç±
+è¿·ç³å°æ¢¦ç¥
 ç»å¶ï¼ä½ä¸ºæ¬é¡¹ç®çä¸é¨åï¼ä½¿ç¨ä¸æ¬é¡¹ç®ç¸åçè®¸å¯è¯å¼æ¾ä½¿ç¨ã
```

