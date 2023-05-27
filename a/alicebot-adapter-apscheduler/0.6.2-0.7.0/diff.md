# Comparing `tmp/alicebot_adapter_apscheduler-0.6.2.tar.gz` & `tmp/alicebot_adapter_apscheduler-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot_adapter_apscheduler-0.6.2.tar", max compression
+gzip compressed data, was "alicebot_adapter_apscheduler-0.7.0.tar", max compression
```

## Comparing `alicebot_adapter_apscheduler-0.6.2.tar` & `alicebot_adapter_apscheduler-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      269 2023-04-25 11:14:36.277730 alicebot_adapter_apscheduler-0.6.2/README.md
--rw-r--r--   0        0        0     4787 2023-04-25 11:14:36.277730 alicebot_adapter_apscheduler-0.6.2/alicebot/adapter/apscheduler/__init__.py
--rw-r--r--   0        0        0      380 2023-04-25 11:14:36.277730 alicebot_adapter_apscheduler-0.6.2/alicebot/adapter/apscheduler/config.py
--rw-r--r--   0        0        0      972 2023-04-25 11:14:36.277730 alicebot_adapter_apscheduler-0.6.2/alicebot/adapter/apscheduler/event.py
--rw-r--r--   0        0        0     1365 2023-04-25 11:14:36.277730 alicebot_adapter_apscheduler-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1405 1970-01-01 00:00:00.000000 alicebot_adapter_apscheduler-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      269 2023-05-27 14:25:34.118713 alicebot_adapter_apscheduler-0.7.0/README.md
+-rw-r--r--   0        0        0     5033 2023-05-27 14:25:34.118713 alicebot_adapter_apscheduler-0.7.0/alicebot/adapter/apscheduler/__init__.py
+-rw-r--r--   0        0        0      380 2023-05-27 14:25:34.118713 alicebot_adapter_apscheduler-0.7.0/alicebot/adapter/apscheduler/config.py
+-rw-r--r--   0        0        0     1035 2023-05-27 14:25:34.118713 alicebot_adapter_apscheduler-0.7.0/alicebot/adapter/apscheduler/event.py
+-rw-r--r--   0        0        0     1099 2023-05-27 14:25:34.118713 alicebot_adapter_apscheduler-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 alicebot_adapter_apscheduler-0.7.0/PKG-INFO
```

### Comparing `alicebot_adapter_apscheduler-0.6.2/alicebot/adapter/apscheduler/__init__.py` & `alicebot_adapter_apscheduler-0.7.0/alicebot/adapter/apscheduler/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """APScheduler 适配器。
 
 本适配器用于实现定时任务，适配器将使用 APScheduler 实现定时任务，在设定的时间产生一个事件供插件处理。
 APScheduler 使用方法请参考: [APScheduler](https://apscheduler.readthedocs.io/) 。
 """
-import asyncio
-import inspect
 from functools import wraps
-from typing import Any, Dict, Type, Union, Callable, Awaitable
+import inspect
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, Dict, Type, Union
 
 from apscheduler.job import Job
-from apscheduler.triggers.base import BaseTrigger
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 
-from alicebot.plugin import Plugin
 from alicebot.adapter import Adapter
-from alicebot.log import logger, error_or_exception
+from alicebot.log import error_or_exception, logger
+from alicebot.plugin import Plugin
+from alicebot.typing import T_Plugin
 
 from .config import Config
 from .event import APSchedulerEvent
 
+if TYPE_CHECKING:
+    from apscheduler.triggers.base import BaseTrigger
+
 __all__ = ["APSchedulerAdapter", "scheduler_decorator"]
 
 
 class APSchedulerAdapter(Adapter[APSchedulerEvent, Config]):
+    """APScheduler 适配器。"""
+
     name: str = "apscheduler"
     Config = Config
 
     scheduler: AsyncIOScheduler
-    plugin_class_to_job: Dict[Type[Plugin], Job]
+    plugin_class_to_job: Dict[Type[Plugin[Any, Any, Any]], Job]
 
     async def startup(self):
-        """创建 AsyncIOScheduler 对象。"""
+        """创建 `AsyncIOScheduler` 对象。"""
         self.scheduler = AsyncIOScheduler(self.config.scheduler_config)
         self.plugin_class_to_job = {}
 
     async def run(self):
         """启动调度器。"""
         for plugin in self.bot.plugins:
             if not hasattr(plugin, "__schedule__"):
@@ -43,16 +47,18 @@
             if not hasattr(plugin, "trigger") or not hasattr(plugin, "trigger_args"):
                 logger.error(
                     f"Plugin {plugin.__name__} __schedule__ is True, "
                     f"but did not set trigger or trigger_args"
                 )
                 continue
 
-            trigger: Union[str, BaseTrigger] = getattr(plugin, "trigger")
-            trigger_args: Dict[str, Any] = getattr(plugin, "trigger_args")
+            trigger: Union[str, "BaseTrigger"] = getattr(  # noqa: B009
+                plugin, "trigger"
+            )
+            trigger_args: Dict[str, Any] = getattr(plugin, "trigger_args")  # noqa: B009
 
             if not isinstance(trigger, str) or not isinstance(trigger_args, dict):
                 logger.error(
                     f"Plugin {plugin.__name__} trigger or trigger_args type error"
                 )
                 continue
 
@@ -72,66 +78,65 @@
 
         self.scheduler.start()
 
     async def shutdown(self):
         """关闭调度器。"""
         self.scheduler.shutdown()
 
-    async def create_event(self, plugin_class: Type[Plugin]):
-        """创建 APSchedulerEvent 事件。
+    async def create_event(self, plugin_class: Type[Plugin[Any, Any, Any]]):
+        """创建 `APSchedulerEvent` 事件。
 
         Args:
-            plugin_class: Plugin 类。
+            plugin_class: `Plugin` 类。
         """
         logger.info(f"APSchedulerEvent set by {plugin_class} is created as scheduled")
-        asyncio.create_task(
-            self.bot.handle_event(
-                APSchedulerEvent(
-                    adapter=self, type="apscheduler", plugin_class=plugin_class
-                ),
-                handle_get=False,
-                show_log=False,
-            )
+        await self.handle_event(
+            APSchedulerEvent(
+                adapter=self, type="apscheduler", plugin_class=plugin_class
+            ),
+            handle_get=False,
+            show_log=False,
         )
 
-    async def send(self, *args: Any, **kwargs: Any):
+    async def send(self, *args: Any, **kwargs: Any) -> Any:
+        """APScheduler 适配器不适用发送消息。"""
         raise NotImplementedError
 
 
 def scheduler_decorator(
     trigger: str, trigger_args: Dict[str, Any], override_rule: bool = False
 ):
     """用于为插件类添加计划任务功能的装饰器。
 
     Args:
         trigger: APScheduler 触发器。
         trigger_args: APScheduler 触发器参数。
-        override_rule: 是否重写 rule() 方法，若为 True ，则会在 rule() 方法中添加处理本插件定义的计划任务事件的逻辑。
+        override_rule: 是否重写 `rule()` 方法。
+            若为 `True`，则会在 `rule()` 方法中添加处理本插件定义的计划任务事件的逻辑。
     """
 
-    def _decorator(cls: Type[Plugin]):
+    def _decorator(cls: Type[T_Plugin]) -> Type[T_Plugin]:
         if not inspect.isclass(cls):
-            raise TypeError(f"can only decorate class")
+            raise TypeError("can only decorate class")
         if not issubclass(cls, Plugin):
-            raise TypeError(f"can only decorate Plugin class")
-        setattr(cls, "__schedule__", True)
-        setattr(cls, "trigger", trigger)
-        setattr(cls, "trigger_args", trigger_args)
+            raise TypeError("can only decorate Plugin class")
+        setattr(cls, "__schedule__", True)  # noqa: B010
+        setattr(cls, "trigger", trigger)  # noqa: B010
+        setattr(cls, "trigger_args", trigger_args)  # noqa: B010
         if override_rule:
 
-            def _rule_decorator(func: Callable[[Plugin], Awaitable[bool]]):
+            def _rule_decorator(func: Callable[[T_Plugin], Awaitable[bool]]):
                 @wraps(func)
-                async def _wrapper(self: Plugin):
+                async def _wrapper(self: T_Plugin):
                     if (
                         self.event.type == "apscheduler"
                         and type(self) == self.event.plugin_class
                     ):
                         return True
-                    else:
-                        return await func(self)
+                    return await func(self)
 
                 return _wrapper
 
             cls.rule = _rule_decorator(cls.rule)
         return cls
 
     return _decorator
```

### Comparing `alicebot_adapter_apscheduler-0.6.2/alicebot/adapter/apscheduler/event.py` & `alicebot_adapter_apscheduler-0.7.0/alicebot/adapter/apscheduler/event.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from alicebot.event import Event
 from alicebot.plugin import Plugin
 
 if TYPE_CHECKING:
     from apscheduler.job import Job
     from apscheduler.triggers.base import BaseTrigger
 
-    from . import APSchedulerAdapter
+    from . import APSchedulerAdapter  # noqa: F401
 
 
 class APSchedulerEvent(Event["APSchedulerAdapter"]):
     """APSchedulerEvent 事件基类。"""
 
-    plugin_class: Type[Plugin]
+    plugin_class: Type[Plugin[Any, Any, Any]]
 
     @property
     def job(self) -> "Job":
-        """产生当前事件的 APScheduler Job 对象。"""
+        """产生当前事件的 APScheduler `Job` 对象。"""
         return self.adapter.plugin_class_to_job[self.plugin_class]
 
     @property
     def trigger(self) -> Union[str, "BaseTrigger"]:
-        """当前事件对应的 Plugin 的 trigger。"""
-        return getattr(self.plugin_class, "trigger")
+        """当前事件对应的 Plugin 的 `trigger`。"""
+        return getattr(self.plugin_class, "trigger")  # noqa: B009
 
     @property
     def trigger_args(self) -> Dict[str, Any]:
-        """当前事件对应的 Plugin 的 trigger_args。"""
-        return getattr(self.plugin_class, "trigger_args")
+        """当前事件对应的 Plugin 的 `trigger_args`。"""
+        return getattr(self.plugin_class, "trigger_args")  # noqa: B009
```

### Comparing `alicebot_adapter_apscheduler-0.6.2/PKG-INFO` & `alicebot_adapter_apscheduler-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot-adapter-apscheduler
-Version: 0.6.2
+Version: 0.7.0
 Summary: APScheduler adapter for AliceBot.
 Home-page: https://docs.alicebot.dev/
 License: MIT
 Keywords: bot,chatbot,scheduling,apscheduler
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
 Requires-Dist: apscheduler (>=3.7,<4.0)
 Project-URL: Documentation, https://docs.alicebot.dev/
 Project-URL: Repository, https://github.com/AliceBotProject/alicebot
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/AliceBotProject/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: alicebot-adapter-apscheduler Version: 0.6.2
+Metadata-Version: 2.1 Name: alicebot-adapter-apscheduler Version: 0.7.0
 Summary: APScheduler adapter for AliceBot. Home-page: https://
 docs.alicebot.dev/ License: MIT Keywords: bot,chatbot,scheduling,apscheduler
 Author: st1020 Author-email: stone_1020@qq.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: Framework :: AsyncIO
 Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
 Framework :: Library Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Classifier: Topic :: Communications :: Chat
-Requires-Dist: alicebot (==0.6.2) Requires-Dist: apscheduler (>=3.7,<4.0)
-Project-URL: Documentation, https://docs.alicebot.dev/ Project-URL: Repository,
-https://github.com/AliceBotProject/alicebot Description-Content-Type: text/
-markdown
+Topic :: Communications :: Chat Requires-Dist: alicebot (==0.7.0) Requires-
+Dist: apscheduler (>=3.7,<4.0) Project-URL: Documentation, https://
+docs.alicebot.dev/ Project-URL: Repository, https://github.com/AliceBotProject/
+alicebot Description-Content-Type: text/markdown
       [logo] # AliceBot-Adapter-APScheduler **APScheduler å®æ¶ä»»å¡**
```

