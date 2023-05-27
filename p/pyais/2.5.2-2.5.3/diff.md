# Comparing `tmp/pyais-2.5.2.tar.gz` & `tmp/pyais-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyais-2.5.2.tar", last modified: Sat Mar  4 13:45:06 2023, max compression
+gzip compressed data, was "dist/pyais-2.5.3.tar", last modified: Sat May 27 11:11:08 2023, max compression
```

## Comparing `pyais-2.5.2.tar` & `pyais-2.5.3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:45:06.000000 pyais-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-03-04 13:45:06.000000 pyais-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18916 2023-03-04 13:44:52.000000 pyais-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:45:06.000000 pyais-2.5.2/pyais/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/ais_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    64682 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-03-04 13:44:52.000000 pyais-2.5.2/pyais/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:45:06.000000 pyais-2.5.2/pyais.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-03-04 13:45:06.000000 pyais-2.5.2/pyais.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-04 13:45:06.000000 pyais-2.5.2/pyais.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 13:45:06.000000 pyais-2.5.2/pyais.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-04 13:45:06.000000 pyais-2.5.2/pyais.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-04 13:45:06.000000 pyais-2.5.2/pyais.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-04 13:45:06.000000 pyais-2.5.2/pyais.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 13:45:06.000000 pyais-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-04 13:44:52.000000 pyais-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:45:06.000000 pyais-2.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/mock_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    58995 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_decode_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    32404 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_file_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_generic_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_nmea.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_tag_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_talker_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_tcp_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/test_udp_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 13:45:06.000000 pyais-2.5.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/utils/generate_msg_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/utils/skip.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-04 13:44:52.000000 pyais-2.5.2/tests/utils/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:11:08.000000 pyais-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    23826 2023-05-27 11:11:08.000000 pyais-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19303 2023-05-27 11:10:57.000000 pyais-2.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:11:08.000000 pyais-2.5.3/pyais/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/ais_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64765 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-05-27 11:10:57.000000 pyais-2.5.3/pyais/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:11:08.000000 pyais-2.5.3/pyais.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23826 2023-05-27 11:11:08.000000 pyais-2.5.3/pyais.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-27 11:11:08.000000 pyais-2.5.3/pyais.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:11:08.000000 pyais-2.5.3/pyais.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 11:11:08.000000 pyais-2.5.3/pyais.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-27 11:11:08.000000 pyais-2.5.3/pyais.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-27 11:11:08.000000 pyais-2.5.3/pyais.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 11:11:08.000000 pyais-2.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-27 11:10:57.000000 pyais-2.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:11:08.000000 pyais-2.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/mock_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58995 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_decode_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32404 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_file_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_generic_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_nmea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_tag_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_talker_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_tcp_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/test_udp_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:11:08.000000 pyais-2.5.3/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/utils/generate_msg_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/utils/skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-27 11:10:57.000000 pyais-2.5.3/tests/utils/timeout.py
```

### Comparing `pyais-2.5.2/PKG-INFO` & `pyais-2.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.5.2
+Version: 2.5.3
 Summary: Ais message decoding
 Home-page: https://github.com/M0r13n/pyais
 Author: Leon Morten Richter
 Author-email: leon.morten@gmail.com
 License: MIT
 Description: # pyais
         
@@ -308,14 +308,22 @@
         ```
         
         Such messages are parsed by **pyais** only when using any of the classes from **pyais.stream**.
         e.g. `FileReaderStream` or `TCPStream`.
         
         Such additional information can then be accessed by the `.wrapper_msg` of every `NMEASentence`. This attribute is `None` by default.
         
+        # Communication State
+        
+        The ITU documentation provides details regarding the Time-division multiple access (TDMA) synchronization.
+        
+        Such details include information used by the slot allocation algorithm (either SOTDMA or ITDMA) including their synchronization state.
+        
+        Refer to [readthedocs](https://pyais.readthedocs.io/en/latest/messages.html#communication-state) for more information.
+        
         # AIS tracker
         
         **pyais** comes with the the ability to collect and maintain the state of individual vessels over time.
         This is necessary because several messages can give different information about a ship.
         In addition, the data changes constantly (e.g. position, speed and course).
         
         Thus the information split across multiple different AIS messages needs to be collected, consolidated and aggregated as a single track.
```

### Comparing `pyais-2.5.2/README.md` & `pyais-2.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,22 @@
 ```
 
 Such messages are parsed by **pyais** only when using any of the classes from **pyais.stream**.
 e.g. `FileReaderStream` or `TCPStream`.
 
 Such additional information can then be accessed by the `.wrapper_msg` of every `NMEASentence`. This attribute is `None` by default.
 
+# Communication State
+
+The ITU documentation provides details regarding the Time-division multiple access (TDMA) synchronization.
+
+Such details include information used by the slot allocation algorithm (either SOTDMA or ITDMA) including their synchronization state.
+
+Refer to [readthedocs](https://pyais.readthedocs.io/en/latest/messages.html#communication-state) for more information.
+
 # AIS tracker
 
 **pyais** comes with the the ability to collect and maintain the state of individual vessels over time.
 This is necessary because several messages can give different information about a ship.
 In addition, the data changes constantly (e.g. position, speed and course).
 
 Thus the information split across multiple different AIS messages needs to be collected, consolidated and aggregated as a single track.
```

### Comparing `pyais-2.5.2/pyais/__init__.py` & `pyais-2.5.3/pyais/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pyais.messages import NMEAMessage, ANY_MESSAGE, AISSentence
 from pyais.stream import TCPConnection, FileReaderStream, IterMessages
 from pyais.encode import encode_dict, encode_msg, ais_to_nmea_0183
 from pyais.decode import decode
 from pyais.tracker import AISTracker, AISTrack
 
 __license__ = 'MIT'
-__version__ = '2.5.2'
+__version__ = '2.5.3'
 __author__ = 'Leon Morten Richter'
 
 __all__ = (
     'encode_dict',
     'encode_msg',
     'ais_to_nmea_0183',
     'NMEAMessage',
```

### Comparing `pyais-2.5.2/pyais/ais_types.py` & `pyais-2.5.3/pyais/ais_types.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/pyais/constants.py` & `pyais-2.5.3/pyais/constants.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/pyais/decode.py` & `pyais-2.5.3/pyais/decode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/pyais/encode.py` & `pyais-2.5.3/pyais/encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/pyais/exceptions.py` & `pyais-2.5.3/pyais/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/pyais/main.py` & `pyais-2.5.3/pyais/main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/pyais/messages.py` & `pyais-2.5.3/pyais/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -798,14 +798,15 @@
     """
 
     radio: int  # Type hint to make mypy happy
 
     MAX_COMM_STATE_VALUE = 0x7ffff
 
     def get_communication_state(self) -> Dict[str, typing.Optional[int]]:
+        """Returns information used by the slot allocation algorithm as a dict."""
         result: Dict[str, typing.Optional[int]] = {
             'received_stations': None,
             'slot_number': None,
             'utc_hour': None,
             'utc_minute': None,
             'slot_offset': None,
             'slot_timeout': None,
```

### Comparing `pyais-2.5.2/pyais/stream.py` & `pyais-2.5.3/pyais/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,23 +219,28 @@
         while True:
             body = self.recv()
 
             # Server closed connection
             if not body:
                 return None
 
-            lines = body.split(b'\r\n')
+            lines = body.splitlines(keepends=True)
 
+            # last incomplete line
             line = partial + lines[0]
             if line:
                 yield line
 
-            yield from (line for line in lines[1:-1] if line)
-
-            partial = lines[-1]
+            if lines[-1].endswith(b'\n'):
+                # all lines are complete
+                yield from lines[1:]
+            else:
+                # the last line was only partially received
+                yield from lines[1:-1]
+                partial = lines[-1]
 
 
 class UDPReceiver(SocketStream):
 
     def __init__(self, host: str, port: int) -> None:
         sock: socket = socket(AF_INET, SOCK_DGRAM)
         sock.bind((host, port))
```

### Comparing `pyais-2.5.2/pyais/tracker.py` & `pyais-2.5.3/pyais/tracker.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/pyais/util.py` & `pyais-2.5.3/pyais/util.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/pyais.egg-info/PKG-INFO` & `pyais-2.5.3/pyais.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.5.2
+Version: 2.5.3
 Summary: Ais message decoding
 Home-page: https://github.com/M0r13n/pyais
 Author: Leon Morten Richter
 Author-email: leon.morten@gmail.com
 License: MIT
 Description: # pyais
         
@@ -308,14 +308,22 @@
         ```
         
         Such messages are parsed by **pyais** only when using any of the classes from **pyais.stream**.
         e.g. `FileReaderStream` or `TCPStream`.
         
         Such additional information can then be accessed by the `.wrapper_msg` of every `NMEASentence`. This attribute is `None` by default.
         
+        # Communication State
+        
+        The ITU documentation provides details regarding the Time-division multiple access (TDMA) synchronization.
+        
+        Such details include information used by the slot allocation algorithm (either SOTDMA or ITDMA) including their synchronization state.
+        
+        Refer to [readthedocs](https://pyais.readthedocs.io/en/latest/messages.html#communication-state) for more information.
+        
         # AIS tracker
         
         **pyais** comes with the the ability to collect and maintain the state of individual vessels over time.
         This is necessary because several messages can give different information about a ship.
         In addition, the data changes constantly (e.g. position, speed and course).
         
         Thus the information split across multiple different AIS messages needs to be collected, consolidated and aggregated as a single track.
```

### Comparing `pyais-2.5.2/pyais.egg-info/SOURCES.txt` & `pyais-2.5.3/pyais.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 tests/test_decode_raw.py
 tests/test_encode.py
 tests/test_examples.py
 tests/test_file_stream.py
 tests/test_generic_stream.py
 tests/test_main.py
 tests/test_nmea.py
+tests/test_socket.py
 tests/test_tag_block.py
 tests/test_talker_ids.py
 tests/test_tcp_stream.py
 tests/test_tracker.py
 tests/test_udp_stream.py
 tests/utils/__init__.py
 tests/utils/generate_msg_interface.py
```

### Comparing `pyais-2.5.2/setup.py` & `pyais-2.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/mock_sender.py` & `pyais-2.5.3/tests/mock_sender.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/mock_server.py` & `pyais-2.5.3/tests/mock_server.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,20 +22,25 @@
     sock.bind((host, port))
     sock.listen(1)
 
     try:
         while True:
             # wait for a connection
             conn, _ = sock.accept()
+            keep_alive = True
             if conn:
-                while True:
+                while keep_alive:
                     print(f"Sending {len(MESSAGES)} messages all at once.")
                     # send all at once and then close
                     for msg in MESSAGES:
-                        conn.send(msg + b"\r\n")
+                        try:
+                            # conn.send(msg + b"\r\n")
+                            conn.send(msg + b"\n")
+                        except BrokenPipeError:
+                            keep_alive = False
 
                     time.sleep(2)
     finally:
         sock.close()
 
 
 if __name__ == '__main__':
```

### Comparing `pyais-2.5.2/tests/test_constants.py` & `pyais-2.5.3/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_decode.py` & `pyais-2.5.3/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_decode_raw.py` & `pyais-2.5.3/tests/test_decode_raw.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_encode.py` & `pyais-2.5.3/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_examples.py` & `pyais-2.5.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_file_stream.py` & `pyais-2.5.3/tests/test_file_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_generic_stream.py` & `pyais-2.5.3/tests/test_generic_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_main.py` & `pyais-2.5.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_nmea.py` & `pyais-2.5.3/tests/test_nmea.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_tag_block.py` & `pyais-2.5.3/tests/test_tag_block.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_talker_ids.py` & `pyais-2.5.3/tests/test_talker_ids.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_tcp_stream.py` & `pyais-2.5.3/tests/test_tcp_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_tracker.py` & `pyais-2.5.3/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/test_udp_stream.py` & `pyais-2.5.3/tests/test_udp_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.2/tests/utils/generate_msg_interface.py` & `pyais-2.5.3/tests/utils/generate_msg_interface.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 for typ, cls in MSG_CLASS.items():
     if not cls.fields():
         continue
     print(cls.__name__, cls.__doc__)
     print()
     print("\tAttributes:")
     for field in cls.fields():
+
         print("\t\t*", f"`{field.name}`")
+        if field.name == 'radio':
+            print('\t\t\t* Further decoded by `.get_communication_state()` ')
+
         if 'mmsi' in field.name:
             print("\t\t\t*", "type:", f"({int}, {str})")
         else:
             print("\t\t\t*", "type:", field.metadata['d_type'])
         print("\t\t\t*", "bit-width:", field.metadata['width'])
         print("\t\t\t*", "default:", field.metadata['default'])
```

