# Comparing `tmp/python_omnilogic_local-0.3.2.tar.gz` & `tmp/python_omnilogic_local-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.3.2.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.3.3.tar", max compression
```

## Comparing `python_omnilogic_local-0.3.2.tar` & `python_omnilogic_local-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1696 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    20177 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3931 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0        0 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     7748 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9535 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-27 13:43:41.348761 python_omnilogic_local-0.3.2/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0     7903 2023-05-27 13:43:41.352761 python_omnilogic_local-0.3.2/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6304 2023-05-27 13:43:41.352761 python_omnilogic_local-0.3.2/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-27 13:43:41.352761 python_omnilogic_local-0.3.2/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-27 13:43:42.268768 python_omnilogic_local-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    20177 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3931 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0        0 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     7748 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9535 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0     8698 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6304 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-27 14:13:25.053436 python_omnilogic_local-0.3.3/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-27 14:13:25.957430 python_omnilogic_local-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.3.3/PKG-INFO
```

### Comparing `python_omnilogic_local-0.3.2/README.md` & `python_omnilogic_local-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.2/pyomnilogic_local/api.py` & `python_omnilogic_local-0.3.3/pyomnilogic_local/api.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.2/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.3.3/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.2/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.3.3/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.2/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.3.3/pyomnilogic_local/models/mspconfig.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.2/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.3.3/pyomnilogic_local/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.2/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.3.3/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.2/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.3.3/pyomnilogic_local/protocol.py`

 * *Files 12% similar despite different names*

```diff
@@ -94,30 +94,38 @@
 
     def error_received(self, exc: Exception) -> None:
         raise exc
 
     async def _wait_for_ack(self, ack_id: int) -> None:
         message = await self.data_queue.get()
         while message.id != ack_id:
-            _LOGGER.debug("We received a message that is not our ACK, lets put it back")
-            await self.data_queue.put(message)
+            _LOGGER.debug("We received a message that is not our ACK, it appears the ACK was dropped")
+            # If the message that we received was either a LEADMESSAGE or a BLOCK MESSAGE, lets put it back and return,
+            # The Omni is continuing on with life, lets not be clingy for an ACK that was dropped and will never come
+            # We will put this new message back into the queue and stop waiting for our ACK
+            if message.type in {MessageType.MSP_LEADMESSAGE, MessageType.MSP_BLOCKMESSAGE}:
+                _LOGGER.debug("Omni has sent a new message, continuing on with the communication")
+                await self.data_queue.put(message)
+                break
+            # In theory, we should never get to this spot, but it's mostly here to cause the code to wait forever so that asyncio will
+            # eventually time out waiting for it, that way we can deal with the dropped packets
             message = await self.data_queue.get()
 
     async def _ensure_sent(self, message: OmniLogicMessage) -> None:
         delivered = False
         while not delivered:
             self.transport.sendto(bytes(message))
 
             # If the message that we just sent is an ACK, we do not need to wait to receive an ACK, we are done
             if message.type in [MessageType.XML_ACK, MessageType.ACK]:
                 return
 
             # Wait for a bit to either receive an ACK for our message, otherwise, we retry delivery
             try:
-                await asyncio.wait_for(self._wait_for_ack(message.id), 1)
+                await asyncio.wait_for(self._wait_for_ack(message.id), 0.25)
                 delivered = True
             except TimeoutError:
                 _LOGGER.debug("ACK not received, re-attempting delivery")
 
     async def send_and_receive(self, msg_type: MessageType, payload: str | None, msg_id: int | None = None) -> str:
         await self.send_message(msg_type, payload, msg_id)
         return await self._receive_file()
```

### Comparing `python_omnilogic_local-0.3.2/pyomnilogic_local/types.py` & `python_omnilogic_local-0.3.3/pyomnilogic_local/types.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.3.2/pyproject.toml` & `python_omnilogic_local-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.3.2"
+version = "0.3.3"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.3.2/PKG-INFO` & `python_omnilogic_local-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.3.2
+Version: 0.3.3
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.3.2 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.3.3 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

