# Comparing `tmp/global_hotkeys-0.0.4.tar.gz` & `tmp/global_hotkeys-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\global_hotkeys-0.0.4.tar", last modified: Wed Dec  2 01:56:21 2020, max compression
+gzip compressed data, was "global_hotkeys-0.0.5.tar", last modified: Sat May 27 08:28:41 2023, max compression
```

## Comparing `global_hotkeys-0.0.4.tar` & `global_hotkeys-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2020-12-02 01:56:21.000000 global_hotkeys-0.0.4/
--rw-rw-rw-   0        0        0      333 2020-12-02 01:56:08.000000 global_hotkeys-0.0.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1051 2020-12-01 08:02:57.000000 global_hotkeys-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2020-11-08 08:19:07.000000 global_hotkeys-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6465 2020-12-02 01:56:21.000000 global_hotkeys-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3569 2020-12-01 21:05:51.000000 global_hotkeys-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2020-12-02 01:56:21.000000 global_hotkeys-0.0.4/global_hotkeys/
--rw-rw-rw-   0        0        0     1455 2020-12-01 13:36:12.000000 global_hotkeys-0.0.4/global_hotkeys/__init__.py
--rw-rw-rw-   0        0        0     4417 2020-12-01 13:28:57.000000 global_hotkeys-0.0.4/global_hotkeys/hotkey_checker.py
--rw-rw-rw-   0        0        0     2525 2020-12-01 11:41:12.000000 global_hotkeys-0.0.4/global_hotkeys/keycodes.py
-drwxrwxrwx   0        0        0        0 2020-12-02 01:56:21.000000 global_hotkeys-0.0.4/global_hotkeys.egg-info/
--rw-rw-rw-   0        0        0     6465 2020-12-02 01:56:21.000000 global_hotkeys-0.0.4/global_hotkeys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2020-12-02 01:56:21.000000 global_hotkeys-0.0.4/global_hotkeys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-02 01:56:21.000000 global_hotkeys-0.0.4/global_hotkeys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2020-12-02 01:56:21.000000 global_hotkeys-0.0.4/global_hotkeys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2020-12-02 01:56:21.000000 global_hotkeys-0.0.4/global_hotkeys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-12-02 01:56:21.000000 global_hotkeys-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      793 2020-12-02 01:51:39.000000 global_hotkeys-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2020-12-02 01:56:21.000000 global_hotkeys-0.0.4/tests/
--rw-rw-rw-   0        0        0      841 2020-12-01 13:32:03.000000 global_hotkeys-0.0.4/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:28:41.220670 global_hotkeys-0.0.5/
+-rw-rw-rw-   0        0        0      439 2023-05-27 08:19:11.000000 global_hotkeys-0.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4914 2023-05-27 08:28:41.220670 global_hotkeys-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3941 2023-05-27 07:59:16.000000 global_hotkeys-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 08:28:41.205671 global_hotkeys-0.0.5/global_hotkeys/
+-rw-rw-rw-   0        0        0     1455 2023-05-27 07:09:18.000000 global_hotkeys-0.0.5/global_hotkeys/__init__.py
+-rw-rw-rw-   0        0        0     6018 2023-05-27 07:48:35.000000 global_hotkeys-0.0.5/global_hotkeys/hotkey_checker.py
+-rw-rw-rw-   0        0        0     2605 2023-05-27 07:53:05.000000 global_hotkeys-0.0.5/global_hotkeys/keycodes.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:28:41.218672 global_hotkeys-0.0.5/global_hotkeys.egg-info/
+-rw-rw-rw-   0        0        0     4914 2023-05-27 08:28:41.000000 global_hotkeys-0.0.5/global_hotkeys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-27 08:28:41.000000 global_hotkeys-0.0.5/global_hotkeys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 08:28:41.000000 global_hotkeys-0.0.5/global_hotkeys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-27 08:28:41.000000 global_hotkeys-0.0.5/global_hotkeys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-27 08:28:41.000000 global_hotkeys-0.0.5/global_hotkeys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 08:28:41.221469 global_hotkeys-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-05-27 08:28:28.000000 global_hotkeys-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:28:41.219671 global_hotkeys-0.0.5/tests/
+-rw-rw-rw-   0        0        0      889 2023-05-27 07:59:21.000000 global_hotkeys-0.0.5/tests/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `global_hotkeys-0.0.4/LICENSE.txt` & `global_hotkeys-0.0.5/LICENSE.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
 Copyright 2020 btsdev
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `global_hotkeys-0.0.4/README.md` & `global_hotkeys-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -91,14 +91,17 @@
 alt
 pause
 caps_lock
 escape
 space   <-- a literal space character (' ') can be used as well.
 page_up
 page_down
+left_window  <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
+right_window <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
+window       <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
 end
 home
 left
 up
 right
 down
 select
```

### Comparing `global_hotkeys-0.0.4/global_hotkeys/__init__.py` & `global_hotkeys-0.0.5/global_hotkeys/__init__.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.0.4/global_hotkeys/hotkey_checker.py` & `global_hotkeys-0.0.5/global_hotkeys/hotkey_checker.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,20 +4,30 @@
 import ctypes
 from ctypes import wintypes
 import win32con
 import win32api
 
 from .keycodes import vk_key_names
 
+
 def _to_virtualkey(key):
     virtual_key = None
     if key.lower() in vk_key_names.keys():
         virtual_key = vk_key_names[key.lower()]
     return virtual_key
 
+full_modifier_list = [
+    _to_virtualkey("control"),
+    _to_virtualkey("shift"),
+    _to_virtualkey("alt"),
+    _to_virtualkey("left_window"),
+    _to_virtualkey("right_window"),
+    _to_virtualkey("window"),
+]
+
 class EngineState:
 
     def __init__(self, active=True):
         self.active = active
 
 
 class HotkeyChecker():
@@ -115,19 +125,45 @@
             for id in id_list:
                 hotkey = self.hotkeys[id]
                 press_callback, release_callback, key_state = self.hotkey_actions[id]
 
                 # check to see if all keys in the hotkey are pressed.
                 pressed = True
                 for key in hotkey:
-                    specific_key_state = win32api.GetAsyncKeyState(key)
-                    if specific_key_state >= 0:
-                        pressed = False
-                        break
+                    if key == "window":
+                        lwin_key_state = win32api.GetAsyncKeyState(win32con.VK_LWIN)
+                        rwin_key_state = win32api.GetAsyncKeyState(win32con.VK_RWIN)
+                        if (lwin_key_state >= 0) and (rwin_key_state >= 0):
+                            pressed = False
+                            break
+                    else:
+                        specific_key_state = win32api.GetAsyncKeyState(key)
+                        if specific_key_state >= 0:
+                            pressed = False
+                            break
                 
+                # ensure that modifiers not in this hotkey aren't pressed
+                non_allowed_modifiers = []
+                for key in full_modifier_list:
+                    if key not in hotkey:
+                        non_allowed_modifiers.append(key)
+                
+                for key in non_allowed_modifiers:
+                    if key == "window":
+                        lwin_key_state = win32api.GetAsyncKeyState(win32con.VK_LWIN)
+                        rwin_key_state = win32api.GetAsyncKeyState(win32con.VK_RWIN)
+                        if (lwin_key_state < 0) or (rwin_key_state < 0):
+                            pressed = False
+                            break
+                    else:
+                        specific_key_state = win32api.GetAsyncKeyState(key)
+                        if specific_key_state < 0:
+                            pressed = False
+                            break                    
+
                 if pressed:
                     self.hotkey_actions[id][2] = True
                     if not key_state:
                         if press_callback != None:
                             press_callback()
                 else:
                     self.hotkey_actions[id][2] = False
```

### Comparing `global_hotkeys-0.0.4/global_hotkeys/keycodes.py` & `global_hotkeys-0.0.5/global_hotkeys/keycodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 	'up':0x26,
 	'right':0x27,
 	'down':0x28,
 	'select':0x29,
 	'print':0x2A,
 	'execute':0x2B,
 	"enter": win32con.VK_RETURN,
+    "left_window": 0x5B,
+    "right_window": 0x5C,
+    "window": "window",
 	'print_screen':0x2C,
 	'insert':0x2D,
 	'delete':0x2E,
 	'help':0x2F,
 	'0':0x30,
 	'1':0x31,
 	'2':0x32,
@@ -118,15 +121,15 @@
 	'browser_forward':0xA7,
 	'browser_refresh':0xA8,
 	'browser_stop':0xA9,
 	'browser_search':0xAA,
 	'browser_favorites':0xAB,
 	'browser_start_and_home':0xAC,
 	'volume_mute':0xAD,
-	'volume_Down':0xAE,
+	'volume_down':0xAE,
 	'volume_up':0xAF,
 	'next_track':0xB0,
 	'previous_track':0xB1,
 	'stop_media':0xB2,
 	'play/pause_media':0xB3,
 	'start_mail':0xB4,
 	'select_media':0xB5,
@@ -146,8 +149,8 @@
 	'`':0xC0,
 	';':0xBA,
 	'[':0xDB,
 	'\\':0xDC,
 	']':0xDD,
 	"'":0xDE,
 	'`':0xC0
-}
+}
```

### Comparing `global_hotkeys-0.0.4/setup.py` & `global_hotkeys-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,23 +6,23 @@
   'Operating System :: Microsoft :: Windows',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='global_hotkeys',
-  version='0.0.4',
+  version='0.0.5',
   description='',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/btsdev',
   author='btsdev',
   author_email='btsdevman@gmail.com',
   license='MIT',
   classifiers=classifiers,
   keywords='hotkeys,shortcuts',
   packages=find_packages(),
-  install_requires=[], # "some_lib ~= 1.0"
+  install_requires=["pywin32"], # "some_lib ~= 1.0"
   extras_require = {
     "dev": [] # "pytest>=3.7"
   }
 )
```

### Comparing `global_hotkeys-0.0.4/tests/test.py` & `global_hotkeys-0.0.5/tests/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 def exit_application():
     global is_alive
     stop_checking_hotkeys()
     is_alive = False
 
 # Declare some key bindings.
 bindings = [
-    [["control", "shift", "7"], None, print_hello],
-    [["control", "shift", "8"], None, print_world],
-    [["control", "shift", "9"], None, exit_application],
+    [["control", "7"], None, print_hello],
+    [["control", "8"], None, print_world],
+    [["8"], None, print_hello],
+    [["window","0"], None, print_hello],
+    [["control", "9"], None, exit_application],
 ]
 
 # Register all of our keybindings
 register_hotkeys(bindings)
 
 # Finally, start listening for keypresses
 start_checking_hotkeys()
```

