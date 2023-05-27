# Comparing `tmp/novelcraft_sdk-0.1.1.tar.gz` & `tmp/novelcraft_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novelcraft_sdk-0.1.1.tar", max compression
+gzip compressed data, was "novelcraft_sdk-0.2.0.tar", max compression
```

## Comparing `novelcraft_sdk-0.1.1.tar` & `novelcraft_sdk-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1211 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/LICENSE
--rw-r--r--   0        0        0      804 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/README.md
--rw-r--r--   0        0        0      604 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       43 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/__init__.py
--rw-r--r--   0        0        0      729 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/__init__.py
--rw-r--r--   0        0        0     5917 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/agent.py
--rw-r--r--   0        0        0     1029 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/block.py
--rw-r--r--   0        0        0     2680 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/block_source.py
--rw-r--r--   0        0        0     3189 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/client.py
--rw-r--r--   0        0        0     1980 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/entity.py
--rw-r--r--   0        0        0     1646 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/entity_source.py
--rw-r--r--   0        0        0     6133 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/inventory.py
--rw-r--r--   0        0        0     1090 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/item_stack.py
--rw-r--r--   0        0        0     2908 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/logger.py
--rw-r--r--   0        0        0     2296 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/message.py
--rw-r--r--   0        0        0      353 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/orientation.py
--rw-r--r--   0        0        0      389 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/position.py
--rw-r--r--   0        0        0    14307 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/sdk.py
--rw-r--r--   0        0        0     1367 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/section.py
--rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 novelcraft_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-05-27 17:21:09.756900 novelcraft_sdk-0.2.0/LICENSE
+-rw-r--r--   0        0        0      804 2023-05-27 17:21:09.756900 novelcraft_sdk-0.2.0/README.md
+-rw-r--r--   0        0        0      604 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/__init__.py
+-rw-r--r--   0        0        0      729 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/__init__.py
+-rw-r--r--   0        0        0     5917 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/agent.py
+-rw-r--r--   0        0        0     1029 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/block.py
+-rw-r--r--   0        0        0     2680 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/block_source.py
+-rw-r--r--   0        0        0     3189 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/client.py
+-rw-r--r--   0        0        0     1980 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/entity.py
+-rw-r--r--   0        0        0     1646 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/entity_source.py
+-rw-r--r--   0        0        0     6133 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/inventory.py
+-rw-r--r--   0        0        0     1090 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/item_stack.py
+-rw-r--r--   0        0        0     2908 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/logger.py
+-rw-r--r--   0        0        0     2296 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/message.py
+-rw-r--r--   0        0        0      353 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/orientation.py
+-rw-r--r--   0        0        0      389 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/position.py
+-rw-r--r--   0        0        0    13538 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/sdk.py
+-rw-r--r--   0        0        0     1367 2023-05-27 17:21:09.760900 novelcraft_sdk-0.2.0/src/novelcraft/sdk/section.py
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 novelcraft_sdk-0.2.0/PKG-INFO
```

### Comparing `novelcraft_sdk-0.1.1/LICENSE` & `novelcraft_sdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/README.md` & `novelcraft_sdk-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/pyproject.toml` & `novelcraft_sdk-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "novelcraft.sdk"
-version = "0.1.1"
+version = "0.2.0"
 description = "A Python library for communicating with NovelCraft Servers and accessing NovelCraft game data"
 authors = ["NovelCraft"]
 license = "Unlicense"
 readme = "README.md"
 packages = [
     { include = "novelcraft", from = "src" }
 ]
```

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/__init__.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/agent.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/agent.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/block.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/block.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/block_source.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/block_source.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/client.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/client.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/entity.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/entity.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/entity_source.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/entity_source.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/inventory.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/inventory.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/item_stack.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/item_stack.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/logger.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/logger.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/message.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/message.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/sdk.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 @dataclass
 class _TickInfo:
     """The tick info."""
     tick: int
     time: datetime
 
 
-GET_INFO_INTERVAL = 1
-PING_INVERVAL = 1
+GET_INFO_INTERVAL = 10
+PING_INVERVAL = 10
 
 _agent: Agent | None = None
 _block_source: BlockSource | None = None
 _client: Client | None = None
 _entity_source: EntitySource | None = None
 _tick_info: _TickInfo | None = None
 _task_list: list[asyncio.Task] = []
@@ -298,31 +298,14 @@
                                 ),
                                 orientation=Orientation[float](
                                     player_info['orientation']['yaw'],
                                     player_info['orientation']['pitch']
                                 )
                                 )
 
-                agent_position = _agent.get_position()
-                agent_position = _agent.get_position()
-
-                request_section_list = [{
-                    'x': int(agent_position.x + x*16),
-                    'y': int(agent_position.y + y*16),
-                    'z': int(agent_position.z + z*16)
-                } for x in range(-1, 2) for y in range(-1, 2) for z in range(-1, 2)]
-
-                # Send get blocks and entities message
-                _client.send(Message({
-                    "bound_to": Message.BoundToKind.SERVER_BOUND.value,
-                    "type": Message.MessageKind.GET_BLOCKS_AND_ENTITIES.value,
-                    "token": _token,
-                    "request_section_list": request_section_list})
-                )
-
             # Update Info
             _agent.set_health(player_info['health'])
             _agent.set_position(Position[float](
                 player_info["position"]['x'],
                 player_info["position"]['y'],
                 player_info["position"]['z']
             ))
```

### Comparing `novelcraft_sdk-0.1.1/src/novelcraft/sdk/section.py` & `novelcraft_sdk-0.2.0/src/novelcraft/sdk/section.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.1/PKG-INFO` & `novelcraft_sdk-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novelcraft-sdk
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python library for communicating with NovelCraft Servers and accessing NovelCraft game data
 License: Unlicense
 Author: NovelCraft
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

