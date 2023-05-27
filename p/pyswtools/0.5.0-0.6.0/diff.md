# Comparing `tmp/pyswtools-0.5.0.tar.gz` & `tmp/pyswtools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyswtools-0.5.0.tar", max compression
+gzip compressed data, was "pyswtools-0.6.0.tar", max compression
```

## Comparing `pyswtools-0.5.0.tar` & `pyswtools-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     3604 2023-05-04 20:45:17.566358 pyswtools-0.5.0/README.md
--rw-r--r--   0        0        0      807 2023-05-04 20:45:17.566358 pyswtools-0.5.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-05-03 14:11:07.498269 pyswtools-0.5.0/pyswtools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 20:45:17.566358 pyswtools-0.5.0/pyswtools/auto_exporter/__init__.py
--rw-r--r--   0        0        0     5406 2023-05-04 20:45:17.566358 pyswtools-0.5.0/pyswtools/auto_exporter/main.py
--rw-r--r--   0        0        0     3415 2023-05-04 08:30:28.502483 pyswtools-0.5.0/pyswtools/config.py
--rw-r--r--   0        0        0        0 2023-05-04 20:45:17.566358 pyswtools-0.5.0/pyswtools/copy_full_assembly/__init__.py
--rw-r--r--   0        0        0     1807 2023-05-04 15:28:13.720447 pyswtools-0.5.0/pyswtools/copy_full_assembly/main.py
--rw-r--r--   0        0        0      737 2023-05-04 20:45:17.566358 pyswtools-0.5.0/pyswtools/main.py
--rw-r--r--   0        0        0        0 2023-05-03 11:48:07.729317 pyswtools-0.5.0/pyswtools/ready_dxf/__init__.py
--rw-r--r--   0        0        0     1326 2023-05-03 13:47:31.066860 pyswtools-0.5.0/pyswtools/ready_dxf/dxf_utilities.py
--rw-r--r--   0        0        0      645 2023-05-03 13:47:31.062860 pyswtools-0.5.0/pyswtools/ready_dxf/file_utilities.py
--rw-r--r--   0        0        0      502 2023-05-03 13:47:31.058860 pyswtools-0.5.0/pyswtools/ready_dxf/main.py
--rw-r--r--   0        0        0      454 2023-05-04 08:29:48.610745 pyswtools-0.5.0/pyswtools/utils.py
--rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 pyswtools-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-26 12:38:39.604629 pyswtools-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4081 2023-05-27 11:49:27.007898 pyswtools-0.6.0/README.md
+-rw-r--r--   0        0        0      807 2023-05-27 11:49:17.907991 pyswtools-0.6.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-05-03 14:11:07.498269 pyswtools-0.6.0/pyswtools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 20:45:17.566358 pyswtools-0.6.0/pyswtools/auto_exporter/__init__.py
+-rw-r--r--   0        0        0     5406 2023-05-04 20:45:17.566358 pyswtools-0.6.0/pyswtools/auto_exporter/main.py
+-rw-r--r--   0        0        0     3415 2023-05-04 08:30:28.502483 pyswtools-0.6.0/pyswtools/config.py
+-rw-r--r--   0        0        0        0 2023-05-04 20:45:17.566358 pyswtools-0.6.0/pyswtools/copy_full_assembly/__init__.py
+-rw-r--r--   0        0        0     1807 2023-05-04 15:28:13.720447 pyswtools-0.6.0/pyswtools/copy_full_assembly/main.py
+-rw-r--r--   0        0        0      787 2023-05-27 11:49:17.907991 pyswtools-0.6.0/pyswtools/main.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:48:07.729317 pyswtools-0.6.0/pyswtools/ready_dxf/__init__.py
+-rw-r--r--   0        0        0     1326 2023-05-03 13:47:31.066860 pyswtools-0.6.0/pyswtools/ready_dxf/dxf_utilities.py
+-rw-r--r--   0        0        0      645 2023-05-03 13:47:31.062860 pyswtools-0.6.0/pyswtools/ready_dxf/file_utilities.py
+-rw-r--r--   0        0        0      502 2023-05-03 13:47:31.058860 pyswtools-0.6.0/pyswtools/ready_dxf/main.py
+-rw-r--r--   0        0        0        0 2023-05-27 11:49:17.907991 pyswtools-0.6.0/pyswtools/stat/__init__.py
+-rw-r--r--   0        0        0     5434 2023-05-27 11:49:17.907991 pyswtools-0.6.0/pyswtools/stat/main.py
+-rw-r--r--   0        0        0      454 2023-05-27 11:36:54.314563 pyswtools-0.6.0/pyswtools/utils.py
+-rw-r--r--   0        0        0     4962 1970-01-01 00:00:00.000000 pyswtools-0.6.0/PKG-INFO
```

### Comparing `pyswtools-0.5.0/README.md` & `pyswtools-0.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 
 ## Contributing
 
 If you found a bug or if you have any idea for the project feel free to open a new issue on github ! And if you want to directly contribute, you are welcome.
 
 List of ressources that can be helpful when starting with the solidworks API:
-- [https://help.solidworks.com/2022/french/SolidWorks/sldworks/c_solidworks_api.htm?verRedirect=1](Solidworks API)
-- [https://mycad.visiativ.com/sites/default/files/questions/answer/15/11/2019/solidworks_python_api.pdf](Python examples)
+- [Solidworks API](https://help.solidworks.com/2022/french/SolidWorks/sldworks/c_solidworks_api.htm?verRedirect=1)
+- [Python examples](https://mycad.visiativ.com/sites/default/files/questions/answer/15/11/2019/solidworks_python_api.pdf)
 
 ## List of modules
 
 ### CLI
 It is the main module of this project. It allows you to select the actions that you want to apply. To directly get help from the tool simply type:
 ```
 pyswtools
@@ -113,7 +113,24 @@
 
 
 ```
 pyswtools auto-export PATH/TO/DIR MODE
 ```
 
 With `Mode` being `AUTO`, `DXF` or `STL`. It will create directory with the extension used  and the corresponding files in it.
+
+### Stat
+This tool help you get stat on an assembly. It can gives you recursive information about the mass of each component of an assembly.
+
+#### How to use
+
+```
+pyswtools stat PATH/TO/ASSEMBLY OPTIONS
+```
+
+You can select the display mode:
+- `--tree`: (default) It will follow the structure from the assembly file
+- `--list`: It will output to a single list
+
+You can select the sort:
+- `--mass`: (default) sort with a decreasing mass
+- `--name`: sort with alphabetical order
```

### Comparing `pyswtools-0.5.0/pyproject.toml` & `pyswtools-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyswtools"
-version = "0.5.0"
+version = "0.6.0"
 description = "Set of tools to improve Solidworks usage"
 authors = ["ldevillez <louis.devillez@gmail.com>"]
 license = "GNU General Public License"
 readme = "README.md"
 homepage = "https://github.com/ldevillez/pySwTools"
 repository = "https://github.com/ldevillez/pySwTools"
```

### Comparing `pyswtools-0.5.0/pyswtools/auto_exporter/main.py` & `pyswtools-0.6.0/pyswtools/auto_exporter/main.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.5.0/pyswtools/config.py` & `pyswtools-0.6.0/pyswtools/config.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.5.0/pyswtools/copy_full_assembly/main.py` & `pyswtools-0.6.0/pyswtools/copy_full_assembly/main.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.5.0/pyswtools/main.py` & `pyswtools-0.6.0/pyswtools/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 import click
 
 from .config import config
 from .ready_dxf.main import ready_dxf
 from .copy_full_assembly.main import copy_full_assembly
 from .auto_exporter.main import auto_export
+from .stat.main import stat
 
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 __author__ = "Devillez Louis"
 __maintainer__ = "Deville Louis"
 __email__ = "louis.devillez@gmail.com"
 
 
 @click.group()
 @click.version_option(__version__, "-v", "--version")
@@ -25,10 +26,11 @@
     """
 
 
 cli.add_command(config)
 cli.add_command(ready_dxf)
 cli.add_command(copy_full_assembly)
 cli.add_command(auto_export)
+cli.add_command(stat)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `pyswtools-0.5.0/pyswtools/ready_dxf/dxf_utilities.py` & `pyswtools-0.6.0/pyswtools/ready_dxf/dxf_utilities.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.5.0/pyswtools/ready_dxf/file_utilities.py` & `pyswtools-0.6.0/pyswtools/ready_dxf/file_utilities.py`

 * *Files identical despite different names*

### Comparing `pyswtools-0.5.0/PKG-INFO` & `pyswtools-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswtools
-Version: 0.5.0
+Version: 0.6.0
 Summary: Set of tools to improve Solidworks usage
 Home-page: https://github.com/ldevillez/pySwTools
 License: GNU General Public License
 Author: ldevillez
 Author-email: louis.devillez@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -41,16 +41,16 @@
 
 
 ## Contributing
 
 If you found a bug or if you have any idea for the project feel free to open a new issue on github ! And if you want to directly contribute, you are welcome.
 
 List of ressources that can be helpful when starting with the solidworks API:
-- [https://help.solidworks.com/2022/french/SolidWorks/sldworks/c_solidworks_api.htm?verRedirect=1](Solidworks API)
-- [https://mycad.visiativ.com/sites/default/files/questions/answer/15/11/2019/solidworks_python_api.pdf](Python examples)
+- [Solidworks API](https://help.solidworks.com/2022/french/SolidWorks/sldworks/c_solidworks_api.htm?verRedirect=1)
+- [Python examples](https://mycad.visiativ.com/sites/default/files/questions/answer/15/11/2019/solidworks_python_api.pdf)
 
 ## List of modules
 
 ### CLI
 It is the main module of this project. It allows you to select the actions that you want to apply. To directly get help from the tool simply type:
 ```
 pyswtools
@@ -137,7 +137,24 @@
 
 ```
 pyswtools auto-export PATH/TO/DIR MODE
 ```
 
 With `Mode` being `AUTO`, `DXF` or `STL`. It will create directory with the extension used  and the corresponding files in it.
 
+### Stat
+This tool help you get stat on an assembly. It can gives you recursive information about the mass of each component of an assembly.
+
+#### How to use
+
+```
+pyswtools stat PATH/TO/ASSEMBLY OPTIONS
+```
+
+You can select the display mode:
+- `--tree`: (default) It will follow the structure from the assembly file
+- `--list`: It will output to a single list
+
+You can select the sort:
+- `--mass`: (default) sort with a decreasing mass
+- `--name`: sort with alphabetical order
+
```

