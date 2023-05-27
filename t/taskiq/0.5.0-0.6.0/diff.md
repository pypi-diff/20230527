# Comparing `tmp/taskiq-0.5.0.tar.gz` & `tmp/taskiq-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.5.0.tar", max compression
+gzip compressed data, was "taskiq-0.6.0.tar", max compression
```

## Comparing `taskiq-0.5.0.tar` & `taskiq-0.6.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0     1075 2023-05-21 22:13:26.880195 taskiq-0.5.0/LICENSE
--rw-r--r--   0        0        0     1875 2023-05-21 22:13:26.880195 taskiq-0.5.0/README.md
--rw-r--r--   0        0        0     2880 2023-05-21 22:13:26.884195 taskiq-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1587 2023-05-21 22:13:26.884195 taskiq-0.5.0/taskiq/__init__.py
--rw-r--r--   0        0        0     2077 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/__init__.py
--rw-r--r--   0        0        0    12064 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/broker.py
--rw-r--r--   0        0        0      323 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      629 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     3002 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1376 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1084 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0       34 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     5679 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2197 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2514 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      197 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     1990 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     3912 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2550 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1517 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     6060 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0      628 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     7497 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     6163 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0      468 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/context.py
--rw-r--r--   0        0        0     2930 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/decor.py
--rw-r--r--   0        0        0      511 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/events.py
--rw-r--r--   0        0        0      941 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      844 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1887 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/funcs.py
--rw-r--r--   0        0        0     5552 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/kicker.py
--rw-r--r--   0        0        0      507 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     4315 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/middlewares/prometheus_middleware.py
--rw-r--r--   0        0        0     2043 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/py.typed
--rw-r--r--   0        0        0      113 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/receiver/__init__.py
--rw-r--r--   0        0        0     2795 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/receiver/params_parser.py
--rw-r--r--   0        0        0    11406 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/receiver/receiver.py
--rw-r--r--   0        0        0     2020 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/result.py
--rw-r--r--   0        0        0       35 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1268 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     1520 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     1717 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0    11302 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/serialization.py
--rw-r--r--   0        0        0     1071 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/state.py
--rw-r--r--   0        0        0     4141 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/task.py
--rw-r--r--   0        0        0      874 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/utils.py
--rw-r--r--   0        0        0      106 2023-05-21 22:13:26.888195 taskiq-0.5.0/taskiq/warnings.py
--rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 taskiq-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-27 09:56:32.561007 taskiq-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1875 2023-05-27 09:56:32.561007 taskiq-0.6.0/README.md
+-rw-r--r--   0        0        0     2880 2023-05-27 09:56:32.569007 taskiq-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2197 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/__init__.py
+-rw-r--r--   0        0        0     2093 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0    12516 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      323 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     3002 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1376 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1084 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0      577 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/acks.py
+-rw-r--r--   0        0        0       34 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     5679 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2197 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2514 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     1990 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     3998 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2550 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1517 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     6060 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      628 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     7497 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     6163 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0      468 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/context.py
+-rw-r--r--   0        0        0     2930 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/decor.py
+-rw-r--r--   0        0        0      511 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/events.py
+-rw-r--r--   0        0        0     1032 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      844 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1887 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/funcs.py
+-rw-r--r--   0        0        0     5552 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4315 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2438 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/py.typed
+-rw-r--r--   0        0        0      113 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2795 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0    12195 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0     2020 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/result.py
+-rw-r--r--   0        0        0       35 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1268 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     1520 2023-05-27 09:56:32.569007 taskiq-0.6.0/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     1717 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0    11302 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/serialization.py
+-rw-r--r--   0        0        0     1071 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/state.py
+-rw-r--r--   0        0        0     4141 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/task.py
+-rw-r--r--   0        0        0      900 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/utils.py
+-rw-r--r--   0        0        0      106 2023-05-27 09:56:32.573007 taskiq-0.6.0/taskiq/warnings.py
+-rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 taskiq-0.6.0/PKG-INFO
```

### Comparing `taskiq-0.5.0/LICENSE` & `taskiq-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/README.md` & `taskiq-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/pyproject.toml` & `taskiq-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.5.0"
+version = "0.6.0"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
```

### Comparing `taskiq-0.5.0/taskiq/__main__.py` & `taskiq-0.6.0/taskiq/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import sys
 from typing import Dict
 
-from importlib_metadata import entry_points, version
+from importlib_metadata import entry_points
 
+from taskiq import __version__
 from taskiq.abc.cmd import TaskiqCMD
 
 
 def main() -> None:  # noqa: WPS210  # pragma: no cover
     """
     Main entrypoint of the taskiq.
 
@@ -56,15 +57,15 @@
                 add_help=False,
             )
             subcommands[entrypoint.name] = cmd_class()
 
     args, _ = parser.parse_known_args()
 
     if args.version:
-        print(version("taskiq"))  # noqa: WPS421
+        print(__version__)  # noqa: WPS421
         return
 
     if args.subcommand is None:
         parser.print_help()
         return
 
     command = subcommands[args.subcommand]
```

### Comparing `taskiq-0.5.0/taskiq/abc/broker.py` & `taskiq-0.6.0/taskiq/abc/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     overload,
 )
 from uuid import uuid4
 
 from typing_extensions import ParamSpec, Self, TypeAlias
 
 from taskiq.abc.middleware import TaskiqMiddleware
+from taskiq.acks import AckableMessage
 from taskiq.decor import AsyncTaskiqDecoratedTask
 from taskiq.events import TaskiqEvents
 from taskiq.formatters.json_formatter import JSONFormatter
 from taskiq.message import BrokerMessage
 from taskiq.result_backends.dummy import DummyResultBackend
 from taskiq.state import TaskiqState
 from taskiq.utils import maybe_awaitable, remove_suffix
@@ -64,15 +65,18 @@
 
     This abstract class must be implemented in order
     to get ability to send tasks to brokers
     in async mode.
     """
 
     available_tasks: Dict[str, AsyncTaskiqDecoratedTask[Any, Any]] = {}
+    # True only if broker runs in worker process.
     is_worker_process: bool = False
+    # True only if broker runs in scheduler process.
+    is_scheduler_process: bool = False
 
     def __init__(
         self,
         result_backend: "Optional[AsyncResultBackend[_T]]" = None,
         task_id_generator: Optional[Callable[[], str]] = None,
     ) -> None:
         if result_backend is None:
@@ -178,21 +182,27 @@
         You don't need to send broker message. It's helper for brokers,
         please send only bytes from message.message.
 
         :param message: name of a task.
         """
 
     @abstractmethod
-    def listen(self) -> AsyncGenerator[bytes, None]:
+    def listen(self) -> AsyncGenerator[Union[bytes, AckableMessage], None]:
         """
         This function listens to new messages and yields them.
 
         This it the main point for workers.
         This function is used to get new tasks from the network.
 
+        If your broker support acknowledgement, then you
+        should wrap your message in AckableMessage dataclass.
+
+        If your messages was wrapped in AckableMessage dataclass,
+        taskiq will call ack when finish processing message.
+
         :yield: incoming messages.
         :return: nothing.
         """
 
     @overload
     def task(
         self,
```

### Comparing `taskiq-0.5.0/taskiq/abc/formatter.py` & `taskiq-0.6.0/taskiq/abc/formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/abc/middleware.py` & `taskiq-0.6.0/taskiq/abc/middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/abc/result_backend.py` & `taskiq-0.6.0/taskiq/abc/result_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/abc/schedule_source.py` & `taskiq-0.6.0/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/brokers/inmemory_broker.py` & `taskiq-0.6.0/taskiq/brokers/inmemory_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/brokers/shared_broker.py` & `taskiq-0.6.0/taskiq/brokers/shared_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/brokers/zmq_broker.py` & `taskiq-0.6.0/taskiq/brokers/zmq_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/cli/scheduler/args.py` & `taskiq-0.6.0/taskiq/cli/scheduler/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/cli/scheduler/cmd.py` & `taskiq-0.6.0/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/cli/scheduler/run.py` & `taskiq-0.6.0/taskiq/cli/scheduler/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 from datetime import datetime, timedelta
 from logging import basicConfig, getLevelName, getLogger
 from typing import List
 
 from pycron import is_now
 
+from taskiq.abc.broker import AsyncBroker
 from taskiq.cli.scheduler.args import SchedulerArgs
 from taskiq.cli.utils import import_object, import_tasks
 from taskiq.kicker import AsyncKicker
 from taskiq.scheduler.scheduler import ScheduledTask, TaskiqScheduler
 
 logger = getLogger(__name__)
 
@@ -66,14 +67,15 @@
     Runs scheduler loop.
 
     This function imports taskiq scheduler
     and runs tasks when needed.
 
     :param args: parsed CLI args.
     """
+    AsyncBroker.is_scheduler_process = True
     scheduler = import_object(args.scheduler)
     if not isinstance(scheduler, TaskiqScheduler):
         print(  # noqa: WPS421
             "Imported scheduler is not a subclass of TaskiqScheduler.",
         )
         exit(1)  # noqa: WPS421
     import_tasks(args.modules, args.tasks_pattern, args.fs_discover)
```

### Comparing `taskiq-0.5.0/taskiq/cli/utils.py` & `taskiq-0.6.0/taskiq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/cli/watcher.py` & `taskiq-0.6.0/taskiq/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/cli/worker/args.py` & `taskiq-0.6.0/taskiq/cli/worker/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/cli/worker/cmd.py` & `taskiq-0.6.0/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/cli/worker/log_collector.py` & `taskiq-0.6.0/taskiq/cli/worker/log_collector.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/cli/worker/process_manager.py` & `taskiq-0.6.0/taskiq/cli/worker/process_manager.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/cli/worker/run.py` & `taskiq-0.6.0/taskiq/cli/worker/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/decor.py` & `taskiq-0.6.0/taskiq/decor.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/exceptions.py` & `taskiq-0.6.0/taskiq/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,7 +32,11 @@
 
 class SecurityError(TaskiqError):
     """Security related exception."""
 
 
 class NoResultError(TaskiqError):
     """Error if user does not want to set result."""
+
+
+class RejectError(TaskiqError):
+    """Error is thrown if message should be rejected."""
```

### Comparing `taskiq-0.5.0/taskiq/formatters/json_formatter.py` & `taskiq-0.6.0/taskiq/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/funcs.py` & `taskiq-0.6.0/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/kicker.py` & `taskiq-0.6.0/taskiq/kicker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/middlewares/prometheus_middleware.py` & `taskiq-0.6.0/taskiq/middlewares/prometheus_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/middlewares/retry_middleware.py` & `taskiq-0.6.0/taskiq/middlewares/retry_middleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from copy import deepcopy
 from logging import getLogger
 from typing import Any
 
 from taskiq.abc.middleware import TaskiqMiddleware
+from taskiq.exceptions import NoResultError
 from taskiq.message import TaskiqMessage
 from taskiq.result import TaskiqResult
 
 logger = getLogger("taskiq.retry_middleware")
 
 
 class SimpleRetryMiddleware(TaskiqMiddleware):
     """Middleware to add retries."""
 
     def __init__(
         self,
         default_retry_count: int = 3,
+        default_retry_label: bool = False,
+        no_result_on_retry: bool = True,
     ) -> None:
         self.default_retry_count = default_retry_count
+        self.default_retry_label = default_retry_label
+        self.no_result_on_retry = no_result_on_retry
 
     async def on_error(
         self,
         message: "TaskiqMessage",
         result: "TaskiqResult[Any]",
         exception: BaseException,
     ) -> None:
@@ -33,30 +38,40 @@
         If error is found during the execution
         this function is invoked.
 
         :param message: Message that caused the error.
         :param result: execution result.
         :param exception: found exception.
         """
+        # Valid exception
+        if isinstance(exception, NoResultError):
+            return
+
         retry_on_error = message.labels.get("retry_on_error")
+        if retry_on_error is None:
+            retry_on_error = "true" if self.default_retry_label else "false"
         # Check if retrying is enabled for the task.
-        if retry_on_error is None or retry_on_error.lower() != "true":
+        if retry_on_error.lower() != "true":
             return
         new_msg = deepcopy(message)
+
         # Getting number of previous retries.
         retries = int(new_msg.labels.get("_retries", 0)) + 1
         new_msg.labels["_retries"] = str(retries)
         max_retries = int(new_msg.labels.get("max_retries", self.default_retry_count))
+
         if retries < max_retries:
             logger.info(
                 "Task '%s' invocation failed. Retrying.",
                 message.task_name,
             )
-            new_msg.labels["_parent"] = message.task_id
-            new_msg.task_id = self.broker.id_generator()
             broker_message = self.broker.formatter.dumps(message=new_msg)
             await self.broker.kick(broker_message)
+
+            if self.no_result_on_retry:
+                result.error = NoResultError()
+
         else:
             logger.warning(
                 "Task '%s' invocation failed. Maximum retries count is reached.",
                 message.task_name,
             )
```

### Comparing `taskiq-0.5.0/taskiq/receiver/params_parser.py` & `taskiq-0.6.0/taskiq/receiver/params_parser.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/receiver/receiver.py` & `taskiq-0.6.0/taskiq/receiver/receiver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import asyncio
 import inspect
 from concurrent.futures import Executor
 from logging import getLogger
 from time import time
-from typing import Any, Callable, Dict, Optional, Set, get_type_hints
+from typing import Any, Callable, Dict, Optional, Set, Union, get_type_hints
 
 import anyio
 from taskiq_dependencies import DependencyGraph
 
-from taskiq.abc.broker import AsyncBroker
+from taskiq.abc.broker import AckableMessage, AsyncBroker
 from taskiq.abc.middleware import TaskiqMiddleware
 from taskiq.context import Context
-from taskiq.exceptions import NoResultError
+from taskiq.exceptions import NoResultError, RejectError
 from taskiq.message import TaskiqMessage
 from taskiq.receiver.params_parser import parse_params
 from taskiq.result import TaskiqResult
 from taskiq.state import TaskiqState
 from taskiq.utils import maybe_awaitable
 
 logger = getLogger(__name__)
@@ -65,37 +65,41 @@
         else:
             logger.warning(
                 "Setting unlimited number of async tasks "
                 + "can result in undefined behavior",
             )
         self.sem_prefetch = asyncio.Semaphore(max_prefetch)
 
-    async def callback(  # noqa: C901, WPS213
+    async def callback(  # noqa: C901, WPS213, WPS217
         self,
-        message: bytes,
+        message: Union[bytes, AckableMessage],
         raise_err: bool = False,
     ) -> None:
         """
         Receive new message and execute tasks.
 
         This method is used to process message,
         that came from brokers.
 
         :raises Exception: if raise_err is true,
             and exception were found while saving result.
         :param message: received message.
         :param raise_err: raise an error if cannot save result in
             result_backend.
         """
+        if isinstance(message, AckableMessage):
+            message_data = message.data
+        else:
+            message_data = message
         try:
-            taskiq_msg = self.broker.formatter.loads(message=message)
+            taskiq_msg = self.broker.formatter.loads(message=message_data)
         except Exception as exc:
             logger.warning(
                 "Cannot parse message: %s. Skipping execution.\n %s",
-                message,
+                message_data,
                 exc,
                 exc_info=True,
             )
             return
         logger.debug(f"Received message: {taskiq_msg}")
         if taskiq_msg.task_name not in self.broker.available_tasks:
             logger.warning(
@@ -120,17 +124,28 @@
             taskiq_msg.task_name,
             taskiq_msg.task_id,
         )
         result = await self.run_task(
             target=self.broker.available_tasks[taskiq_msg.task_name].original_func,
             message=taskiq_msg,
         )
+
+        # If broker has an ability to ack or reject messages.
+        if isinstance(message, AckableMessage):
+            # If we received an error for negative acknowledgement.
+            if message.reject is not None and isinstance(result.error, RejectError):
+                await maybe_awaitable(message.reject())
+            # Otherwise we positively acknowledge the message.
+            else:
+                await maybe_awaitable(message.ack())
+
         for middleware in self.broker.middlewares:
             if middleware.__class__.post_execute != TaskiqMiddleware.post_execute:
                 await maybe_awaitable(middleware.post_execute(taskiq_msg, result))
+
         try:
             if not isinstance(result.error, NoResultError):
                 await self.broker.result_backend.set_result(taskiq_msg.task_id, result)
                 for middleware in self.broker.middlewares:
                     if middleware.__class__.post_save != TaskiqMiddleware.post_save:
                         await maybe_awaitable(middleware.post_save(taskiq_msg, result))
         except Exception as exc:
@@ -251,21 +266,24 @@
         This function iterates over tasks asynchronously.
 
         It uses listen() method of an AsyncBroker
         to get new messages from queues.
         """
         await self.broker.startup()
         logger.info("Listening started.")
-        queue: asyncio.Queue[bytes] = asyncio.Queue()
+        queue: "asyncio.Queue[Union[bytes, AckableMessage]]" = asyncio.Queue()
 
         async with anyio.create_task_group() as gr:
             gr.start_soon(self.prefetcher, queue)
             gr.start_soon(self.runner, queue)
 
-    async def prefetcher(self, queue: "asyncio.Queue[Any]") -> None:
+    async def prefetcher(
+        self,
+        queue: "asyncio.Queue[Union[bytes, AckableMessage]]",
+    ) -> None:
         """
         Prefetch tasks data.
 
         :param queue: queue for prefetched data.
         """
         iterator = self.broker.listen()
 
@@ -276,15 +294,18 @@
                 await queue.put(message)
 
             except StopAsyncIteration:
                 break
 
         await queue.put(QUEUE_DONE)
 
-    async def runner(self, queue: "asyncio.Queue[bytes]") -> None:
+    async def runner(
+        self,
+        queue: "asyncio.Queue[Union[bytes, AckableMessage]]",
+    ) -> None:
         """
         Run tasks.
 
         :param queue: queue with prefetched data.
         """
         tasks: Set[asyncio.Task[Any]] = set()
```

### Comparing `taskiq-0.5.0/taskiq/result.py` & `taskiq-0.6.0/taskiq/result.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/result_backends/dummy.py` & `taskiq-0.6.0/taskiq/result_backends/dummy.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/schedule_sources/label_based.py` & `taskiq-0.6.0/taskiq/schedule_sources/label_based.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/scheduler/merge_functions.py` & `taskiq-0.6.0/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/scheduler/scheduler.py` & `taskiq-0.6.0/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/serialization.py` & `taskiq-0.6.0/taskiq/serialization.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/state.py` & `taskiq-0.6.0/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/taskiq/task.py` & `taskiq-0.6.0/taskiq/task.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.5.0/PKG-INFO` & `taskiq-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq
-Version: 0.5.0
+Version: 0.6.0
 Summary: Distributed task queue with full async support
 Home-page: https://taskiq-python.github.io/
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Maintainer: Pavel Kirilin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskiq Version: 0.5.0 Summary: Distributed task
+Metadata-Version: 2.1 Name: taskiq Version: 0.6.0 Summary: Distributed task
 queue with full async support Home-page: https://taskiq-python.github.io/
 License: LICENSE Keywords: taskiq,tasks,distributed,async Author: Pavel Kirilin
 Author-email: win10@list.ru Maintainer: Pavel Kirilin Maintainer-email:
 win10@list.ru Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

