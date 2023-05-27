# Comparing `tmp/gqylpy_ssh-1.2.5-py3-none-any.whl.zip` & `tmp/gqylpy_ssh-1.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 19056 bytes, number of entries: 7
--rw-r--r--  2.0 unx    21469 b- defN 23-Apr-29 01:56 gqylpy_ssh/__init__.py
--rw-r--r--  2.0 unx    10214 b- defN 23-Apr-29 01:56 gqylpy_ssh/g ssh.py
--rw-r--r--  2.0 unx    26436 b- defN 23-Apr-29 01:56 gqylpy_ssh-1.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2192 b- defN 23-Apr-29 01:56 gqylpy_ssh-1.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 01:56 gqylpy_ssh-1.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-29 01:56 gqylpy_ssh-1.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      559 b- defN 23-Apr-29 01:56 gqylpy_ssh-1.2.5.dist-info/RECORD
-7 files, 60973 bytes uncompressed, 18072 bytes compressed:  70.4%
+Zip file size: 19159 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    21612 b- defN 23-May-27 05:04 gqylpy_ssh/__init__.py
+-rw-r--r--  2.0 unx    10278 b- defN 23-May-27 05:04 gqylpy_ssh/g ssh.py
+-rw-r--r--  2.0 unx    26436 b- defN 23-May-27 05:04 gqylpy_ssh-1.2.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2256 b- defN 23-May-27 05:04 gqylpy_ssh-1.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-27 05:04 gqylpy_ssh-1.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-27 05:04 gqylpy_ssh-1.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      559 b- defN 23-May-27 05:04 gqylpy_ssh-1.2.6.dist-info/RECORD
+7 files, 61244 bytes uncompressed, 18175 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: gqylpy_ssh/__init__.py
 Comment: 
 
 Filename: gqylpy_ssh/g ssh.py
 Comment: 
 
-Filename: gqylpy_ssh-1.2.5.dist-info/LICENSE
+Filename: gqylpy_ssh-1.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: gqylpy_ssh-1.2.5.dist-info/METADATA
+Filename: gqylpy_ssh-1.2.6.dist-info/METADATA
 Comment: 
 
-Filename: gqylpy_ssh-1.2.5.dist-info/WHEEL
+Filename: gqylpy_ssh-1.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: gqylpy_ssh-1.2.5.dist-info/top_level.txt
+Filename: gqylpy_ssh-1.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: gqylpy_ssh-1.2.5.dist-info/RECORD
+Filename: gqylpy_ssh-1.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gqylpy_ssh/__init__.py

```diff
@@ -6,15 +6,15 @@
 
     >>> from gqylpy_ssh import GqylpySSH, Command
     >>> ssh = GqylpySSH('192.168.1.7', 22, username='gqylpy', password=...)
     >>> c: Command = ssh.cmd('echo Hi, GQYLPY')
     >>> c.status_output
     (True, 'Hi, GQYLPY')
 
-    @version: 1.2.5
+    @version: 1.2.6
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-ssh
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 This file is part of gqylpy-ssh.
@@ -100,15 +100,15 @@
     @param passphrase:          Used for decrypting private keys.
     @param disabled_algorithms: An optional dictionary passed to `Transport` and
                                 its namesake keyword argument.
     @param sock:                An open socket or socket-like object (such as a
                                 `.Channel`) to use for communication to the
                                 target host.
     @param auto_sudo:           Automatically add "sudo" to the front of the
-                                command.
+                                command, always invalid for root user.
     @param reconnect:           If the ssh connection is disconnected when you
                                 call method `self.cmd`, will attempt to
                                 reconnect.
 
     @param gname: Create a pointer to an instance of `GqylpySSH` in the
                   `gqylpy_ssh` module, if not None.
 
@@ -140,18 +140,15 @@
         reconnect          =reconnect
     )
 
     if gname is None:
         return gobj
 
     gpack = globals()
-
-    if '__first__' not in gpack:
-        gpack['__first__'] = gobj
-
+    gpack.setdefault('__first__', gobj)
     gpack[gname] = gobj
 
 
 class GqylpySSH(paramiko.SSHClient):
 
     def __init__(
         self,
@@ -211,15 +208,15 @@
         @param passphrase:          Used for decrypting private keys.
         @param disabled_algorithms: An optional dictionary passed to `Transport`
                                     and its namesake keyword argument.
         @param sock:                An open socket or socket-like object (such
                                     as a `.Channel`) to use for communication to
                                     the target host.
         @param auto_sudo:           Automatically add "sudo" to the front of the
-                                    command.
+                                    command, always invalid for root user.
         @param reconnect:           If the ssh connection is disconnected when
                                     you call method `self.cmd`, will attempt to
                                     reconnect.
         """
         super().__init__()
 
         self.connect(
@@ -269,15 +266,17 @@
         @param command: A command string.
         @param timeout: Execute command timeout, default permanent.
         @param bufsize: Buffer size, default permanent.
         @param get_pty: Whether to enable pseudo-terminal, default False.
         @param env:     A dictionary of environment variables. Indication:
                         server may reject environment variables.
         """
-        if self.auto_sudo and not command.startswith('sudo '):
+        if self.auto_sudo and not (
+                self.params['username'] == 'root' or command.startswith('sudo ')
+        ):
             command = f'sudo {command}'
 
         if command[-1] == '&':
             return self.cmd_async(
                 command=command,
                 timeout=timeout,
                 bufsize=bufsize,
@@ -542,14 +541,18 @@
 IncompatiblePeer          = paramiko.ssh_exception.IncompatiblePeer
 ProxyCommandFailure       = paramiko.ssh_exception.ProxyCommandFailure
 NoValidConnectionsError   = paramiko.ssh_exception.NoValidConnectionsError
 CouldNotCanonicalize      = paramiko.ssh_exception.CouldNotCanonicalize
 ConfigParseError          = paramiko.ssh_exception.ConfigParseError
 
 
+class SSHCommandError(SSHException):
+    ...
+
+
 class _xe6_xad_x8c_xe7_x90_xaa_xe6_x80_xa1_xe7_x8e_xb2_xe8_x90_x8d_xe4_xba_x91:
     gpack = globals()
     gpath = f'{__name__}.g {__name__[7:]}'
     gcode = __import__(gpath, fromlist=...)
 
     for gname in gpack:
         try:
```

## gqylpy_ssh/g ssh.py

```diff
@@ -11,15 +11,14 @@
 gqylpy-ssh is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License along
 with gqylpy-ssh. If not, see <https://www.gnu.org/licenses/>.
 """
-import sys
 import builtins
 import warnings
 import functools
 import threading
 
 import paramiko
 
@@ -30,16 +29,16 @@
 from paramiko.ssh_exception import NoValidConnectionsError
 
 from paramiko.channel import ChannelFile
 from paramiko.channel import ChannelStderrFile
 
 first: 'GqylpySSH'
 
-gpack = sys.modules[__package__]
-gcode = sys.modules[__name__]
+gpack = __import__(__package__)
+gcode = globals()
 
 
 def __init__(
         hostname: str,
         port:     int = 22,
         *,
         gname:    str = None,
@@ -50,16 +49,16 @@
     if gname is None:
         return gobj
 
     if gname.__class__ is not str:
         x: str = gname.__class__.__name__
         raise TypeError(f'gname type must be "str", not "{x}".')
 
-    if not hasattr(gcode, 'first'):
-        gcode.first = gobj
+    if 'first' not in gcode:
+        gcode['first'] = gobj
 
     setattr(gpack, gname, gobj)
 
 
 class GqylpySSH(SSHClient):
 
     def __init__(self, hostname: str, port: int = 22, **params):
@@ -131,18 +130,20 @@
                 command=command,
                 timeout=timeout,
                 bufsize=bufsize,
                 get_pty=get_pty,
                 env=env
             )
 
-        if self.auto_sudo and not command.startswith('sudo '):
+        if self.auto_sudo and not (
+                self.params['username'] == 'root' or command.startswith('sudo ')
+        ):
             command = f'sudo {command}'
 
-        command += '&& echo 4289077'
+        command += ' && echo 4289077'
         timeout = timeout or self.command_timeout
 
         try:
             _, stdout, stderr = self.exec_command(
                 command=command,
                 timeout=timeout,
                 bufsize=bufsize,
@@ -161,15 +162,15 @@
                     command=command,
                     timeout=timeout,
                     bufsize=bufsize,
                     get_pty=get_pty,
                     environment=env
                 )
 
-        return Command(command, stdout, stderr)
+        return Command(command[:-16], stdout, stderr)
 
     def cmd_many(self, commands: (tuple, list), **kw):
         if commands.__class__ is tuple:
             for c in commands:
                 c: str = c.rstrip()
                 if c[-1] == '&':
                     c = c[:-1]
@@ -278,15 +279,15 @@
         )
 
 
 def gname2gobj(func):
     @functools.wraps(func)
     def inner(*a, gname: (str, GqylpySSH) = None, **kw):
         if gname is None:
-            if not hasattr(gcode, 'first'):
+            if 'first' not in gcode:
                 raise RuntimeError(
                     'you did not create the default GqylpySSH instance.'
                 )
             gobj: GqylpySSH = first
         elif gname.__class__ is str:
             gobj: GqylpySSH = getattr(gpack, gname, None)
             if gobj.__class__ is not GqylpySSH:
@@ -318,12 +319,12 @@
 @gname2gobj
 def cmd_async(
         command: str, *, gobj: GqylpySSH = None, **kw
 ) -> threading.Thread:
     return gobj.cmd_async(command, **kw)
 
 
-class SSHCommandError(Exception):
+class SSHCommandError(SSHException):
     __module__ = 'builtins'
 
 
-builtins.SSHCommandError = SSHCommandError
+gpack.SSHCommandError = builtins.SSHCommandError = SSHCommandError
```

## Comparing `gqylpy_ssh-1.2.5.dist-info/LICENSE` & `gqylpy_ssh-1.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gqylpy_ssh-1.2.5.dist-info/METADATA` & `gqylpy_ssh-1.2.6.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: gqylpy-ssh
-Version: 1.2.5
+Version: 1.2.6
 Summary: 在远程服务器执行命令并得到执行结果，它是对 paramiko 库的二次封装。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: LGPL
 Project-URL: Source, https://github.com/gqylpy/gqylpy-ssh
-Classifier: Environment :: Web Environment
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Utilities
-Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Terminals :: Telnet
+Classifier: Topic :: Security :: Cryptography
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6, <4
@@ -26,15 +27,15 @@
 License-File: LICENSE
 Requires-Dist: paramiko (<4.0,>=3.1.0)
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-ssh.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-ssh/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_ssh)](https://pypi.org/project/gqylpy_ssh)
 [![License](https://img.shields.io/pypi/l/gqylpy_ssh)](https://github.com/gqylpy/gqylpy-ssh/blob/master/LICENSE)
-[![Downloads](https://pepy.tech/badge/gqylpy_ssh/month)](https://pepy.tech/project/gqylpy_ssh)
+[![Downloads](https://pepy.tech/badge/gqylpy_ssh)](https://pepy.tech/project/gqylpy_ssh)
 
 # gqylpy-ssh
 
 > 在远程服务器执行命令并得到执行结果，它是对 paramiko 库的二次封装。在 `Command` 对象中，提供了多种方法用于判断命令执行结果是否如期。
 
 <kbd>pip3 install gqylpy_ssh</kbd>
```

