# Comparing `tmp/greenstalk-2.0.0.tar.gz` & `tmp/greenstalk-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/greenstalk-2.0.0.tar", last modified: Sat Jun 20 14:24:08 2020, max compression
+gzip compressed data, was "greenstalk-2.0.1.tar", last modified: Sat May 27 15:20:16 2023, max compression
```

## Comparing `greenstalk-2.0.0.tar` & `greenstalk-2.0.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-06-20 14:24:08.000000 greenstalk-2.0.0/
--rw-r--r--   0 justin    (1000) justin    (1000)     1057 2017-06-18 17:12:41.000000 greenstalk-2.0.0/LICENSE
--rw-r--r--   0 justin    (1000) justin    (1000)     2184 2020-06-20 14:24:08.000000 greenstalk-2.0.0/PKG-INFO
--rw-r--r--   0 justin    (1000) justin    (1000)     1197 2020-06-20 14:13:17.000000 greenstalk-2.0.0/README.rst
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-06-20 14:24:08.000000 greenstalk-2.0.0/greenstalk.egg-info/
--rw-r--r--   0 justin    (1000) justin    (1000)     2184 2020-06-20 14:24:08.000000 greenstalk-2.0.0/greenstalk.egg-info/PKG-INFO
--rw-r--r--   0 justin    (1000) justin    (1000)      187 2020-06-20 14:24:08.000000 greenstalk-2.0.0/greenstalk.egg-info/SOURCES.txt
--rw-r--r--   0 justin    (1000) justin    (1000)        1 2020-06-20 14:24:08.000000 greenstalk-2.0.0/greenstalk.egg-info/dependency_links.txt
--rw-r--r--   0 justin    (1000) justin    (1000)       11 2020-06-20 14:24:08.000000 greenstalk-2.0.0/greenstalk.egg-info/top_level.txt
--rw-r--r--   0 justin    (1000) justin    (1000)    14411 2020-06-20 14:14:36.000000 greenstalk-2.0.0/greenstalk.py
--rw-r--r--   0 justin    (1000) justin    (1000)      123 2020-06-20 14:24:08.000000 greenstalk-2.0.0/setup.cfg
--rw-r--r--   0 justin    (1000) justin    (1000)      820 2020-04-08 22:46:43.000000 greenstalk-2.0.0/setup.py
+drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-27 15:20:16.169826 greenstalk-2.0.1/
+-rw-r--r--   0 justin    (1000) users      (984)     1057 2023-05-26 15:48:09.000000 greenstalk-2.0.1/LICENSE
+-rw-r--r--   0 justin    (1000) users      (984)     1655 2023-05-27 15:20:16.169826 greenstalk-2.0.1/PKG-INFO
+-rw-r--r--   0 justin    (1000) users      (984)     1018 2023-05-27 15:09:53.000000 greenstalk-2.0.1/README.rst
+drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-27 15:20:16.169826 greenstalk-2.0.1/greenstalk.egg-info/
+-rw-r--r--   0 justin    (1000) users      (984)     1655 2023-05-27 15:20:16.000000 greenstalk-2.0.1/greenstalk.egg-info/PKG-INFO
+-rw-r--r--   0 justin    (1000) users      (984)      206 2023-05-27 15:20:16.000000 greenstalk-2.0.1/greenstalk.egg-info/SOURCES.txt
+-rw-r--r--   0 justin    (1000) users      (984)        1 2023-05-27 15:20:16.000000 greenstalk-2.0.1/greenstalk.egg-info/dependency_links.txt
+-rw-r--r--   0 justin    (1000) users      (984)       11 2023-05-27 15:20:16.000000 greenstalk-2.0.1/greenstalk.egg-info/top_level.txt
+-rw-r--r--   0 justin    (1000) users      (984)       90 2023-05-26 19:54:29.000000 greenstalk-2.0.1/pyproject.toml
+-rw-r--r--   0 justin    (1000) users      (984)      810 2023-05-27 15:20:16.169826 greenstalk-2.0.1/setup.cfg
+drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-27 15:20:16.169826 greenstalk-2.0.1/src/
+drwxr-xr-x   0 justin    (1000) users      (984)        0 2023-05-27 15:20:16.169826 greenstalk-2.0.1/src/greenstalk/
+-rw-r--r--   0 justin    (1000) users      (984)    15489 2023-05-27 15:09:53.000000 greenstalk-2.0.1/src/greenstalk/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `greenstalk-2.0.0/LICENSE` & `greenstalk-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `greenstalk-2.0.0/PKG-INFO` & `greenstalk-2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,53 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: greenstalk
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python 3 client for the beanstalkd work queue
 Home-page: https://github.com/justinmayhew/greenstalk
 Author: Justin Mayhew
 Author-email: mayhew@live.ca
 License: MIT
-Description: Greenstalk
-        ==========
-        
-        Greenstalk is a small and unopinionated Python client library for communicating
-        with the `beanstalkd`_ work queue. The API provided mostly maps one-to-one with
-        commands in the `protocol`_.
-        
-        .. image:: https://img.shields.io/pypi/v/greenstalk.svg
-            :target: https://pypi.org/project/greenstalk/
-        
-        .. image:: https://secure.travis-ci.org/justinmayhew/greenstalk.svg?branch=master
-            :target: https://travis-ci.org/justinmayhew/greenstalk
-        
-        .. image:: https://codecov.io/github/justinmayhew/greenstalk/coverage.svg?branch=master
-            :target: https://codecov.io/github/justinmayhew/greenstalk
-        
-        Getting Started
-        ---------------
-        
-        .. code-block:: pycon
-        
-            >>> import greenstalk
-            >>> client = greenstalk.Client(('127.0.0.1', 11300))
-            >>> client.put('hello')
-            1
-            >>> job = client.reserve()
-            >>> job.id
-            1
-            >>> job.body
-            'hello'
-            >>> client.delete(job)
-            >>> client.close()
-        
-        Documentation
-        -------------
-        
-        Documentation is available on `Read the Docs`_.
-        
-        .. _`beanstalkd`: https://beanstalkd.github.io/
-        .. _`protocol`: https://raw.githubusercontent.com/beanstalkd/beanstalkd/master/doc/protocol.txt
-        .. _`Read the Docs`: https://greenstalk.readthedocs.io/
-        
-Platform: UNKNOWN
+Project-URL: Documentation, https://greenstalk.readthedocs.io/
+Project-URL: Source, https://github.com/justinmayhew/greenstalk
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Greenstalk
+==========
+
+Greenstalk is a small and unopinionated Python client library for communicating
+with the `beanstalkd`_ work queue. The API provided mostly maps one-to-one with
+commands in the `protocol`_.
+
+.. image:: https://img.shields.io/pypi/v/greenstalk.svg
+    :target: https://pypi.org/project/greenstalk/
+
+.. image:: https://github.com/justinmayhew/greenstalk/workflows/CI/badge.svg?branch=main
+    :target: https://github.com/justinmayhew/greenstalk/actions
+
+Quickstart
+----------
+
+.. code-block:: pycon
+
+    >>> import greenstalk
+    >>> client = greenstalk.Client(('127.0.0.1', 11300))
+    >>> client.put('hello')
+    1
+    >>> job = client.reserve()
+    >>> job.id
+    1
+    >>> job.body
+    'hello'
+    >>> client.delete(job)
+    >>> client.close()
+
+Documentation is available on `Read the Docs`_.
+
+.. _`beanstalkd`: https://beanstalkd.github.io/
+.. _`protocol`: https://raw.githubusercontent.com/beanstalkd/beanstalkd/master/doc/protocol.txt
+.. _`Read the Docs`: https://greenstalk.readthedocs.io/
```

### Comparing `greenstalk-2.0.0/README.rst` & `greenstalk-2.0.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 Greenstalk is a small and unopinionated Python client library for communicating
 with the `beanstalkd`_ work queue. The API provided mostly maps one-to-one with
 commands in the `protocol`_.
 
 .. image:: https://img.shields.io/pypi/v/greenstalk.svg
     :target: https://pypi.org/project/greenstalk/
 
-.. image:: https://secure.travis-ci.org/justinmayhew/greenstalk.svg?branch=master
-    :target: https://travis-ci.org/justinmayhew/greenstalk
+.. image:: https://github.com/justinmayhew/greenstalk/workflows/CI/badge.svg?branch=main
+    :target: https://github.com/justinmayhew/greenstalk/actions
 
-.. image:: https://codecov.io/github/justinmayhew/greenstalk/coverage.svg?branch=master
-    :target: https://codecov.io/github/justinmayhew/greenstalk
-
-Getting Started
----------------
+Quickstart
+----------
 
 .. code-block:: pycon
 
     >>> import greenstalk
     >>> client = greenstalk.Client(('127.0.0.1', 11300))
     >>> client.put('hello')
     1
@@ -27,15 +24,12 @@
     >>> job.id
     1
     >>> job.body
     'hello'
     >>> client.delete(job)
     >>> client.close()
 
-Documentation
--------------
-
 Documentation is available on `Read the Docs`_.
 
 .. _`beanstalkd`: https://beanstalkd.github.io/
 .. _`protocol`: https://raw.githubusercontent.com/beanstalkd/beanstalkd/master/doc/protocol.txt
 .. _`Read the Docs`: https://greenstalk.readthedocs.io/
```

### Comparing `greenstalk-2.0.0/greenstalk.egg-info/PKG-INFO` & `greenstalk-2.0.1/greenstalk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,53 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: greenstalk
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Python 3 client for the beanstalkd work queue
 Home-page: https://github.com/justinmayhew/greenstalk
 Author: Justin Mayhew
 Author-email: mayhew@live.ca
 License: MIT
-Description: Greenstalk
-        ==========
-        
-        Greenstalk is a small and unopinionated Python client library for communicating
-        with the `beanstalkd`_ work queue. The API provided mostly maps one-to-one with
-        commands in the `protocol`_.
-        
-        .. image:: https://img.shields.io/pypi/v/greenstalk.svg
-            :target: https://pypi.org/project/greenstalk/
-        
-        .. image:: https://secure.travis-ci.org/justinmayhew/greenstalk.svg?branch=master
-            :target: https://travis-ci.org/justinmayhew/greenstalk
-        
-        .. image:: https://codecov.io/github/justinmayhew/greenstalk/coverage.svg?branch=master
-            :target: https://codecov.io/github/justinmayhew/greenstalk
-        
-        Getting Started
-        ---------------
-        
-        .. code-block:: pycon
-        
-            >>> import greenstalk
-            >>> client = greenstalk.Client(('127.0.0.1', 11300))
-            >>> client.put('hello')
-            1
-            >>> job = client.reserve()
-            >>> job.id
-            1
-            >>> job.body
-            'hello'
-            >>> client.delete(job)
-            >>> client.close()
-        
-        Documentation
-        -------------
-        
-        Documentation is available on `Read the Docs`_.
-        
-        .. _`beanstalkd`: https://beanstalkd.github.io/
-        .. _`protocol`: https://raw.githubusercontent.com/beanstalkd/beanstalkd/master/doc/protocol.txt
-        .. _`Read the Docs`: https://greenstalk.readthedocs.io/
-        
-Platform: UNKNOWN
+Project-URL: Documentation, https://greenstalk.readthedocs.io/
+Project-URL: Source, https://github.com/justinmayhew/greenstalk
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Greenstalk
+==========
+
+Greenstalk is a small and unopinionated Python client library for communicating
+with the `beanstalkd`_ work queue. The API provided mostly maps one-to-one with
+commands in the `protocol`_.
+
+.. image:: https://img.shields.io/pypi/v/greenstalk.svg
+    :target: https://pypi.org/project/greenstalk/
+
+.. image:: https://github.com/justinmayhew/greenstalk/workflows/CI/badge.svg?branch=main
+    :target: https://github.com/justinmayhew/greenstalk/actions
+
+Quickstart
+----------
+
+.. code-block:: pycon
+
+    >>> import greenstalk
+    >>> client = greenstalk.Client(('127.0.0.1', 11300))
+    >>> client.put('hello')
+    1
+    >>> job = client.reserve()
+    >>> job.id
+    1
+    >>> job.body
+    'hello'
+    >>> client.delete(job)
+    >>> client.close()
+
+Documentation is available on `Read the Docs`_.
+
+.. _`beanstalkd`: https://beanstalkd.github.io/
+.. _`protocol`: https://raw.githubusercontent.com/beanstalkd/beanstalkd/master/doc/protocol.txt
+.. _`Read the Docs`: https://greenstalk.readthedocs.io/
```

### Comparing `greenstalk-2.0.0/greenstalk.py` & `greenstalk-2.0.1/src/greenstalk/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import socket
-from typing import Any, BinaryIO, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
-__version__ = '2.0.0'
+__version__ = "2.0.1"
 
 Address = Union[Tuple[str, int], str]
 Body = Union[bytes, str]
 Stats = Dict[str, Union[str, int]]
 
-DEFAULT_TUBE = 'default'
+DEFAULT_TUBE = "default"
 DEFAULT_PRIORITY = 2**16
 DEFAULT_DELAY = 0
 DEFAULT_TTR = 60
 
 
 class Job:
     """A job returned from the server."""
-    __slots__ = ('id', 'body')
 
     def __init__(self, id: int, body: Body) -> None:
-        self.id = id
-        self.body = body
+        #: A server-generated unique identifier assigned to the job on creation.
+        self.id: int = id
+
+        #: The content of the job. Also referred to as the message or payload.
+        #: Producers and consumers need to agree on how these bytes are interpreted.
+        self.body: Body = body
+
+    def __repr__(self) -> str:
+        return f"greenstalk.Job(id={self.id!r}, body={self.body!r})"
 
 
 JobOrID = Union[Job, int]
 
 
 class Error(Exception):
     """Base class for non-connection related exceptions. Connection related
@@ -31,34 +37,42 @@
     """
 
 
 class UnknownResponseError(Error):
     """The server sent a response that this client does not understand."""
 
     def __init__(self, status: bytes, values: List[bytes]) -> None:
-        self.status = status
-        self.values = values
+        #: The status code of the response.
+        #: Contains ``b'SOME_ERROR'`` for the response ``b'SOME_ERROR 1 2 3\r\n'``.
+        self.status: bytes = status
+
+        #: The remaining split values after the status code.
+        #: Contains ``[b'1', b'2', b'3']`` for the response ``b'SOME_ERROR 1 2 3\r\n'``.
+        self.values: List[bytes] = values
 
 
 class BeanstalkdError(Error):
     """Base class for error messages returned from the server."""
 
 
 class BadFormatError(BeanstalkdError):
     """The client sent a malformed command."""
 
 
 class BuriedError(BeanstalkdError):
     """The server ran out of memory trying to grow the priority queue and had to
     bury the job.
+
+    This can be raised in response to a put or release command.
     """
 
-    def __init__(self, values: List[bytes] = None) -> None:
+    def __init__(self, values: Optional[List[bytes]] = None) -> None:
         if values:
-            self.id = int(values[0])  # type: Optional[int]
+            #: A server-generated unique identifier that was assigned to the buried job.
+            self.id: Optional[int] = int(values[0])
         else:
             self.id = None
 
 
 class DeadlineSoonError(BeanstalkdError):
     """The client has a reserved job timing out within the next second."""
 
@@ -101,52 +115,55 @@
 
 
 class UnknownCommandError(BeanstalkdError):
     """The client sent a command that the server does not understand."""
 
 
 ERROR_RESPONSES = {
-    b'BAD_FORMAT':      BadFormatError,
-    b'BURIED':          BuriedError,
-    b'DEADLINE_SOON':   DeadlineSoonError,
-    b'DRAINING':        DrainingError,
-    b'EXPECTED_CRLF':   ExpectedCrlfError,
-    b'INTERNAL_ERROR':  InternalError,
-    b'JOB_TOO_BIG':     JobTooBigError,
-    b'NOT_FOUND':       NotFoundError,
-    b'NOT_IGNORED':     NotIgnoredError,
-    b'OUT_OF_MEMORY':   OutOfMemoryError,
-    b'TIMED_OUT':       TimedOutError,
-    b'UNKNOWN_COMMAND': UnknownCommandError,
+    b"BAD_FORMAT": BadFormatError,
+    b"BURIED": BuriedError,
+    b"DEADLINE_SOON": DeadlineSoonError,
+    b"DRAINING": DrainingError,
+    b"EXPECTED_CRLF": ExpectedCrlfError,
+    b"INTERNAL_ERROR": InternalError,
+    b"JOB_TOO_BIG": JobTooBigError,
+    b"NOT_FOUND": NotFoundError,
+    b"NOT_IGNORED": NotIgnoredError,
+    b"OUT_OF_MEMORY": OutOfMemoryError,
+    b"TIMED_OUT": TimedOutError,
+    b"UNKNOWN_COMMAND": UnknownCommandError,
 }
 
 
 class Client:
     """A client implementing the beanstalk protocol. Upon creation a connection
     with beanstalkd is established and tubes are initialized.
 
     :param address: A socket address pair (host, port) or a Unix domain socket path.
     :param encoding: The encoding used to encode and decode job bodies.
     :param use: The tube to use after connecting.
     :param watch: The tubes to watch after connecting. The ``default`` tube will
                   be ignored if it's not included.
     """
 
-    def __init__(self,
-                 address: Address,
-                 encoding: Optional[str] = 'utf-8',
-                 use: str = DEFAULT_TUBE,
-                 watch: Union[str, Iterable[str]] = DEFAULT_TUBE) -> None:
+    def __init__(
+        self,
+        address: Address,
+        encoding: Optional[str] = "utf-8",
+        use: str = DEFAULT_TUBE,
+        watch: Union[str, Iterable[str]] = DEFAULT_TUBE,
+    ) -> None:
         if isinstance(address, str):
             self._sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
             self._sock.connect(address)
         else:
             self._sock = socket.create_connection(address)
 
-        self._reader = self._sock.makefile('rb')  # type: BinaryIO
+        self._reader = self._sock.makefile("rb")
+        self._address = address
         self.encoding = encoding
 
         if use != DEFAULT_TUBE:
             self.use(use)
 
         if isinstance(watch, str):
             if watch != DEFAULT_TUBE:
@@ -154,302 +171,319 @@
                 self.ignore(DEFAULT_TUBE)
         else:
             for tube in watch:
                 self.watch(tube)
             if DEFAULT_TUBE not in watch:
                 self.ignore(DEFAULT_TUBE)
 
-    def __enter__(self) -> 'Client':
+    def __enter__(self) -> "Client":
         return self
 
     def __exit__(self, *args: Any) -> None:
         self.close()
 
     def close(self) -> None:
         """Closes the connection to beanstalkd. The client instance should not
         be used after calling this method."""
         self._reader.close()
         self._sock.close()
 
     def _send_cmd(self, cmd: bytes, expected: bytes) -> List[bytes]:
-        self._sock.sendall(cmd + b'\r\n')
+        self._sock.sendall(cmd + b"\r\n")
         line = self._reader.readline()
         return _parse_response(line, expected)
 
     def _read_chunk(self, size: int) -> bytes:
         data = self._reader.read(size + 2)
         return _parse_chunk(data, size)
 
     def _int_cmd(self, cmd: bytes, expected: bytes) -> int:
-        n, = self._send_cmd(cmd, expected)
+        (n,) = self._send_cmd(cmd, expected)
         return int(n)
 
     def _job_cmd(self, cmd: bytes, expected: bytes) -> Job:
         id, size = (int(n) for n in self._send_cmd(cmd, expected))
         chunk = self._read_chunk(size)
         if self.encoding is None:
-            body = chunk  # type: Body
+            body: Body = chunk
         else:
             body = chunk.decode(self.encoding)
         return Job(id, body)
 
     def _peek_cmd(self, cmd: bytes) -> Job:
-        return self._job_cmd(cmd, b'FOUND')
+        return self._job_cmd(cmd, b"FOUND")
 
     def _stats_cmd(self, cmd: bytes) -> Stats:
-        size = self._int_cmd(cmd, b'OK')
+        size = self._int_cmd(cmd, b"OK")
         chunk = self._read_chunk(size)
-        return _parse_simple_yaml(chunk)
+        return _parse_stats(chunk)
 
     def _list_cmd(self, cmd: bytes) -> List[str]:
-        size = self._int_cmd(cmd, b'OK')
+        size = self._int_cmd(cmd, b"OK")
         chunk = self._read_chunk(size)
-        return _parse_simple_yaml_list(chunk)
+        return _parse_list(chunk)
 
-    def put(self,
-            body: Body,
-            priority: int = DEFAULT_PRIORITY,
-            delay: int = DEFAULT_DELAY,
-            ttr: int = DEFAULT_TTR) -> int:
+    def put(
+        self,
+        body: Body,
+        priority: int = DEFAULT_PRIORITY,
+        delay: int = DEFAULT_DELAY,
+        ttr: int = DEFAULT_TTR,
+    ) -> int:
         """Inserts a job into the currently used tube and returns the job ID.
 
         :param body: The data representing the job.
         :param priority: An integer between 0 and 4,294,967,295 where 0 is the
                          most urgent.
         :param delay: The number of seconds to delay the job for.
         :param ttr: The maximum number of seconds the job can be reserved for
                     before timing out.
         """
         if isinstance(body, str):
             if self.encoding is None:
                 raise TypeError("Unable to encode string with no encoding set")
             body = body.encode(self.encoding)
-        cmd = b'put %d %d %d %d\r\n%b' % (priority, delay, ttr, len(body), body)
-        return self._int_cmd(cmd, b'INSERTED')
+        cmd = b"put %d %d %d %d\r\n%b" % (priority, delay, ttr, len(body), body)
+        return self._int_cmd(cmd, b"INSERTED")
 
     def use(self, tube: str) -> None:
         """Changes the currently used tube.
 
         :param tube: The tube to use.
         """
-        self._send_cmd(b'use %b' % tube.encode('ascii'), b'USING')
+        self._send_cmd(b"use %b" % tube.encode("ascii"), b"USING")
 
     def reserve(self, timeout: Optional[int] = None) -> Job:
         """Reserves a job from a tube on the watch list, giving this client
         exclusive access to it for the TTR. Returns the reserved job.
 
         This blocks until a job is reserved unless a ``timeout`` is given,
         which will raise a :class:`TimedOutError <greenstalk.TimedOutError>` if
         a job cannot be reserved within that time.
 
         :param timeout: The maximum number of seconds to wait.
         """
         if timeout is None:
-            cmd = b'reserve'
+            cmd = b"reserve"
         else:
-            cmd = b'reserve-with-timeout %d' % timeout
-        return self._job_cmd(cmd, b'RESERVED')
+            cmd = b"reserve-with-timeout %d" % timeout
+        return self._job_cmd(cmd, b"RESERVED")
 
     def reserve_job(self, id: int) -> Job:
         """Reserves a job by ID, giving this client exclusive access to it for
         the TTR. Returns the reserved job.
 
         A :class:`NotFoundError <greenstalk.NotFoundError>` is raised if a job
         with the specified ID could not be reserved.
 
         :param id: The ID of the job to reserve.
         """
-        return self._job_cmd(b'reserve-job %d' % id, b'RESERVED')
+        return self._job_cmd(b"reserve-job %d" % id, b"RESERVED")
 
     def delete(self, job: JobOrID) -> None:
         """Deletes a job.
 
         :param job: The job or job ID to delete.
         """
-        self._send_cmd(b'delete %d' % _to_id(job), b'DELETED')
+        self._send_cmd(b"delete %d" % _to_id(job), b"DELETED")
 
-    def release(self,
-                job: Job,
-                priority: int = DEFAULT_PRIORITY,
-                delay: int = DEFAULT_DELAY) -> None:
+    def release(
+        self,
+        job: Job,
+        priority: int = DEFAULT_PRIORITY,
+        delay: int = DEFAULT_DELAY,
+    ) -> None:
         """Releases a reserved job.
 
         :param job: The job to release.
         :param priority: An integer between 0 and 4,294,967,295 where 0 is the
                          most urgent.
         :param delay: The number of seconds to delay the job for.
         """
-        self._send_cmd(b'release %d %d %d' % (job.id, priority, delay), b'RELEASED')
+        self._send_cmd(b"release %d %d %d" % (job.id, priority, delay), b"RELEASED")
 
     def bury(self, job: Job, priority: int = DEFAULT_PRIORITY) -> None:
         """Buries a reserved job.
 
         :param job: The job to bury.
         :param priority: An integer between 0 and 4,294,967,295 where 0 is the
                          most urgent.
         """
-        self._send_cmd(b'bury %d %d' % (job.id, priority), b'BURIED')
+        self._send_cmd(b"bury %d %d" % (job.id, priority), b"BURIED")
 
     def touch(self, job: Job) -> None:
         """Refreshes the TTR of a reserved job.
 
         :param job: The job to touch.
         """
-        self._send_cmd(b'touch %d' % job.id, b'TOUCHED')
+        self._send_cmd(b"touch %d" % job.id, b"TOUCHED")
 
     def watch(self, tube: str) -> int:
         """Adds a tube to the watch list. Returns the number of tubes this
         client is watching.
 
         :param tube: The tube to watch.
         """
-        return self._int_cmd(b'watch %b' % tube.encode('ascii'), b'WATCHING')
+        return self._int_cmd(b"watch %b" % tube.encode("ascii"), b"WATCHING")
 
     def ignore(self, tube: str) -> int:
         """Removes a tube from the watch list. Returns the number of tubes this
         client is watching.
 
         :param tube: The tube to ignore.
         """
-        return self._int_cmd(b'ignore %b' % tube.encode('ascii'), b'WATCHING')
+        return self._int_cmd(b"ignore %b" % tube.encode("ascii"), b"WATCHING")
 
     def peek(self, id: int) -> Job:
         """Returns a job by ID.
 
         :param id: The ID of the job to peek.
         """
-        return self._peek_cmd(b'peek %d' % id)
+        return self._peek_cmd(b"peek %d" % id)
 
     def peek_ready(self) -> Job:
         """Returns the next ready job in the currently used tube."""
-        return self._peek_cmd(b'peek-ready')
+        return self._peek_cmd(b"peek-ready")
 
     def peek_delayed(self) -> Job:
         """Returns the next available delayed job in the currently used tube."""
-        return self._peek_cmd(b'peek-delayed')
+        return self._peek_cmd(b"peek-delayed")
 
     def peek_buried(self) -> Job:
         """Returns the oldest buried job in the currently used tube."""
-        return self._peek_cmd(b'peek-buried')
+        return self._peek_cmd(b"peek-buried")
 
     def kick(self, bound: int) -> int:
         """Moves delayed and buried jobs into the ready queue and returns the
         number of jobs effected.
 
         Only jobs from the currently used tube are moved.
 
         A kick will only move jobs in a single state. If there are any buried
         jobs, only those will be moved. Otherwise delayed jobs will be moved.
 
         :param bound: The maximum number of jobs to kick.
         """
-        return self._int_cmd(b'kick %d' % bound, b'KICKED')
+        return self._int_cmd(b"kick %d" % bound, b"KICKED")
 
     def kick_job(self, job: JobOrID) -> None:
         """Moves a delayed or buried job into the ready queue.
 
         :param job: The job or job ID to kick.
         """
-        self._send_cmd(b'kick-job %d' % _to_id(job), b'KICKED')
+        self._send_cmd(b"kick-job %d" % _to_id(job), b"KICKED")
 
     def stats_job(self, job: JobOrID) -> Stats:
         """Returns job statistics.
 
         :param job: The job or job ID to return statistics for.
         """
-        return self._stats_cmd(b'stats-job %d' % _to_id(job))
+        return self._stats_cmd(b"stats-job %d" % _to_id(job))
 
     def stats_tube(self, tube: str) -> Stats:
         """Returns tube statistics.
 
         :param tube: The tube to return statistics for.
         """
-        return self._stats_cmd(b'stats-tube %b' % tube.encode('ascii'))
+        return self._stats_cmd(b"stats-tube %b" % tube.encode("ascii"))
 
     def stats(self) -> Stats:
         """Returns system statistics."""
-        return self._stats_cmd(b'stats')
+        return self._stats_cmd(b"stats")
 
     def tubes(self) -> List[str]:
         """Returns a list of all existing tubes."""
-        return self._list_cmd(b'list-tubes')
+        return self._list_cmd(b"list-tubes")
 
     def using(self) -> str:
         """Returns the tube currently being used by the client."""
-        tube, = self._send_cmd(b'list-tube-used', b'USING')
-        return tube.decode('ascii')
+        (tube,) = self._send_cmd(b"list-tube-used", b"USING")
+        return tube.decode("ascii")
 
     def watching(self) -> List[str]:
         """Returns a list of tubes currently being watched by the client."""
-        return self._list_cmd(b'list-tubes-watched')
+        return self._list_cmd(b"list-tubes-watched")
 
     def pause_tube(self, tube: str, delay: int) -> None:
         """Prevents jobs from being reserved from a tube for a period of time.
 
         :param tube: The tube to pause.
         :param delay: The number of seconds to pause the tube for.
         """
-        self._send_cmd(b'pause-tube %b %d' % (tube.encode('ascii'), delay), b'PAUSED')
+        self._send_cmd(b"pause-tube %b %d" % (tube.encode("ascii"), delay), b"PAUSED")
+
+    def __repr__(self) -> str:
+        if isinstance(self._address, str):
+            return f"greenstalk.Client(socket={self._address!r})"
+
+        host, port = self._address
+        return f"greenstalk.Client(host={host!r}, port={port!r})"
 
 
 def _to_id(j: JobOrID) -> int:
     return j.id if isinstance(j, Job) else j
 
 
 def _parse_response(line: bytes, expected: bytes) -> List[bytes]:
     if not line:
         raise ConnectionError("Unexpected EOF")
 
-    assert line[-2:] == b'\r\n'
+    assert line[-2:] == b"\r\n"
     line = line[:-2]
 
     status, *values = line.split()
 
     if status == expected:
         return values
 
     if status in ERROR_RESPONSES:
         raise ERROR_RESPONSES[status](values)
 
     raise UnknownResponseError(status, values)
 
 
 def _parse_chunk(data: bytes, size: int) -> bytes:
-    assert data[-2:] == b'\r\n'
+    assert data[-2:] == b"\r\n"
     data = data[:-2]
 
     if len(data) != size:
         raise ConnectionError("Unexpected EOF reading chunk")
 
     return data
 
 
-def _parse_simple_yaml(buf: bytes) -> Stats:
-    data = buf.decode('ascii')
+def _parse_stats(buf: bytes) -> Stats:
+    data = buf.decode("ascii")
 
-    assert data[:4] == '---\n'
+    assert data[:4] == "---\n"
     data = data[4:]  # strip YAML head
 
-    stats = {}
+    stats: Stats = {}
     for line in data.splitlines():
-        key, value = line.split(': ', 1)
+        key, value = line.split(": ", 1)
         try:
-            v = int(value)  # type: Union[int, str]
+            v: Union[int, str] = int(value)
         except ValueError:
-            v = value
+            v = _maybe_strip_quotes(value)
         stats[key] = v
 
     return stats
 
 
-def _parse_simple_yaml_list(buf: bytes) -> List[str]:
-    data = buf.decode('ascii')
+def _parse_list(buf: bytes) -> List[str]:
+    data = buf.decode("ascii")
 
-    assert data[:4] == '---\n'
+    assert data[:4] == "---\n"
     data = data[4:]  # strip YAML head
 
-    list = []
+    values: List[str] = []
     for line in data.splitlines():
-        assert line.startswith('- ')
-        list.append(line[2:])
+        assert line.startswith("- ")
+        values.append(line[2:])
+
+    return values
+
 
-    return list
+def _maybe_strip_quotes(s: str) -> str:
+    if len(s) >= 2 and s[0] == '"' and s[-1] == '"':
+        return s[1:-1]
+    return s
```

