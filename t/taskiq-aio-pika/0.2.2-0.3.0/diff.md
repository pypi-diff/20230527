# Comparing `tmp/taskiq_aio_pika-0.2.2.tar.gz` & `tmp/taskiq_aio_pika-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aio_pika-0.2.2.tar", max compression
+gzip compressed data, was "taskiq_aio_pika-0.3.0.tar", max compression
```

## Comparing `taskiq_aio_pika-0.2.2.tar` & `taskiq_aio_pika-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4517 2023-05-21 16:19:07.936297 taskiq_aio_pika-0.2.2/README.md
--rw-r--r--   0        0        0     1536 2023-05-21 16:19:07.936297 taskiq_aio_pika-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      118 2023-05-21 16:19:07.936297 taskiq_aio_pika-0.2.2/taskiq_aio_pika/__init__.py
--rw-r--r--   0        0        0    10305 2023-05-21 16:19:07.936297 taskiq_aio_pika-0.2.2/taskiq_aio_pika/broker.py
--rw-r--r--   0        0        0     5384 1970-01-01 00:00:00.000000 taskiq_aio_pika-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4517 2023-05-27 12:57:45.638355 taskiq_aio_pika-0.3.0/README.md
+-rw-r--r--   0        0        0     1603 2023-05-27 12:57:45.642355 taskiq_aio_pika-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      347 2023-05-27 12:57:45.642355 taskiq_aio_pika-0.3.0/taskiq_aio_pika/__init__.py
+-rw-r--r--   0        0        0    10340 2023-05-27 12:57:45.642355 taskiq_aio_pika-0.3.0/taskiq_aio_pika/broker.py
+-rw-r--r--   0        0        0     5464 1970-01-01 00:00:00.000000 taskiq_aio_pika-0.3.0/PKG-INFO
```

### Comparing `taskiq_aio_pika-0.2.2/README.md` & `taskiq_aio_pika-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_aio_pika-0.2.2/pyproject.toml` & `taskiq_aio_pika-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-aio-pika"
-version = "0.2.2"
+version = "0.3.0"
 description = "RabbitMQ broker for taskiq"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -16,16 +16,17 @@
 ]
 homepage = "https://github.com/taskiq-python/taskiq-aio-pika"
 repository = "https://github.com/taskiq-python/taskiq-aio-pika"
 keywords = ["taskiq", "tasks", "distributed", "async", "aio-pika"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-taskiq = "^0"
+taskiq = ">=0.6.0,<1"
 aio-pika = "^9.0"
+importlib-metadata = {version = "^4.0.0", python = "<3.8"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 isort = "^5.10.1"
 mypy = "^0.971"
 black = "^22.6.0"
 flake8 = "^4"
```

### Comparing `taskiq_aio_pika-0.2.2/taskiq_aio_pika/broker.py` & `taskiq_aio_pika-0.3.0/taskiq_aio_pika/broker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import asyncio
 from datetime import timedelta
 from logging import getLogger
 from typing import Any, AsyncGenerator, Callable, Dict, Optional, TypeVar
 
 from aio_pika import DeliveryMode, ExchangeType, Message, connect_robust
 from aio_pika.abc import AbstractChannel, AbstractQueue, AbstractRobustConnection
-from taskiq.abc.broker import AsyncBroker
-from taskiq.abc.result_backend import AsyncResultBackend
-from taskiq.message import BrokerMessage
+from taskiq import AckableMessage, AsyncBroker, AsyncResultBackend, BrokerMessage
 
 _T = TypeVar("_T")  # noqa: WPS111
 
 logger = getLogger("taskiq.aio_pika_broker")
 
 
 def parse_val(
@@ -224,29 +222,28 @@
 
         :raises ValueError: if startup wasn't called.
         :param message: message to send.
         """
         if self.write_channel is None:
             raise ValueError("Please run startup before kicking.")
 
-        message_base_params: dict[str, Any] = {
+        message_base_params: Dict[str, Any] = {
             "body": message.message,
             "headers": {
                 "task_id": message.task_id,
                 "task_name": message.task_name,
                 **message.labels,
             },
             "delivery_mode": DeliveryMode.PERSISTENT,
+            "priority": parse_val(
+                int,
+                message.labels.get("priority"),
+            ),
         }
 
-        message_base_params["priority"] = parse_val(
-            int,
-            message.labels.get("priority"),
-        )
-
         delay: Optional[int] = parse_val(int, message.labels.get("delay"))
         rmq_message: Message = Message(**message_base_params)
 
         if delay is None:
             exchange = await self.write_channel.get_exchange(
                 self._exchange_name,
                 ensure=False,
@@ -264,15 +261,15 @@
         else:
             rmq_message.expiration = timedelta(seconds=delay)
             await self.write_channel.default_exchange.publish(
                 rmq_message,
                 routing_key=self._delay_queue_name,
             )
 
-    async def listen(self) -> AsyncGenerator[bytes, None]:
+    async def listen(self) -> AsyncGenerator[AckableMessage, None]:
         """
         Listen to queue.
 
         This function listens to queue and
         yields every new message.
 
         :yields: parsed broker message.
@@ -280,9 +277,12 @@
         """
         if self.read_channel is None:
             raise ValueError("Call startup before starting listening.")
         await self.read_channel.set_qos(prefetch_count=self._qos)
         queue = await self.declare_queues(self.read_channel)
         async with queue.iterator() as iterator:
             async for message in iterator:
-                async with message.process():
-                    yield message.body
+                yield AckableMessage(
+                    data=message.body,
+                    ack=message.ack,
+                    reject=message.reject,
+                )
```

### Comparing `taskiq_aio_pika-0.2.2/PKG-INFO` & `taskiq_aio_pika-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-aio-pika
-Version: 0.2.2
+Version: 0.3.0
 Summary: RabbitMQ broker for taskiq
 Home-page: https://github.com/taskiq-python/taskiq-aio-pika
 Keywords: taskiq,tasks,distributed,async,aio-pika
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python
@@ -12,15 +12,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: aio-pika (>=9.0,<10.0)
-Requires-Dist: taskiq (>=0,<1)
+Requires-Dist: importlib-metadata (>=4.0.0,<5.0.0) ; python_version < "3.8"
+Requires-Dist: taskiq (>=0.6.0,<1)
 Project-URL: Repository, https://github.com/taskiq-python/taskiq-aio-pika
 Description-Content-Type: text/markdown
 
 # AioPika broker for taskiq
 
 This lirary provides you with aio-pika broker for taskiq.
```

