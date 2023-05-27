# Comparing `tmp/async_dramatiq-0.1.5.tar.gz` & `tmp/async_dramatiq-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_dramatiq-0.1.5.tar", max compression
+gzip compressed data, was "async_dramatiq-0.1.6.tar", max compression
```

## Comparing `async_dramatiq-0.1.5.tar` & `async_dramatiq-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1065 2023-05-26 08:26:10.164949 async_dramatiq-0.1.5/LICENSE
--rw-r--r--   0        0        0       45 2023-05-25 20:37:01.348380 async_dramatiq-0.1.5/README.md
--rw-r--r--   0        0        0     3489 2023-05-26 10:45:25.162274 async_dramatiq-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      253 2023-05-26 10:02:22.898402 async_dramatiq-0.1.5/src/async_dramatiq/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-26 10:45:38.596903 async_dramatiq-0.1.5/src/async_dramatiq/actors.py
--rw-r--r--   0        0        0      491 2023-05-26 07:37:33.566566 async_dramatiq-0.1.5/src/async_dramatiq/backends/__init__.py
--rw-r--r--   0        0        0     1577 2023-05-26 07:37:33.566695 async_dramatiq-0.1.5/src/async_dramatiq/backends/async_redis.py
--rw-r--r--   0        0        0     1758 2023-05-26 07:37:33.566814 async_dramatiq-0.1.5/src/async_dramatiq/backends/async_stub.py
--rw-r--r--   0        0        0      112 2023-05-26 07:37:33.566965 async_dramatiq-0.1.5/src/async_dramatiq/middleware/__init__.py
--rw-r--r--   0        0        0      823 2023-05-26 10:45:12.402088 async_dramatiq-0.1.5/src/async_dramatiq/middleware/async_base.py
--rw-r--r--   0        0        0      728 2023-05-26 07:37:33.567263 async_dramatiq-0.1.5/src/async_dramatiq/middleware/async_stub.py
--rw-r--r--   0        0        0      961 2023-05-26 07:37:33.567386 async_dramatiq-0.1.5/src/async_dramatiq/scheduler.py
--rw-r--r--   0        0        0      342 2023-05-26 07:37:33.567506 async_dramatiq-0.1.5/src/async_dramatiq/types.py
--rw-r--r--   0        0        0     1112 2023-05-26 07:37:33.567624 async_dramatiq-0.1.5/src/async_dramatiq/worker.py
--rw-r--r--   0        0        0        0 2023-05-26 08:26:10.167650 async_dramatiq-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     1471 2023-05-26 08:26:10.167926 async_dramatiq-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0     3812 2023-05-26 09:10:55.772756 async_dramatiq-0.1.5/tests/test_actors.py
--rw-r--r--   0        0        0     2563 2023-05-26 08:26:10.168282 async_dramatiq-0.1.5/tests/test_backends.py
--rw-r--r--   0        0        0     1024 2023-05-26 08:26:10.168435 async_dramatiq-0.1.5/tests/test_scheduler.py
--rw-r--r--   0        0        0      595 2023-05-26 08:26:10.168609 async_dramatiq-0.1.5/tests/test_workers.py
--rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 async_dramatiq-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-26 08:26:10.164949 async_dramatiq-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2936 2023-05-26 23:57:12.060719 async_dramatiq-0.1.6/README.md
+-rw-r--r--   0        0        0     3506 2023-05-27 00:23:13.868376 async_dramatiq-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      254 2023-05-26 11:00:24.176230 async_dramatiq-0.1.6/src/async_dramatiq/__init__.py
+-rw-r--r--   0        0        0     3182 2023-05-26 23:41:05.167085 async_dramatiq-0.1.6/src/async_dramatiq/actors.py
+-rw-r--r--   0        0        0      491 2023-05-26 07:37:33.566566 async_dramatiq-0.1.6/src/async_dramatiq/backends/__init__.py
+-rw-r--r--   0        0        0     1700 2023-05-27 00:15:20.555394 async_dramatiq-0.1.6/src/async_dramatiq/backends/async_redis.py
+-rw-r--r--   0        0        0     1758 2023-05-26 07:37:33.566814 async_dramatiq-0.1.6/src/async_dramatiq/backends/async_stub.py
+-rw-r--r--   0        0        0      112 2023-05-26 07:37:33.566965 async_dramatiq-0.1.6/src/async_dramatiq/middleware/__init__.py
+-rw-r--r--   0        0        0      934 2023-05-27 00:22:09.609050 async_dramatiq-0.1.6/src/async_dramatiq/middleware/async_base.py
+-rw-r--r--   0        0        0     1159 2023-05-26 18:57:12.390516 async_dramatiq-0.1.6/src/async_dramatiq/middleware/async_stub.py
+-rw-r--r--   0        0        0     1416 2023-05-26 18:47:19.511369 async_dramatiq-0.1.6/src/async_dramatiq/scheduler.py
+-rw-r--r--   0        0        0      485 2023-05-27 00:22:09.606670 async_dramatiq-0.1.6/src/async_dramatiq/types.py
+-rw-r--r--   0        0        0     1232 2023-05-26 18:42:58.013316 async_dramatiq-0.1.6/src/async_dramatiq/worker.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:26:10.167650 async_dramatiq-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     1471 2023-05-26 08:26:10.167926 async_dramatiq-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0     3812 2023-05-26 09:10:55.772756 async_dramatiq-0.1.6/tests/test_actors.py
+-rw-r--r--   0        0        0     2563 2023-05-26 08:26:10.168282 async_dramatiq-0.1.6/tests/test_backends.py
+-rw-r--r--   0        0        0     1024 2023-05-26 08:26:10.168435 async_dramatiq-0.1.6/tests/test_scheduler.py
+-rw-r--r--   0        0        0      595 2023-05-26 08:26:10.168609 async_dramatiq-0.1.6/tests/test_workers.py
+-rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 async_dramatiq-0.1.6/PKG-INFO
```

### Comparing `async_dramatiq-0.1.5/LICENSE` & `async_dramatiq-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.5/pyproject.toml` & `async_dramatiq-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async_dramatiq"
-version = "0.1.5"
+version = "0.1.6"
 description = "Dramatiq with Asyncio support and some other goodies"
 authors = ["Ryan Houlihan <ryan@rhoulihan.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{ include = "async_dramatiq", from = "src" }]
 include = [{ path = "tests", format = "sdist" }]
 homepage = "https://github.com/motherofcoconuts/async-dramatiq"
@@ -24,14 +24,15 @@
 coverage = "^7.2.5"
 pytest-asyncio = "*"
 pytest = "*"
 pytest-cov = "*"
 vulture = "*"
 isort = "*"
 autoflake = "*"
+pre-commit = "*"
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 junit_family = "xunit2"
@@ -109,15 +110,15 @@
 make_whitelist = true
 min_confidence = 80
 paths = ["async_dramatiq"]
 sort_by_size = true
 verbose = false
 
 [tool.mypy]
-python_version = "3.11"
+python_version = "^3.8"
 ignore_missing_imports = true
 scripts_are_modules = true
 implicit_reexport = true
 
 check_untyped_defs = true
 warn_unused_ignores = true 
 warn_return_any = true
```

### Comparing `async_dramatiq-0.1.5/src/async_dramatiq/actors.py` & `async_dramatiq-0.1.6/src/async_dramatiq/actors.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,28 @@
         """
         try:
             running_event_loop = asyncio.get_running_loop()
         except RuntimeError:
             running_event_loop = None
 
         if inspect.iscoroutinefunction(self.fn):
-            if running_event_loop:  # Call function directly
+            if running_event_loop:  # Call function directly on running event loop
                 result = self.fn(*args, **kwargs)
-            elif (  # Call function through worker thread
+            elif (  # Run function async worker thread event loop
                 self.event_loop and self.event_loop.is_running()
             ):
                 future = asyncio.run_coroutine_threadsafe(
                     self.fn(*args, **kwargs), self.event_loop
                 )
                 result = future.result()
             else:  # This should not happen
                 raise RuntimeError("No event")
-        else:
+        else:  # Call function directly
             result = self.fn(*args, **kwargs)
+
         return result
 
     def set_event_loop(self, loop: asyncio.BaseEventLoop | None) -> None:
         self.event_loop = loop
 
 
 def async_dramatiq_actor(
@@ -58,15 +59,15 @@
     actor_class: type[AsyncActor] = AsyncActor,
     queue_name: str = "default",
     **kwargs: Any,
 ) -> Any:
     """Thin wrapper which turns a function into a dramatiq actor.
 
     :param interval: Run this function at a defined interval
-    :param crontab: Run this function as a cron job
+    :param crontab: Run this function as a cron job. See https://crontab.guru/.
     :param priority: The actor's global priority.  If two tasks have
         been pulled on a worker concurrently and one has a higher
         priority than the other then it will be processed first.
         Lower numbers represent higher priorities.
     :param actor_class: The actor class to use
     :param queue_name: The name of the queue to send messages to
     :param kwargs: Input parameters for the dramatiq actor
```

### Comparing `async_dramatiq-0.1.5/src/async_dramatiq/backends/async_redis.py` & `async_dramatiq-0.1.6/src/async_dramatiq/backends/async_redis.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,24 @@
     ResultMissing,
     ResultTimeout,
 )
 from dramatiq.results.backends.redis import RedisBackend
 
 
 class AsyncRedisBackend(RedisBackend):
+    """A Redis backend that supports async redis client.
+
+    TODO: Use async redis client instead of sync client
+    """
+
     async def get_result(
         self, message: dq.Message, *, block: bool = False, timeout: int | None = None
     ) -> Result:
-        """Get a result from the backend.
-        Sub-second timeouts are not respected by this backend.
+        """Get a result from the backend. Sub-second timeouts are not respected by
+        this backend.
 
         :param message: The dramatiq message object
         :param block: Whether or not to block until a result is set.
         :param timeout: The maximum amount of time, in ms, to wait for
           a result when block is True.  Defaults to 10 seconds.
 
         :raise ResultMissing: When block is False and the result isn't set.
```

### Comparing `async_dramatiq-0.1.5/src/async_dramatiq/backends/async_stub.py` & `async_dramatiq-0.1.6/src/async_dramatiq/backends/async_stub.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.5/src/async_dramatiq/scheduler.py` & `async_dramatiq-0.1.6/src/async_dramatiq/scheduler.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 @dataclass
 class ScheduledFunction:
     trigger: CronTrigger | IntervalTrigger
     module_path: str
     func_name: str
 
 
+# Global list of scheduled jobs
 scheduled_jobs: list[ScheduledFunction] = []
 
 
 def _add_trigger(
     trigger: CronTrigger | IntervalTrigger, func: Callable[..., Any]
 ) -> None:
     global scheduled_jobs
@@ -25,12 +26,23 @@
         ScheduledFunction(
             trigger=trigger, module_path=func.__module__, func_name=func.__name__
         )
     )
 
 
 def register_cron(func: Callable[..., Any], crontab: str) -> None:
+    """Register a function to be called on a cron schedule.
+
+    :param func: The function to call.
+    :param crontab: The cron schedule at which to call the function at.
+        Check out https://crontab.guru/ for help.
+    """
     _add_trigger(CronTrigger.from_crontab(crontab), func)
 
 
 def register_interval(func: Callable[..., Any], interval: timedelta) -> None:
+    """Register a function to be called on an interval.
+
+    :param func: The function to call.
+    :param interval: The interval at which to call the function at. This is a timedelta.
+    """
     _add_trigger(IntervalTrigger(seconds=interval.total_seconds()), func)
```

### Comparing `async_dramatiq-0.1.5/tests/conftest.py` & `async_dramatiq-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.5/tests/test_actors.py` & `async_dramatiq-0.1.6/tests/test_actors.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.5/tests/test_backends.py` & `async_dramatiq-0.1.6/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.5/tests/test_scheduler.py` & `async_dramatiq-0.1.6/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.5/tests/test_workers.py` & `async_dramatiq-0.1.6/tests/test_workers.py`

 * *Files identical despite different names*

