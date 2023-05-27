# Comparing `tmp/opd-100.tar.gz` & `tmp/opd-101.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opd-100.tar", last modified: Sat May 27 05:07:16 2023, max compression
+gzip compressed data, was "opd-101.tar", last modified: Sat May 27 12:39:43 2023, max compression
```

## Comparing `opd-100.tar` & `opd-101.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 05:07:16.270583 opd-100/
--rw-r--r--   0 nop       (1000) nop       (1000)     3906 2023-05-27 05:07:16.270583 opd-100/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     2321 2023-05-26 16:41:51.000000 opd-100/README.rst
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 05:07:16.266583 opd-100/opd/
--rw-r--r--   0 nop       (1000) nop       (1000)       64 2023-05-26 14:47:52.000000 opd-100/opd/__init__.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2799 2023-05-27 04:34:06.000000 opd-100/opd/__main__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      437 2023-05-26 12:08:11.000000 opd-100/opd/clients.py
--rw-r--r--   0 nop       (1000) nop       (1000)      983 2023-05-25 21:36:10.000000 opd-100/opd/clocked.py
--rw-r--r--   0 nop       (1000) nop       (1000)      808 2023-05-26 12:20:06.000000 opd-100/opd/command.py
--rw-r--r--   0 nop       (1000) nop       (1000)      648 2023-05-26 12:56:50.000000 opd-100/opd/decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      341 2023-05-25 21:36:54.000000 opd-100/opd/default.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1037 2023-05-26 12:57:04.000000 opd-100/opd/encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      314 2023-05-25 21:37:10.000000 opd-100/opd/errored.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1705 2023-05-26 15:41:32.000000 opd-100/opd/handler.py
--rw-r--r--   0 nop       (1000) nop       (1000)      795 2023-05-25 21:37:44.000000 opd-100/opd/listens.py
--rw-r--r--   0 nop       (1000) nop       (1000)      310 2023-05-26 09:39:02.000000 opd-100/opd/loggers.py
--rw-r--r--   0 nop       (1000) nop       (1000)      810 2023-05-27 04:33:32.000000 opd-100/opd/message.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 05:07:16.270583 opd-100/opd/modules/
--rw-r--r--   0 nop       (1000) nop       (1000)      411 2023-05-25 22:24:59.000000 opd-100/opd/modules/__init__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      144 2023-05-26 12:10:51.000000 opd-100/opd/modules/cmd.py
--rw-r--r--   0 nop       (1000) nop       (1000)      351 2023-05-25 21:39:47.000000 opd-100/opd/modules/err.py
--rw-r--r--   0 nop       (1000) nop       (1000)      367 2023-05-25 21:39:56.000000 opd-100/opd/modules/flt.py
--rw-r--r--   0 nop       (1000) nop       (1000)      913 2023-05-26 12:58:20.000000 opd-100/opd/modules/fnd.py
--rw-r--r--   0 nop       (1000) nop       (1000)    19751 2023-05-26 17:02:44.000000 opd-100/opd/modules/irc.py
--rw-r--r--   0 nop       (1000) nop       (1000)      654 2023-05-26 17:03:14.000000 opd-100/opd/modules/log.py
--rw-r--r--   0 nop       (1000) nop       (1000)      122 2023-05-25 21:45:05.000000 opd-100/opd/modules/mod.py
--rw-r--r--   0 nop       (1000) nop       (1000)     7637 2023-05-26 17:03:43.000000 opd-100/opd/modules/rss.py
--rw-r--r--   0 nop       (1000) nop       (1000)      281 2023-05-25 21:41:41.000000 opd-100/opd/modules/sts.py
--rw-r--r--   0 nop       (1000) nop       (1000)      878 2023-05-26 17:04:05.000000 opd-100/opd/modules/tdo.py
--rw-r--r--   0 nop       (1000) nop       (1000)      969 2023-05-26 09:47:40.000000 opd-100/opd/modules/thr.py
--rw-r--r--   0 nop       (1000) nop       (1000)      182 2023-05-25 21:42:19.000000 opd-100/opd/modules/upt.py
--rw-r--r--   0 nop       (1000) nop       (1000)     3535 2023-05-26 18:40:47.000000 opd-100/opd/objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1273 2023-05-27 04:24:05.000000 opd-100/opd/parsers.py
--rw-r--r--   0 nop       (1000) nop       (1000)     3949 2023-05-26 14:13:59.000000 opd-100/opd/persist.py
--rw-r--r--   0 nop       (1000) nop       (1000)      220 2023-05-25 21:39:02.000000 opd-100/opd/repeats.py
--rw-r--r--   0 nop       (1000) nop       (1000)      750 2023-05-27 04:16:12.000000 opd-100/opd/runtime.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1727 2023-05-26 09:43:52.000000 opd-100/opd/threads.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2123 2023-05-26 13:53:13.000000 opd-100/opd/utility.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 05:07:16.266583 opd-100/opd.egg-info/
--rw-r--r--   0 nop       (1000) nop       (1000)     3906 2023-05-27 05:07:16.000000 opd-100/opd.egg-info/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)      808 2023-05-27 05:07:16.000000 opd-100/opd.egg-info/SOURCES.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-27 05:07:16.000000 opd-100/opd.egg-info/dependency_links.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        4 2023-05-27 05:07:16.000000 opd-100/opd.egg-info/top_level.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-27 05:07:16.000000 opd-100/opd.egg-info/zip-safe
--rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-05-27 05:07:16.270583 opd-100/setup.cfg
--rw-r--r--   0 nop       (1000) nop       (1000)      770 2023-05-27 05:06:36.000000 opd-100/setup.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 05:07:16.270583 opd-100/test/
--rw-r--r--   0 nop       (1000) nop       (1000)      464 2023-05-26 12:36:11.000000 opd-100/test/test_decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      369 2023-05-26 12:36:20.000000 opd-100/test/test_encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      883 2023-05-26 12:36:32.000000 opd-100/test/test_inherit.py
--rw-r--r--   0 nop       (1000) nop       (1000)     4545 2023-05-26 14:15:36.000000 opd-100/test/test_objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)      977 2023-05-26 14:14:19.000000 opd-100/test/test_storage.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 12:39:43.730480 opd-101/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4008 2023-05-27 12:39:43.730480 opd-101/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     2383 2023-05-27 05:18:59.000000 opd-101/README.rst
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 12:39:43.730480 opd-101/opd/
+-rw-r--r--   0 nop       (1000) nop       (1000)       64 2023-05-26 14:47:52.000000 opd-101/opd/__init__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2837 2023-05-27 11:31:03.000000 opd-101/opd/__main__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      527 2023-05-27 09:45:38.000000 opd-101/opd/clients.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1050 2023-05-27 10:01:17.000000 opd-101/opd/clocked.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      923 2023-05-27 09:47:08.000000 opd-101/opd/command.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      760 2023-05-27 09:47:20.000000 opd-101/opd/decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      341 2023-05-25 21:36:54.000000 opd-101/opd/default.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1149 2023-05-27 09:47:26.000000 opd-101/opd/encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      368 2023-05-27 09:47:37.000000 opd-101/opd/errored.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1913 2023-05-27 12:12:22.000000 opd-101/opd/handler.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      903 2023-05-27 09:48:47.000000 opd-101/opd/listens.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      400 2023-05-27 09:48:56.000000 opd-101/opd/loggers.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      929 2023-05-27 11:18:58.000000 opd-101/opd/message.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 12:39:43.730480 opd-101/opd/modules/
+-rw-r--r--   0 nop       (1000) nop       (1000)      435 2023-05-27 07:50:18.000000 opd-101/opd/modules/__init__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      158 2023-05-27 10:45:11.000000 opd-101/opd/modules/cmd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      365 2023-05-27 10:45:22.000000 opd-101/opd/modules/err.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      402 2023-05-27 10:45:32.000000 opd-101/opd/modules/flt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      948 2023-05-27 10:45:43.000000 opd-101/opd/modules/fnd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)    19809 2023-05-27 10:42:32.000000 opd-101/opd/modules/irc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      668 2023-05-27 07:43:07.000000 opd-101/opd/modules/log.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      136 2023-05-27 10:46:22.000000 opd-101/opd/modules/mod.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     7638 2023-05-27 10:01:48.000000 opd-101/opd/modules/rss.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      295 2023-05-27 10:46:46.000000 opd-101/opd/modules/sts.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      892 2023-05-27 07:45:32.000000 opd-101/opd/modules/tdo.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      989 2023-05-27 10:44:37.000000 opd-101/opd/modules/thr.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      202 2023-05-27 10:44:51.000000 opd-101/opd/modules/upt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      157 2023-05-27 10:47:40.000000 opd-101/opd/modules/ver.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1640 2023-05-27 09:50:07.000000 opd-101/opd/objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2057 2023-05-27 10:27:52.000000 opd-101/opd/objfunc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1756 2023-05-27 11:38:06.000000 opd-101/opd/parsers.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     3985 2023-05-27 10:37:50.000000 opd-101/opd/persist.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      287 2023-05-27 10:01:28.000000 opd-101/opd/repeats.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1425 2023-05-27 12:12:02.000000 opd-101/opd/runtime.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      878 2023-05-27 09:59:26.000000 opd-101/opd/threads.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2884 2023-05-27 09:57:34.000000 opd-101/opd/utility.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 12:39:43.730480 opd-101/opd.egg-info/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4008 2023-05-27 12:39:43.000000 opd-101/opd.egg-info/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)      842 2023-05-27 12:39:43.000000 opd-101/opd.egg-info/SOURCES.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-27 12:39:43.000000 opd-101/opd.egg-info/dependency_links.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        4 2023-05-27 12:39:43.000000 opd-101/opd.egg-info/top_level.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-27 12:39:43.000000 opd-101/opd.egg-info/zip-safe
+-rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-05-27 12:39:43.730480 opd-101/setup.cfg
+-rw-r--r--   0 nop       (1000) nop       (1000)      770 2023-05-27 12:15:39.000000 opd-101/setup.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 12:39:43.730480 opd-101/test/
+-rw-r--r--   0 nop       (1000) nop       (1000)      471 2023-05-27 12:35:15.000000 opd-101/test/test_decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      369 2023-05-26 12:36:20.000000 opd-101/test/test_encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      883 2023-05-26 12:36:32.000000 opd-101/test/test_inherit.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     4568 2023-05-27 10:29:48.000000 opd-101/test/test_objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1031 2023-05-27 12:33:24.000000 opd-101/test/test_storage.py
```

### Comparing `opd-100/PKG-INFO` & `opd-101/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opd
-Version: 100
+Version: 101
 Summary: operator daemon
 Home-page: http://github.com/nopaths/opd
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
         
@@ -38,18 +38,23 @@
         
         **opd** stores it's data on disk where objects are time versioned and the
         last version saved on disk is served to the user layer. Files are JSON dumps
         and paths carry the type in the path name what makes reconstruction from
         filename easier then reading type from the object.
         
         
-        *INSTALL**
+        **INSTALL**
         
         
-        download the tarball from https://github.com/nopaths/opd/releases/
+        install from pypi::
+        
+         $ sudo python3 -m pip install opd
+        
+        
+        or download the tarball from https://github.com/nopaths/opd/releases/
         
         
         **USAGE**
         
         
         use an alias for easier typing::
```

### Comparing `opd-100/README.rst` & `opd-101/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,23 @@
 
 **opd** stores it's data on disk where objects are time versioned and the
 last version saved on disk is served to the user layer. Files are JSON dumps
 and paths carry the type in the path name what makes reconstruction from
 filename easier then reading type from the object.
 
 
-*INSTALL**
+**INSTALL**
 
 
-download the tarball from https://github.com/nopaths/opd/releases/
+install from pypi::
+
+ $ sudo python3 -m pip install opd
+
+
+or download the tarball from https://github.com/nopaths/opd/releases/
 
 
 **USAGE**
 
 
 use an alias for easier typing::
```

### Comparing `opd-100/opd/__main__.py` & `opd-101/opd/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 
 from .clients import Client
 from .command import Commands
 from .errored import Errors
 from .loggers import Logging
 from .objects import update
 from .persist import Persist, write
-from .runtime import Cfg, command, parse_cli
-from .threads import launch
+from .runtime import DATE, Cfg, command, launch, parse_cli
 from .utility import spl
 
 
 import opd.modules
 
 
 Persist.workdir = os.path.expanduser(f"~/.{Cfg.name}")
@@ -35,30 +34,32 @@
 
 class CLI(Client):
 
     def announce(self, txt):
         pass
 
     def raw(self, txt):
-        print(txt)
-        sys.stdout.flush()
+        cprint(txt)
 
 
 class Console(CLI):
 
     def handle(self, evt):
         CLI.handle(self, evt)
         evt.wait()
 
     def poll(self):
         return self.event(input("> "))
 
 
+## UTILITY
+
+
 def banner():
-    cprint(f"{Cfg.name.upper()} started at {Cfg.date}")
+    cprint(f"{Cfg.name.upper()} started at {DATE}")
     
 
 def daemon():
     pid = os.fork()
     if pid != 0:
         os._exit(0)
     os.setsid()
@@ -108,33 +109,36 @@
         print('')
     finally:
         if gotterm:
             termios.tcsetattr(fds, termios.TCSADRAIN, old)
         waiter()
 
 
+## RUNTIME
+
+
 def main():
     parse_cli(' '.join(sys.argv[1:]))
-    csl = Console()
-    if "v" in Cfg.opts:
+    if "v" in Cfg.opts and "d" not in Cfg.opts:
         Logging.debug = cprint
         banner()
     dowait = False
     if Cfg.txt:
         scanstr(Cfg.mod, "a" in Cfg.opts)
         cli = CLI()
         command(cli, Cfg.otxt)
     elif 'd' in Cfg.opts:
         daemon()
         dowait = True
     if "c" in Cfg.opts:
         dowait = True
     if dowait:
         scanstr(Cfg.mod, True)
-        if 'c' in Cfg.opts:
+        if 'c' in Cfg.opts and "d" not in Cfg.opts:
+            csl = Console()
             csl.start()
         while 1:
             time.sleep(1.0)
             waiter()
 
 
 if __name__ == "__main__":
```

### Comparing `opd-100/opd/command.py` & `opd-101/opd/command.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,34 @@
 
 
 import inspect
 
 
 from .errored import Errors
 from .objects import Object
+from .message import Message
 from .utility import spl
 
 
+def __dir__():
+    return (
+            'Commands',
+           )
+
+
 class Commands(Object):
 
     cmds = Object()
 
     @staticmethod
-    def add(cmd, func):
+    def add(cmd, func) -> None:
         setattr(Commands.cmds, cmd, func)
 
     @staticmethod
-    def handle(evt):
+    def handle(evt) -> Message:
         evt.parse(evt.txt)
         func = getattr(Commands.cmds, evt.cmd, None)
         if func:
             try:
                 func(evt)
                 evt.show()
             except Exception as ex:
```

### Comparing `opd-100/opd/decoder.py` & `opd-101/opd/decoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 import json
 
 
 from .objects import Object, copy
 
 
+def __dir__():
+    return (
+            'ObjectDecoder',
+            'load',
+            'loads'
+           )
+
+
 class ObjectDecoder(json.JSONDecoder):
 
     def decode(self, s, _w=None) -> Object:
         val = json.JSONDecoder.decode(self, s)
         if not val:
             val = {}
         obj = Object()
```

### Comparing `opd-100/opd/encoder.py` & `opd-101/opd/encoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 import json
 
 
 from .objects import Object
 
 
+def __dir__():
+    return (
+            'ObjectEncoder',
+            'dump',
+            'dumps'
+           )
+
+
 class ObjectEncoder(json.JSONEncoder):
 
 
     def default(self, o) -> str:
         if isinstance(o, dict):
             return o.items()
         if isinstance(o, Object):
```

### Comparing `opd-100/opd/handler.py` & `opd-101/opd/handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,71 +5,83 @@
 import ssl
 import threading
 
 
 from .errored import Errors
 from .objects import Object
 from .message import Message
-from .threads import launch
+from .runtime import Cfg, launch
+
+
+def __dir__():
+    return (
+            'Handler',
+           )
 
 
 class Handler(Object):
 
     def __init__(self):
         Object.__init__(self)
         self.cbs = Object()
         self.queue = queue.Queue()
         self.stopped = threading.Event()
-        self.register('command', self.handle)
+        self.threaded = True
 
-    @staticmethod
-    def dispatch(func, evt):
-        try:
-            func(evt)
-        except Exception as ex:
-            exc = ex.with_traceback(ex.__traceback__)
-            Errors.errors.append(exc)
-            evt.ready()
-
-    def event(self, txt):
+    def event(self, txt) -> Message:
         msg = Message()
         msg.type = 'command'
         msg.orig = repr(self)
         msg.parse(txt)
         return msg
 
-    def handle(self, evt):
+    def handle(self, evt) -> Message:
         func = getattr(self.cbs, evt.type, None)
         if func:
-            evt._thr = launch(self.dispatch, func, evt, name=evt.cmd)
+            if "t" in Cfg.opts:
+                evt._thr = launch(dispatch, func, evt, name=evt.cmd)
+            else:
+                dispatch(func, evt)
         return evt
 
-    def loop(self):
+    def loop(self) -> None:
         while not self.stopped.is_set():
             try:
                 self.handle(self.poll())
             except (ssl.SSLError, EOFError, KeyboardInterrupt) as ex:
                 Errors.handle(ex)
                 self.restart()
 
-    def one(self, txt):
+    def one(self, txt) -> Message:
         return self.handle(self.event(txt))
 
-    def poll(self):
+    def poll(self) -> Message:
         return self.queue.get()
 
-    def put(self, evt):
+    def put(self, evt) -> None:
         self.queue.put_nowait(evt)
 
-    def register(self, cmd, func):
+    def register(self, cmd, func) -> None:
         setattr(self.cbs, cmd, func)
 
-    def restart(self):
+    def restart(self) -> None:
         self.stop()
         self.start()
 
-    def start(self):
+    def start(self) -> None:
         launch(self.loop)
 
-    def stop(self):
+    def stop(self) -> None:
         self.stopped.set()
         self.queue.put_nowait(None)
+
+
+## HANDLERS
+
+
+def dispatch(func, evt) -> None:
+    try:
+        func(evt)
+    except Exception as ex:
+        exc = ex.with_traceback(ex.__traceback__)
+        Errors.errors.append(exc)
+        evt.ready()
```

### Comparing `opd-100/opd/listens.py` & `opd-101/opd/listens.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 # This file is placed in the Public Domain.
 
 
 from .objects import Object
 
 
+def __dir__():
+    return (
+            'Listens',
+           )
+
+
 class Listens(Object):
 
     objs = []
 
     @staticmethod
-    def add(obj):
+    def add(obj) -> None:
         Listens.objs.append(obj)
 
     @staticmethod
-    def announce(txt):
+    def announce(txt) -> None:
         for obj in Listens.objs:
             obj.announce(txt)
 
     @staticmethod
-    def byorig(orig):
+    def byorig(orig) -> Object:
         for obj in Listens.objs:
             if repr(obj) == orig:
                 return obj
         return None
 
     @staticmethod
-    def remove(bot):
+    def remove(bot) -> None:
         try:
             Listens.objs.remove(bot)
         except ValueError:
             pass
 
     @staticmethod
-    def say(orig, txt, channel=None):
+    def say(orig, txt, channel=None) -> None:
         bot = Listens.byorig(orig)
         if bot:
             if channel:
                 bot.say(channel, txt)
             else:
                 bot.raw(txt)
```

### Comparing `opd-100/opd/modules/fnd.py` & `opd-101/opd/modules/fnd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # This file is placed in the Public Domain.
 
 
 import time
 
 
-from ..objects import keys, prt
+from ..objects import keys
+from ..objfunc import prt
 from ..persist import Persist
 from ..utility import elapsed, fntime
 
 
+## COMMANDS
+
+
 def fnd(event):
     if not event.args:
         res = ','.join(sorted([x.split('.')[-1].lower() for x in Persist.files()]))
         if res:
             event.reply(res)
         else:
             event.reply('no types yet.')
```

### Comparing `opd-100/opd/modules/irc.py` & `opd-101/opd/modules/irc.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,31 +18,39 @@
 from ..clients import Client
 from ..command import Commands
 from ..default import Default
 from ..errored import Errors
 from ..message import Message
 from ..listens import Listens
 from ..loggers import Logging
-from ..objects import Object, copy, edit, keys, prt, update
+from ..objects import Object, copy, keys, update
+from ..objfunc import edit, prt
 from ..persist import Persist, last, write
-from ..runtime import Cfg
-from ..threads import launch
+from ..runtime import Cfg, launch
 from ..utility import elapsed, fntime
 
 
 saylock = _thread.allocate_lock()
 
 
 def start():
     irc = IRC()
     irc.start()
     irc.joined.wait()
     return irc
 
 
+class NoUser(Exception):
+
+    pass
+
+
+## CONFIG
+
+
 class Config(Default):
 
     channel = '#%s' % Cfg.name
     control = '!'
     nick = Cfg.name
     password = ''
     port = 6667
@@ -71,14 +79,17 @@
         self.users = Config.users
         self.verbose = Config.verbose
 
 
 Persist.add(Config)
 
 
+## OUTPUT
+
+
 class TextWrap(textwrap.TextWrapper):
 
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = True
         self.fix_sentence_endings = True
@@ -153,14 +164,17 @@
         return self
 
     def stop(self):
         self.dostop.set()
         self.oqueue.put_nowait((None, None))
 
 
+## IRC
+
+
 class IRC(Client, Output):
 
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
@@ -553,17 +567,28 @@
     def stop(self):
         Listens.remove(self)
         Client.stop(self)
         Output.stop(self)
         self.disconnect()
 
 
-class NoUser(Exception):
+## USERS
 
-    pass
+
+class User(Object):
+
+    def __init__(self, val=None):
+        Object.__init__(self)
+        self.user = ''
+        self.perms = []
+        if val:
+            update(self, val)
+
+
+Persist.add(User)
 
 
 class Users(Object):
 
     @staticmethod
     def allowed(origin, perm):
         perm = perm.upper()
@@ -605,25 +630,15 @@
             raise NoUser(origin)
         if permission.upper() not in user.perms:
             user.perms.append(permission.upper())
             write(user)
         return user
 
 
-class User(Object):
-
-    def __init__(self, val=None):
-        Object.__init__(self)
-        self.user = ''
-        self.perms = []
-        if val:
-            update(self, val)
-
-
-Persist.add(User)
+## COMMANDS
 
 
 def cfg(event):
     config = Config()
     last(config)
     if not event.sets:
         event.reply(prt(
```

### Comparing `opd-100/opd/modules/log.py` & `opd-101/opd/modules/log.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,17 @@
         super().__init__()
         self.txt = ''
 
 
 Persist.add(Log)
 
 
+## COMMANDS
+
+
 def log(event):
     if not event.rest:
         nmr = 0
         for obj in Persist.find('log'):
             lap = elapsed(time.time() - fntime(obj.__oid__))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
```

### Comparing `opd-100/opd/modules/rss.py` & `opd-101/opd/modules/rss.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
 from ..listens import Listens
-from ..objects import Object, prt, update
+from ..objects import Object, update
+from ..objfunc import prt
 from ..persist import Persist, last, write
 from ..repeats import Repeater
-from ..runtime import Cfg
-from ..threads import launch, threaded
+from ..runtime import Cfg, launch, threaded
 from ..utility import elapsed, fntime, spl
 
 
 def start():
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
@@ -168,15 +168,15 @@
             obj = Object()
             for itm in spl(item):
                 setattr(obj, itm, Parser.getitem(line, itm))
             res.append(obj)
         return res
 
 
-## utilties
+## UTILITIES
 
 
 def getfeed(url, item):
     if Cfg.debug:
         return [Object(), Object()]
     try:
         result = geturl(url)
@@ -224,15 +224,15 @@
     return html.unescape(txt)
 
 
 def useragent(txt):
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
-## commands
+## COMMANDS
 
 
 def dpl(event):
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
```

### Comparing `opd-100/opd/modules/tdo.py` & `opd-101/opd/modules/tdo.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,17 @@
         super().__init__()
         self.txt = ''
 
 
 Persist.add(Todo)
 
 
+## COMMANDS
+
+
 def dne(event):
     if not event.args:
         return
     selector = {'txt': event.args[0]}
     for obj in Persist.find('todo', selector):
         obj.__deleted__ = True
         write(obj)
```

### Comparing `opd-100/opd/modules/thr.py` & `opd-101/opd/modules/thr.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 
 
 import threading
 import time
 
 
 from ..objects import Object, update
+from ..runtime import STARTTIME
 from ..utility import elapsed
 
 
-starttime = time.time()
+## COMMANDS
 
 
 def thr(event):
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.getName()):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
             uptime = obj.sleep - int(time.time() - obj.state.latest)
         elif getattr(obj, 'starttime', None):
             uptime = int(time.time() - obj.starttime)
         else:
-            uptime = int(time.time() - starttime)
+            uptime = int(time.time() - STARTTIME)
         result.append((uptime, thread.name))
     res = []
     for uptime, txt in sorted(result, key=lambda x: x[0]):
         lap = elapsed(uptime)
         res.append(f'{txt}/{lap}')
     if res:
         event.reply(' '.join(res))
```

### Comparing `opd-100/opd/persist.py` & `opd-101/opd/persist.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 import time
 import _thread
 
 
 from .decoder import ObjectDecoder, load
 from .default import Default
 from .encoder import dump
-from .errored import NoClassError
-from .objects import Object, kind, search, update
+from .objects import Object, kind, update
+from .objfunc import search
 from .utility import cdir, fnclass, fntime, strip
 
 
 def __dir__():
     return (
             'Persist',
+            'last',
+            'read',
+            'write'
            )
 
-__all__ = __dir__()
-
 
 disklock = _thread.allocate_lock()
 
 
 class Persist(Object):
 
     cls = Default()
@@ -77,27 +78,27 @@
                             yield strip(path2)
 
     @staticmethod
     def get(cmd) -> type:
         return getattr(Persist.cls, cmd, None)
 
     @staticmethod
-    def hook(otp) -> Object:
+    def hook(otp) -> type:
         clz = fnclass(otp)
         cls = Persist.get(clz)
         if cls:
             obj = cls()
             read(obj, otp)
             return obj
         obj = Object()
         read(obj, otp)
         return obj
 
     @staticmethod
-    def logdir():
+    def logdir() -> str:
         return os.path.join(Persist.workdir, "logs")
 
     @staticmethod
     def match(mtc, selector=None) -> []:
         if selector is None:
             selector = {}
         for tpe in Persist.clz(mtc):
@@ -109,21 +110,20 @@
                     continue
                 yield obj
 
     @staticmethod
     def path(pth) -> str:
         return os.path.join(Persist.workdir, 'store', pth)
 
-
     @staticmethod
     def remove(clz) -> None:
         delattr(Persist.cls, f"{clz.__module__}.{clz.__name__}")
 
     @staticmethod
-    def storedir():
+    def storedir() -> str:
         return os.path.join(Persist.workdir, "store")
 
 
 def last(obj, selector=None) -> None:
     if selector is None:
         selector = {}
     result = sorted(
```

### Comparing `opd-100/opd/utility.py` & `opd-101/opd/utility.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 # This file is placed in the Public Domain.
 
 
 import os
 import pathlib
 import time
+import types
+
+
+def __dir__():
+    return (
+            'cdir',
+            'doskip',
+            'elapsed',
+            'fnclass',
+            'fntime',
+            'name',
+            'spl',
+            'strip',
+            'touch'
+           )
 
 
 def cdir(pth) -> None:
     if not pth.endswith(os.sep):
         pth = os.path.dirname(pth)
     pth = pathlib.Path(pth)
     os.makedirs(pth, exist_ok=True)
@@ -80,14 +95,29 @@
     if rest:
         tme += float('.' + rest)
     else:
         tme = 0
     return tme
 
 
+def name(obj):
+    typ = type(obj)
+    if isinstance(typ, types.ModuleType):
+        return obj.__name__
+    if '__self__' in dir(obj):
+        return '%s.%s' % (obj.__self__.__class__.__name__, obj.__name__)
+    if '__class__' in dir(obj) and '__name__' in dir(obj):
+        return '%s.%s' % (obj.__class__.__name__, obj.__name__)
+    if '__class__' in dir(obj):
+        return obj.__class__.__name__
+    if '__name__' in dir(obj):
+        return '%s.%s' % (obj.__class__.__name__, obj.__name__)
+    return None
+
+
 def spl(txt) -> []:
     try:
         res = txt.split(',')
     except (TypeError, ValueError):
         res = txt
     return [x for x in res if x]
```

### Comparing `opd-100/opd.egg-info/PKG-INFO` & `opd-101/opd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opd
-Version: 100
+Version: 101
 Summary: operator daemon
 Home-page: http://github.com/nopaths/opd
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
         
@@ -38,18 +38,23 @@
         
         **opd** stores it's data on disk where objects are time versioned and the
         last version saved on disk is served to the user layer. Files are JSON dumps
         and paths carry the type in the path name what makes reconstruction from
         filename easier then reading type from the object.
         
         
-        *INSTALL**
+        **INSTALL**
         
         
-        download the tarball from https://github.com/nopaths/opd/releases/
+        install from pypi::
+        
+         $ sudo python3 -m pip install opd
+        
+        
+        or download the tarball from https://github.com/nopaths/opd/releases/
         
         
         **USAGE**
         
         
         use an alias for easier typing::
```

### Comparing `opd-100/opd.egg-info/SOURCES.txt` & `opd-101/opd.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 opd/encoder.py
 opd/errored.py
 opd/handler.py
 opd/listens.py
 opd/loggers.py
 opd/message.py
 opd/objects.py
+opd/objfunc.py
 opd/parsers.py
 opd/persist.py
 opd/repeats.py
 opd/runtime.py
 opd/threads.py
 opd/utility.py
 opd.egg-info/PKG-INFO
@@ -34,12 +35,13 @@
 opd/modules/log.py
 opd/modules/mod.py
 opd/modules/rss.py
 opd/modules/sts.py
 opd/modules/tdo.py
 opd/modules/thr.py
 opd/modules/upt.py
+opd/modules/ver.py
 test/test_decoder.py
 test/test_encoder.py
 test/test_inherit.py
 test/test_objects.py
 test/test_storage.py
```

### Comparing `opd-100/setup.py` & `opd-101/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def read():
     return open("README.rst", "r").read()
 
 
 setup(
     name="opd",
-    version="100",
+    version="101",
     author="No Paths <nopaths@proton.me>",
     author_email="nopaths@proton.me",
     url="http://github.com/nopaths/opd",
     zip_safe=True,
     description="operator daemon",
     long_description=read(),
     long_description_content_type="text/x-rst",
```

### Comparing `opd-100/test/test_inherit.py` & `opd-101/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `opd-100/test/test_objects.py` & `opd-101/test/test_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import sys
 import unittest
 
 
 sys.path.insert(0, "..")
 
 
-from opd.objects import Object, items, keys, kind, prt, update, values
+from opd.objects import Object, items, keys, kind, update, values
+from opd.objfunc import prt
 
 
 VALIDJSON = '{"test": "bla"}'
 
 
 attrs1 = (
          'Object',
```

### Comparing `opd-100/test/test_storage.py` & `opd-101/test/test_storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
 
 Persist.workdir = '.test'
 
 
 ATTRS1 = (
           'Persist',
+          'last',
+          'read',
+          'write'
          )
 
 
 class TestStorage(unittest.TestCase):
 
     def test_constructor(self):
         obj = Persist()
```

