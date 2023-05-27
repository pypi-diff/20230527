# Comparing `tmp/fritzbox-tray-1.0.59.tar.gz` & `tmp/fritzbox-tray-1.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fritzbox-tray-1.0.59.tar", last modified: Mon Mar 27 13:32:30 2023, max compression
+gzip compressed data, was "fritzbox-tray-1.0.60.tar", last modified: Sat May 27 16:18:00 2023, max compression
```

## Comparing `fritzbox-tray-1.0.59.tar` & `fritzbox-tray-1.0.60.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 13:32:30.121174 fritzbox-tray-1.0.59/
--rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 fritzbox-tray-1.0.59/LICENSE
--rw-rw-rw-   0        0        0     3909 2023-03-27 13:32:30.118174 fritzbox-tray-1.0.59/PKG-INFO
--rw-rw-rw-   0        0        0     2846 2023-03-27 13:29:29.000000 fritzbox-tray-1.0.59/README.md
--rw-rw-rw-   0        0        0       42 2023-03-27 13:32:30.121174 fritzbox-tray-1.0.59/setup.cfg
--rw-rw-rw-   0        0        0     2637 2023-03-27 13:32:22.000000 fritzbox-tray-1.0.59/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-27 13:32:30.077171 fritzbox-tray-1.0.59/src/
-drwxrwxrwx   0        0        0        0 2023-03-27 13:32:30.091172 fritzbox-tray-1.0.59/src/fritzbox_tray/
--rw-rw-rw-   0        0        0        0 2023-01-07 15:15:29.000000 fritzbox-tray-1.0.59/src/fritzbox_tray/__init__.py
--rw-rw-rw-   0        0        0     5007 2023-01-09 16:05:59.000000 fritzbox-tray-1.0.59/src/fritzbox_tray/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 13:32:30.115171 fritzbox-tray-1.0.59/src/fritzbox_tray/resources/
--rw-rw-rw-   0        0        0   121004 2023-01-08 16:34:44.000000 fritzbox-tray-1.0.59/src/fritzbox_tray/resources/ft.ico
-drwxrwxrwx   0        0        0        0 2023-03-27 13:32:30.113171 fritzbox-tray-1.0.59/src/fritzbox_tray.egg-info/
--rw-rw-rw-   0        0        0     3909 2023-03-27 13:32:30.000000 fritzbox-tray-1.0.59/src/fritzbox_tray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-03-27 13:32:30.000000 fritzbox-tray-1.0.59/src/fritzbox_tray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 13:32:30.000000 fritzbox-tray-1.0.59/src/fritzbox_tray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-03-27 13:32:30.000000 fritzbox-tray-1.0.59/src/fritzbox_tray.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-03-27 13:32:30.000000 fritzbox-tray-1.0.59/src/fritzbox_tray.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-27 13:32:30.000000 fritzbox-tray-1.0.59/src/fritzbox_tray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 16:18:00.243425 fritzbox-tray-1.0.60/
+-rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 fritzbox-tray-1.0.60/LICENSE
+-rw-rw-rw-   0        0        0     3892 2023-05-27 16:18:00.236425 fritzbox-tray-1.0.60/PKG-INFO
+-rw-rw-rw-   0        0        0     2829 2023-05-27 15:06:54.000000 fritzbox-tray-1.0.60/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 16:18:00.243425 fritzbox-tray-1.0.60/setup.cfg
+-rw-rw-rw-   0        0        0     2637 2023-05-27 16:16:48.000000 fritzbox-tray-1.0.60/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 16:18:00.191753 fritzbox-tray-1.0.60/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 16:18:00.207281 fritzbox-tray-1.0.60/src/fritzbox_tray/
+-rw-rw-rw-   0        0        0        0 2023-01-07 15:15:29.000000 fritzbox-tray-1.0.60/src/fritzbox_tray/__init__.py
+-rw-rw-rw-   0        0        0     5007 2023-04-30 12:36:27.000000 fritzbox-tray-1.0.60/src/fritzbox_tray/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 16:18:00.232426 fritzbox-tray-1.0.60/src/fritzbox_tray/resources/
+-rw-rw-rw-   0        0        0   121004 2023-01-08 16:34:44.000000 fritzbox-tray-1.0.60/src/fritzbox_tray/resources/ft.ico
+drwxrwxrwx   0        0        0        0 2023-05-27 16:18:00.230428 fritzbox-tray-1.0.60/src/fritzbox_tray.egg-info/
+-rw-rw-rw-   0        0        0     3892 2023-05-27 16:18:00.000000 fritzbox-tray-1.0.60/src/fritzbox_tray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-27 16:18:00.000000 fritzbox-tray-1.0.60/src/fritzbox_tray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 16:18:00.000000 fritzbox-tray-1.0.60/src/fritzbox_tray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-27 16:18:00.000000 fritzbox-tray-1.0.60/src/fritzbox_tray.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-05-27 16:18:00.000000 fritzbox-tray-1.0.60/src/fritzbox_tray.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-27 16:18:00.000000 fritzbox-tray-1.0.60/src/fritzbox_tray.egg-info/top_level.txt
```

### Comparing `fritzbox-tray-1.0.59/LICENSE` & `fritzbox-tray-1.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `fritzbox-tray-1.0.59/PKG-INFO` & `fritzbox-tray-1.0.60/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fritzbox-tray
-Version: 1.0.59
+Version: 1.0.60
 Summary: A system tray application for interacting with FRITZ!Box devices.
 Home-page: https://github.com/aviolaris/fritzbox-tray
 Author: Andreas Violaris
 Keywords: fritz,fritzbox,fritz-box,fritzbox-tray,fritzbox_tray,avm-fritz,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
@@ -23,21 +23,21 @@
 # FritzBox Tray
 
 ### A system tray application for interacting with FRITZ!Box devices.
 
 [![fritzbox-tray](https://user-images.githubusercontent.com/48277853/211208943-1cbb41fb-60a7-44d1-a697-5d0493bb167c.png)](https://github.com/aviolaris/fritzbox-tray)
 
 ![python-versions](https://img.shields.io/pypi/pyversions/fritzbox-tray)
-![code-size](https://img.shields.io/github/languages/code-size/aviolaris/fritzbox-tray)
-![repo-size](https://img.shields.io/github/repo-size/aviolaris/fritzbox-tray)
+[![pypi-downloads](https://img.shields.io/pypi/dm/fritzbox-tray.svg?color=blue&label=downloads&logo=pypi&logoColor=gold)](https://pypistats.org/packages/fritzbox-tray)
 
-![status](https://img.shields.io/pypi/status/fritzbox-tray)
 [![license](https://img.shields.io/pypi/l/fritzbox-tray?color=blueviolet)](https://github.com/aviolaris/fritzbox-tray/blob/master/LICENSE)
 ![format](https://img.shields.io/pypi/format/fritzbox-tray?color=blueviolet)
-[![pypi-downloads](https://img.shields.io/pypi/dm/fritzbox-tray?color=brightgreen&label=pypi%20downloads)](https://pypistats.org/packages/fritzbox-tray)
+![status](https://img.shields.io/pypi/status/fritzbox-tray?color=blue)
+![GitHub Repo stars](https://img.shields.io/github/stars/aviolaris/fritzbox-tray?color=blue&logo=github&logoColor=white)
+
 
 ## Features
 
 - Display current external IP address
 - Renew IP address
 
 ## Requirements
@@ -50,15 +50,15 @@
 
     pip install fritzbox-tray
 
 ## Usage
 
 To launch FritzBox Tray:
 
- - **On Windows**, double-click the `fritzbox-tray.exe` (usually located in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts` or run the `fritzbox-tray` command from the command prompt.
+ - **On Windows**, double-click the `fritzbox-tray.exe` (usually located in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts`) or run the `fritzbox-tray` command from the command prompt.
 
 
  - **On Linux**, double-click the `fritzbox-tray` (usually located in `~/.local/bin`) or run the `./fritzbox-tray` command from the terminal.
 
 Once the program is running, an icon will be added to the system tray. By right-clicking on the icon, a menu will appear containing the following options:
 
  - **Display Current IP Address**: This option will trigger a notification displaying the current external IP address of the FRITZ!Box device.
```

### Comparing `fritzbox-tray-1.0.59/README.md` & `fritzbox-tray-1.0.60/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # FritzBox Tray
 
 ### A system tray application for interacting with FRITZ!Box devices.
 
 [![fritzbox-tray](https://user-images.githubusercontent.com/48277853/211208943-1cbb41fb-60a7-44d1-a697-5d0493bb167c.png)](https://github.com/aviolaris/fritzbox-tray)
 
 ![python-versions](https://img.shields.io/pypi/pyversions/fritzbox-tray)
-![code-size](https://img.shields.io/github/languages/code-size/aviolaris/fritzbox-tray)
-![repo-size](https://img.shields.io/github/repo-size/aviolaris/fritzbox-tray)
+[![pypi-downloads](https://img.shields.io/pypi/dm/fritzbox-tray.svg?color=blue&label=downloads&logo=pypi&logoColor=gold)](https://pypistats.org/packages/fritzbox-tray)
 
-![status](https://img.shields.io/pypi/status/fritzbox-tray)
 [![license](https://img.shields.io/pypi/l/fritzbox-tray?color=blueviolet)](https://github.com/aviolaris/fritzbox-tray/blob/master/LICENSE)
 ![format](https://img.shields.io/pypi/format/fritzbox-tray?color=blueviolet)
-[![pypi-downloads](https://img.shields.io/pypi/dm/fritzbox-tray?color=brightgreen&label=pypi%20downloads)](https://pypistats.org/packages/fritzbox-tray)
+![status](https://img.shields.io/pypi/status/fritzbox-tray?color=blue)
+![GitHub Repo stars](https://img.shields.io/github/stars/aviolaris/fritzbox-tray?color=blue&logo=github&logoColor=white)
+
 
 ## Features
 
 - Display current external IP address
 - Renew IP address
 
 ## Requirements
@@ -28,15 +28,15 @@
 
     pip install fritzbox-tray
 
 ## Usage
 
 To launch FritzBox Tray:
 
- - **On Windows**, double-click the `fritzbox-tray.exe` (usually located in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts` or run the `fritzbox-tray` command from the command prompt.
+ - **On Windows**, double-click the `fritzbox-tray.exe` (usually located in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts`) or run the `fritzbox-tray` command from the command prompt.
 
 
  - **On Linux**, double-click the `fritzbox-tray` (usually located in `~/.local/bin`) or run the `./fritzbox-tray` command from the terminal.
 
 Once the program is running, an icon will be added to the system tray. By right-clicking on the icon, a menu will appear containing the following options:
 
  - **Display Current IP Address**: This option will trigger a notification displaying the current external IP address of the FRITZ!Box device.
```

### Comparing `fritzbox-tray-1.0.59/setup.py` & `fritzbox-tray-1.0.60/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open('requirements.txt', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='fritzbox-tray',
-    version='1.0.59',
+    version='1.0.60',
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "fritzbox_tray": ["*.py"],
         "fritzbox_tray.resources": ["*.ico"],
     },
     description='A system tray application for interacting with FRITZ!Box devices.',
```

### Comparing `fritzbox-tray-1.0.59/src/fritzbox_tray/__main__.py` & `fritzbox-tray-1.0.60/src/fritzbox_tray/__main__.py`

 * *Files identical despite different names*

### Comparing `fritzbox-tray-1.0.59/src/fritzbox_tray/resources/ft.ico` & `fritzbox-tray-1.0.60/src/fritzbox_tray/resources/ft.ico`

 * *Files identical despite different names*

### Comparing `fritzbox-tray-1.0.59/src/fritzbox_tray.egg-info/PKG-INFO` & `fritzbox-tray-1.0.60/src/fritzbox_tray.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fritzbox-tray
-Version: 1.0.59
+Version: 1.0.60
 Summary: A system tray application for interacting with FRITZ!Box devices.
 Home-page: https://github.com/aviolaris/fritzbox-tray
 Author: Andreas Violaris
 Keywords: fritz,fritzbox,fritz-box,fritzbox-tray,fritzbox_tray,avm-fritz,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
@@ -23,21 +23,21 @@
 # FritzBox Tray
 
 ### A system tray application for interacting with FRITZ!Box devices.
 
 [![fritzbox-tray](https://user-images.githubusercontent.com/48277853/211208943-1cbb41fb-60a7-44d1-a697-5d0493bb167c.png)](https://github.com/aviolaris/fritzbox-tray)
 
 ![python-versions](https://img.shields.io/pypi/pyversions/fritzbox-tray)
-![code-size](https://img.shields.io/github/languages/code-size/aviolaris/fritzbox-tray)
-![repo-size](https://img.shields.io/github/repo-size/aviolaris/fritzbox-tray)
+[![pypi-downloads](https://img.shields.io/pypi/dm/fritzbox-tray.svg?color=blue&label=downloads&logo=pypi&logoColor=gold)](https://pypistats.org/packages/fritzbox-tray)
 
-![status](https://img.shields.io/pypi/status/fritzbox-tray)
 [![license](https://img.shields.io/pypi/l/fritzbox-tray?color=blueviolet)](https://github.com/aviolaris/fritzbox-tray/blob/master/LICENSE)
 ![format](https://img.shields.io/pypi/format/fritzbox-tray?color=blueviolet)
-[![pypi-downloads](https://img.shields.io/pypi/dm/fritzbox-tray?color=brightgreen&label=pypi%20downloads)](https://pypistats.org/packages/fritzbox-tray)
+![status](https://img.shields.io/pypi/status/fritzbox-tray?color=blue)
+![GitHub Repo stars](https://img.shields.io/github/stars/aviolaris/fritzbox-tray?color=blue&logo=github&logoColor=white)
+
 
 ## Features
 
 - Display current external IP address
 - Renew IP address
 
 ## Requirements
@@ -50,15 +50,15 @@
 
     pip install fritzbox-tray
 
 ## Usage
 
 To launch FritzBox Tray:
 
- - **On Windows**, double-click the `fritzbox-tray.exe` (usually located in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts` or run the `fritzbox-tray` command from the command prompt.
+ - **On Windows**, double-click the `fritzbox-tray.exe` (usually located in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts`) or run the `fritzbox-tray` command from the command prompt.
 
 
  - **On Linux**, double-click the `fritzbox-tray` (usually located in `~/.local/bin`) or run the `./fritzbox-tray` command from the terminal.
 
 Once the program is running, an icon will be added to the system tray. By right-clicking on the icon, a menu will appear containing the following options:
 
  - **Display Current IP Address**: This option will trigger a notification displaying the current external IP address of the FRITZ!Box device.
```

