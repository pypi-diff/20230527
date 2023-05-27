# Comparing `tmp/pytask_parallel-0.3.0.tar.gz` & `tmp/pytask_parallel-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytask_parallel-0.3.0.tar", last modified: Mon Jan 23 10:47:10 2023, max compression
+gzip compressed data, was "pytask_parallel-0.3.1.tar", last modified: Sat May 27 10:27:08 2023, max compression
```

## Comparing `pytask_parallel-0.3.0.tar` & `pytask_parallel-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:47:10.431280 pytask_parallel-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:47:10.427280 pytask_parallel-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:47:10.427280 pytask_parallel-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:47:10.427280 pytask_parallel-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-01-23 10:47:10.431280 pytask_parallel-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-01-23 10:47:10.431280 pytask_parallel-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:47:10.427280 pytask_parallel-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:47:10.431280 pytask_parallel-0.3.0/src/pytask_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/src/pytask_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-23 10:47:10.000000 pytask_parallel-0.3.0/src/pytask_parallel/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/src/pytask_parallel/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/src/pytask_parallel/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/src/pytask_parallel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12489 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/src/pytask_parallel/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/src/pytask_parallel/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/src/pytask_parallel/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 10:46:58.000000 pytask_parallel-0.3.0/src/pytask_parallel/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:47:10.431280 pytask_parallel-0.3.0/src/pytask_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-01-23 10:47:10.000000 pytask_parallel-0.3.0/src/pytask_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-23 10:47:10.000000 pytask_parallel-0.3.0/src/pytask_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 10:47:10.000000 pytask_parallel-0.3.0/src/pytask_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-23 10:47:10.000000 pytask_parallel-0.3.0/src/pytask_parallel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 10:47:10.000000 pytask_parallel-0.3.0/src/pytask_parallel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-23 10:47:10.000000 pytask_parallel-0.3.0/src/pytask_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-23 10:47:10.000000 pytask_parallel-0.3.0/src/pytask_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:27:08.245646 pytask_parallel-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:27:08.237646 pytask_parallel-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:27:08.241646 pytask_parallel-0.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:27:08.241646 pytask_parallel-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-27 10:27:08.245646 pytask_parallel-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-27 10:27:08.249646 pytask_parallel-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:27:08.237646 pytask_parallel-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:27:08.245646 pytask_parallel-0.3.1/src/pytask_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/src/pytask_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-27 10:27:08.000000 pytask_parallel-0.3.1/src/pytask_parallel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/src/pytask_parallel/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/src/pytask_parallel/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/src/pytask_parallel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/src/pytask_parallel/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/src/pytask_parallel/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/src/pytask_parallel/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:58.000000 pytask_parallel-0.3.1/src/pytask_parallel/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:27:08.245646 pytask_parallel-0.3.1/src/pytask_parallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-27 10:27:08.000000 pytask_parallel-0.3.1/src/pytask_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-27 10:27:08.000000 pytask_parallel-0.3.1/src/pytask_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:27:08.000000 pytask_parallel-0.3.1/src/pytask_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-27 10:27:08.000000 pytask_parallel-0.3.1/src/pytask_parallel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:27:07.000000 pytask_parallel-0.3.1/src/pytask_parallel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 10:27:08.000000 pytask_parallel-0.3.1/src/pytask_parallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 10:27:08.000000 pytask_parallel-0.3.1/src/pytask_parallel.egg-info/top_level.txt
```

### Comparing `pytask_parallel-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `pytask_parallel-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pytask_parallel-0.3.0/.github/ISSUE_TEMPLATE/documentation.md` & `pytask_parallel-0.3.1/.github/ISSUE_TEMPLATE/documentation.md`

 * *Files identical despite different names*

### Comparing `pytask_parallel-0.3.0/.github/ISSUE_TEMPLATE/enhancement.md` & `pytask_parallel-0.3.1/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `pytask_parallel-0.3.0/.github/ISSUE_TEMPLATE/question.md` & `pytask_parallel-0.3.1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `pytask_parallel-0.3.0/.github/workflows/main.yml` & `pytask_parallel-0.3.1/.github/workflows/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     strategy:
       fail-fast: false
       matrix:
         os: ['ubuntu-latest', 'macos-latest', 'windows-latest']
         python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - uses: conda-incubator/setup-miniconda@v2
         with:
           auto-update-conda: false
           python-version: ${{ matrix.python-version }}
           channels: conda-forge,nodefaults
           miniforge-variant: Mambaforge
```

### Comparing `pytask_parallel-0.3.0/.github/workflows/publish-to-pypi.yml` & `pytask_parallel-0.3.1/.github/workflows/publish-to-pypi.yml`

 * *Files 21% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 on: push
 
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@master
+    - uses: actions/checkout@v3
 
     - name: Set up Python 3.8
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
 
     - name: Install pypa/build
       run: >-
         python -m
         pip install
```

### Comparing `pytask_parallel-0.3.0/LICENSE` & `pytask_parallel-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytask_parallel-0.3.0/PKG-INFO` & `pytask_parallel-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytask_parallel
-Version: 0.3.0
+Version: 0.3.1
 Summary: Parallelize the execution of tasks with pytask.
 Home-page: https://github.com/pytask-dev/pytask-parallel
 Author: Tobias Raabe
 Author-email: raabe@posteo.de
 License: MIT
 Project-URL: Changelog, https://github.com/pytask-dev/pytask-parallel/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/pytask-dev/pytask-parallel
@@ -46,17 +46,17 @@
 $ pip install pytask-parallel
 
 # or
 
 $ conda install -c conda-forge pytask-parallel
 ```
 
-By default, the plugin uses `loky`'s robust implementation of the `ProcessPoolExecutor`.
+By default, the plugin uses `concurrent.futures.ProcessPoolExecutor`.
 
-It is also possible to select the `ProcessPoolExecutor` or `ThreadPoolExecutor` from the
+It is also possible to select the executor from loky or `ThreadPoolExecutor` from the
 [concurrent.futures](https://docs.python.org/3/library/concurrent.futures.html) module
 as backends to execute tasks asynchronously.
 
 ## Usage
 
 To parallelize your tasks across many workers, pass an integer greater than 1 or
 `'auto'` to the command-line interface.
@@ -83,15 +83,15 @@
 You can also set the options in a `pyproject.toml`.
 
 ```toml
 # This is the default configuration. Note that, parallelization is turned off.
 
 [tool.pytask.ini_options]
 n_workers = 1
-parallel_backend = "loky"  # or processes or threads
+parallel_backend = "processes"  # or loky or threads
 ```
 
 ## Some implementation details
 
 ### Parallelization and Debugging
 
 It is not possible to combine parallelization with debugging. That is why `--pdb` or
```

### Comparing `pytask_parallel-0.3.0/README.md` & `pytask_parallel-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 $ pip install pytask-parallel
 
 # or
 
 $ conda install -c conda-forge pytask-parallel
 ```
 
-By default, the plugin uses `loky`'s robust implementation of the `ProcessPoolExecutor`.
+By default, the plugin uses `concurrent.futures.ProcessPoolExecutor`.
 
-It is also possible to select the `ProcessPoolExecutor` or `ThreadPoolExecutor` from the
+It is also possible to select the executor from loky or `ThreadPoolExecutor` from the
 [concurrent.futures](https://docs.python.org/3/library/concurrent.futures.html) module
 as backends to execute tasks asynchronously.
 
 ## Usage
 
 To parallelize your tasks across many workers, pass an integer greater than 1 or
 `'auto'` to the command-line interface.
@@ -61,15 +61,15 @@
 You can also set the options in a `pyproject.toml`.
 
 ```toml
 # This is the default configuration. Note that, parallelization is turned off.
 
 [tool.pytask.ini_options]
 n_workers = 1
-parallel_backend = "loky"  # or processes or threads
+parallel_backend = "processes"  # or loky or threads
 ```
 
 ## Some implementation details
 
 ### Parallelization and Debugging
 
 It is not possible to combine parallelization with debugging. That is why `--pdb` or
```

### Comparing `pytask_parallel-0.3.0/setup.cfg` & `pytask_parallel-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytask_parallel-0.3.0/src/pytask_parallel/build.py` & `pytask_parallel-0.3.1/src/pytask_parallel/build.py`

 * *Files identical despite different names*

### Comparing `pytask_parallel-0.3.0/src/pytask_parallel/config.py` & `pytask_parallel-0.3.1/src/pytask_parallel/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pytask import hookimpl
 from pytask_parallel.backends import ParallelBackendChoices
 
 
 @hookimpl
 def pytask_parse_config(config: dict[str, Any]) -> None:
     """Parse the configuration."""
-    if config["n_workers"] == "auto":  # noqa: PLR2004
+    if config["n_workers"] == "auto":
         config["n_workers"] = max(os.cpu_count() - 1, 1)
 
     if (
         isinstance(config["parallel_backend"], str)
         and config["parallel_backend"] in ParallelBackendChoices._value2member_map_
     ):
         config["parallel_backend"] = ParallelBackendChoices(config["parallel_backend"])
```

### Comparing `pytask_parallel-0.3.0/src/pytask_parallel/execute.py` & `pytask_parallel-0.3.1/src/pytask_parallel/execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from concurrent.futures import Future
 from types import TracebackType
 from typing import Any
 from typing import Callable
 from typing import List
 
 import attr
-import cloudpickle
 from pybaum.tree_util import tree_map
 from pytask import console
 from pytask import ExecutionReport
 from pytask import get_marks
 from pytask import hookimpl
 from pytask import Mark
 from pytask import parse_warning_filter
@@ -37,15 +36,15 @@
     if config["parallel_backend"] == ParallelBackendChoices.THREADS:
         config["pm"].register(DefaultBackendNameSpace)
     else:
         config["pm"].register(ProcessesNameSpace)
 
 
 @hookimpl(tryfirst=True)
-def pytask_execute_build(session: Session) -> bool | None:
+def pytask_execute_build(session: Session) -> bool | None:  # noqa: C901, PLR0915
     """Execute tasks with a parallel backend.
 
     There are three phases while the scheduler has tasks which need to be executed.
 
     1. Take all ready tasks, set up their execution and submit them.
     2. For all tasks which are running, find those which have finished and turn them
        into a report.
@@ -55,20 +54,18 @@
     if session.config["n_workers"] > 1:
         reports = session.execution_reports
         running_tasks: dict[str, Future[Any]] = {}
 
         parallel_backend = PARALLEL_BACKENDS[session.config["parallel_backend"]]
 
         with parallel_backend(max_workers=session.config["n_workers"]) as executor:
-
             session.config["_parallel_executor"] = executor
             sleeper = _Sleeper()
 
             while session.scheduler.is_active():
-
                 try:
                     newly_collected_reports = []
                     n_new_tasks = session.config["n_workers"] - len(running_tasks)
 
                     ready_tasks = (
                         list(session.scheduler.get_ready(n_new_tasks))
                         if n_new_tasks >= 1
@@ -153,22 +150,18 @@
                     break
 
         return True
     return None
 
 
 def _parse_future_exception(
-    exception: BaseException | None,
+    exc: BaseException | None,
 ) -> tuple[type[BaseException], BaseException, TracebackType] | None:
-    """Parse a future exception."""
-    return (
-        None
-        if exception is None
-        else (type(exception), exception, exception.__traceback__)
-    )
+    """Parse a future exception into the format of ``sys.exc_info``."""
+    return None if exc is None else (type(exc), exc, exc.__traceback__)
 
 
 class ProcessesNameSpace:
     """The name space for hooks related to processes."""
 
     @staticmethod
     @hookimpl(tryfirst=True)
@@ -177,50 +170,44 @@
 
         Take a task, pickle it and send the bytes over to another process.
 
         """
         if session.config["n_workers"] > 1:
             kwargs = _create_kwargs_for_task(task)
 
-            bytes_function = cloudpickle.dumps(task)
-            bytes_kwargs = cloudpickle.dumps(kwargs)
-
             return session.config["_parallel_executor"].submit(
                 _unserialize_and_execute_task,
-                bytes_function=bytes_function,
-                bytes_kwargs=bytes_kwargs,
+                task=task,
+                kwargs=kwargs,
                 show_locals=session.config["show_locals"],
                 console_options=console.options,
                 session_filterwarnings=session.config["filterwarnings"],
                 task_filterwarnings=get_marks(task, "filterwarnings"),
                 task_short_name=task.short_name,
             )
         return None
 
 
-def _unserialize_and_execute_task(
-    bytes_function: bytes,
-    bytes_kwargs: bytes,
+def _unserialize_and_execute_task(  # noqa: PLR0913
+    task: Task,
+    kwargs: dict[str, Any],
     show_locals: bool,
     console_options: ConsoleOptions,
     session_filterwarnings: tuple[str, ...],
     task_filterwarnings: tuple[Mark, ...],
     task_short_name: str,
 ) -> tuple[list[WarningReport], tuple[type[BaseException], BaseException, str] | None]:
     """Unserialize and execute task.
 
     This function receives bytes and unpickles them to a task which is them execute in a
     spawned process or thread.
 
     """
     __tracebackhide__ = True
 
-    task = cloudpickle.loads(bytes_function)
-    kwargs = cloudpickle.loads(bytes_kwargs)
-
     with warnings.catch_warnings(record=True) as log:
         # mypy can't infer that record=True means log is not None; help it.
         assert log is not None
 
         for arg in session_filterwarnings:
             warnings.filterwarnings(*parse_warning_filter(arg, escape=False))
```

### Comparing `pytask_parallel-0.3.0/src/pytask_parallel.egg-info/PKG-INFO` & `pytask_parallel-0.3.1/src/pytask_parallel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytask-parallel
-Version: 0.3.0
+Version: 0.3.1
 Summary: Parallelize the execution of tasks with pytask.
 Home-page: https://github.com/pytask-dev/pytask-parallel
 Author: Tobias Raabe
 Author-email: raabe@posteo.de
 License: MIT
 Project-URL: Changelog, https://github.com/pytask-dev/pytask-parallel/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/pytask-dev/pytask-parallel
@@ -46,17 +46,17 @@
 $ pip install pytask-parallel
 
 # or
 
 $ conda install -c conda-forge pytask-parallel
 ```
 
-By default, the plugin uses `loky`'s robust implementation of the `ProcessPoolExecutor`.
+By default, the plugin uses `concurrent.futures.ProcessPoolExecutor`.
 
-It is also possible to select the `ProcessPoolExecutor` or `ThreadPoolExecutor` from the
+It is also possible to select the executor from loky or `ThreadPoolExecutor` from the
 [concurrent.futures](https://docs.python.org/3/library/concurrent.futures.html) module
 as backends to execute tasks asynchronously.
 
 ## Usage
 
 To parallelize your tasks across many workers, pass an integer greater than 1 or
 `'auto'` to the command-line interface.
@@ -83,15 +83,15 @@
 You can also set the options in a `pyproject.toml`.
 
 ```toml
 # This is the default configuration. Note that, parallelization is turned off.
 
 [tool.pytask.ini_options]
 n_workers = 1
-parallel_backend = "loky"  # or processes or threads
+parallel_backend = "processes"  # or loky or threads
 ```
 
 ## Some implementation details
 
 ### Parallelization and Debugging
 
 It is not possible to combine parallelization with debugging. That is why `--pdb` or
```

### Comparing `pytask_parallel-0.3.0/src/pytask_parallel.egg-info/SOURCES.txt` & `pytask_parallel-0.3.1/src/pytask_parallel.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
+.github/dependabot.yml
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/documentation.md
 .github/ISSUE_TEMPLATE/enhancement.md
 .github/ISSUE_TEMPLATE/question.md
 .github/workflows/main.yml
 .github/workflows/publish-to-pypi.yml
```

