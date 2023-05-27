# Comparing `tmp/chatai-agent-0.0.1.tar.gz` & `tmp/chatai-agent-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatai-agent-0.0.1.tar", last modified: Wed May 24 13:48:50 2023, max compression
+gzip compressed data, was "chatai-agent-1.0.0.tar", last modified: Sat May 27 02:05:35 2023, max compression
```

## Comparing `chatai-agent-0.0.1.tar` & `chatai-agent-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-24 13:48:50.103826 chatai-agent-0.0.1/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-21 01:45:14.000000 chatai-agent-0.0.1/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-05-24 13:48:50.103826 chatai-agent-0.0.1/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     5990 2023-05-24 13:48:34.000000 chatai-agent-0.0.1/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-05-24 13:48:50.103826 chatai-agent-0.0.1/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1176 2023-05-24 13:48:34.000000 chatai-agent-0.0.1/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-24 13:48:50.103826 chatai-agent-0.0.1/src/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3120 2023-05-24 13:48:34.000000 chatai-agent-0.0.1/src/ChatAIAgent.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       49 2023-05-24 13:48:34.000000 chatai-agent-0.0.1/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-24 13:48:50.103826 chatai-agent-0.0.1/src/chatai_agent.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-05-24 13:48:50.000000 chatai-agent-0.0.1/src/chatai_agent.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      299 2023-05-24 13:48:50.000000 chatai-agent-0.0.1/src/chatai_agent.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-24 13:48:50.000000 chatai-agent-0.0.1/src/chatai_agent.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-24 13:48:50.000000 chatai-agent-0.0.1/src/chatai_agent.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-05-24 13:48:50.000000 chatai-agent-0.0.1/src/chatai_agent.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       21 2023-05-24 13:48:50.000000 chatai-agent-0.0.1/src/chatai_agent.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 02:05:35.172859 chatai-agent-1.0.0/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-21 01:45:14.000000 chatai-agent-1.0.0/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-05-27 02:05:35.172859 chatai-agent-1.0.0/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     6097 2023-05-27 02:04:52.000000 chatai-agent-1.0.0/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-05-27 02:05:35.172859 chatai-agent-1.0.0/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1176 2023-05-27 02:04:52.000000 chatai-agent-1.0.0/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 02:05:35.172859 chatai-agent-1.0.0/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3230 2023-05-27 02:04:52.000000 chatai-agent-1.0.0/src/ChatAIAgent.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       49 2023-05-27 02:04:52.000000 chatai-agent-1.0.0/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 02:05:35.172859 chatai-agent-1.0.0/src/chatai_agent.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      609 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      299 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       21 2023-05-27 02:05:35.000000 chatai-agent-1.0.0/src/chatai_agent.egg-info/top_level.txt
```

### Comparing `chatai-agent-0.0.1/LICENSE` & `chatai-agent-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatai-agent-0.0.1/PKG-INFO` & `chatai-agent-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-agent
-Version: 0.0.1
+Version: 1.0.0
 Summary: Send messages to ChatGPT and get answers conveniently.
 Home-page: https://github.com/GeneralYadoc/ChatAIAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chatai-agent-0.0.1/README.md` & `chatai-agent-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-# StreamChatAgent
+# ChatAIAgent
 Message broker between user and ChatGPT.
 
 ## The user of this library can
 - easily give role and messages to ChatGPT, and obtain answers.
 - spool messages which given before ChatGPT finish generating current answer.
 
 ## Hou to install
+
+### Install from PyPI
+- Install package to your environment.<br>
+    ```install
+    $ pip install chatai-agent
+    ```
+
+### Install from GitHub repository
 - Clone this repository.<br>
   ```clone
   $ clone https://github.com/GeneralYadoc/ChatAIAgent.git
   ```
 - Change directory to the root of the repository.<br>
   ```cd
   $ cd ChatAIAgent
@@ -42,19 +50,22 @@
   # ChatGPT API Key is given from command line in this example.
   if len(sys.argv) <= 1:
     exit(0)
 
   system_role="You are a cheerful assistant who speek English and can get conversation exciting with user."
 
   # Create ChatAIAgent instance.
-  agent = ca.ChatAIAgent( api_key=sys.argv[1],
-                          system_role=system_role,
-                          ask_cb=ask_cb,
-                          answer_cb=answer_cb,
-                          max_tokens_per_request = 2048 )
+  params = ca.params(
+    api_key=sys.argv[1],
+    system_role=system_role,
+    ask_cb=ask_cb,
+    answer_cb=answer_cb,
+    max_tokens_per_request = 2048
+  )
+  agent = ca.ChatAIAgent( params )
 
   # Wake up internal thread on which ChatGPT answer messages will be generated.
   agent.start()
 
   while True:
     message = input("")
     if message == "":
@@ -83,16 +94,16 @@
 
   Would you make sound of a cat?
 
   [question 17:31:14] Would you make sound of a cat?
 
   [answer 17:31:16] Meow! Meow! That's the sound a cat makes. Is there anything else you would like me to assist you with?
     ```
-## Arguments of Constractor
-- StreamChatAgent object can be configured with following arguments of its constractor.
+## Arguments of Constructor
+- ChatAIAgent object can be configured with following params given to constructor.
 
     | name | description | default |
     |------|------------|---------|
     | api_key | API Key string of OpenAI | - |
     | system_role | API Key string of OpenAI | - |
     | ask_cb | user message given to ChatGPT is thrown to this callback | None |
     | max_messages_in_context | Max messages in context given to ChatGPT | 20 |
```

### Comparing `chatai-agent-0.0.1/setup.py` & `chatai-agent-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="chatai-agent",
-    version="0.0.1",
+    version="1.0.0",
     license="MIT",
     description="Send messages to ChatGPT and get answers conveniently.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `chatai-agent-0.0.1/src/ChatAIAgent.py` & `chatai-agent-1.0.0/src/ChatAIAgent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 import queue
 import time
 import math
+from typing import Callable
+from dataclasses import dataclass
 import threading
 import openai
 
+@dataclass
 class userMessage:
-  def __init__(self, message, extern=None):
-    self.message = message
-    self.extern = extern
+  message: str = ""
+  extern: any = None
+
+@dataclass
+class params:
+  api_key: str
+  system_role: str = "You are a helpful assistant."
+  ask_cb: Callable[[userMessage,], None] = None
+  max_messages_in_context: int = 20
+  answer_cb: Callable[[userMessage, any], None] = None
+  max_queue_size: int = 10
+  model: str = 'gpt-3.5-turbo'
+  max_tokens_per_request: int = 256
+  interval_sec: float = 20.0
 
 class ChatAIAgent(threading.Thread):
-  def __init__( self,
-                api_key="",
-                system_role = "You are a helpful assistant.",
-                ask_cb=None,
-                max_messages_in_context=20,
-                answer_cb=None,
-                max_queue_size=10,
-                model = 'gpt-3.5-turbo',
-                max_tokens_per_request = 256,
-                interval_sec=20.0 ):
-    self.__user_message_queue = queue.Queue(maxsize=max_queue_size)
-    openai.api_key = api_key
-    self.__current_context = [{"role": "system", "content": system_role}]
-    self.__ask_cb = ask_cb
-    self.__max_messages_in_context = max_messages_in_context
-    self.__interval_sec=interval_sec
-    self.__answer_cb = answer_cb
-    self.__model = model
-    self.__max_tokens_per_request = max_tokens_per_request
+  def __init__( self, params ):
+    self.__user_message_queue = queue.Queue(maxsize=params.max_queue_size)
+    openai.api_key = params.api_key
+    self.__current_context = [{"role": "system", "content": params.system_role}]
+    self.__ask_cb = params.ask_cb
+    self.__max_messages_in_context = params.max_messages_in_context
+    self.__interval_sec=params.interval_sec
+    self.__answer_cb = params.answer_cb
+    self.__model = params.model
+    self.__max_tokens_per_request = params.max_tokens_per_request
     self.__keeping_connection = False
     super(ChatAIAgent, self).__init__(daemon=True)
 
   def connect(self):
     self.start()
     self.join()
 
@@ -58,19 +63,20 @@
         completion = None
         while self.__keeping_connection and not completion:
           try:
             completion = openai.ChatCompletion.create(model=self.__model, max_tokens=self.__max_tokens_per_request, messages=self.__current_context)
           except:
             completion = None
           time.sleep(0.1)
-        if self.__answer_cb and completion:
-          self.__answer_cb(user_message=user_message, completion=completion)
-        self.__current_context.append({"role": "assistant", "content": completion.choices[0]["message"]["content"]})
-        if len(self.__current_context) >= self.__max_messages_in_context:
-          self.__current_context.pop(1)
+        if completion:
+          if self.__answer_cb:
+            self.__answer_cb(user_message=user_message, completion=completion)
+          self.__current_context.append({"role": "assistant", "content": completion.choices[0]["message"]["content"]})
+          if len(self.__current_context) >= self.__max_messages_in_context:
+            self.__current_context.pop(1)
         self.__sleep_from(start_time)
         start_time = time.time()
 
   def __sleep_from(self, start_time, interval_sec=None):
     if not interval_sec:
       interval_sec = self.__interval_sec
     cur_time = time.time()
```

### Comparing `chatai-agent-0.0.1/src/chatai_agent.egg-info/PKG-INFO` & `chatai-agent-1.0.0/src/chatai_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatai-agent
-Version: 0.0.1
+Version: 1.0.0
 Summary: Send messages to ChatGPT and get answers conveniently.
 Home-page: https://github.com/GeneralYadoc/ChatAIAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

