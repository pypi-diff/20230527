# Comparing `tmp/pyemenu-0.0.2.dev0.tar.gz` & `tmp/pyemenu-0.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyemenu-0.0.2.dev0.tar", last modified: Fri May 26 21:52:28 2023, max compression
+gzip compressed data, was "pyemenu-0.0.3.dev0.tar", last modified: Fri May 26 22:00:28 2023, max compression
```

## Comparing `pyemenu-0.0.2.dev0.tar` & `pyemenu-0.0.3.dev0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 21:52:28.880108 pyemenu-0.0.2.dev0/
--rw-r--r--   0 zero      (1000) zero      (1000)     1083 2023-05-26 17:53:37.000000 pyemenu-0.0.2.dev0/LICENSE.txt
--rw-r--r--   0 zero      (1000) zero      (1000)     4253 2023-05-26 21:52:28.876775 pyemenu-0.0.2.dev0/PKG-INFO
--rw-r--r--   0 zero      (1000) zero      (1000)     3283 2023-05-26 21:26:51.000000 pyemenu-0.0.2.dev0/README.md
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 21:52:28.876775 pyemenu-0.0.2.dev0/pyemenu/
--rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-05-26 21:52:08.000000 pyemenu-0.0.2.dev0/pyemenu/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)     3308 2023-05-26 21:04:58.000000 pyemenu-0.0.2.dev0/pyemenu/pyemenu.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 21:52:28.876775 pyemenu-0.0.2.dev0/pyemenu.egg-info/
--rw-r--r--   0 zero      (1000) zero      (1000)     4253 2023-05-26 21:52:28.000000 pyemenu-0.0.2.dev0/pyemenu.egg-info/PKG-INFO
--rw-r--r--   0 zero      (1000) zero      (1000)      237 2023-05-26 21:52:28.000000 pyemenu-0.0.2.dev0/pyemenu.egg-info/SOURCES.txt
--rw-r--r--   0 zero      (1000) zero      (1000)        1 2023-05-26 21:52:28.000000 pyemenu-0.0.2.dev0/pyemenu.egg-info/dependency_links.txt
--rw-r--r--   0 zero      (1000) zero      (1000)        9 2023-05-26 21:52:28.000000 pyemenu-0.0.2.dev0/pyemenu.egg-info/requires.txt
--rw-r--r--   0 zero      (1000) zero      (1000)        8 2023-05-26 21:52:28.000000 pyemenu-0.0.2.dev0/pyemenu.egg-info/top_level.txt
--rw-r--r--   0 zero      (1000) zero      (1000)       38 2023-05-26 21:52:28.880108 pyemenu-0.0.2.dev0/setup.cfg
--rw-r--r--   0 zero      (1000) zero      (1000)     2116 2023-05-26 21:52:22.000000 pyemenu-0.0.2.dev0/setup.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 21:52:28.876775 pyemenu-0.0.2.dev0/tests/
--rw-r--r--   0 zero      (1000) zero      (1000)        2 2023-05-26 19:16:06.000000 pyemenu-0.0.2.dev0/tests/test.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:00:28.533217 pyemenu-0.0.3.dev0/
+-rw-r--r--   0 zero      (1000) zero      (1000)     1083 2023-05-26 17:53:37.000000 pyemenu-0.0.3.dev0/LICENSE.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)     4253 2023-05-26 22:00:28.529884 pyemenu-0.0.3.dev0/PKG-INFO
+-rw-r--r--   0 zero      (1000) zero      (1000)     3283 2023-05-26 21:26:51.000000 pyemenu-0.0.3.dev0/README.md
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:00:28.529884 pyemenu-0.0.3.dev0/pyemenu/
+-rw-r--r--   0 zero      (1000) zero      (1000)       22 2023-05-26 22:00:08.000000 pyemenu-0.0.3.dev0/pyemenu/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     3308 2023-05-26 21:04:58.000000 pyemenu-0.0.3.dev0/pyemenu/pyemenu.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:00:28.529884 pyemenu-0.0.3.dev0/pyemenu.egg-info/
+-rw-r--r--   0 zero      (1000) zero      (1000)     4253 2023-05-26 22:00:28.000000 pyemenu-0.0.3.dev0/pyemenu.egg-info/PKG-INFO
+-rw-r--r--   0 zero      (1000) zero      (1000)      237 2023-05-26 22:00:28.000000 pyemenu-0.0.3.dev0/pyemenu.egg-info/SOURCES.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)        1 2023-05-26 22:00:28.000000 pyemenu-0.0.3.dev0/pyemenu.egg-info/dependency_links.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)        9 2023-05-26 22:00:28.000000 pyemenu-0.0.3.dev0/pyemenu.egg-info/requires.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)        8 2023-05-26 22:00:28.000000 pyemenu-0.0.3.dev0/pyemenu.egg-info/top_level.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)       38 2023-05-26 22:00:28.533217 pyemenu-0.0.3.dev0/setup.cfg
+-rw-r--r--   0 zero      (1000) zero      (1000)     2116 2023-05-26 22:00:24.000000 pyemenu-0.0.3.dev0/setup.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:00:28.529884 pyemenu-0.0.3.dev0/tests/
+-rw-r--r--   0 zero      (1000) zero      (1000)        2 2023-05-26 19:16:06.000000 pyemenu-0.0.3.dev0/tests/test.py
```

### Comparing `pyemenu-0.0.2.dev0/LICENSE.txt` & `pyemenu-0.0.3.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyemenu-0.0.2.dev0/PKG-INFO` & `pyemenu-0.0.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemenu
-Version: 0.0.2.dev0
+Version: 0.0.3.dev0
 Summary: Easy customizable menu for CLI
 Home-page: https://github.com/FreireAlexander/PyeMenu
 Download-URL: https://github.com/FreireAlexander/PyeMenu/releases/tag/0.0.1
 Author: Freire Alexander Palomino Palma
 Author-email: freirealexander0214@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/FreireAlexander/PyeMenu/issues
```

### Comparing `pyemenu-0.0.2.dev0/README.md` & `pyemenu-0.0.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `pyemenu-0.0.2.dev0/pyemenu/pyemenu.py` & `pyemenu-0.0.3.dev0/pyemenu/pyemenu.py`

 * *Files identical despite different names*

### Comparing `pyemenu-0.0.2.dev0/pyemenu.egg-info/PKG-INFO` & `pyemenu-0.0.3.dev0/pyemenu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemenu
-Version: 0.0.2.dev0
+Version: 0.0.3.dev0
 Summary: Easy customizable menu for CLI
 Home-page: https://github.com/FreireAlexander/PyeMenu
 Download-URL: https://github.com/FreireAlexander/PyeMenu/releases/tag/0.0.1
 Author: Freire Alexander Palomino Palma
 Author-email: freirealexander0214@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/FreireAlexander/PyeMenu/issues
```

### Comparing `pyemenu-0.0.2.dev0/setup.py` & `pyemenu-0.0.3.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 with open("README.md", "r", encoding= "utf-8") as fh:
   long_description = fh.read()
 
 setuptools.setup(
     name = 'pyemenu',         # How you named your package folder (MyLib)
     packages = ['pyemenu'],
-    version = '0.0.2-dev',      # Start with a small number and increase it with every change you make
+    version = '0.0.3-dev',      # Start with a small number and increase it with every change you make
     author = 'Freire Alexander Palomino Palma',                   # Type in your name
     author_email = 'freirealexander0214@gmail.com',      # Type in your E-Mail
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Easy customizable menu for CLI',   # Give a short description about your library
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/FreireAlexander/PyeMenu',   # Provide either the link to your github or to your website
```

