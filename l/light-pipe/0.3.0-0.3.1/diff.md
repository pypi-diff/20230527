# Comparing `tmp/light-pipe-0.3.0.tar.gz` & `tmp/light-pipe-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "light-pipe-0.3.0.tar", last modified: Fri May 26 21:15:57 2023, max compression
+gzip compressed data, was "light-pipe-0.3.1.tar", last modified: Sat May 27 19:28:29 2023, max compression
```

## Comparing `light-pipe-0.3.0.tar` & `light-pipe-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-26 21:15:57.307282 light-pipe-0.3.0/
--rw-r--r--   0 richardcorrero   (501) staff       (20)     1465 2022-12-24 21:34:11.000000 light-pipe-0.3.0/LICENSE
-drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-26 21:15:57.294447 light-pipe-0.3.0/Light_Pipe.egg-info/
--rw-r--r--   0 richardcorrero   (501) staff       (20)     1100 2023-05-26 21:15:57.000000 light-pipe-0.3.0/Light_Pipe.egg-info/PKG-INFO
--rw-r--r--   0 richardcorrero   (501) staff       (20)      446 2023-05-26 21:15:57.000000 light-pipe-0.3.0/Light_Pipe.egg-info/SOURCES.txt
--rw-r--r--   0 richardcorrero   (501) staff       (20)        1 2023-05-26 21:15:57.000000 light-pipe-0.3.0/Light_Pipe.egg-info/dependency_links.txt
--rw-r--r--   0 richardcorrero   (501) staff       (20)       11 2023-05-26 21:15:57.000000 light-pipe-0.3.0/Light_Pipe.egg-info/top_level.txt
--rw-r--r--   0 richardcorrero   (501) staff       (20)     1100 2023-05-26 21:15:57.306588 light-pipe-0.3.0/PKG-INFO
--rw-r--r--   0 richardcorrero   (501) staff       (20)     1915 2023-05-26 21:13:35.000000 light-pipe-0.3.0/README.md
-drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-26 21:15:57.302267 light-pipe-0.3.0/light_pipe/
--rw-r--r--   0 richardcorrero   (501) staff       (20)     1171 2023-02-06 18:59:25.000000 light-pipe-0.3.0/light_pipe/__init__.py
--rw-r--r--   0 richardcorrero   (501) staff       (20)     3680 2023-05-26 19:43:35.000000 light-pipe-0.3.0/light_pipe/data.py
--rw-r--r--   0 richardcorrero   (501) staff       (20)    11386 2023-05-26 20:48:32.000000 light-pipe-0.3.0/light_pipe/parallelizer.py
--rw-r--r--   0 richardcorrero   (501) staff       (20)     4083 2023-05-26 20:51:46.000000 light-pipe-0.3.0/light_pipe/transformer.py
--rw-r--r--   0 richardcorrero   (501) staff       (20)       38 2023-05-26 21:15:57.307397 light-pipe-0.3.0/setup.cfg
--rw-r--r--   0 richardcorrero   (501) staff       (20)     1180 2023-05-26 21:15:10.000000 light-pipe-0.3.0/setup.py
-drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-26 21:15:57.304593 light-pipe-0.3.0/tests/
--rw-r--r--   0 richardcorrero   (501) staff       (20)     2103 2023-05-26 19:58:45.000000 light-pipe-0.3.0/tests/test_parallelizer.py
--rw-r--r--   0 richardcorrero   (501) staff       (20)     1313 2023-05-26 19:58:49.000000 light-pipe-0.3.0/tests/test_transformer.py
+drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-27 19:28:29.761559 light-pipe-0.3.1/
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1465 2022-12-24 21:34:11.000000 light-pipe-0.3.1/LICENSE
+drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-27 19:28:29.756027 light-pipe-0.3.1/Light_Pipe.egg-info/
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1099 2023-05-27 19:28:29.000000 light-pipe-0.3.1/Light_Pipe.egg-info/PKG-INFO
+-rw-r--r--   0 richardcorrero   (501) staff       (20)      446 2023-05-27 19:28:29.000000 light-pipe-0.3.1/Light_Pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 richardcorrero   (501) staff       (20)        1 2023-05-27 19:28:29.000000 light-pipe-0.3.1/Light_Pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 richardcorrero   (501) staff       (20)       11 2023-05-27 19:28:29.000000 light-pipe-0.3.1/Light_Pipe.egg-info/top_level.txt
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1099 2023-05-27 19:28:29.760797 light-pipe-0.3.1/PKG-INFO
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     2703 2023-05-27 19:08:03.000000 light-pipe-0.3.1/README.md
+drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-27 19:28:29.758197 light-pipe-0.3.1/light_pipe/
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     2860 2023-05-27 19:09:18.000000 light-pipe-0.3.1/light_pipe/__init__.py
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     3758 2023-05-27 15:46:32.000000 light-pipe-0.3.1/light_pipe/data.py
+-rw-r--r--   0 richardcorrero   (501) staff       (20)    19299 2023-05-27 19:25:58.000000 light-pipe-0.3.1/light_pipe/parallelizer.py
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     5000 2023-05-27 17:11:27.000000 light-pipe-0.3.1/light_pipe/transformer.py
+-rw-r--r--   0 richardcorrero   (501) staff       (20)       38 2023-05-27 19:28:29.761665 light-pipe-0.3.1/setup.cfg
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1179 2023-05-27 19:10:05.000000 light-pipe-0.3.1/setup.py
+drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-27 19:28:29.760269 light-pipe-0.3.1/tests/
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     2129 2023-05-27 19:27:39.000000 light-pipe-0.3.1/tests/test_parallelizer.py
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1313 2023-05-27 19:27:46.000000 light-pipe-0.3.1/tests/test_transformer.py
```

### Comparing `light-pipe-0.3.0/LICENSE` & `light-pipe-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `light-pipe-0.3.0/Light_Pipe.egg-info/PKG-INFO` & `light-pipe-0.3.1/Light_Pipe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: light-pipe
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/rcorrero/light-pipe
 Author: Richard Correro
 Author-email: richard@richardcorrero.com
 License: BSD 3-Clause
 License-File: LICENSE
 
 
-        Light-Pipe makes data processing pipeline development quick and painless. It is an extensible, light-weight Python framework for data pipelines that scale effortlessly, with zero non-standard dependencies. It abstracts away the implementation details of the pipeline itself, meaning that the developer only has to define the transformations performed within the pipeline on individual units of data.
+        Light-Pipe makes data processing pipeline development quick and painless. It is an extensible, light-weight Python framework with zero non-standard dependencies for data pipelines that scale effortlessly. It abstracts away the implementation details of the pipeline itself, meaning that the developer only has to define the transformations performed within the pipeline on individual units of data.
 
         Pipelines defined using Light-Pipe scale effortlessly, with native support for all forms of concurrency, allowing for the mixing and matching of asynchronous, multi-threaded, and multi-process operations all within a single pipeline. It's also super fast and efficient, having been used to perform critical geospatial data processing tasks at least an order of magnitude faster than existing systems.
 
         Light-Pipe is released under a BSD-3-Clause License.
```

### Comparing `light-pipe-0.3.0/PKG-INFO` & `light-pipe-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: light-pipe
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/rcorrero/light-pipe
 Author: Richard Correro
 Author-email: richard@richardcorrero.com
 License: BSD 3-Clause
 License-File: LICENSE
 
 
-        Light-Pipe makes data processing pipeline development quick and painless. It is an extensible, light-weight Python framework for data pipelines that scale effortlessly, with zero non-standard dependencies. It abstracts away the implementation details of the pipeline itself, meaning that the developer only has to define the transformations performed within the pipeline on individual units of data.
+        Light-Pipe makes data processing pipeline development quick and painless. It is an extensible, light-weight Python framework with zero non-standard dependencies for data pipelines that scale effortlessly. It abstracts away the implementation details of the pipeline itself, meaning that the developer only has to define the transformations performed within the pipeline on individual units of data.
 
         Pipelines defined using Light-Pipe scale effortlessly, with native support for all forms of concurrency, allowing for the mixing and matching of asynchronous, multi-threaded, and multi-process operations all within a single pipeline. It's also super fast and efficient, having been used to perform critical geospatial data processing tasks at least an order of magnitude faster than existing systems.
 
         Light-Pipe is released under a BSD-3-Clause License.
```

### Comparing `light-pipe-0.3.0/README.md` & `light-pipe-0.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # [Light-Pipe](https://github.com/rcorrero/light-pipe)
 
 ---
 
 ## Overview
 
-[Light-Pipe](https://www.light-pipe.io/) makes data processing pipeline development quick and painless. It is an extensible, light-weight Python framework for data pipelines that scale effortlessly, with zero non-standard dependencies. It abstracts away the implementation details of the pipeline itself, meaning that the developer only has to define the transformations performed within the pipeline on individual units of data.
+[Light-Pipe](https://www.light-pipe.io/) makes data processing pipeline development quick and painless. It is an extensible, light-weight Python framework with zero non-standard dependencies for data pipelines that scale effortlessly. It abstracts away the implementation details of the pipeline itself, meaning that the developer only has to define the transformations performed within the pipeline on individual units of data.
 
 Pipelines defined using Light-Pipe scale effortlessly, with native support for all forms of concurrency, allowing for the mixing and matching of asynchronous, multi-threaded, and multi-process operations all within a single pipeline. It's also super fast and efficient, having been used to perform critical geospatial data processing tasks [at least an order of magnitude faster than existing systems](https://github.com/rcorrero/light-pipe/blob/depth_first/data/plots/test_geo_tiling.png).
 
 Light-Pipe is released under a [BSD-3-Clause License](https://opensource.org/licenses/BSD-3-Clause).
 
-## Basic Example
+## Installing Light-Pipe
+
+```
+pip install light-pipe
+```
+
+## A Basic Example
 
 ```
 >>> from light_pipe import make_data, make_transformer
 >>> 
 >>> 
 >>> @make_data
 >>> def gen_dicts(x: int):
@@ -40,14 +46,52 @@
 Third: 8
 [2, 5, 8]
 >>>
 >>> print(data(block=True))
 [2, 5, 8]
 ```
 
+## A (Slightly) More Interesting Example
+
+```
+>>> import asyncio
+>>> import time
+>>> 
+>>> from light_pipe import AsyncGatherer, make_data, make_transformer
+>>> 
+>>> 
+>>> @make_data
+>>> def gen(x: int):
+>>>     yield from range(x)
+>>> 
+>>> 
+>>> @make_transformer
+>>> async def add_one(x: int):
+>>>     await asyncio.sleep(1)
+>>>     return x + 1
+>>> 
+>>> 
+>>> data = gen(x=8)
+>>> 
+>>> t = add_one(parallelizer=AsyncGatherer())
+>>> 
+>>> 
+>>> for _ in range(10):
+>>>     data >> t
+>>> 
+>>> start = time.time()
+>>> print(data(block=True))
+[12, 10, 14, 11, 16, 15, 13, 17]
+>>> 
+>>> end = time.time()
+>>> diff = end - start
+>>> print(f"Total time to execute tasks: {diff:.1f} seconds.")
+Total time to execute tasks: 10.0 seconds.
+```
+
 ## More Information
 
 - [GitHub](https://github.com/rcorrero/light-pipe)
 
 - [Documentation](https://www.light-pipe.io/)
 
 ---
```

### Comparing `light-pipe-0.3.0/light_pipe/data.py` & `light-pipe-0.3.1/light_pipe/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 __author__ = "Richard Correro (richard@richardcorrero.com)"
 
 
+import functools
 from typing import Callable, Iterable, List, Optional, Union
 
 
 class Data:
     def __init__(
         self, generator: Optional[Union[Callable, Iterable]] = None, 
         store_results: Optional[bool] = False,
@@ -108,13 +109,15 @@
         args = (*args, *self.args)
         kwargs = {**kwargs, **self.kwargs}
         return self._copy(
            *args, generator=generator, store_results=store_results, 
            _results_stored=_results_stored, **kwargs
         )
 
+
 def make_data(
-    generator: Optional[Union[Callable, Iterable]] = None
+    generator: Union[Callable, Iterable]
 ) -> Callable:
+    @functools.wraps(generator if isinstance(generator, Callable) else None)
     def data_wrapper(*args, **kwargs) -> Data:
         return Data(generator=generator, *args, **kwargs)
     return data_wrapper
```

### Comparing `light-pipe-0.3.0/setup.py` & `light-pipe-0.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 
 setup(
     name="light-pipe",
-    version="0.3.0",
+    version="0.3.1",
     long_description="""
-        Light-Pipe makes data processing pipeline development quick and painless. It is an extensible, light-weight Python framework for data pipelines that scale effortlessly, with zero non-standard dependencies. It abstracts away the implementation details of the pipeline itself, meaning that the developer only has to define the transformations performed within the pipeline on individual units of data.
+        Light-Pipe makes data processing pipeline development quick and painless. It is an extensible, light-weight Python framework with zero non-standard dependencies for data pipelines that scale effortlessly. It abstracts away the implementation details of the pipeline itself, meaning that the developer only has to define the transformations performed within the pipeline on individual units of data.
 
         Pipelines defined using Light-Pipe scale effortlessly, with native support for all forms of concurrency, allowing for the mixing and matching of asynchronous, multi-threaded, and multi-process operations all within a single pipeline. It's also super fast and efficient, having been used to perform critical geospatial data processing tasks at least an order of magnitude faster than existing systems.
 
         Light-Pipe is released under a BSD-3-Clause License.
     """,
     url="https://github.com/rcorrero/light-pipe",
     author="Richard Correro",
```

### Comparing `light-pipe-0.3.0/tests/test_parallelizer.py` & `light-pipe-0.3.1/tests/test_parallelizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         num_tasks = 1000
         iterable = gen(num_tasks=num_tasks)
 
         max_workers = 8
         queue_size = 3
         p = BlockingThreadPooler(max_workers=max_workers, queue_size=queue_size)        
         for _ in p(iterable=iterable):
-            assert num_tasks_submitted[0] <= queue_size
+            self.assertLessEqual(num_tasks_submitted[0], queue_size)
             num_tasks_submitted[0] -= 1
 
 
     def test_blocking_process_pooler(self):
         num_tasks_submitted = [0]
 
 
@@ -51,15 +51,15 @@
         num_tasks = 1000
         iterable = gen(num_tasks=num_tasks)
 
         max_workers = 8
         queue_size = 3
         p = BlockingProcessPooler(max_workers=max_workers, queue_size=queue_size)        
         for _ in p(iterable=iterable):
-            assert num_tasks_submitted[0] <= queue_size
+            self.assertLessEqual(num_tasks_submitted[0], queue_size)
             num_tasks_submitted[0] -= 1            
         
 
     def test_async_gatherer(self):
         async def sleep(seconds: int, *args, **kwargs):
             await asyncio.sleep(seconds)
```

### Comparing `light-pipe-0.3.0/tests/test_transformer.py` & `light-pipe-0.3.1/tests/test_transformer.py`

 * *Files identical despite different names*

