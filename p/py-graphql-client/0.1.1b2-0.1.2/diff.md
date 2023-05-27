# Comparing `tmp/py-graphql-client-0.1.1b2.tar.gz` & `tmp/py-graphql-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-graphql-client-0.1.1b2.tar", last modified: Sun Apr  5 15:59:49 2020, max compression
+gzip compressed data, was "py-graphql-client-0.1.2.tar", last modified: Sat May 27 13:15:00 2023, max compression
```

## Comparing `py-graphql-client-0.1.1b2.tar` & `py-graphql-client-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 ecthiender  (1000) ecthiender  (1000)        0 2020-04-05 15:59:49.276545 py-graphql-client-0.1.1b2/
--rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)     3236 2020-04-05 15:59:49.276545 py-graphql-client-0.1.1b2/PKG-INFO
--rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)     1629 2020-03-31 17:56:23.000000 py-graphql-client-0.1.1b2/README.md
-drwxr-xr-x   0 ecthiender  (1000) ecthiender  (1000)        0 2020-04-05 15:59:49.273212 py-graphql-client-0.1.1b2/graphql_client/
--rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)     9162 2020-04-05 12:38:55.000000 py-graphql-client-0.1.1b2/graphql_client/__init__.py
-drwxr-xr-x   0 ecthiender  (1000) ecthiender  (1000)        0 2020-04-05 15:59:49.276545 py-graphql-client-0.1.1b2/py_graphql_client.egg-info/
--rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)     3236 2020-04-05 15:59:49.000000 py-graphql-client-0.1.1b2/py_graphql_client.egg-info/PKG-INFO
--rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)      289 2020-04-05 15:59:49.000000 py-graphql-client-0.1.1b2/py_graphql_client.egg-info/SOURCES.txt
--rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)        1 2020-04-05 15:59:49.000000 py-graphql-client-0.1.1b2/py_graphql_client.egg-info/dependency_links.txt
--rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)        1 2020-04-05 10:59:17.000000 py-graphql-client-0.1.1b2/py_graphql_client.egg-info/not-zip-safe
--rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)       25 2020-04-05 15:59:49.000000 py-graphql-client-0.1.1b2/py_graphql_client.egg-info/requires.txt
--rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)       15 2020-04-05 15:59:49.000000 py-graphql-client-0.1.1b2/py_graphql_client.egg-info/top_level.txt
--rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)       38 2020-04-05 15:59:49.276545 py-graphql-client-0.1.1b2/setup.cfg
--rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)     1554 2020-04-05 15:54:20.000000 py-graphql-client-0.1.1b2/setup.py
+drwxr-xr-x   0 ecthiender  (1000) ecthiender  (1000)        0 2023-05-27 13:15:00.959592 py-graphql-client-0.1.2/
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)     1513 2020-04-28 12:46:46.000000 py-graphql-client-0.1.2/LICENSE
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)     3744 2023-05-27 13:15:00.959592 py-graphql-client-0.1.2/PKG-INFO
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)     2836 2021-12-28 07:09:29.000000 py-graphql-client-0.1.2/README.md
+drwxr-xr-x   0 ecthiender  (1000) ecthiender  (1000)        0 2023-05-27 13:15:00.959592 py-graphql-client-0.1.2/graphql_client/
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)    10341 2023-05-27 12:56:53.000000 py-graphql-client-0.1.2/graphql_client/__init__.py
+drwxr-xr-x   0 ecthiender  (1000) ecthiender  (1000)        0 2023-05-27 13:15:00.959592 py-graphql-client-0.1.2/py_graphql_client.egg-info/
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)     3744 2023-05-27 13:15:00.000000 py-graphql-client-0.1.2/py_graphql_client.egg-info/PKG-INFO
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)      297 2023-05-27 13:15:00.000000 py-graphql-client-0.1.2/py_graphql_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)        1 2023-05-27 13:15:00.000000 py-graphql-client-0.1.2/py_graphql_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)        1 2023-05-27 13:15:00.000000 py-graphql-client-0.1.2/py_graphql_client.egg-info/not-zip-safe
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)       25 2023-05-27 13:15:00.000000 py-graphql-client-0.1.2/py_graphql_client.egg-info/requires.txt
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)       15 2023-05-27 13:15:00.000000 py-graphql-client-0.1.2/py_graphql_client.egg-info/top_level.txt
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)       38 2023-05-27 13:15:00.959592 py-graphql-client-0.1.2/setup.cfg
+-rw-r--r--   0 ecthiender  (1000) ecthiender  (1000)     1547 2023-05-27 13:01:53.000000 py-graphql-client-0.1.2/setup.py
```

### Comparing `py-graphql-client-0.1.1b2/PKG-INFO` & `py-graphql-client-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,163 @@
 Metadata-Version: 2.1
 Name: py-graphql-client
-Version: 0.1.1b2
+Version: 0.1.2
 Summary: A dead-simple GraphQL client that supports subscriptions over websockets
 Home-page: https://github.com/ecthiender/py-graphql-client
 Author: Anon Ray
 Author-email: rayanon004@gmail.com
 License: BSD3
-Description: # py-graphql-client
-        Dead-simple to use GraphQL client over websocket. Using the
-        [apollo-transport-ws](https://github.com/apollographql/subscriptions-transport-ws/blob/master/PROTOCOL.md)
-        protocol.
-        
-        ## Install
-        
-        ```bash
-        pip install py-graphql-client
-        ```
-        
-        ## Examples
-        
-        ### Setup subscriptions super easily
-        
-        ```python
-        from graphql_client import GraphQLClient
-        
-        ws = GraphQLClient('ws://localhost:8080/graphql')
-        def callback(_id, data):
-          print("got new data..")
-          print(f"msg id: {_id}. data: {data}")
-        
-        query = """
-          subscription {
-            notifications {
-              id
-              title
-              content
-            }
-          }
-        """
-        sub_id = ws.subscribe(query, callback=callback)
-        ...
-        # later stop the subscription
-        ws.stop_subscribe(sub_id)
-        ws.close()
-        ```
-        
-        ### Variables can be passed
-        
-        ```python
-        from graphql_client import GraphQLClient
-        
-        ws = GraphQLClient('ws://localhost:8080/graphql')
-        def callback(_id, data):
-          print("got new data..")
-          print(f"msg id: {_id}. data: {data}")
-        
-        query = """
-          subscription ($limit: Int!) {
-            notifications (order_by: {created: "desc"}, limit: $limit) {
-              id
-              title
-              content
-            }
-          }
-        """
-        sub_id = ws.subscribe(query, variables={'limit': 10}, callback=callback)
-        ```
-        
-        ### Normal queries and mutations work too
-        
-        ```python
-        from graphql_client import GraphQLClient
-        
-        ws = GraphQLClient('ws://localhost:8080/graphql')
-        query = """
-          query ($limit: Int!) {
-            notifications (order_by: {created: "desc"}, limit: $limit) {
-              id
-              title
-              content
-            }
-          }
-        """
-        res = ws.query(query, variables={'limit': 10})
-        print(res)
-        ws.close()
-        ```
-        
-        
-        ## TODO
-        - tests
-        - support http as well
-        - should use asyncio websocket library?
-        
 Keywords: graphql,websocket,subscriptions,graphql-client
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Other Environment
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# py-graphql-client
+Dead-simple to use GraphQL client over websocket. Using the
+[apollo-transport-ws](https://github.com/apollographql/subscriptions-transport-ws/blob/master/PROTOCOL.md)
+protocol.
+
+## Install
+
+```bash
+pip install py-graphql-client
+```
+
+## Examples
+
+### Setup subscriptions super easily
+
+```python
+from graphql_client import GraphQLClient
+
+query = """
+  subscription {
+    notifications {
+      id
+      title
+      content
+    }
+  }
+"""
+
+with GraphQLClient('ws://localhost:8080/graphql') as client:
+
+  sub_id = client.subscribe(query, callback=callback)
+  # do other stuff
+  # ...
+  # later stop the subscription
+  client.stop_subscribe(sub_id)
+
+def callback(_id, data):
+  print("got new data..")
+  print(f"msg id: {_id}. data: {data}")
+```
+
+### Variables can be passed
+
+```python
+from graphql_client import GraphQLClient
+
+query = """
+    subscription ($limit: Int!) {
+      notifications (order_by: {created: "desc"}, limit: $limit) {
+        id
+        title
+        content
+      }
+    }
+  """
+
+with GraphQLClient('ws://localhost:8080/graphql') as client:
+  sub_id = client.subscribe(query, variables={'limit': 10}, callback=callback)
+  # ...
+
+def callback(_id, data):
+  print("got new data..")
+  print(f"msg id: {_id}. data: {data}")
+
+```
+
+### Headers can be passed too
+
+```python
+from graphql_client import GraphQLClient
+
+query = """
+    subscription ($limit: Int!) {
+      notifications (order_by: {created: "desc"}, limit: $limit) {
+        id
+        title
+        content
+      }
+    }
+  """
+
+with GraphQLClient('ws://localhost:8080/graphql') as client:
+  sub_id = client.subscribe(query,
+                            variables={'limit': 10},
+                            headers={'Authorization': 'Bearer xxxx'},
+                            callback=callback)
+  ...
+  client.stop_subscribe(sub_id)
+
+def callback(_id, data):
+  print("got new data..")
+  print(f"msg id: {_id}. data: {data}")
+```
+
+### Normal queries and mutations work too
+
+```python
+from graphql_client import GraphQLClient
+
+query = """
+  query ($limit: Int!) {
+    notifications (order_by: {created: "desc"}, limit: $limit) {
+      id
+      title
+      content
+    }
+  }
+"""
+
+with GraphQLClient('ws://localhost:8080/graphql') as client:
+    res = client.query(query, variables={'limit': 10}, headers={'Authorization': 'Bearer xxxx'})
+    print(res)
+```
+
+### Without the context manager API
+
+```python
+from graphql_client import GraphQLClient
+
+query = """
+  query ($limit: Int!) {
+    notifications (order_by: {created: "desc"}, limit: $limit) {
+      id
+      title
+      content
+    }
+  }
+"""
+
+client = GraphQLClient('ws://localhost:8080/graphql')
+res = client.query(query, variables={'limit': 10}, headers={'Authorization': 'Bearer xxxx'})
+print(res)
+client.close()
+```
+
+
+## TODO
+- support http as well
+- should use asyncio websocket library?
```

### Comparing `py-graphql-client-0.1.1b2/graphql_client/__init__.py` & `py-graphql-client-0.1.2/graphql_client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 GQL_CONNECTION_ERROR = 'connection_error'
 GQL_CONNECTION_ACK = 'connection_ack'
 GQL_DATA = 'data'
 GQL_ERROR = 'error'
 GQL_COMPLETE = 'complete'
 GQL_CONNECTION_KEEP_ALIVE = 'ka'
 
-logging.basicConfig()
+logger = logging.getLogger(__name__)
+logger.addHandler(logging.NullHandler())
 
 
 class ConnectionException(Exception):
     """Exception thrown during connection errors to the GraphQL server"""
 
 class InvalidPayloadException(Exception):
     """Exception thrown if payload recived from server is mal-formed or cannot be parsed """
@@ -54,55 +55,75 @@
         # map of subscriber id to a callback function
         self._subscriber_callbacks = {}
         # our general receive queue
         self._queue = queue.Queue()
         # map of queues for each subscriber
         self._subscriber_queues = {}
         self._shutdown_receiver = False
+        self._subscriptions = []
         self.connect()
 
     def connect(self) -> None:
         """
         Initializes a connection with the server.
         """
         self._connection = websocket.create_connection(self.ws_url,
                                                        subprotocols=[GQL_WS_SUBPROTOCOL])
         # start the reciever thread
         self._recevier_thread = threading.Thread(target=self._receiver_task)
         self._recevier_thread.start()
 
+    def _reconnect(self):
+        subscriptions = self._subscriptions
+        self.__init__(self.ws_url)
+
+        for subscription in subscriptions:
+            self.subscribe(query=subscription['query'],
+                           variables=subscription['variables'],
+                           headers=subscription['headers'],
+                           callback=subscription['callback'])
+
     def __dump_queues(self):
-        logging.debug('[GQL_CLIENT] => Dump of all the internal queues')
-        logging.debug('[GQL_CLIENT] => Global queue => \n %s', self._queue.queue)
+        logger.debug('[GQL_CLIENT] => Dump of all the internal queues')
+        logger.debug('[GQL_CLIENT] => Global queue => \n %s', self._queue.queue)
         dumps = list(map(lambda q: (q[0], q[1].queue), self._subscriber_queues.items()))
-        logging.debug('[GQL_CLIENT] => Operation queues: \n %s', dumps)
+        logger.debug('[GQL_CLIENT] => Operation queues: \n %s', dumps)
 
     # wait for any valid message, while ignoring GQL_CONNECTION_KEEP_ALIVE
     def _receiver_task(self):
         """the recieve function of the client. Which validates response from the
         server and queues data """
-        while not self._shutdown_receiver:
+        reconnected = False
+        while not self._shutdown_receiver and not reconnected:
             self.__dump_queues()
-            res = self._connection.recv()
+            try:
+                res = self._connection.recv()
+            except websocket._exceptions.WebSocketConnectionClosedException as e:
+                self._reconnect()
+                reconnected = True
+                continue
+
             try:
                 msg = json.loads(res)
             except json.JSONDecodeError as err:
-                logging.warning('Ignoring. Server sent invalid JSON data: %s \n %s', res, err)
+                logger.warning('Ignoring. Server sent invalid JSON data: %s \n %s', res, err)
+                continue
 
             # ignore messages which are GQL_CONNECTION_KEEP_ALIVE
             if msg['type'] != GQL_CONNECTION_KEEP_ALIVE:
 
                 # check all GQL_DATA and GQL_COMPLETE should have 'id'.
                 # Otherwise, server is sending malformed responses, error out!
                 if msg['type'] in [GQL_DATA, GQL_COMPLETE] and 'id' not in msg:
                     # TODO: main thread can't catch this exception; setup
                     # exception queues. but this scenario will only happen with
                     # servers having glaring holes in implementing the protocol
                     # correctly, which is rare. hence this is not very urgent
-                    raise InvalidPayloadException(f'Protocol Violation. Expected "id" in {msg}, but could not find')
+                    err = f'Protocol Violation.\nExpected "id" in {msg}, but could not find.'
+                    raise InvalidPayloadException(err)
 
                 # if the message has an id, it is meant for a particular operation
                 if 'id' in msg:
                     op_id = msg['id']
 
                     # put it in the correct operation/subscriber queue
                     if op_id in self._subscriber_queues:
@@ -116,15 +137,14 @@
                         user_fn = self._subscriber_callbacks[op_id]
                         user_fn(op_id, msg)
 
                 # if it doesn't have an id, put in the global queue
                 else:
                     self._queue.put(msg)
 
-
     def _insert_subscriber(self, op_id, callback_fn):
         self._subscriber_callbacks[op_id] = callback_fn
 
     def _remove_subscriber(self, op_id):
         del self._subscriber_callbacks[op_id]
 
     def _create_operation_queue(self, op_id):
@@ -185,15 +205,15 @@
         self._connection_init(headers)
         payload = {'headers': headers, 'query': query, 'variables': variables}
         op_id = self._start(payload)
         res = self._get_operation_result(op_id)
         self._stop(op_id)
         ack = self._get_operation_result(op_id)
         if ack['type'] != GQL_COMPLETE:
-            logging.warning('Expected to recieve complete, but received: %s', ack)
+            logger.warning('Expected to recieve complete, but received: %s', ack)
         self._remove_operation_queue(op_id)
         return res
 
     def subscribe(self, query: str, variables: dict = None, headers: dict = None,
                   callback: Callable[[str, dict], None] = None) -> str:
         """
         Run a GraphQL subscription.
@@ -207,20 +227,26 @@
         headers (dict): (optional) a dictionary of headers for the session
 
         Returns:
         op_id (str): The operation id (a UUIDv4) for this subscription operation
         """
 
         # sanity check that the user passed a valid function
-        if not callback and not callable(callback):
+        if not callback or not callable(callback):
             raise TypeError('the argument `callback` is mandatory and it should be a function')
 
         self._connection_init(headers)
         payload = {'headers': headers, 'query': query, 'variables': variables}
         op_id = self._start(payload, callback)
+        self._subscriptions.append({
+            'query': query,
+            'variables': variables,
+            'headers': headers,
+            'callback': callback
+        })
         return op_id
 
     def stop_subscribe(self, op_id: str) -> None:
         """
         Stop a subscription. Takes an operation ID (`op_id`) and stops the
         subscription.
         """
@@ -230,9 +256,17 @@
 
     def close(self) -> None:
         """
         Close the connection with the server. To reconnect, use the `connect`
         method.
         """
         self._shutdown_receiver = True
-        self._connection.close()
         self._recevier_thread.join()
+        self._connection.close()
+
+    def __enter__(self):
+        """ enter method for context manager """
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        """ exit method for context manager """
+        self.close()
```

### Comparing `py-graphql-client-0.1.1b2/py_graphql_client.egg-info/PKG-INFO` & `py-graphql-client-0.1.2/py_graphql_client.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,163 @@
 Metadata-Version: 2.1
 Name: py-graphql-client
-Version: 0.1.1b2
+Version: 0.1.2
 Summary: A dead-simple GraphQL client that supports subscriptions over websockets
 Home-page: https://github.com/ecthiender/py-graphql-client
 Author: Anon Ray
 Author-email: rayanon004@gmail.com
 License: BSD3
-Description: # py-graphql-client
-        Dead-simple to use GraphQL client over websocket. Using the
-        [apollo-transport-ws](https://github.com/apollographql/subscriptions-transport-ws/blob/master/PROTOCOL.md)
-        protocol.
-        
-        ## Install
-        
-        ```bash
-        pip install py-graphql-client
-        ```
-        
-        ## Examples
-        
-        ### Setup subscriptions super easily
-        
-        ```python
-        from graphql_client import GraphQLClient
-        
-        ws = GraphQLClient('ws://localhost:8080/graphql')
-        def callback(_id, data):
-          print("got new data..")
-          print(f"msg id: {_id}. data: {data}")
-        
-        query = """
-          subscription {
-            notifications {
-              id
-              title
-              content
-            }
-          }
-        """
-        sub_id = ws.subscribe(query, callback=callback)
-        ...
-        # later stop the subscription
-        ws.stop_subscribe(sub_id)
-        ws.close()
-        ```
-        
-        ### Variables can be passed
-        
-        ```python
-        from graphql_client import GraphQLClient
-        
-        ws = GraphQLClient('ws://localhost:8080/graphql')
-        def callback(_id, data):
-          print("got new data..")
-          print(f"msg id: {_id}. data: {data}")
-        
-        query = """
-          subscription ($limit: Int!) {
-            notifications (order_by: {created: "desc"}, limit: $limit) {
-              id
-              title
-              content
-            }
-          }
-        """
-        sub_id = ws.subscribe(query, variables={'limit': 10}, callback=callback)
-        ```
-        
-        ### Normal queries and mutations work too
-        
-        ```python
-        from graphql_client import GraphQLClient
-        
-        ws = GraphQLClient('ws://localhost:8080/graphql')
-        query = """
-          query ($limit: Int!) {
-            notifications (order_by: {created: "desc"}, limit: $limit) {
-              id
-              title
-              content
-            }
-          }
-        """
-        res = ws.query(query, variables={'limit': 10})
-        print(res)
-        ws.close()
-        ```
-        
-        
-        ## TODO
-        - tests
-        - support http as well
-        - should use asyncio websocket library?
-        
 Keywords: graphql,websocket,subscriptions,graphql-client
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Other Environment
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# py-graphql-client
+Dead-simple to use GraphQL client over websocket. Using the
+[apollo-transport-ws](https://github.com/apollographql/subscriptions-transport-ws/blob/master/PROTOCOL.md)
+protocol.
+
+## Install
+
+```bash
+pip install py-graphql-client
+```
+
+## Examples
+
+### Setup subscriptions super easily
+
+```python
+from graphql_client import GraphQLClient
+
+query = """
+  subscription {
+    notifications {
+      id
+      title
+      content
+    }
+  }
+"""
+
+with GraphQLClient('ws://localhost:8080/graphql') as client:
+
+  sub_id = client.subscribe(query, callback=callback)
+  # do other stuff
+  # ...
+  # later stop the subscription
+  client.stop_subscribe(sub_id)
+
+def callback(_id, data):
+  print("got new data..")
+  print(f"msg id: {_id}. data: {data}")
+```
+
+### Variables can be passed
+
+```python
+from graphql_client import GraphQLClient
+
+query = """
+    subscription ($limit: Int!) {
+      notifications (order_by: {created: "desc"}, limit: $limit) {
+        id
+        title
+        content
+      }
+    }
+  """
+
+with GraphQLClient('ws://localhost:8080/graphql') as client:
+  sub_id = client.subscribe(query, variables={'limit': 10}, callback=callback)
+  # ...
+
+def callback(_id, data):
+  print("got new data..")
+  print(f"msg id: {_id}. data: {data}")
+
+```
+
+### Headers can be passed too
+
+```python
+from graphql_client import GraphQLClient
+
+query = """
+    subscription ($limit: Int!) {
+      notifications (order_by: {created: "desc"}, limit: $limit) {
+        id
+        title
+        content
+      }
+    }
+  """
+
+with GraphQLClient('ws://localhost:8080/graphql') as client:
+  sub_id = client.subscribe(query,
+                            variables={'limit': 10},
+                            headers={'Authorization': 'Bearer xxxx'},
+                            callback=callback)
+  ...
+  client.stop_subscribe(sub_id)
+
+def callback(_id, data):
+  print("got new data..")
+  print(f"msg id: {_id}. data: {data}")
+```
+
+### Normal queries and mutations work too
+
+```python
+from graphql_client import GraphQLClient
+
+query = """
+  query ($limit: Int!) {
+    notifications (order_by: {created: "desc"}, limit: $limit) {
+      id
+      title
+      content
+    }
+  }
+"""
+
+with GraphQLClient('ws://localhost:8080/graphql') as client:
+    res = client.query(query, variables={'limit': 10}, headers={'Authorization': 'Bearer xxxx'})
+    print(res)
+```
+
+### Without the context manager API
+
+```python
+from graphql_client import GraphQLClient
+
+query = """
+  query ($limit: Int!) {
+    notifications (order_by: {created: "desc"}, limit: $limit) {
+      id
+      title
+      content
+    }
+  }
+"""
+
+client = GraphQLClient('ws://localhost:8080/graphql')
+res = client.query(query, variables={'limit': 10}, headers={'Authorization': 'Bearer xxxx'})
+print(res)
+client.close()
+```
+
+
+## TODO
+- support http as well
+- should use asyncio websocket library?
```

### Comparing `py-graphql-client-0.1.1b2/setup.py` & `py-graphql-client-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 
-__version__ = "0.1.1-beta.2"
+__version__ = "0.1.2"
 __desc__ = "A dead-simple GraphQL client that supports subscriptions over websockets"
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 requirements = [
     'websocket-client==0.54.0'
```

