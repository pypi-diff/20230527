# Comparing `tmp/async_dramatiq-0.1.7.tar.gz` & `tmp/async_dramatiq-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_dramatiq-0.1.7.tar", max compression
+gzip compressed data, was "async_dramatiq-0.1.8.tar", max compression
```

## Comparing `async_dramatiq-0.1.7.tar` & `async_dramatiq-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1065 2023-05-26 08:26:10.164949 async_dramatiq-0.1.7/LICENSE
--rw-r--r--   0        0        0     2936 2023-05-27 01:25:25.985962 async_dramatiq-0.1.7/README.md
--rw-r--r--   0        0        0     3506 2023-05-27 01:27:35.394466 async_dramatiq-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      254 2023-05-27 01:25:25.990049 async_dramatiq-0.1.7/src/async_dramatiq/__init__.py
--rw-r--r--   0        0        0     3182 2023-05-27 01:25:25.990257 async_dramatiq-0.1.7/src/async_dramatiq/actors.py
--rw-r--r--   0        0        0      491 2023-05-26 07:37:33.566566 async_dramatiq-0.1.7/src/async_dramatiq/backends/__init__.py
--rw-r--r--   0        0        0     1700 2023-05-27 01:25:25.990467 async_dramatiq-0.1.7/src/async_dramatiq/backends/async_redis.py
--rw-r--r--   0        0        0     1758 2023-05-26 07:37:33.566814 async_dramatiq-0.1.7/src/async_dramatiq/backends/async_stub.py
--rw-r--r--   0        0        0      112 2023-05-26 07:37:33.566965 async_dramatiq-0.1.7/src/async_dramatiq/middleware/__init__.py
--rw-r--r--   0        0        0      934 2023-05-27 01:25:25.990649 async_dramatiq-0.1.7/src/async_dramatiq/middleware/async_base.py
--rw-r--r--   0        0        0     1159 2023-05-27 01:25:25.990830 async_dramatiq-0.1.7/src/async_dramatiq/middleware/async_stub.py
--rw-r--r--   0        0        0     1416 2023-05-27 01:25:25.991007 async_dramatiq-0.1.7/src/async_dramatiq/scheduler.py
--rw-r--r--   0        0        0      485 2023-05-27 01:25:25.991283 async_dramatiq-0.1.7/src/async_dramatiq/types.py
--rw-r--r--   0        0        0     1232 2023-05-27 01:25:25.991465 async_dramatiq-0.1.7/src/async_dramatiq/worker.py
--rw-r--r--   0        0        0        0 2023-05-26 08:26:10.167650 async_dramatiq-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     1471 2023-05-26 08:26:10.167926 async_dramatiq-0.1.7/tests/conftest.py
--rw-r--r--   0        0        0     3812 2023-05-26 09:10:55.772756 async_dramatiq-0.1.7/tests/test_actors.py
--rw-r--r--   0        0        0     2563 2023-05-26 08:26:10.168282 async_dramatiq-0.1.7/tests/test_backends.py
--rw-r--r--   0        0        0     1024 2023-05-26 08:26:10.168435 async_dramatiq-0.1.7/tests/test_scheduler.py
--rw-r--r--   0        0        0      595 2023-05-26 08:26:10.168609 async_dramatiq-0.1.7/tests/test_workers.py
--rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 async_dramatiq-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-26 08:26:10.164949 async_dramatiq-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3296 2023-05-27 09:00:42.102545 async_dramatiq-0.1.8/README.md
+-rw-r--r--   0        0        0     3507 2023-05-27 09:00:42.105202 async_dramatiq-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-05-27 09:00:42.105490 async_dramatiq-0.1.8/src/async_dramatiq/__init__.py
+-rw-r--r--   0        0        0     3161 2023-05-27 09:00:42.105655 async_dramatiq-0.1.8/src/async_dramatiq/actor.py
+-rw-r--r--   0        0        0      491 2023-05-26 07:37:33.566566 async_dramatiq-0.1.8/src/async_dramatiq/backends/__init__.py
+-rw-r--r--   0        0        0     1700 2023-05-27 02:24:09.186989 async_dramatiq-0.1.8/src/async_dramatiq/backends/async_redis.py
+-rw-r--r--   0        0        0     1758 2023-05-26 07:37:33.566814 async_dramatiq-0.1.8/src/async_dramatiq/backends/async_stub.py
+-rw-r--r--   0        0        0      112 2023-05-26 07:37:33.566965 async_dramatiq-0.1.8/src/async_dramatiq/middleware/__init__.py
+-rw-r--r--   0        0        0      934 2023-05-27 02:24:09.187202 async_dramatiq-0.1.8/src/async_dramatiq/middleware/async_base.py
+-rw-r--r--   0        0        0     1159 2023-05-27 02:24:09.187430 async_dramatiq-0.1.8/src/async_dramatiq/middleware/async_stub.py
+-rw-r--r--   0        0        0     1416 2023-05-27 02:24:09.187850 async_dramatiq-0.1.8/src/async_dramatiq/scheduler.py
+-rw-r--r--   0        0        0      485 2023-05-27 02:24:09.188053 async_dramatiq-0.1.8/src/async_dramatiq/types.py
+-rw-r--r--   0        0        0     1196 2023-05-27 09:00:42.105843 async_dramatiq-0.1.8/src/async_dramatiq/worker.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:26:10.167650 async_dramatiq-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0     1471 2023-05-26 08:26:10.167926 async_dramatiq-0.1.8/tests/conftest.py
+-rw-r--r--   0        0        0     3705 2023-05-27 09:00:42.106036 async_dramatiq-0.1.8/tests/test_actors.py
+-rw-r--r--   0        0        0     2819 2023-05-27 09:00:42.106249 async_dramatiq-0.1.8/tests/test_backends.py
+-rw-r--r--   0        0        0     1024 2023-05-26 08:26:10.168435 async_dramatiq-0.1.8/tests/test_scheduler.py
+-rw-r--r--   0        0        0      595 2023-05-26 08:26:10.168609 async_dramatiq-0.1.8/tests/test_workers.py
+-rw-r--r--   0        0        0     3928 1970-01-01 00:00:00.000000 async_dramatiq-0.1.8/PKG-INFO
```

### Comparing `async_dramatiq-0.1.7/LICENSE` & `async_dramatiq-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.7/README.md` & `async_dramatiq-0.1.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,52 @@
-# Dramatiq with Asyncio
-[Dramatiq](https://dramatiq.io/) is a background task processing library for Python with a focus on simplicity, reliability and performance.
+# Quick Start
+## Background
+[Dramatiq](https://dramatiq.io/) is a background task-processing library for Python with a focus on simplicity, reliability and performance.
 
-This package extends dramatiq to provide the following:
+This package, [async-dramatiq](https://pypi.org/project/async-dramatiq/), extends Dramatiq to provide the following:
   1. Support for Asyncio ( [issue #238](https://github.com/Bogdanp/dramatiq/issues/238) )
   2. Message scheduling support ( [scheduling cookbook](https://dramatiq.io/cookbook.html#scheduling-messages) )
 
-### Getting Started
-The quickest way to get started is by playing around with the [worker heartbeat example](examples/worker_heartbeat/README.md).
-
-# The Code
-## Async Middleware
-### Broker
+## Setup
 To provide async support for your actors all you need to do is add the `AsyncMiddleware` to your broker.
 #### RabbitMQ Broker
 
 ```
 import dramatiq
-
 from dramatiq.brokers.rabbitmq import RabbitmqBroker
 
-
 rabbitmq_broker = RabbitmqBroker(host="rabbitmq")
 rabbitmq_broker.add_middleware(AsyncMiddleware())  # <--- Here
 dramatiq.set_broker(rabbitmq_broker)
 ```
 
 #### Redis Broker
 
 ```
 import dramatiq
-import dramatiq
-
 from dramatiq.brokers.redis import RedisBroker
 
-
 redis_broker = RedisBroker(host="redis")
 redis_broker.add_middleware(AsyncMiddleware()) # <--- Here
 dramatiq.set_broker(redis_broker)
 ```
 
+## Running
+#### The Scheduler
+We leverage [apscheduler](https://pypi.org/project/APScheduler/) as our scheduling system. Check out [run_scheduler.py](examples/worker_heartbeat/run_scheduler.py) for an example of running this scheduler.
+#### Dramatiq Worker
+For more details check out the official guide to [dramatiq](https://dramatiq.io/guide.html#workers) or [docker-compose.yaml](examples/worker_heartbeat/docker-compose.yaml) for a specific example.
+
+
+## Example
+Play around with [worker-heartbeat-example](examples/worker_heartbeat/README.md). A functioning and featured example implementation.
+
+----
+# Async Middleware
+`AsyncMiddleware` will start a `AsyncWorker` which will be used to run the event loop. This event loop will be shared across the Worker threads. 
 ### Startup and Shutdown Events
 To startup and shutdown any resources the `AsyncMiddleware` provides two hooks:
 1. Before the event loop is started
 2. After the event loop is stopped
 To allow for standing up or tearing down of shared async resources
 #### Example
 ```
@@ -66,32 +70,26 @@
     def after_async_worker_thread_shutdown(
         self, _: RabbitmqBroker, thread: AsyncWorker, **kwargs: dict[str, Any]
     ) -> None:
         thread.event_loop.run_until_complete(shutdown())
         thread.event_loop.close()
 ```
 
-## Async Actor
-The async actor, `async_dramatiq_actor`,  acts as a thin wrapper around the dramatiq actor providing a variety of new functionality.
+# Async Actor
+The async actor, `async_actor`,  acts as a thin wrapper around the Dramatiq actor providing a variety of new functionality.
 
-#### Interval Jobs
+## Interval Jobs
 Run a job at some interval
 ```
-@async_dramatiq_actor(interval=timedelta(seconds=5))
+@async_actor(interval=timedelta(seconds=5))
 def run_every_5_seconds() -> None:
     pass
 ```
 
-#### Cron Jobs
+## Cron Jobs
 Run a job on a crontab ( See https://crontab.guru/. )
 ```
-@async_dramatiq_actor(interval="0 0 * * *")
+@async_actor(interval="0 0 * * *")
 def run_at_midnight() -> None:
   pass
 ```
 
-## Running
-### The Scheduler
-Checkout [run_scheduler.py](examples/worker_heartbeat/run_scheduler.py) for an example on running the scheduler.
-### Dramatiq Worker
-Check out the offical guide [dramatiq](https://dramatiq.io/guide.html#workers)
-
```

### Comparing `async_dramatiq-0.1.7/pyproject.toml` & `async_dramatiq-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "async_dramatiq"
-version = "0.1.7"
+version = "0.1.8"
 description = "Dramatiq with Asyncio support and some other goodies"
 authors = ["Ryan Houlihan <ryan@rhoulihan.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{ include = "async_dramatiq", from = "src" }]
 include = [{ path = "tests", format = "sdist" }]
 homepage = "https://github.com/motherofcoconuts/async-dramatiq"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/motherofcoconuts/async-dramatiq/issues"
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = "^3.10.1"
 dramatiq = { extras = ["redis", "rabbitmq", "watch"], version = "*"}
 apscheduler = "*"
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.3.0"
 flake8 = "^6.0.0"
 black = "^23.3.0"
@@ -110,15 +110,15 @@
 make_whitelist = true
 min_confidence = 80
 paths = ["async_dramatiq"]
 sort_by_size = true
 verbose = false
 
 [tool.mypy]
-python_version = "^3.8"
+python_version = "3.10"
 ignore_missing_imports = true
 scripts_are_modules = true
 implicit_reexport = true
 
 check_untyped_defs = true
 warn_unused_ignores = true 
 warn_return_any = true
```

### Comparing `async_dramatiq-0.1.7/src/async_dramatiq/actors.py` & `async_dramatiq-0.1.8/src/async_dramatiq/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 # Standard Library Imports
 import asyncio
 import inspect
 from datetime import timedelta
 from typing import Any, Callable
 
 import dramatiq as dq
@@ -14,15 +12,15 @@
 
 class AsyncActor(dq.Actor):
     def __init__(self, *args: Any, **kwargs: dict[str, Any]) -> None:
         super().__init__(*args, **kwargs)
         self.event_loop: asyncio.BaseEventLoop | None = None
 
     def __call__(self, *args: Any, **kwargs: dict[str, Any]) -> Any:
-        """Synchronously call this actor.
+        """Call this function apropriately depending on its type.
 
         :param *args: Positional arguments to send to the actor.
         :param **kwargs: Keyword arguments to send to the actor.
 
         :return: Whatever the underlying function backing this actor returns.
         """
         try:
@@ -47,15 +45,15 @@
 
         return result
 
     def set_event_loop(self, loop: asyncio.BaseEventLoop | None) -> None:
         self.event_loop = loop
 
 
-def async_dramatiq_actor(
+def async_actor(
     *,
     interval: timedelta | None = None,
     crontab: str | None = None,
     priority: DramatiqWorkerPriority = DramatiqWorkerPriority.MEDIUM,
     actor_class: type[AsyncActor] = AsyncActor,
     queue_name: str = "default",
     **kwargs: Any,
```

### Comparing `async_dramatiq-0.1.7/src/async_dramatiq/backends/async_redis.py` & `async_dramatiq-0.1.8/src/async_dramatiq/backends/async_redis.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.7/src/async_dramatiq/backends/async_stub.py` & `async_dramatiq-0.1.8/src/async_dramatiq/backends/async_stub.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.7/src/async_dramatiq/middleware/async_base.py` & `async_dramatiq-0.1.8/src/async_dramatiq/middleware/async_base.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.7/src/async_dramatiq/middleware/async_stub.py` & `async_dramatiq-0.1.8/src/async_dramatiq/middleware/async_stub.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.7/src/async_dramatiq/scheduler.py` & `async_dramatiq-0.1.8/src/async_dramatiq/scheduler.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.7/src/async_dramatiq/worker.py` & `async_dramatiq-0.1.8/src/async_dramatiq/worker.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 # Standard Library Imports
 import asyncio
 from threading import Event, Thread
 
 import dramatiq as dq
```

### Comparing `async_dramatiq-0.1.7/tests/conftest.py` & `async_dramatiq-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.7/tests/test_actors.py` & `async_dramatiq-0.1.8/tests/test_actors.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 
 import pytest
 from apscheduler.triggers.cron import CronTrigger
 from apscheduler.triggers.interval import IntervalTrigger
 from dramatiq import Worker
 
 # Local Application Imports
-from async_dramatiq.actors import async_dramatiq_actor
+from async_dramatiq.actor import async_actor
 from async_dramatiq.backends import AsyncStubBackend, get_backend
 from async_dramatiq.scheduler import scheduled_jobs
 
 F = TypeVar("F", bound=Callable[..., Any])
 
-def test_async_dramatiq_actor() -> None:
+
+def test_async_actor() -> None:
     scheduled_jobs_len = len(scheduled_jobs)
 
-    @async_dramatiq_actor(interval=timedelta(seconds=5))
+    @async_actor(interval=timedelta(seconds=5))
     def test_interval():
         return None
 
-    @async_dramatiq_actor(crontab="* * * * *")
+    @async_actor(crontab="* * * * *")
     def test_cron():
         return None
 
-    @async_dramatiq_actor()
+    @async_actor()
     async def test_async():
         return None
 
     assert len(scheduled_jobs) == scheduled_jobs_len + 2
     assert isinstance(scheduled_jobs[-1].trigger, CronTrigger)
     assert scheduled_jobs[-1].module_path, test_cron.__module__
     assert scheduled_jobs[-1].func_name, test_cron.__name__
@@ -39,39 +40,40 @@
     assert scheduled_jobs[-2].module_path, test_interval.__module__
     assert scheduled_jobs[-2].func_name, test_interval.__name__
 
 
 async def test_async_actor_func(event_loop: asyncio.BaseEventLoop) -> None:
     result = "generic result"
 
-    @async_dramatiq_actor()
+    @async_actor()
     async def test_async():
         return result
 
     # Test generic run
     assert result == await test_async()
 
+
 def test_async_actor_func_no_loop() -> None:
     result = "generic result"
 
-    @async_dramatiq_actor()
+    @async_actor()
     async def test_async():
         return result
 
     # Test generic run
     with pytest.raises(RuntimeError):
         test_async()
 
 
 async def test_async_actor_func_in_thread(
     worker: Worker, async_stub_backend: AsyncStubBackend
 ) -> None:
     result = "generic result"
 
-    @async_dramatiq_actor(store_results=True)
+    @async_actor(store_results=True)
     async def test_async():
         return result
 
     # Setup actor event loop
     loop = (w.event_loop for w in worker.workers if hasattr(w, "event_loop"))
     test_async.event_loop = next(loop, None)
 
@@ -82,37 +84,37 @@
     return_result = await get_backend().get_result(msg, block=True)
     assert return_result == result
 
 
 async def test_sync_actor_func() -> None:
     result = "generic result"
 
-    @async_dramatiq_actor()
+    @async_actor()
     def test_sync():
         return result
 
     assert result == test_sync()
 
 
 def test_sync_actor_func_no_loop() -> None:
     result = "generic result"
 
-    @async_dramatiq_actor()
+    @async_actor()
     def test_sync():
         return result
 
     assert result == test_sync()
 
 
 async def test_sync_actor_func_in_thread(
     worker: Worker, async_stub_backend: AsyncStubBackend
 ) -> None:
     result = "generic result"
 
-    @async_dramatiq_actor(store_results=True)
+    @async_actor(store_results=True)
     def test_async():
         return result
 
     # Send actor to worker
     msg = test_async.send()
     worker.join()
 
@@ -120,15 +122,15 @@
 
     assert return_result == result
 
 
 async def test_async_request(
     worker: Worker, async_stub_backend: AsyncStubBackend
 ) -> None:
-    @async_dramatiq_actor(store_results=True)
+    @async_actor(store_results=True)
     async def test_async():
         await asyncio.sleep(0.25)
         return True
 
     # Setup actor event loop
     loop = (w.event_loop for w in worker.workers if hasattr(w, "event_loop"))
     test_async.event_loop = next(loop, None)
```

### Comparing `async_dramatiq-0.1.7/tests/test_backends.py` & `async_dramatiq-0.1.8/tests/test_backends.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # Standard Library Imports
+import os
 import time
 from threading import Thread
 
 import pytest
 from dramatiq import Message
 from dramatiq.actor import actor
 from dramatiq.results.backend import ResultMissing, ResultTimeout
 
 # Local Application Imports
 from async_dramatiq.backends import AsyncRedisBackend, AsyncStubBackend, set_backend
 
+REDIS_HOST = os.getenv("REDIS_HOST", "localhost")
+REDIS_PORT = os.getenv("REDIS_PORT", 6379)
+
 
 def get_message() -> Message:
     @actor(queue_name="test_queue", store_results=True)
     def my_func():
         pass
 
     return my_func.message()
@@ -32,40 +36,46 @@
 def delayed_store(
     backend: AsyncRedisBackend | AsyncStubBackend, msg: Message, result: str, ttl: int
 ) -> None:
     time.sleep(0.1)
     backend.store_result(message=msg, result=result, ttl=ttl)
 
 
-@pytest.mark.parametrize("backend", [AsyncRedisBackend(), AsyncStubBackend()])
+@pytest.mark.parametrize(
+    "backend", [AsyncRedisBackend(host=REDIS_HOST, port=REDIS_PORT), AsyncStubBackend()]
+)
 async def test_get_result_happy_path(
     backend: AsyncRedisBackend | AsyncStubBackend,
 ) -> None:
     set_backend(backend)
 
     msg = get_message()
     result = "this is a result"
     backend.store_result(message=msg, result=result, ttl=100000)
     returned_result = await backend.get_result(msg)
     assert returned_result == result
 
 
-@pytest.mark.parametrize("backend", [AsyncRedisBackend(), AsyncStubBackend()])
+@pytest.mark.parametrize(
+    "backend", [AsyncRedisBackend(host=REDIS_HOST, port=REDIS_PORT), AsyncStubBackend()]
+)
 async def test_get_result_result_missing(
     backend: AsyncRedisBackend | AsyncStubBackend,
 ) -> None:
     set_backend(backend)
 
     msg = get_message()
 
     with pytest.raises(ResultMissing):
         await backend.get_result(msg)
 
 
-@pytest.mark.parametrize("backend", [AsyncRedisBackend(), AsyncStubBackend()])
+@pytest.mark.parametrize(
+    "backend", [AsyncRedisBackend(host=REDIS_HOST, port=REDIS_PORT), AsyncStubBackend()]
+)
 async def test_get_result_blocking_happy_path(
     backend: AsyncRedisBackend | AsyncStubBackend,
 ) -> None:
     set_backend(backend)
 
     msg = get_message()
     result = "this is a result"
@@ -74,15 +84,17 @@
     t1.start()
 
     await assert_result(backend, msg, result)
 
     t1.join()
 
 
-@pytest.mark.parametrize("backend", [AsyncRedisBackend(), AsyncStubBackend()])
+@pytest.mark.parametrize(
+    "backend", [AsyncRedisBackend(host=REDIS_HOST, port=REDIS_PORT), AsyncStubBackend()]
+)
 async def test_get_result_blocking_timeout(
     backend: AsyncRedisBackend | AsyncStubBackend,
 ) -> None:
     set_backend(backend)
 
     msg = get_message()
     result = "this is a result"
```

### Comparing `async_dramatiq-0.1.7/tests/test_scheduler.py` & `async_dramatiq-0.1.8/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.7/tests/test_workers.py` & `async_dramatiq-0.1.8/tests/test_workers.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.7/PKG-INFO` & `async_dramatiq-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 Metadata-Version: 2.1
 Name: async-dramatiq
-Version: 0.1.7
+Version: 0.1.8
 Summary: Dramatiq with Asyncio support and some other goodies
 Home-page: https://github.com/motherofcoconuts/async-dramatiq
 License: MIT
 Author: Ryan Houlihan
 Author-email: ryan@rhoulihan.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.10.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: apscheduler
 Requires-Dist: dramatiq[rabbitmq,redis,watch]
 Project-URL: Bug Tracker, https://github.com/motherofcoconuts/async-dramatiq/issues
 Description-Content-Type: text/markdown
 
-# Dramatiq with Asyncio
-[Dramatiq](https://dramatiq.io/) is a background task processing library for Python with a focus on simplicity, reliability and performance.
+# Quick Start
+## Background
+[Dramatiq](https://dramatiq.io/) is a background task-processing library for Python with a focus on simplicity, reliability and performance.
 
-This package extends dramatiq to provide the following:
+This package, [async-dramatiq](https://pypi.org/project/async-dramatiq/), extends Dramatiq to provide the following:
   1. Support for Asyncio ( [issue #238](https://github.com/Bogdanp/dramatiq/issues/238) )
   2. Message scheduling support ( [scheduling cookbook](https://dramatiq.io/cookbook.html#scheduling-messages) )
 
-### Getting Started
-The quickest way to get started is by playing around with the [worker heartbeat example](examples/worker_heartbeat/README.md).
-
-# The Code
-## Async Middleware
-### Broker
+## Setup
 To provide async support for your actors all you need to do is add the `AsyncMiddleware` to your broker.
 #### RabbitMQ Broker
 
 ```
 import dramatiq
-
 from dramatiq.brokers.rabbitmq import RabbitmqBroker
 
-
 rabbitmq_broker = RabbitmqBroker(host="rabbitmq")
 rabbitmq_broker.add_middleware(AsyncMiddleware())  # <--- Here
 dramatiq.set_broker(rabbitmq_broker)
 ```
 
 #### Redis Broker
 
 ```
 import dramatiq
-import dramatiq
-
 from dramatiq.brokers.redis import RedisBroker
 
-
 redis_broker = RedisBroker(host="redis")
 redis_broker.add_middleware(AsyncMiddleware()) # <--- Here
 dramatiq.set_broker(redis_broker)
 ```
 
+## Running
+#### The Scheduler
+We leverage [apscheduler](https://pypi.org/project/APScheduler/) as our scheduling system. Check out [run_scheduler.py](examples/worker_heartbeat/run_scheduler.py) for an example of running this scheduler.
+#### Dramatiq Worker
+For more details check out the official guide to [dramatiq](https://dramatiq.io/guide.html#workers) or [docker-compose.yaml](examples/worker_heartbeat/docker-compose.yaml) for a specific example.
+
+
+## Example
+Play around with [worker-heartbeat-example](examples/worker_heartbeat/README.md). A functioning and featured example implementation.
+
+----
+# Async Middleware
+`AsyncMiddleware` will start a `AsyncWorker` which will be used to run the event loop. This event loop will be shared across the Worker threads. 
 ### Startup and Shutdown Events
 To startup and shutdown any resources the `AsyncMiddleware` provides two hooks:
 1. Before the event loop is started
 2. After the event loop is stopped
 To allow for standing up or tearing down of shared async resources
 #### Example
 ```
@@ -85,33 +87,27 @@
     def after_async_worker_thread_shutdown(
         self, _: RabbitmqBroker, thread: AsyncWorker, **kwargs: dict[str, Any]
     ) -> None:
         thread.event_loop.run_until_complete(shutdown())
         thread.event_loop.close()
 ```
 
-## Async Actor
-The async actor, `async_dramatiq_actor`,  acts as a thin wrapper around the dramatiq actor providing a variety of new functionality.
+# Async Actor
+The async actor, `async_actor`,  acts as a thin wrapper around the Dramatiq actor providing a variety of new functionality.
 
-#### Interval Jobs
+## Interval Jobs
 Run a job at some interval
 ```
-@async_dramatiq_actor(interval=timedelta(seconds=5))
+@async_actor(interval=timedelta(seconds=5))
 def run_every_5_seconds() -> None:
     pass
 ```
 
-#### Cron Jobs
+## Cron Jobs
 Run a job on a crontab ( See https://crontab.guru/. )
 ```
-@async_dramatiq_actor(interval="0 0 * * *")
+@async_actor(interval="0 0 * * *")
 def run_at_midnight() -> None:
   pass
 ```
 
-## Running
-### The Scheduler
-Checkout [run_scheduler.py](examples/worker_heartbeat/run_scheduler.py) for an example on running the scheduler.
-### Dramatiq Worker
-Check out the offical guide [dramatiq](https://dramatiq.io/guide.html#workers)
-
```

