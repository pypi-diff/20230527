# Comparing `tmp/homeduino-0.0.7.5.tar.gz` & `tmp/homeduino-0.0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeduino-0.0.7.5.tar", last modified: Tue May 16 23:53:55 2023, max compression
+gzip compressed data, was "homeduino-0.0.7.6.tar", last modified: Sat May 27 10:13:24 2023, max compression
```

## Comparing `homeduino-0.0.7.5.tar` & `homeduino-0.0.7.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:53:55.944230 homeduino-0.0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-16 23:53:42.000000 homeduino-0.0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 23:53:55.944230 homeduino-0.0.7.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:53:55.944230 homeduino-0.0.7.5/homeduino/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-16 23:53:42.000000 homeduino-0.0.7.5/homeduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-16 23:53:42.000000 homeduino-0.0.7.5/homeduino/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-05-16 23:53:42.000000 homeduino-0.0.7.5/homeduino/homeduino.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 23:53:55.944230 homeduino-0.0.7.5/homeduino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 23:53:55.000000 homeduino-0.0.7.5/homeduino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-16 23:53:55.000000 homeduino-0.0.7.5/homeduino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 23:53:55.000000 homeduino-0.0.7.5/homeduino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 23:53:55.000000 homeduino-0.0.7.5/homeduino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 23:53:55.000000 homeduino-0.0.7.5/homeduino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 23:53:42.000000 homeduino-0.0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 23:53:55.944230 homeduino-0.0.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:13:24.071511 homeduino-0.0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-27 10:13:10.000000 homeduino-0.0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-27 10:13:24.071511 homeduino-0.0.7.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:13:24.071511 homeduino-0.0.7.6/homeduino/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-27 10:13:10.000000 homeduino-0.0.7.6/homeduino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-27 10:13:10.000000 homeduino-0.0.7.6/homeduino/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-05-27 10:13:10.000000 homeduino-0.0.7.6/homeduino/homeduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:13:24.071511 homeduino-0.0.7.6/homeduino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-27 10:13:24.000000 homeduino-0.0.7.6/homeduino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-27 10:13:24.000000 homeduino-0.0.7.6/homeduino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:13:24.000000 homeduino-0.0.7.6/homeduino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 10:13:24.000000 homeduino-0.0.7.6/homeduino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 10:13:24.000000 homeduino-0.0.7.6/homeduino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-27 10:13:10.000000 homeduino-0.0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 10:13:24.071511 homeduino-0.0.7.6/setup.cfg
```

### Comparing `homeduino-0.0.7.5/LICENSE` & `homeduino-0.0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.7.5/PKG-INFO` & `homeduino-0.0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.7.5
+Version: 0.0.7.6
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.7.5/homeduino/__main__.py` & `homeduino-0.0.7.6/homeduino/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 @author: Rogier van Staveren
 """
 import argparse
 import asyncio
 import json
 import logging
 import sys
-import time
 
 from serial.serialutil import SerialException
 
 from homeduino import Homeduino
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `homeduino-0.0.7.5/homeduino/homeduino.py` & `homeduino-0.0.7.6/homeduino/homeduino.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 class HomeduinoProtocol(asyncio.Protocol):
     rf_receive_callbacks = []
 
     transport: SerialTransport = None
 
     ready = False
-    _tx_busy = False
+    _tx_busy_since = None
     _ack = None
 
     _str_buffer = ""
     str_buffer = deque()
 
     def __init__(
         self,
@@ -103,15 +103,15 @@
                 line = line.strip()
                 if line == "ready":
                     self.handle_ready()
                 elif line.startswith("RF receive "):
                     self.handle_rf_receive(line)
                 elif line.startswith("KP "):
                     self.handle_key_press(line)
-                elif line != "" and self._tx_busy:
+                elif line != "" and self.busy():
                     self.str_buffer.append(line)
                 elif line != "":
                     logger.error("Unhandled data received '%s'", line)
 
     def handle_ready(self) -> None:
         self.ready = True
         logger.info("Homeduino is connected")
@@ -149,48 +149,53 @@
         if not self.transport:
             raise DisconnectedError("Homeduino is not connected")
 
         if not self.ready:
             logger.error("Not ready")
             raise NotReadyError("Homeduino is not ready")
 
-        start_time = datetime.now()
-        while self._tx_busy:
-            if (datetime.now() - start_time).total_seconds() > _BUSY_TIMEOUT:
+        while self.busy():
+            if (datetime.now() - self._tx_busy_since).total_seconds() > _BUSY_TIMEOUT:
                 logger.error("Too busy to send %s", packet)
                 raise TooBusyError("Homeduino is too busy to send a command")
             logger.debug("Busy")
             await asyncio.sleep(0.01)
-        self._tx_busy = True
+        self._tx_busy_since = datetime.now()
 
         try:
             data = packet + "\n"
             logger.debug("Writing data: %s", repr(data))
             # type ignore: transport from create_connection is documented to be
             # implementation specific bidirectional, even though typed as
             # BaseTransport
             self.transport.write(data.encode())  # type: ignore
 
             # Wait for response
-            start_time = datetime.now()
             while len(self.str_buffer) == 0:
-                if (datetime.now() - start_time).total_seconds() > _RESPONSE_TIMEOUT:
+                if (
+                    datetime.now() - self._tx_busy_since
+                ).total_seconds() > _RESPONSE_TIMEOUT:
                     logger.error("Timeout while waiting for command response")
-                    raise ResponseTimeoutError("Timeout while waiting for command response")
+                    raise ResponseTimeoutError(
+                        "Timeout while waiting for command response"
+                    )
                 logger.debug("Waiting for command response")
                 await asyncio.sleep(0.01)
 
             response = self.str_buffer.pop()
             logger.debug("Command response received: %s", response)
             return response.strip()
         finally:
-            self._tx_busy = False
+            self._tx_busy_since = None
 
         return None
 
+    def busy(self):
+        return self._tx_busy_since is not None
+
     def connection_lost(self, exc: Optional[Exception]) -> None:
         logger.info("Port closed")
         if exc:
             logger.exception("Disconnected due to exception")
         else:
             logger.info("Disconnected because of close/abort")
 
@@ -242,24 +247,24 @@
                     parity=serial_asyncio.serial.PARITY_NONE,
                     stopbits=serial_asyncio.serial.STOPBITS_ONE,
                 )
 
                 start_time = datetime.now()
                 while not self.protocol.ready:
                     if (datetime.now() - start_time).total_seconds() > _READY_TIMEOUT:
-                        logger.error("Timeout while waiting for Homeduino to become ready")
+                        logger.error(
+                            "Timeout while waiting for Homeduino to become ready"
+                        )
                         raise ResponseTimeoutError(
                             "Timeout while waiting for Homeduino to become ready"
                         )
                     logger.debug("Waiting for Homeduino to become ready")
                     await asyncio.sleep(0.01)
 
-                await self.protocol.set_receive_interrupt(
-                    self.receive_interrupt
-                )
+                await self.protocol.set_receive_interrupt(self.receive_interrupt)
 
                 for rf_receive_callback in self.rf_receive_callbacks:
                     self.protocol.add_rf_receive_callback(rf_receive_callback)
 
                 return True
             except SerialException as ex:
                 logger.error(ex)
@@ -284,23 +289,26 @@
                     raise ResponseTimeoutError(
                         "Timeout while waiting for Homeduino to disconnect"
                     )
                 logger.debug("Waiting for Homeduino to disconnect")
                 await asyncio.sleep(0.01)
 
             self.protocol = None
-            return True
             logger.debug("Homeduino disconnected")
+            return True
 
         return False
 
     async def ping(self) -> bool:
         if not self.connected():
             raise DisconnectedError("Homeduino is not connected")
 
+        if self.protocol.busy():
+            return True
+
         logger.debug("Pinging Homeduino")
         message = f"PING {time.time()}"
         response = await self.protocol.send(message)
         if response == message:
             logger.debug("Pinging Homeduino successful")
             return True
 
@@ -340,19 +348,18 @@
     async def send(self, command) -> str:
         if not self.connected():
             raise DisconnectedError("Homeduino is not connected")
 
         return await self.protocol.send(command)
 
     @staticmethod
-    def get_protocols() -> []:
+    def get_protocols() -> [str]:
+        """Returns the supported protocols in natural sorted order"""
+
         def convert(text):
             return int(text) if text.isdigit() else text.lower()
 
         def alphanum_key(key: str):
             return [convert(c) for c in re.split("([0-9]+)", key)]
 
-        def natural_sort(li):
-            return sorted(li, key=alphanum_key)
-
         protocol_names = [protocol.name for protocol in controller.get_all_protocols()]
-        return natural_sort(protocol_names)
+        return sorted(protocol_names, key=alphanum_key)
```

### Comparing `homeduino-0.0.7.5/homeduino.egg-info/PKG-INFO` & `homeduino-0.0.7.6/homeduino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.7.5
+Version: 0.0.7.6
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.7.5/pyproject.toml` & `homeduino-0.0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "homeduino"
-version = "0.0.7.5"
+version = "0.0.7.6"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Homeduino library"
 readme = "README.md"
 requires-python = ">=3.7"
```

