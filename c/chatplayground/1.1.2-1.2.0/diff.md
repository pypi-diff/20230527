# Comparing `tmp/chatplayground-1.1.2.tar.gz` & `tmp/chatplayground-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatplayground-1.1.2.tar", max compression
+gzip compressed data, was "chatplayground-1.2.0.tar", max compression
```

## Comparing `chatplayground-1.1.2.tar` & `chatplayground-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-05-11 15:26:03.377943 chatplayground-1.1.2/LICENSE
--rw-r--r--   0        0        0     4574 2023-05-11 15:26:03.381943 chatplayground-1.1.2/README.md
--rw-r--r--   0        0        0       17 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/.gitignore
--rw-r--r--   0        0        0       22 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/app/__init__.py
--rw-r--r--   0        0        0   109826 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/app/app.py
--rw-r--r--   0        0        0    15406 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/assets/favicon.ico
--rw-r--r--   0        0        0     1281 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/assets/react-json-view-lite.css
--rw-r--r--   0        0        0   178190 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json
--rw-r--r--   0        0        0      921 2023-05-11 15:26:03.381943 chatplayground-1.1.2/chatplayground/pcconfig.py
--rw-r--r--   0        0        0     3081 2023-05-11 15:26:03.409944 chatplayground-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     6941 1970-01-01 00:00:00.000000 chatplayground-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-27 11:25:13.638138 chatplayground-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4574 2023-05-27 11:25:13.638138 chatplayground-1.2.0/README.md
+-rw-r--r--   0        0        0       17 2023-05-27 11:25:13.638138 chatplayground-1.2.0/chatplayground/.gitignore
+-rw-r--r--   0        0        0       22 2023-05-27 11:25:13.638138 chatplayground-1.2.0/chatplayground/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 11:25:13.638138 chatplayground-1.2.0/chatplayground/app/__init__.py
+-rw-r--r--   0        0        0   106802 2023-05-27 11:25:13.642138 chatplayground-1.2.0/chatplayground/app/app.py
+-rw-r--r--   0        0        0    15406 2023-05-27 11:25:13.642138 chatplayground-1.2.0/chatplayground/assets/favicon.ico
+-rw-r--r--   0        0        0     1281 2023-05-27 11:25:13.642138 chatplayground-1.2.0/chatplayground/assets/react-json-view-lite.css
+-rw-r--r--   0        0        0   178190 2023-05-27 11:25:13.642138 chatplayground-1.2.0/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json
+-rw-r--r--   0        0        0      921 2023-05-27 11:25:13.642138 chatplayground-1.2.0/chatplayground/pcconfig.py
+-rw-r--r--   0        0        0     3081 2023-05-27 11:25:13.670139 chatplayground-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6842 1970-01-01 00:00:00.000000 chatplayground-1.2.0/PKG-INFO
```

### Comparing `chatplayground-1.1.2/LICENSE` & `chatplayground-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.2/README.md` & `chatplayground-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.2/chatplayground/app/app.py` & `chatplayground-1.2.0/chatplayground/app/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1348,20 +1348,20 @@
     )
 
 
 def render_message_menu(message: StyledMessage):
     """Render the menu of a message."""
     return pc.popover(
         pc.popover_trigger(
-            render_tooltip(
+            # render_tooltip(
                 pc.button(
                     pc.icon(tag="hamburger"), size='xs', variant='ghost', is_disabled=EditableMessageState.is_editing
                 ),
-                label="Show the message menu with more available actions",
-            )
+            #    label="Show the message menu with more available actions",
+            # )
         ),
         pc.popover_content(
             pc.popover_arrow(),
             pc.popover_body(
                 pc.hstack(
                     # pc.button(pc.icon(tag="add"), size='xs', variant='ghost'),
                     render_tooltip(
@@ -2596,50 +2596,34 @@
     events = pc.event.fix_events([event_handler], state.get_token())
     state_update = pc.state.StateUpdate(delta={}, events=events)
     state_update_json = state_update.json()
 
     await app.sio.emit(str(pc.constants.SocketEvent.EVENT), state_update_json, to=state.get_sid(), namespace="/event")
 
 
-class PartialResponsePayload(typing.TypedDict):
-    """The payload of a partial response from the receiver thread."""
-
-    uid: str
-    content: str
-
-
 def run_coroutine_in_thread(coroutine, *args, **kwargs):
     """Run a coroutine in a separate thread.
 
     TODO(black): this is part of a workaround to get around the fact that the events are being dropped when using
         app.sio.emit.
     """
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     asyncio.run(coroutine(*args, **kwargs))
 
 
 def helper_thread(coroutine, *args, **kwargs):
-    """Trying to fix issues with streaming messages.
-
-    Events keep getting dropped, so I've tried various things to fix it.
-
-    This is the latest attempt, which is to run the coroutine in a separate thread and use a barrier
-    and minimum delays. Sadly, this is a lot more of a hack than I'd like.
-    """
+    """Trying to fix issues with streaming messages."""
     t = threading.Thread(target=run_coroutine_in_thread, args=(coroutine, *args), kwargs=kwargs)
     t.start()
 
 
 class ModelRequestsState(State):
     """The state for LLM requests."""
 
-    # TODO: this is a hack to get around the fact that the events are being dropped when using app.sio.emit.
-    _request_barrier = threading.Barrier(2)
-
     model_type: str = "GPT-3.5"
     temperature: float = 0.7
     max_tokens: int = 512
     top_p: float = 1.0
     frequency_penalty: float = 0.0
     presence_penalty: float = 0.0
 
@@ -2677,67 +2661,56 @@
         if self._active_message is None:
             return
         self._active_message.error = "Canceled by user."
         self._active_message = None
         self._update_message_exploration_registry(self)
         self.mark_dirty()
 
-    def receive_partial_response(self, payload_str: str):
-        """Receive a partial response from the receiver thread.
-
-        We currently use a barrier to sync the different threads to avoid messages being dropped.
+    def receive_finish(self, uid: str):
+        """Receive a finish message from the receiver thread."""
+        # parse uid
+        uid = json.loads(uid)
+        if self._active_message is None or self._active_message.uid != uid:
+            return
 
-        Maybe adding a delay of 50ms was already enough, but I don't trust it anymore and don't want to have any
-        dropped words anymore.
+        self._active_message = None
+        self._update_message_exploration_registry(self)
+        self.mark_dirty()
 
-        TODO(blackhc): split a receive_finished_response method out of this (content="None" means finished).
-        """
-        # parse payload_str into a PartialResponsePayload using json.loads
-        payload: PartialResponsePayload = json.loads(payload_str)
+    def receive_partial_response(self, uid: str):
+        """Receive a partial response from the receiver thread."""
+        # parse uid
+        uid = json.loads(uid)
 
-        if self._active_message is None or self._active_message.uid != payload['uid']:
+        if self._active_message is None or self._active_message.uid != uid:
             return
 
-        if payload['content'] is None:
-            self._active_message = None
-            self._update_message_exploration_registry(self)
-        else:
-            assert isinstance(payload['content'], str)
-            assert self._active_message.content is not None
-            self._active_message.content += payload['content']
-
-            last_updated = message_explorations_singleton.get_last_updated_timestamp(self.message_exploration_uid)
-            # This seems to slow down the app too much
-            if last_updated + 1 < time.time():
-                self._update_message_exploration_registry(self)  # type: ignore
+        last_updated = message_explorations_singleton.get_last_updated_timestamp(self.message_exploration_uid)
+        # This seems to slow down the app too much
+        if last_updated + 1 < time.time():
+            self._update_message_exploration_registry(self)  # type: ignore
         self.mark_dirty()
 
-        # Signal to the other thread that we're done. (If this times out, that's not bad by itself.)
-        try:
-            self._request_barrier.wait(timeout=0.1)
-        except threading.BrokenBarrierError:
-            pass
-
-    def receive_error(self, payload_str: str):
+    def receive_error(self, uid: str):
         """Receive an error from the receiver thread."""
-        # parse payload_str into a PartialResponsePayload using json.loads
-        payload: PartialResponsePayload = json.loads(payload_str)
+        # parse uid
+        uid = json.loads(uid)
 
-        if self._active_message is None or self._active_message.uid != payload['uid']:
+        if self._active_message is None or self._active_message.uid != uid:
             return
 
-        self._active_message.error = payload['content']
         self._active_message = None
         self._update_message_exploration_registry(self)  # type: ignore
         self.mark_dirty()
 
-    async def _query_openai(self, active_message, openai_messages):
+    async def _query_openai(self, active_message: Message, openai_messages):
         try:
             response = await active_message.source.query_openai(openai_messages)
-            residual_content = ""
+            content = ""
+            last_timestamp = time.time()
             async with aclosing(response):
                 async for partial_response in response:
                     if self._active_message is None or self._active_message.uid != active_message.uid:
                         return
 
                     # finish reason?
                     if partial_response['choices'][0]['finish_reason'] == 'stop':
@@ -2747,89 +2720,49 @@
 
                     if 'role' in delta:
                         assert delta['role'] == 'assistant'
 
                     if 'content' not in delta:
                         continue
 
-                    content = residual_content + delta['content']
+                    content += delta['content']
+
+                    if last_timestamp + 1/30 > time.time():
+                        continue
+                    last_timestamp = time.time()
+
+                    active_message.content = content
+
                     # noinspection PyNoneFunctionAssignment,PyArgumentList
                     event_handler: pc.event.EventHandler = ModelRequestsState.receive_partial_response(  # type: ignore
-                        PartialResponsePayload(
-                            uid=active_message.uid,
-                            content=content,
-                        )
+                        active_message.uid
                     )
                     await send_event(self, event_handler)
 
-                    try:
-                        self._request_barrier.wait(timeout=1.0)
-                        residual_content = ""
-                    except threading.BrokenBarrierError:
-                        residual_content += content
-                        self._request_barrier = threading.Barrier(2)
-
-                    # Minimum wait time to avoid dropped packets.
-                    await asyncio.sleep(0.01)
-
-            # Make sure any residual content is still sent.
-            while residual_content:
-                if self._active_message is None or self._active_message.uid != active_message.uid:
-                    return
-                # noinspection PyNoneFunctionAssignment,PyArgumentList
-                event_handler: pc.event.EventHandler = ModelRequestsState.receive_partial_response(  # type: ignore
-                    PartialResponsePayload(
-                        uid=active_message.uid,
-                        content=content,
-                    )
-                )
-                await send_event(self, event_handler)
-
-                try:
-                    self._request_barrier.wait(timeout=1.0)
-                except threading.BrokenBarrierError:
-                    self._request_barrier = threading.Barrier(2)
-                else:
-                    break
-
-                await asyncio.sleep(0.01)
-
             # noinspection PyNoneFunctionAssignment,PyArgumentList
-            event_handler: pc.event.EventHandler = ModelRequestsState.receive_partial_response(  # type: ignore
-                PartialResponsePayload(
-                    uid=active_message.uid,
-                    content=None,
-                )
+            event_handler: pc.event.EventHandler = ModelRequestsState.receive_finish(  # type: ignore
+                active_message.uid
             )
-            while True:
+
+            while self._active_message is not None and self._active_message.uid == active_message.uid:
                 await send_event(self, event_handler)
-                try:
-                    self._request_barrier.wait(timeout=1.0)
-                except threading.BrokenBarrierError:
-                    pass
-                else:
-                    break
+                await asyncio.sleep(0.1)
 
-                await asyncio.sleep(0.01)
         except asyncio.TimeoutError:
             # noinspection PyNoneFunctionAssignment,PyArgumentList
+            active_message.error = "Request Timeout Error"
             event_handler: pc.event.EventHandler = ModelRequestsState.receive_error(  # type: ignore
-                PartialResponsePayload(
-                    uid=active_message.uid,
-                    content="Request Timeout Error",
-                )
+                active_message.uid,
             )
             await send_event(self, event_handler)
         except Exception as e:
             # noinspection PyNoneFunctionAssignment,PyArgumentList
+            active_message.error = str(e)
             event_handler: pc.event.EventHandler = ModelRequestsState.receive_error(  # type: ignore
-                PartialResponsePayload(
-                    uid=active_message.uid,
-                    content=str(e),
-                )
+                active_message.uid
             )
             await send_event(self, event_handler)
             raise
 
     def _request_chat_model_completion(self):
         """Helper function to request a chat model completion."""
         active_message = Message(
```

### Comparing `chatplayground-1.1.2/chatplayground/assets/favicon.ico` & `chatplayground-1.2.0/chatplayground/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.2/chatplayground/assets/react-json-view-lite.css` & `chatplayground-1.2.0/chatplayground/assets/react-json-view-lite.css`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.2/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json` & `chatplayground-1.2.0/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.2/chatplayground/pcconfig.py` & `chatplayground-1.2.0/chatplayground/pcconfig.py`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.2/pyproject.toml` & `chatplayground-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatplayground"
-version = "1.1.2"
+version = "1.2.0"
 homepage = "https://github.com/blackhc/chatplayground"
 description = "ChatPlayground for LLMs"
 authors = ["Andreas Kirsch <blackhc@gmail.com>"]
 readme = "README.md"
 license =  "GPL-3.0-only"
 classifiers=[
     'Development Status :: 4 - Beta',
```

### Comparing `chatplayground-1.1.2/PKG-INFO` & `chatplayground-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: chatplayground
-Version: 1.1.2
+Version: 1.2.0
 Summary: ChatPlayground for LLMs
 Home-page: https://github.com/blackhc/chatplayground
 License: GPL-3.0-only
 Author: Andreas Kirsch
 Author-email: blackhc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: black (>=22.12.0,<23.0.0) ; extra == "test"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: click (==8.0.1)
 Requires-Dist: flake8 (>=6.0.0,<7.0.0) ; extra == "test"
```

