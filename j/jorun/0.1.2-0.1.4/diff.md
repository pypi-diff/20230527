# Comparing `tmp/jorun-0.1.2.tar.gz` & `tmp/jorun-0.1.4.tar.gz`

## Comparing `jorun-0.1.2.tar` & `jorun-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/__init__.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/configuration.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/constants.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/errors.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/logger.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/main.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/runner.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/handler/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/handler/base.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/handler/docker.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/handler/group.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/handler/shell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/palette/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/palette/base.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/palette/darcula.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/types/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/types/options.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/types/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/ui/__init__.py
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/ui/application.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/ui/data_signals.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/ui/main_window.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/ui/pane.py
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 jorun-0.1.2/src/jorun/ui/task_panel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jorun-0.1.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jorun-0.1.2/LICENSE
--rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 jorun-0.1.2/README.md
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jorun-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 jorun-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 jorun-0.1.4/jorun.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/configuration.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/constants.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/errors.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/logger.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/main.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/runner.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/runner_thread.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/handler/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/handler/base.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/handler/docker.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/handler/group.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/handler/shell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/palette/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/palette/base.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/palette/darcula.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/types/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/types/options.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/types/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/__init__.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/application.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/data_signals.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/main_window.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/pane.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/task_panel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jorun-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jorun-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 jorun-0.1.4/README.md
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jorun-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 jorun-0.1.4/PKG-INFO
```

### Comparing `jorun-0.1.2/src/jorun/logger.py` & `jorun-0.1.4/src/jorun/logger.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.2/src/jorun/runner.py` & `jorun-0.1.4/src/jorun/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import asyncio
 import logging
 import os.path
 from asyncio.subprocess import Process
 from datetime import datetime
 from logging import Logger
 from typing import Optional, Callable, List, Union
+from tinyioc import inject
 
 from .handler.base import BaseTaskHandler
 from .scanner import AsyncScanner
 from .types.options import TaskOptions
 from .types.task import Task
+from .configuration import AppConfiguration
 
 OUTPUT_READ_INTERVAL = 0.015
 
 
 class TaskRunner:
     _handlers: List[BaseTaskHandler]
     _handler: BaseTaskHandler
@@ -23,18 +25,19 @@
     _completion_callback: Optional[Callable]
     _scanner: AsyncScanner
     _log_handler: logging.Handler
 
     _logger: Logger
     _err_logger: Logger
 
-    def __init__(self, task: Task, handlers: List[BaseTaskHandler], file_output_dir: Optional[str],
-                 log_level: Union[int, str], log_handler: logging.Handler):
+    @inject()
+    def __init__(self, task: Task, file_output_dir: Optional[str], log_level: Union[int, str],
+                 log_handler: logging.Handler, configuration: AppConfiguration):
         self._task = task
-        self._handlers = handlers
+        self._handlers = configuration.handlers
         self._process = None
         self._running = True
         self._completion_callback = None
         self._log_handler = log_handler
 
         self._handler = next(h for h in self._handlers if h.task_type == task['type'])
 
@@ -54,14 +57,18 @@
             output_file = os.path.join(file_output_dir, f"{task['name']}_{now_time}.log")
             file_handler = logging.FileHandler(output_file)
             file_handler.terminator = ''
 
             self._logger.addHandler(file_handler)
             self._err_logger.addHandler(file_handler)
 
+    @property
+    def name(self):
+        return self._task["name"]
+
     def _on_stop(self):
         self._handler.on_exit(self._task[self._handler.task_type], self._process)
 
     def stop(self):
         if self._process and self._process.returncode is None:
             self._on_stop()
             self._process.terminate()
```

### Comparing `jorun-0.1.2/src/jorun/scanner.py` & `jorun-0.1.4/src/jorun/scanner.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.2/src/jorun/handler/base.py` & `jorun-0.1.4/src/jorun/handler/base.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.2/src/jorun/handler/docker.py` & `jorun-0.1.4/src/jorun/handler/docker.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.2/src/jorun/handler/group.py` & `jorun-0.1.4/src/jorun/handler/group.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.2/src/jorun/handler/shell.py` & `jorun-0.1.4/src/jorun/handler/shell.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.2/src/jorun/types/task.py` & `jorun-0.1.4/src/jorun/types/task.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.2/src/jorun/ui/application.py` & `jorun-0.1.4/src/jorun/ui/application.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,53 +8,45 @@
 
 from .main_window import MainWindow
 from ..logger import logger
 from ..types.task import PaneConfiguration
 
 
 class UiApplication:
-    _ui_thread: Thread
-    _running: bool
-
     _app: QApplication
     _window: Optional[MainWindow]
     _config: Optional[Dict[str, PaneConfiguration]]
 
     _task_list: List[str]
     _streams_queue: Queue
     _close_handler: Callable
 
     _stream_dequeue_thread: Thread
     _stream_dequeue_running: bool
 
     _trigger_close_handler: bool
 
-    def __init__(self, tasks: List[str], close_handler: Callable, task_streams_queue: Queue,
+    def __init__(self, tasks: List[str], task_streams_queue: Queue,
                  config: Optional[Dict[str, PaneConfiguration]]):
         self._window = None
         self._trigger_close_handler = True
         self._config = config
         self._task_list = tasks
-        self._close_handler = close_handler
         self._streams_queue = task_streams_queue
 
     def _app_quitting(self):
         self._stream_dequeue_running = False
         self._stream_dequeue_thread.join()
 
-        self._close_handler()
-
     def start_ui(self):
         self._stream_dequeue_running = True
         self._stream_dequeue_thread = Thread(target=self._dequeue_stream)
         self._stream_dequeue_thread.start()
 
-        self._running = True
-        self._ui_thread = Thread(target=self._run_ui_thread)
-        self._ui_thread.start()
+        self._run_ui_thread()
 
     def _dequeue_stream(self):
         while self._stream_dequeue_running:
             if self._window:
                 try:
                     stream_record = self._streams_queue.get(block=True, timeout=0.5)
                     self._window.dispatch_stream_record(stream_record)
@@ -71,15 +63,10 @@
         self._window.show()
 
         self._app.exec()
         self._running = False
         self._app_quitting()
 
     def stop_ui(self):
-        if self._running:
-            self._trigger_close_handler = False
-            self._window.dispatch_app_termination()
-
-            try:
-                self._ui_thread.join(timeout=3)
-            except RuntimeError:
-                logger.warning("Couldn't stop the UI thread, ignoring it")
+        if self._stream_dequeue_running:
+            self._stream_dequeue_running = False
+            self._stream_dequeue_thread.join()
```

### Comparing `jorun-0.1.2/src/jorun/ui/main_window.py` & `jorun-0.1.4/src/jorun/ui/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from logging import LogRecord
 from typing import Dict, List, Optional
 
+from PySide6.QtCore import Slot
 from PySide6.QtWidgets import QMainWindow, QTabWidget
 from tinyioc import inject
 
 from .data_signals import DataUpdateSignalEmitter, MainWindowSignals
 from .pane import TasksPane
 from .. import constants
 from ..palette.base import BaseColorPalette
@@ -69,14 +70,15 @@
             extra_pane = TasksPane(None, list(tasks_bucket))
             extra_pane.setAutoFillBackground(True)
             self._tab_widget.addTab(extra_pane, "-")
             self._panes.append(extra_pane)
 
         self.signals.data_received.connect(self._handle_stream_record)
 
+    @Slot()
     def _handle_stream_record(self, record: LogRecord):
         for p in self._panes:
             p.dispatch_log_record(record)
 
     # noinspection PyUnresolvedReferences
     def dispatch_stream_record(self, record: LogRecord):
         self.signals.data_received.emit(record)
```

### Comparing `jorun-0.1.2/src/jorun/ui/pane.py` & `jorun-0.1.4/src/jorun/ui/pane.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.2/src/jorun/ui/task_panel.py` & `jorun-0.1.4/src/jorun/ui/task_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from logging import LogRecord
 from typing import Optional
 
+from PySide6.QtCore import Slot
 from PySide6.QtWidgets import QGroupBox, QVBoxLayout, QWidget, QPlainTextEdit, QLabel, QLineEdit, QSizePolicy
 from tinyioc import inject
 
 from ..palette.base import BaseColorPalette
 
 from .. import constants
 
@@ -97,9 +98,10 @@
                 if filter_input in line:
                     filtered_text += line
         else:
             filtered_text = self._output_stream
 
         self._output_stream_edit_text.setPlainText(filtered_text)
 
+    @Slot()
     def _filter_changed(self):
         self._update_output_edit_text()
```

### Comparing `jorun-0.1.2/LICENSE` & `jorun-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jorun-0.1.2/README.md` & `jorun-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jorun-0.1.2/pyproject.toml` & `jorun-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jorun"
-version = "0.1.2"
+version = "0.1.4"
 authors = [
   { name="Paolo Infante", email="info@paoloinfante.it" },
 ]
 description = "A customizable task runner"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jorun-0.1.2/PKG-INFO` & `jorun-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jorun
-Version: 0.1.2
+Version: 0.1.4
 Summary: A customizable task runner
 Project-URL: Homepage, https://github.com/paolo-projects/jorun
 Project-URL: Bug Tracker, https://github.com/paolo-projects/jorun/issues
 Author-email: Paolo Infante <info@paoloinfante.it>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

