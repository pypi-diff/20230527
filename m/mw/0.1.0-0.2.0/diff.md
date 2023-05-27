# Comparing `tmp/mw-0.1.0.tar.gz` & `tmp/mw-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mw-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mw-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mw-0.1.0.tar` & `mw-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1319 2023-05-25 06:23:29.988392 mw-0.1.0/README.md
--rw-r--r--   0        0        0     5847 2023-05-25 06:23:29.988392 mw-0.1.0/data/share/man/man1/mw.1
--rw-r--r--   0        0        0      117 2023-05-25 06:23:29.988392 mw-0.1.0/mw/__init__.py
--rw-r--r--   0        0        0      772 2023-05-25 06:23:29.988392 mw-0.1.0/mw/__main__.py
--rw-r--r--   0        0        0     1819 2023-05-25 06:23:29.988392 mw-0.1.0/mw/app.py
--rw-r--r--   0        0        0     8160 2023-05-25 06:23:29.988392 mw-0.1.0/mw/command_handler.py
--rw-r--r--   0        0        0     3775 2023-05-25 06:23:29.988392 mw-0.1.0/mw/display.py
--rw-r--r--   0        0        0     4988 2023-05-25 06:23:29.988392 mw-0.1.0/mw/stack.py
--rw-r--r--   0        0        0       74 2023-05-25 06:23:29.988392 mw-0.1.0/mw/types.py
--rw-r--r--   0        0        0     1688 2023-05-25 06:23:29.988392 mw-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 mw-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1319 2023-05-27 06:35:15.007786 mw-0.2.0/README.md
+-rw-r--r--   0        0        0     6176 2023-05-27 06:35:15.007786 mw-0.2.0/data/share/man/man1/mw.1
+-rw-r--r--   0        0        0      117 2023-05-27 06:35:15.007786 mw-0.2.0/mw/__init__.py
+-rw-r--r--   0        0        0      772 2023-05-27 06:35:15.007786 mw-0.2.0/mw/__main__.py
+-rw-r--r--   0        0        0     1819 2023-05-27 06:35:15.007786 mw-0.2.0/mw/app.py
+-rw-r--r--   0        0        0     8735 2023-05-27 06:35:15.007786 mw-0.2.0/mw/command_handler.py
+-rw-r--r--   0        0        0     3775 2023-05-27 06:35:15.007786 mw-0.2.0/mw/display.py
+-rw-r--r--   0        0        0     5467 2023-05-27 06:35:15.007786 mw-0.2.0/mw/stack.py
+-rw-r--r--   0        0        0       74 2023-05-27 06:35:15.007786 mw-0.2.0/mw/types.py
+-rw-r--r--   0        0        0     1688 2023-05-27 06:35:15.007786 mw-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 mw-0.2.0/PKG-INFO
```

### Comparing `mw-0.1.0/README.md` & `mw-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mw-0.1.0/data/share/man/man1/mw.1` & `mw-0.2.0/data/share/man/man1/mw.1`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .TH mw 1 "2023-05-23" "Jamie Hardt" "User Manuals"
 .SH NAME 
 mw \- audio sample editor
 .SH SYNOPSIS
 .SY mw
-.RI "[\-c " COMMAND " ]"
+.RI "[\-e " COMMAND "]"
 .RI "[" "FILE ..." "]"
-.YS
 .SH DESCRIPTION
 .B mw
 is an interactive, text-mode audio sample editor. Audio files provided as arguments
 on the command line can be inspected, edited, mixed and exported.
 .SS MOTIVATION
 .B mw
 is an audio sample editor, designed to edit individual, contiguous sounds in a manner 
@@ -45,20 +44,22 @@
 .PP
 Each individual sound on the stack is contained in a 
 .B
 frame
 which also maintains editing context pertinent to the sound, such as the location of the
 cursor and selection in- and out-points.
 .SH OPTIONS
-.IP "\-c COMMAND"
+.IP "\-e COMMAND, \-\-exec=COMMAND"
 Execute 
 .I COMMAND
 after loading 
 .IR FILE "s."
 Can be used multiple times to run multiple commands.
+.IP "\-h, \-\-help"
+Print brief help.
 .SH COMMANDS
 The command prompt in 
 .B mw
 accepts lines of commands which begin with a command
 .I keyword
 followed by zero or more arguments.
 .P
@@ -133,14 +134,24 @@
 Inserts silence of length
 .I dur
 milliseconds at the cursor.
 .IP split
 Splits the sound at the cursor position. The current sound is popped off the stack. 
 Two new sounds are pushed onto the stack, the first made of the samples preceding the
 cursor and the second of samples following the cursor.
+.IP append
+Appends the 2nd-highest sound on the stack to the end of the top sound on the stack. 
+.IP prepend 
+Prepends the 2nd-highest sound on the stack to the end of the top sound on the stack. 
+(Reverses a 
+.IR split ")."
+.IP loop [count]
+Loops the selection
+.I count
+times.
 .IP fadein
 Applies a linear fade to the sound, increasing from the beginning of the sound to the 
 cursor.
 .IP fadeout
 Applies a linear fade to the sound, decreasing from the cursor to the end of the sound.
 .IP play
 Plays the sound.
```

### Comparing `mw-0.1.0/mw/__main__.py` & `mw-0.2.0/mw/__main__.py`

 * *Files identical despite different names*

### Comparing `mw-0.1.0/mw/app.py` & `mw-0.2.0/mw/app.py`

 * *Files identical despite different names*

### Comparing `mw-0.1.0/mw/command_handler.py` & `mw-0.2.0/mw/command_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import inspect
 from copy import deepcopy
 from typing import List, Callable, Optional
 import sys, os
 
 import mw
+from mw.stack import StackFrame
 from mw.types import Milliseconds
 
 def parse_numeric(base_value: int, val: str):
     """
     A helper function for converting numeric entries from the command prompt.
     """
     if val[0] in ["+","-"] and val[1:].isdigit():
@@ -183,14 +184,32 @@
 
     def split(self, app:'mw.app.App'):
         "Split sound"
         if app.stack.top:
             app.stack.split()
         app.display.print_stack(app.stack)
 
+    def append(self, app:'mw.app.App'):
+        "Append sound"
+        if len(app.stack.entries) > 1:
+            app.stack.append()
+        app.display.print_stack(app.stack)
+
+    def prepend(self, app:'mw.app.App'):
+        "Prepend sound"
+        if len(app.stack.entries) > 1:
+            app.stack.prepend()
+        app.display.print_stack(app.stack)
+
+    def loop(self, app:'mw.app.App', count = "2"):
+        "Loop sound"
+        if app.stack.top:
+            app.stack.loop(count=int(count))
+        app.display.print_head(app.stack)
+
     def fadein(self, app:'mw.app.App'):
         "Fade in from cilp start to cursor"
         if app.stack.top:
             app.stack.top.fade_in(app.stack.top.cursor)
 
         app.display.print_head(app.stack)
```

### Comparing `mw-0.1.0/mw/display.py` & `mw-0.2.0/mw/display.py`

 * *Files identical despite different names*

### Comparing `mw-0.1.0/mw/stack.py` & `mw-0.2.0/mw/stack.py`

 * *Files 14% similar despite different names*

```diff
@@ -130,18 +130,36 @@
         at = self.top.cursor
         a = cast(AudioSegment, to_split[0:at])
         b = cast(AudioSegment, to_split[at:])
         self.entries.pop()
         self.entries.append(StackFrame(a))
         self.entries.append(StackFrame(b))
 
-        self.cursor = 0
-        self.in_point = None
-        self.out_point = None
-    
+   
+    def append(self):
+        assert len(self.entries) > 1
+
+        a = self.entries.pop().segment
+        b = self.entries.pop().segment
+        self.entries.append(StackFrame(a + b))
+
+        
+    def prepend(self):
+        assert len(self.entries) > 1
+
+        a = self.entries.pop().segment
+        b = self.entries.pop().segment
+        self.entries.append(StackFrame(b + a))
+
+    def loop(self, count: int = 2):
+        assert len(self.entries) > 0
+        a = self.entries.pop()
+        segment = cast(AudioSegment, a.segment[a.in_point or 0:a.out_point or len(a.segment)])
+        self.entries.append(StackFrame(segment * count))
+
     def bounce(self):
         assert len(self.entries) > 1
         
         a = self.entries[-1].segment
         b = self.entries[-2].segment
 
         if len(a) < len(b):
@@ -149,15 +167,11 @@
 
         self.entries.pop()
         self.entries.pop()
 
         self.entries.append(StackFrame(a.overlay(b)))
 
 
-
-
     def length(self) -> Milliseconds:
-        if len(self.entries) > 0:
-            return Milliseconds(max(map(lambda x: len(x.clip()), self.entries)))
-        else:
-            return Milliseconds(0)
+        return Milliseconds(max(list(map(lambda x: len(x.clip()), self.entries)) + [0]))
+
```

### Comparing `mw-0.1.0/pyproject.toml` & `mw-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mw-0.1.0/PKG-INFO` & `mw-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mw
-Version: 0.1.0
+Version: 0.2.0
 Summary: mw is an audio sample editor for the terminal.
 Keywords: waveform,metadata,audio,console
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
```

