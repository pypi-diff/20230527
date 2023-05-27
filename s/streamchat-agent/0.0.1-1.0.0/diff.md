# Comparing `tmp/streamchat-agent-0.0.1.tar.gz` & `tmp/streamchat-agent-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamchat-agent-0.0.1.tar", last modified: Sun May 21 22:40:49 2023, max compression
+gzip compressed data, was "streamchat-agent-1.0.0.tar", last modified: Sat May 27 00:43:04 2023, max compression
```

## Comparing `streamchat-agent-0.0.1.tar` & `streamchat-agent-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-21 22:40:49.623328 streamchat-agent-0.0.1/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-21 00:56:35.000000 streamchat-agent-0.0.1/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       24 2023-05-21 00:56:35.000000 streamchat-agent-0.0.1/MANIFEST.in
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-05-21 22:40:49.623328 streamchat-agent-0.0.1/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     5386 2023-05-21 22:29:06.000000 streamchat-agent-0.0.1/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       14 2023-05-21 00:56:35.000000 streamchat-agent-0.0.1/requirements.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-05-21 22:40:49.623328 streamchat-agent-0.0.1/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1177 2023-05-21 00:56:35.000000 streamchat-agent-0.0.1/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-21 22:40:49.623328 streamchat-agent-0.0.1/src/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3211 2023-05-21 00:56:35.000000 streamchat-agent-0.0.1/src/StreamChatAgent.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       53 2023-05-21 00:56:35.000000 streamchat-agent-0.0.1/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-21 22:40:49.623328 streamchat-agent-0.0.1/src/streamchat_agent.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-05-21 22:40:49.000000 streamchat-agent-0.0.1/src/streamchat_agent.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      356 2023-05-21 22:40:49.000000 streamchat-agent-0.0.1/src/streamchat_agent.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-21 22:40:49.000000 streamchat-agent-0.0.1/src/streamchat_agent.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-21 22:40:49.000000 streamchat-agent-0.0.1/src/streamchat_agent.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-05-21 22:40:49.000000 streamchat-agent-0.0.1/src/streamchat_agent.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       25 2023-05-21 22:40:49.000000 streamchat-agent-0.0.1/src/streamchat_agent.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 00:43:04.502859 streamchat-agent-1.0.0/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-27 00:41:12.000000 streamchat-agent-1.0.0/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       24 2023-05-27 00:41:12.000000 streamchat-agent-1.0.0/MANIFEST.in
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-05-27 00:43:04.502859 streamchat-agent-1.0.0/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     5588 2023-05-27 00:41:34.000000 streamchat-agent-1.0.0/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       14 2023-05-27 00:41:12.000000 streamchat-agent-1.0.0/requirements.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-05-27 00:43:04.502859 streamchat-agent-1.0.0/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1177 2023-05-27 00:41:34.000000 streamchat-agent-1.0.0/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 00:43:04.502859 streamchat-agent-1.0.0/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3351 2023-05-27 00:41:34.000000 streamchat-agent-1.0.0/src/StreamChatAgent.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       53 2023-05-27 00:41:34.000000 streamchat-agent-1.0.0/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 00:43:04.502859 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      356 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       25 2023-05-27 00:43:04.000000 streamchat-agent-1.0.0/src/streamchat_agent.egg-info/top_level.txt
```

### Comparing `streamchat-agent-0.0.1/LICENSE` & `streamchat-agent-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamchat-agent-0.0.1/PKG-INFO` & `streamchat-agent-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamchat-agent
-Version: 0.0.1
+Version: 1.0.0
 Summary: Get YouTube chat comments with minimum time lag
 Home-page: https://github.com/GeneralYadoc/StreamChatAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `streamchat-agent-0.0.1/README.md` & `streamchat-agent-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 YouTube chat poller which can get massages very smothly by using internal queue.
 
 ## The user of this library can
 - receive YouTube chat messages continiously by registering callback.
 - natively obtain high performance by using internal queue.
 
 ## Hou to install
+You can select from following ways.
+
+### Install from PyPI
+- Install package to your environment.<br>
+    ```install
+    $ pip install streamchat-agent
+    ```
+
+### Install from GitHub repository
 - Clone this repository.<br>
     ```clone
     $ clone https://github.com/GeneralYadoc/StreamChatAgent.git
     ```
 - Change directory to the root of the repository.<br>
     ```cd
     $ cd StreamChatAgent
@@ -17,50 +26,53 @@
 - Install package to your environment.<br>
     ```install
     $ pip install .
     ```
 
 ## How to use
 
-- Sample codes
+- Sample codes exists [here](samples/sample.py)<br>
     ``` sample.py
     import sys
     import re
     import StreamChatAgent as sca  # Import this.
 
-    # callback for getting YouTube chat items
+    # callback for getting YouTube chat item
     # You can implement several processes in it.
     # This example prints datetime, ahthor name, message, of each item.
     def get_item_cb(c):
       print(f"{c.datetime} [{c.author.name}]- {c.message}")
 
     # pre putting queue filter
-    # You can edit YouTube chat items before putting internal queue.
+    # You can edit YouTube chat item before putting internal queue.
     # You can avoid putting internal queue by returning None.
-    # This example removes items whose message consists of stamps only.
+    # This example removes item whose message consists of stamps only.
     def pre_filter_cb(c):
       return None if re.match(r'^(:[^:]+:)+$', c.message) else c
 
     # post getting queue filter
-    # You can edit YouTube chat items after popping internal queue.
-    # You can avoid sending items to get_item_cb by returning None.
-    # This example removes stamps from message of items.
+    # You can edit YouTube chat item after popping internal queue.
+    # You can avoid sending item to get_item_cb by returning None.
+    # This example removes stamps from message of item.
     def post_filter_cb(c):
       c.message = re.sub(r':[^:]+:','', c.message)
       return c
 
     # Video ID is given from command line in this example.
     if len(sys.argv) <= 1:
       exit(0)
 
     # Create StreamChatAgent instance.
-    agent = sca.StreamChatAgent( video_id=sys.argv[1],
-                                 get_item_cb=get_item_cb,
-                                 pre_filter_cb=pre_filter_cb,
-                                 post_filter_cb=post_filter_cb )
+    params = sca.params(
+      video_id = sys.argv[1],
+      get_item_cb = get_item_cb,
+      pre_filter_cb = pre_filter_cb,
+      post_filter_cb = post_filter_cb
+    )
+    agent = sca.StreamChatAgent( params )
 
     # Start async getting YouTube chat items.
     # Then get_item_cb is called continuosly.
     agent.start()
 
     # Wait any key inputted from keyboad.
     input()
@@ -73,20 +85,20 @@
     agent.join()
 
     del agent
     ```
 
 - Output of the sample
     ```output
-    % ./test.py MB57rMXXXXs
+    % python3 ./sample.py MB57rMXXXXs
     2023-05-19 05:21:26 [John]- Hello!
     2023-05-19 05:21:27 [Kelly]- Hello everyone!
     2023-05-19 05:21:27 [Taro]- Welcome to our stream.
     ```
-## Arguments of Constractor
+## Params given to Constructor
 - StreamChatAgent object can be configured with following arguments of its constractor.
 
     | name | description | default |
     |------|------------|---------|
     | video_id | String following after 'v=' in url of target YouTube live | - |
     | get_item_cb | Chat items are thrown to this callback | - |
     | pre_filter_cb | Filter set before internal queue | None |
@@ -112,31 +124,30 @@
 - Request to terminate polling and calling user callbacks.
 - Internal process will be terminated soon after.
 - No arguments required, nothing returns.
 
 And other [threading.Thread](https://docs.python.org/3/library/threading.html) public pethods are available.
 
 ## Callbacks
-### get_item_callback
+### get_item_cb
 - Callback for getting YouTube chat items.
 - You can implement several processes in it.
 - YouTube chat item is thrown as an argument.
 - It's not be assumed that any values are returned.
-### pre_filter_callback
+### pre_filter_cb
 - pre putting queue filter.
 - YouTube chat item is thrown as an argument.
 - You can edit YouTube chat items before putting internal queue.
 - It's required that edited chat item is returned.
 - You can avoid putting internal queue by returning None.
-### post_filter_callback
+### post_filter_cb
 - post getting queue filter
 - You can edit YouTube chat items after popping internal queue.
 - It's required that edited chat item is returned.
-- You can avoid sending items to get_item_cb by returning None.
-
+- You can avoid sending item to get_item_cb by returning None.
 
 ## Type of YouTube Chat item
 - Please refer [pytchat README](https://github.com/taizan-hokuto/pytchat)
 
 ## Concept of design
 - Putting thread is separated from getting thread in order to avoid locking polling.<br>
 Unexpected sleep of pytchat may reduce by ths approach.
```

### Comparing `streamchat-agent-0.0.1/setup.py` & `streamchat-agent-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="streamchat-agent",
-    version="0.0.1",
+    version="1.0.0",
     license="MIT",
     description="Get YouTube chat comments with minimum time lag",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `streamchat-agent-0.0.1/src/StreamChatAgent.py` & `streamchat-agent-1.0.0/src/StreamChatAgent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import time
 import threading
 import queue
 import math
 import pytchat
+from typing import Callable
+from dataclasses import dataclass
+
+@dataclass
+class params:
+  video_id: str
+  get_item_cb: Callable[[any,],None]
+  pre_filter_cb: Callable[[any,],any] = None
+  post_filter_cb: Callable[[any,],any] = None
+  max_queue_size: int = 1000
+  interval_sec: float = 0.01
 
 class StreamChatAgent(threading.Thread):
-  def __init__( self,
-                video_id,
-                get_item_cb,
-                pre_filter_cb=None,
-                post_filter_cb=None,
-                max_queue_size=1000,
-                interval_sec=0.01 ):
-    self.__get_item_cb = get_item_cb
-    self.__pre_filter_cb = pre_filter_cb
-    self.__post_filter_cb = post_filter_cb
-    self.__item_queue = queue.Queue(max_queue_size)
-    self.__interval_sec = interval_sec
+  def __init__( self, params ):
+    self.__get_item_cb = params.get_item_cb
+    self.__pre_filter_cb = params.pre_filter_cb
+    self.__post_filter_cb = params.post_filter_cb
+    self.__item_queue = queue.Queue(params.max_queue_size)
+    self.__interval_sec = params.interval_sec
     self.__keeping_connection = False
 
-    self.__chat = pytchat.create(video_id=video_id)
+    self.__chat = pytchat.create(video_id=params.video_id)
 
     self.__my_put_thread = threading.Thread(target=self.__put_items)
     self.__my_get_thread = threading.Thread(target=self.__get_items)
 
     super(StreamChatAgent, self).__init__(daemon=True)
 
   def connect(self):
```

### Comparing `streamchat-agent-0.0.1/src/streamchat_agent.egg-info/PKG-INFO` & `streamchat-agent-1.0.0/src/streamchat_agent.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamchat-agent
-Version: 0.0.1
+Version: 1.0.0
 Summary: Get YouTube chat comments with minimum time lag
 Home-page: https://github.com/GeneralYadoc/StreamChatAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

