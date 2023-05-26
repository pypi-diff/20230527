# Comparing `tmp/pyemenu-0.0.3.dev2.tar.gz` & `tmp/pyemenu-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyemenu-0.0.3.dev2.tar", last modified: Fri May 26 22:20:00 2023, max compression
+gzip compressed data, was "pyemenu-0.1.0.tar", last modified: Fri May 26 22:37:13 2023, max compression
```

## Comparing `pyemenu-0.0.3.dev2.tar` & `pyemenu-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:20:00.706812 pyemenu-0.0.3.dev2/
--rw-r--r--   0 zero      (1000) zero      (1000)     1083 2023-05-26 17:53:37.000000 pyemenu-0.0.3.dev2/LICENSE.txt
--rw-r--r--   0 zero      (1000) zero      (1000)     4256 2023-05-26 22:20:00.703478 pyemenu-0.0.3.dev2/PKG-INFO
--rw-r--r--   0 zero      (1000) zero      (1000)     3286 2023-05-26 22:12:25.000000 pyemenu-0.0.3.dev2/README.md
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:20:00.703478 pyemenu-0.0.3.dev2/pyemenu/
--rw-r--r--   0 zero      (1000) zero      (1000)       22 2023-05-26 22:18:14.000000 pyemenu-0.0.3.dev2/pyemenu/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)     3308 2023-05-26 21:04:58.000000 pyemenu-0.0.3.dev2/pyemenu/menu.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:20:00.703478 pyemenu-0.0.3.dev2/pyemenu.egg-info/
--rw-r--r--   0 zero      (1000) zero      (1000)     4256 2023-05-26 22:20:00.000000 pyemenu-0.0.3.dev2/pyemenu.egg-info/PKG-INFO
--rw-r--r--   0 zero      (1000) zero      (1000)      234 2023-05-26 22:20:00.000000 pyemenu-0.0.3.dev2/pyemenu.egg-info/SOURCES.txt
--rw-r--r--   0 zero      (1000) zero      (1000)        1 2023-05-26 22:20:00.000000 pyemenu-0.0.3.dev2/pyemenu.egg-info/dependency_links.txt
--rw-r--r--   0 zero      (1000) zero      (1000)        9 2023-05-26 22:20:00.000000 pyemenu-0.0.3.dev2/pyemenu.egg-info/requires.txt
--rw-r--r--   0 zero      (1000) zero      (1000)        8 2023-05-26 22:20:00.000000 pyemenu-0.0.3.dev2/pyemenu.egg-info/top_level.txt
--rw-r--r--   0 zero      (1000) zero      (1000)       38 2023-05-26 22:20:00.706812 pyemenu-0.0.3.dev2/setup.cfg
--rw-r--r--   0 zero      (1000) zero      (1000)     2117 2023-05-26 22:17:48.000000 pyemenu-0.0.3.dev2/setup.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:20:00.703478 pyemenu-0.0.3.dev2/tests/
--rw-r--r--   0 zero      (1000) zero      (1000)        2 2023-05-26 19:16:06.000000 pyemenu-0.0.3.dev2/tests/test.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:37:13.426324 pyemenu-0.1.0/
+-rw-r--r--   0 zero      (1000) zero      (1000)     1083 2023-05-26 17:53:37.000000 pyemenu-0.1.0/LICENSE.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)     4659 2023-05-26 22:37:13.426324 pyemenu-0.1.0/PKG-INFO
+-rw-r--r--   0 zero      (1000) zero      (1000)     3694 2023-05-26 22:34:11.000000 pyemenu-0.1.0/README.md
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:37:13.426324 pyemenu-0.1.0/pyemenu/
+-rw-r--r--   0 zero      (1000) zero      (1000)       22 2023-05-26 22:18:14.000000 pyemenu-0.1.0/pyemenu/__init__.py
+-rw-r--r--   0 zero      (1000) zero      (1000)     3308 2023-05-26 21:04:58.000000 pyemenu-0.1.0/pyemenu/menu.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:37:13.426324 pyemenu-0.1.0/pyemenu.egg-info/
+-rw-r--r--   0 zero      (1000) zero      (1000)     4659 2023-05-26 22:37:13.000000 pyemenu-0.1.0/pyemenu.egg-info/PKG-INFO
+-rw-r--r--   0 zero      (1000) zero      (1000)      234 2023-05-26 22:37:13.000000 pyemenu-0.1.0/pyemenu.egg-info/SOURCES.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)        1 2023-05-26 22:37:13.000000 pyemenu-0.1.0/pyemenu.egg-info/dependency_links.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)        9 2023-05-26 22:37:13.000000 pyemenu-0.1.0/pyemenu.egg-info/requires.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)        8 2023-05-26 22:37:13.000000 pyemenu-0.1.0/pyemenu.egg-info/top_level.txt
+-rw-r--r--   0 zero      (1000) zero      (1000)       38 2023-05-26 22:37:13.426324 pyemenu-0.1.0/setup.cfg
+-rw-r--r--   0 zero      (1000) zero      (1000)     2112 2023-05-26 22:36:35.000000 pyemenu-0.1.0/setup.py
+drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:37:13.426324 pyemenu-0.1.0/tests/
+-rw-r--r--   0 zero      (1000) zero      (1000)        2 2023-05-26 19:16:06.000000 pyemenu-0.1.0/tests/test.py
```

### Comparing `pyemenu-0.0.3.dev2/LICENSE.txt` & `pyemenu-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyemenu-0.0.3.dev2/PKG-INFO` & `pyemenu-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyemenu
-Version: 0.0.3.dev2
+Version: 0.1.0
 Summary: Easy customizable menu for CLI
 Home-page: https://github.com/FreireAlexander/PyeMenu
-Download-URL: https://github.com/FreireAlexander/PyeMenu/releases/tag/0.0.1
+Download-URL: https://github.com/FreireAlexander/PyeMenu/releases/tag/0.1.0
 Author: Freire Alexander Palomino Palma
 Author-email: freirealexander0214@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/FreireAlexander/PyeMenu/issues
 Keywords: MENU,CLI,command line
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,16 +19,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![GitHub Repository](https://img.shields.io/badge/-GitHub-%230D0D0D?logo=github&labelColor=gray)](https://github.com/FreireAlexander/PyeMenu)
+[![Latest PyPi version](https://img.shields.io/pypi/v/pyemenu.svg)](https://pypi.python.org/pypi/pyemenu)<br>
+[![supported Python versions](https://img.shields.io/pypi/pyversions/pyemenu)](https://pypi.python.org/pypi/pyemenu)
+[![Project licence](https://img.shields.io/pypi/l/pyemenu?color=blue)](LICENCE) <br>
+[![Number of PyPi downloads](https://img.shields.io/pypi/dd/pyemenu.svg)](https://pypi.python.org/pypi/pyemenu)
 
-# Python - PyeMenu Version 0.0.1
+
+
+# Python - PyeMenu Version 0.1.0
 
 PyeMenu is a simple and interactive CLI menu for Python apps __'by now'__ It is intend in future to add more features including other types of menus as checkbox an similars. Right now, it is possible to customize the title and the cursor __'icon'__ 
 
 ## Installation
 
 Simply installing it via `pip`:
 
@@ -123,16 +129,14 @@
 <div style="text-align:center">
     <img src="images/Example3.png" alt="Example number 1">
 </div>
 
 <p></p>
 
 
-## Documentation
-
 ## OS Support
 Right now it only been tested on Windows Os and Linux Os
 ______________________________________________________________________
 
 
 ## LICENSE
```

### Comparing `pyemenu-0.0.3.dev2/README.md` & `pyemenu-0.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 [![GitHub Repository](https://img.shields.io/badge/-GitHub-%230D0D0D?logo=github&labelColor=gray)](https://github.com/FreireAlexander/PyeMenu)
+[![Latest PyPi version](https://img.shields.io/pypi/v/pyemenu.svg)](https://pypi.python.org/pypi/pyemenu)<br>
+[![supported Python versions](https://img.shields.io/pypi/pyversions/pyemenu)](https://pypi.python.org/pypi/pyemenu)
+[![Project licence](https://img.shields.io/pypi/l/pyemenu?color=blue)](LICENCE) <br>
+[![Number of PyPi downloads](https://img.shields.io/pypi/dd/pyemenu.svg)](https://pypi.python.org/pypi/pyemenu)
 
-# Python - PyeMenu Version 0.0.1
+
+
+# Python - PyeMenu Version 0.1.0
 
 PyeMenu is a simple and interactive CLI menu for Python apps __'by now'__ It is intend in future to add more features including other types of menus as checkbox an similars. Right now, it is possible to customize the title and the cursor __'icon'__ 
 
 ## Installation
 
 Simply installing it via `pip`:
 
@@ -99,16 +105,14 @@
 <div style="text-align:center">
     <img src="images/Example3.png" alt="Example number 1">
 </div>
 
 <p></p>
 
 
-## Documentation
-
 ## OS Support
 Right now it only been tested on Windows Os and Linux Os
 ______________________________________________________________________
 
 
 ## LICENSE
```

### Comparing `pyemenu-0.0.3.dev2/pyemenu/menu.py` & `pyemenu-0.1.0/pyemenu/menu.py`

 * *Files identical despite different names*

### Comparing `pyemenu-0.0.3.dev2/pyemenu.egg-info/PKG-INFO` & `pyemenu-0.1.0/pyemenu.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyemenu
-Version: 0.0.3.dev2
+Version: 0.1.0
 Summary: Easy customizable menu for CLI
 Home-page: https://github.com/FreireAlexander/PyeMenu
-Download-URL: https://github.com/FreireAlexander/PyeMenu/releases/tag/0.0.1
+Download-URL: https://github.com/FreireAlexander/PyeMenu/releases/tag/0.1.0
 Author: Freire Alexander Palomino Palma
 Author-email: freirealexander0214@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/FreireAlexander/PyeMenu/issues
 Keywords: MENU,CLI,command line
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,16 +19,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![GitHub Repository](https://img.shields.io/badge/-GitHub-%230D0D0D?logo=github&labelColor=gray)](https://github.com/FreireAlexander/PyeMenu)
+[![Latest PyPi version](https://img.shields.io/pypi/v/pyemenu.svg)](https://pypi.python.org/pypi/pyemenu)<br>
+[![supported Python versions](https://img.shields.io/pypi/pyversions/pyemenu)](https://pypi.python.org/pypi/pyemenu)
+[![Project licence](https://img.shields.io/pypi/l/pyemenu?color=blue)](LICENCE) <br>
+[![Number of PyPi downloads](https://img.shields.io/pypi/dd/pyemenu.svg)](https://pypi.python.org/pypi/pyemenu)
 
-# Python - PyeMenu Version 0.0.1
+
+
+# Python - PyeMenu Version 0.1.0
 
 PyeMenu is a simple and interactive CLI menu for Python apps __'by now'__ It is intend in future to add more features including other types of menus as checkbox an similars. Right now, it is possible to customize the title and the cursor __'icon'__ 
 
 ## Installation
 
 Simply installing it via `pip`:
 
@@ -123,16 +129,14 @@
 <div style="text-align:center">
     <img src="images/Example3.png" alt="Example number 1">
 </div>
 
 <p></p>
 
 
-## Documentation
-
 ## OS Support
 Right now it only been tested on Windows Os and Linux Os
 ______________________________________________________________________
 
 
 ## LICENSE
```

### Comparing `pyemenu-0.0.3.dev2/setup.py` & `pyemenu-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 with open("README.md", "r", encoding= "utf-8") as fh:
   long_description = fh.read()
 
 setuptools.setup(
     name = 'pyemenu',         # How you named your package folder (MyLib)
     packages = ['pyemenu'],
-    version = '0.0.3-dev2',      # Start with a small number and increase it with every change you make
+    version = '0.1.0',      # Start with a small number and increase it with every change you make
     author = 'Freire Alexander Palomino Palma',                   # Type in your name
     author_email = 'freirealexander0214@gmail.com',      # Type in your E-Mail
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Easy customizable menu for CLI',   # Give a short description about your library
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/FreireAlexander/PyeMenu',   # Provide either the link to your github or to your website
-    download_url = 'https://github.com/FreireAlexander/PyeMenu/releases/tag/0.0.1',
+    download_url = 'https://github.com/FreireAlexander/PyeMenu/releases/tag/0.1.0',
     project_urls = {
         "Bug Tracker": "https://github.com/FreireAlexander/PyeMenu/issues",
     },
     #download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
     keywords = ['MENU', 'CLI', 'command line'],   # Keywords that define your package best
     install_requires=[            # I get to this in a second
             'readchar',
```

