# Comparing `tmp/streamchat-agent-1.0.0.tar.gz` & `tmp/streamchat-agent-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamchat-agent-1.0.0.tar", last modified: Sat May 27 00:43:04 2023, max compression
+gzip compressed data, was "streamchat-agent-1.0.1.tar", last modified: Sat May 27 15:21:05 2023, max compression
```

## Comparing `streamchat-agent-1.0.0.tar` & `streamchat-agent-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 00:43:04.502859 streamchat-agent-1.0.0/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-27 00:41:12.000000 streamchat-agent-1.0.0/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       24 2023-05-27 00:41:12.000000 streamchat-agent-1.0.0/MANIFEST.in
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-05-27 00:43:04.502859 streamchat-agent-1.0.0/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     5588 2023-05-27 00:41:34.000000 streamchat-agent-1.0.0/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       14 2023-05-27 00:41:12.000000 streamchat-agent-1.0.0/requirements.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-05-27 00:43:04.502859 streamchat-agent-1.0.0/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1177 2023-05-27 00:41:34.000000 streamchat-agent-1.0.0/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 00:43:04.502859 streamchat-agent-1.0.0/src/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3351 2023-05-27 00:41:34.000000 streamchat-agent-1.0.0/src/StreamChatAgent.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       53 2023-05-27 00:41:34.000000 streamchat-agent-1.0.0/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 00:43:04.502859 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      356 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       25 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 15:21:05.367494 streamchat-agent-1.0.1/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-27 00:41:12.000000 streamchat-agent-1.0.1/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       24 2023-05-27 00:41:12.000000 streamchat-agent-1.0.1/MANIFEST.in
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-05-27 15:21:05.367494 streamchat-agent-1.0.1/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     5590 2023-05-27 15:05:43.000000 streamchat-agent-1.0.1/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       14 2023-05-27 00:41:12.000000 streamchat-agent-1.0.1/requirements.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-05-27 15:21:05.367494 streamchat-agent-1.0.1/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1177 2023-05-27 15:02:40.000000 streamchat-agent-1.0.1/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 15:21:05.367494 streamchat-agent-1.0.1/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3381 2023-05-27 14:35:40.000000 streamchat-agent-1.0.1/src/StreamChatAgent.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       53 2023-05-27 15:03:02.000000 streamchat-agent-1.0.1/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 15:21:05.367494 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      356 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       25 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/top_level.txt
```

### Comparing `streamchat-agent-1.0.0/LICENSE` & `streamchat-agent-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamchat-agent-1.0.0/PKG-INFO` & `streamchat-agent-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamchat-agent
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get YouTube chat comments with minimum time lag
 Home-page: https://github.com/GeneralYadoc/StreamChatAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `streamchat-agent-1.0.0/README.md` & `streamchat-agent-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -91,20 +91,20 @@
     ```output
     % python3 ./sample.py MB57rMXXXXs
     2023-05-19 05:21:26 [John]- Hello!
     2023-05-19 05:21:27 [Kelly]- Hello everyone!
     2023-05-19 05:21:27 [Taro]- Welcome to our stream.
     ```
 ## Params given to Constructor
-- StreamChatAgent object can be configured with following arguments of its constractor.
+- StreamChatAgent object can be configured with following params given to constructor.
 
     | name | description | default |
     |------|------------|---------|
     | video_id | String following after 'v=' in url of target YouTube live | - |
-    | get_item_cb | Chat items are thrown to this callback | - |
+    | get_item_cb | Chat items are thrown to this callback | None |
     | pre_filter_cb | Filter set before internal queue | None |
     | post_filter_cb | Filter set between internal queue and get_item_cb | None |
     | max_queue_size | Max slots of internal queue (0 is no limit) | 1000 |
     | interval_sec | Polling interval of picking up items from YouTube | 0.01 \[sec\] | 
 
 ## Methods
 ### start()
```

### Comparing `streamchat-agent-1.0.0/setup.py` & `streamchat-agent-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="streamchat-agent",
-    version="1.0.0",
+    version="1.0.1",
     license="MIT",
     description="Get YouTube chat comments with minimum time lag",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `streamchat-agent-1.0.0/src/StreamChatAgent.py` & `streamchat-agent-1.0.1/src/StreamChatAgent.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytchat
 from typing import Callable
 from dataclasses import dataclass
 
 @dataclass
 class params:
   video_id: str
-  get_item_cb: Callable[[any,],None]
+  get_item_cb: Callable[[any,],None] = None
   pre_filter_cb: Callable[[any,],any] = None
   post_filter_cb: Callable[[any,],any] = None
   max_queue_size: int = 1000
   interval_sec: float = 0.01
 
 class StreamChatAgent(threading.Thread):
   def __init__( self, params ):
@@ -87,15 +87,15 @@
     start_time = time.time()
     while self.__is_alive(immediate=False):
       while self.__keeping_connection and not self.__item_queue.empty():
         c = self.__item_queue.get()
         postfiltered_c = c
         if self.__post_filter_cb:
           postfiltered_c = self.__post_filter_cb(c)
-        if postfiltered_c:
+        if postfiltered_c and self.__get_item_cb:
           self.__get_item_cb(postfiltered_c)
       self.__sleep_from(start_time, 0.01)
       start_time = time.time()
     self.__keeping_connection = False
 
   def __sleep_from(self, start_time, interval_sec=None):
     if not interval_sec:
```

### Comparing `streamchat-agent-1.0.0/src/streamchat_agent.egg-info/PKG-INFO` & `streamchat-agent-1.0.1/src/streamchat_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamchat-agent
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get YouTube chat comments with minimum time lag
 Home-page: https://github.com/GeneralYadoc/StreamChatAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

