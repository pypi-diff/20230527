# Comparing `tmp/global_hotkeys-0.0.5.tar.gz` & `tmp/global_hotkeys-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_hotkeys-0.0.5.tar", last modified: Sat May 27 08:28:41 2023, max compression
+gzip compressed data, was "global_hotkeys-0.0.6.tar", last modified: Sat May 27 09:50:05 2023, max compression
```

## Comparing `global_hotkeys-0.0.5.tar` & `global_hotkeys-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 08:28:41.220670 global_hotkeys-0.0.5/
--rw-rw-rw-   0        0        0      439 2023-05-27 08:19:11.000000 global_hotkeys-0.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4914 2023-05-27 08:28:41.220670 global_hotkeys-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3941 2023-05-27 07:59:16.000000 global_hotkeys-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 08:28:41.205671 global_hotkeys-0.0.5/global_hotkeys/
--rw-rw-rw-   0        0        0     1455 2023-05-27 07:09:18.000000 global_hotkeys-0.0.5/global_hotkeys/__init__.py
--rw-rw-rw-   0        0        0     6018 2023-05-27 07:48:35.000000 global_hotkeys-0.0.5/global_hotkeys/hotkey_checker.py
--rw-rw-rw-   0        0        0     2605 2023-05-27 07:53:05.000000 global_hotkeys-0.0.5/global_hotkeys/keycodes.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:28:41.218672 global_hotkeys-0.0.5/global_hotkeys.egg-info/
--rw-rw-rw-   0        0        0     4914 2023-05-27 08:28:41.000000 global_hotkeys-0.0.5/global_hotkeys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-05-27 08:28:41.000000 global_hotkeys-0.0.5/global_hotkeys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 08:28:41.000000 global_hotkeys-0.0.5/global_hotkeys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-27 08:28:41.000000 global_hotkeys-0.0.5/global_hotkeys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-27 08:28:41.000000 global_hotkeys-0.0.5/global_hotkeys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 08:28:41.221469 global_hotkeys-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-05-27 08:28:28.000000 global_hotkeys-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:28:41.219671 global_hotkeys-0.0.5/tests/
--rw-rw-rw-   0        0        0      889 2023-05-27 07:59:21.000000 global_hotkeys-0.0.5/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:50:05.685204 global_hotkeys-0.0.6/
+-rw-rw-rw-   0        0        0      510 2023-05-27 09:40:22.000000 global_hotkeys-0.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4648 2023-05-27 09:50:05.685204 global_hotkeys-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3604 2023-05-27 09:48:24.000000 global_hotkeys-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 09:50:05.664204 global_hotkeys-0.0.6/global_hotkeys/
+-rw-rw-rw-   0        0        0     1455 2023-05-27 07:09:18.000000 global_hotkeys-0.0.6/global_hotkeys/__init__.py
+-rw-rw-rw-   0        0        0     6445 2023-05-27 09:45:49.000000 global_hotkeys-0.0.6/global_hotkeys/hotkey_checker.py
+-rw-rw-rw-   0        0        0     2605 2023-05-27 07:53:05.000000 global_hotkeys-0.0.6/global_hotkeys/keycodes.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:50:05.680204 global_hotkeys-0.0.6/global_hotkeys.egg-info/
+-rw-rw-rw-   0        0        0     4648 2023-05-27 09:50:05.000000 global_hotkeys-0.0.6/global_hotkeys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-27 09:50:05.000000 global_hotkeys-0.0.6/global_hotkeys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 09:50:05.000000 global_hotkeys-0.0.6/global_hotkeys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-27 09:50:05.000000 global_hotkeys-0.0.6/global_hotkeys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-27 09:50:05.000000 global_hotkeys-0.0.6/global_hotkeys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 09:50:05.685204 global_hotkeys-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-05-27 09:47:39.000000 global_hotkeys-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:50:05.684216 global_hotkeys-0.0.6/tests/
+-rw-rw-rw-   0        0        0      808 2023-05-27 09:47:24.000000 global_hotkeys-0.0.6/tests/test.py
```

### Comparing `global_hotkeys-0.0.5/LICENSE.txt` & `global_hotkeys-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.0.5/PKG-INFO` & `global_hotkeys-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global_hotkeys
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -108,17 +108,17 @@
 alt
 pause
 caps_lock
 escape
 space   <-- a literal space character (' ') can be used as well.
 page_up
 page_down
-left_window  <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
-right_window <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
-window       <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
+left_window
+right_window
+window
 end
 home
 left
 up
 right
 down
 select
@@ -251,14 +251,18 @@
 '
 `
 ```
 
 Change Log
 ==========
 
+0.0.6 (12/1/2020)
+-----------------
+- Fixed window key detection.
+
 0.0.5 (12/1/2020)
 -----------------
 - Fixed unwanted modifier keys bug. Added pywin32 as dependency.
 
 0.0.4 (12/1/2020)
 -----------------
 - Fixed Development Status: It's now set to Beta.
```

### Comparing `global_hotkeys-0.0.5/README.md` & `global_hotkeys-0.0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -91,17 +91,17 @@
 alt
 pause
 caps_lock
 escape
 space   <-- a literal space character (' ') can be used as well.
 page_up
 page_down
-left_window  <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
-right_window <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
-window       <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
+left_window
+right_window
+window
 end
 home
 left
 up
 right
 down
 select
```

### Comparing `global_hotkeys-0.0.5/global_hotkeys/__init__.py` & `global_hotkeys-0.0.6/global_hotkeys/__init__.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.0.5/global_hotkeys/hotkey_checker.py` & `global_hotkeys-0.0.6/global_hotkeys/hotkey_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         id_list = self.hotkeys.keys()
 
         while state.active:
             time.sleep(0.02)
             # Exit out if the main thread has terminated.
             if not main_thread().is_alive():
                 break
-            
+
             for id in id_list:
                 hotkey = self.hotkeys[id]
                 press_callback, release_callback, key_state = self.hotkey_actions[id]
 
                 # check to see if all keys in the hotkey are pressed.
                 pressed = True
                 for key in hotkey:
@@ -141,14 +141,20 @@
                             pressed = False
                             break
                 
                 # ensure that modifiers not in this hotkey aren't pressed
                 non_allowed_modifiers = []
                 for key in full_modifier_list:
                     if key not in hotkey:
+                        if((key == "window") and ((_to_virtualkey("left_window") in hotkey) or _to_virtualkey("right_window") in hotkey)):
+                            continue
+                        if(key == _to_virtualkey("left_window")) and ("window" in hotkey):
+                            continue
+                        if(key == _to_virtualkey("right_window")) and ("window" in hotkey):
+                            continue
                         non_allowed_modifiers.append(key)
                 
                 for key in non_allowed_modifiers:
                     if key == "window":
                         lwin_key_state = win32api.GetAsyncKeyState(win32con.VK_LWIN)
                         rwin_key_state = win32api.GetAsyncKeyState(win32con.VK_RWIN)
                         if (lwin_key_state < 0) or (rwin_key_state < 0):
```

### Comparing `global_hotkeys-0.0.5/global_hotkeys/keycodes.py` & `global_hotkeys-0.0.6/global_hotkeys/keycodes.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.0.5/global_hotkeys.egg-info/PKG-INFO` & `global_hotkeys-0.0.6/global_hotkeys.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global-hotkeys
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -108,17 +108,17 @@
 alt
 pause
 caps_lock
 escape
 space   <-- a literal space character (' ') can be used as well.
 page_up
 page_down
-left_window  <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
-right_window <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
-window       <-- I couldn't get these to work on my keyboard (the microsoft docs say it's for microsoft natural keyboard?)
+left_window
+right_window
+window
 end
 home
 left
 up
 right
 down
 select
@@ -251,14 +251,18 @@
 '
 `
 ```
 
 Change Log
 ==========
 
+0.0.6 (12/1/2020)
+-----------------
+- Fixed window key detection.
+
 0.0.5 (12/1/2020)
 -----------------
 - Fixed unwanted modifier keys bug. Added pywin32 as dependency.
 
 0.0.4 (12/1/2020)
 -----------------
 - Fixed Development Status: It's now set to Beta.
```

### Comparing `global_hotkeys-0.0.5/tests/test.py` & `global_hotkeys-0.0.6/tests/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,17 +15,15 @@
     global is_alive
     stop_checking_hotkeys()
     is_alive = False
 
 # Declare some key bindings.
 bindings = [
     [["control", "7"], None, print_hello],
-    [["control", "8"], None, print_world],
-    [["8"], None, print_hello],
-    [["window","0"], None, print_hello],
+    [["window"], None, print_hello],
     [["control", "9"], None, exit_application],
 ]
 
 # Register all of our keybindings
 register_hotkeys(bindings)
 
 # Finally, start listening for keypresses
```

