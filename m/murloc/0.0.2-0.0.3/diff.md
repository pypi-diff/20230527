# Comparing `tmp/murloc-0.0.2.tar.gz` & `tmp/murloc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murloc-0.0.2.tar", last modified: Fri May 26 21:45:30 2023, max compression
+gzip compressed data, was "murloc-0.0.3.tar", last modified: Sat May 27 20:49:48 2023, max compression
```

## Comparing `murloc-0.0.2.tar` & `murloc-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-26 21:45:30.158213 murloc-0.0.2/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1068 2023-05-26 21:19:51.000000 murloc-0.0.2/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      799 2023-05-26 21:45:30.158213 murloc-0.0.2/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      435 2023-05-26 21:35:46.000000 murloc-0.0.2/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-26 21:45:30.157213 murloc-0.0.2/murloc/
--rw-rw-r--   0 chris     (1000) chris     (1000)       25 2023-05-26 20:30:24.000000 murloc-0.0.2/murloc/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3972 2023-05-26 21:33:46.000000 murloc-0.0.2/murloc/murloc.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-26 21:45:30.158213 murloc-0.0.2/murloc.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      799 2023-05-26 21:45:30.000000 murloc-0.0.2/murloc.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      182 2023-05-26 21:45:30.000000 murloc-0.0.2/murloc.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-26 21:45:30.000000 murloc-0.0.2/murloc.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-05-26 21:45:30.000000 murloc-0.0.2/murloc.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-05-26 21:45:30.158213 murloc-0.0.2/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)      584 2023-05-26 21:34:41.000000 murloc-0.0.2/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 20:49:48.910487 murloc-0.0.3/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1068 2023-05-26 21:19:51.000000 murloc-0.0.3/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3182 2023-05-27 20:49:48.910487 murloc-0.0.3/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2818 2023-05-27 20:48:16.000000 murloc-0.0.3/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 20:49:48.909487 murloc-0.0.3/murloc/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       25 2023-05-26 20:30:24.000000 murloc-0.0.3/murloc/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4409 2023-05-27 19:45:13.000000 murloc-0.0.3/murloc/murloc.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-27 20:49:48.910487 murloc-0.0.3/murloc.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3182 2023-05-27 20:49:48.000000 murloc-0.0.3/murloc.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      182 2023-05-27 20:49:48.000000 murloc-0.0.3/murloc.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-27 20:49:48.000000 murloc-0.0.3/murloc.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-05-27 20:49:48.000000 murloc-0.0.3/murloc.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-05-27 20:49:48.910487 murloc-0.0.3/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)      584 2023-05-27 20:49:24.000000 murloc-0.0.3/setup.py
```

### Comparing `murloc-0.0.2/LICENSE` & `murloc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `murloc-0.0.2/murloc/murloc.py` & `murloc-0.0.3/murloc/murloc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,59 @@
 #!/usr/bin/env python3
 
 import os
 import sys
 import time
+import json
 import struct
 import signal
 import socket
 import inspect
 
+
 def init(*args, **kwargs):
     return Murloc(*args, **kwargs)
 
+
 class Murloc:
     def __init__(
         self,
         version="1.0.0",
         host=socket.inet_ntoa(struct.pack("!L", socket.INADDR_LOOPBACK)),
         port=8048,
         name="murloc",
         mode="default",
-        url="https://github.com/chrisvarga/murloc",
-        methods=[],
+        url="Aaaaaughibbrgubugbugrguburgle!",
+        methods=dict(),
         logfile=None,
     ):
         self.version = version
         self.host = host
         self.port = port
         self.name = name
         self.mode = mode
         self.url = url
         self.methods = methods
         self.logfile = logfile
         self.pid = os.getpid()
         self.boot = inspect.cleandoc(
-            """\n
+            f"""\n
                     
                  ___
                 /\  \ 
-               /::\  \       %s %s
+               /::\  \       {self.name} {self.version}
               /:/\:\  \ 
              /:/  \:\  \ 
-            /:/__/ \:\__\    Running in %s mode
-            \:\  \ /:/  /    Port: %-10s 
-             \:\  /:/  /     PID:  %-10s 
+            /:/__/ \:\__\    Running in {self.mode} mode
+            \:\  \ /:/  /    Port: {self.port:<4}
+             \:\  /:/  /     PID:  {self.pid:<4}
               \:\/:/  / 
-               \::/  /             %s
+               \::/  /             {self.url}
                 \/__/ 
                     """
-            % (
-                self.name,
-                self.version,
-                self.mode,
-                self.port,
-                self.pid,
-                self.url,
-            )
         )
 
     def log(self, s):
         date = time.strftime("%Y-%m-%d %H:%M:%S")
         if self.mode == "debug":
             n = inspect.currentframe().f_back.f_lineno
             msg = f"[{date}] [{__file__}:{n}] [{os.getpid()}] {s}"
@@ -69,46 +64,60 @@
         else:
             try:
                 with open(self.logfile, "a") as f:
                     f.write(f"{msg}\n")
             except:
                 print(msg)
 
-    def handle(self, method, args):
+    def handle(self, method, params):
         if method not in self.methods:
-            return f"(error) method '{method}' is not defined"
-        return self.methods[method](self, args)
+            return '{"err":1,"data":"method not defined"}'
+        return self.methods[method](self, params)
 
     def parse(self, req):
-        args = req.split(" ")
-        method = args.pop(0)
-        return self.handle(method, args)
+        try:
+            js = json.loads(req)
+        except Exception as e:
+            if self.mode == "debug":
+                self.log(f"json.loads: {req}: {e}")
+            return '{"err":1,"data":"invalid json request"}'
+        try:
+            method = js["method"]
+        except:
+            return '{"err":1,"data":"request lacks method"}'
+        try:
+            params = js["params"]
+        except:
+            return '{"err":1,"data":"request lacks params"}'
+        return self.handle(method, params)
 
     def recvall(self, conn):
         data = b""
         while True:
             packet = conn.recv(1024)
             data += packet
             if len(packet) < 1024:
                 break
         return data
 
     def handle_connection(self, conn, addr):
         while True:
             try:
                 data = self.recvall(conn)
-            except:
+            except Exception as e:
+                if self.mode == "debug":
+                    self.log(f"recv: {e}")
                 conn.close()
                 break
             if not data:
                 conn.close()
                 break
-            req = data.decode("utf-8").strip()
-            res = self.parse(req) + "\n"
-            conn.sendall(res.encode("utf-8"))
+            req = data.decode().strip()
+            res = f"{self.parse(req)}\n"
+            conn.sendall(res.encode())
 
     def handle_sigint(self, sig, frame):
         print()
         sys.exit(0)
 
     def handle_sigchild(self, sig, frame):
         os.waitpid(-1, os.WNOHANG)
@@ -121,19 +130,21 @@
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         sock.bind((self.host, self.port))
         sock.listen()
         self.log(f"Listening at {self.host}:{self.port}")
         while True:
             try:
                 conn, addr = sock.accept()
-                conn.settimeout(10)
-                # Fork to handle the new connection; this allows us to use
-                # os.system() etc, which is problematic within a thread.
-                pid = os.fork()
-                if pid == 0:
-                    self.log(f"Connection from {addr}")
-                    self.handle_connection(conn, addr)
-                    sys.exit(0)
-                else:
-                    continue
-            except:
+            except Exception as e:
+                if self.mode == "debug":
+                    self.log(f"accept: {e}")
                 break
+            conn.settimeout(10)
+            # Fork to handle the new connection; this allows us to use
+            # os.system() etc, which is problematic within a thread.
+            pid = os.fork()
+            if pid == 0:
+                self.log(f"Connection from {addr}")
+                self.handle_connection(conn, addr)
+                sys.exit(0)
+            else:
+                continue
```

### Comparing `murloc-0.0.2/setup.py` & `murloc-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="murloc",
-    version="0.0.2",
+    version="0.0.3",
     author="Chris Varga",
     author_email="",
     description="extensible api server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=find_packages(),
```

