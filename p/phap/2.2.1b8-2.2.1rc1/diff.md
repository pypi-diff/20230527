# Comparing `tmp/phap-2.2.1b8.tar.gz` & `tmp/phap-2.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phap-2.2.1b8.tar", last modified: Fri May 26 11:44:27 2023, max compression
+gzip compressed data, was "phap-2.2.1rc1.tar", last modified: Sat May 27 02:53:42 2023, max compression
```

## Comparing `phap-2.2.1b8.tar` & `phap-2.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 11:44:27.676654 phap-2.2.1b8/
--rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-2.2.1b8/LICENSE
--rw-rw-rw-   0        0        0     1718 2023-05-26 11:44:27.674656 phap-2.2.1b8/PKG-INFO
--rw-rw-rw-   0        0        0      919 2023-05-26 11:44:02.000000 phap-2.2.1b8/README.md
--rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-2.2.1b8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 11:44:27.676654 phap-2.2.1b8/setup.cfg
--rw-rw-rw-   0        0        0     1685 2023-05-26 11:43:55.000000 phap-2.2.1b8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:44:27.640884 phap-2.2.1b8/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 11:44:27.653117 phap-2.2.1b8/src/numalgo/
--rw-rw-rw-   0        0        0       62 2023-05-26 11:43:30.000000 phap-2.2.1b8/src/numalgo/__init__.py
--rw-rw-rw-   0        0        0      452 2023-05-26 09:54:41.000000 phap-2.2.1b8/src/numalgo/deskcheck.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:44:27.654116 phap-2.2.1b8/src/phap/
--rw-rw-rw-   0        0        0      881 2023-05-26 10:49:29.000000 phap-2.2.1b8/src/phap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:44:27.662649 phap-2.2.1b8/src/phap.egg-info/
--rw-rw-rw-   0        0        0     1718 2023-05-26 11:44:27.000000 phap-2.2.1b8/src/phap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-05-26 11:44:27.000000 phap-2.2.1b8/src/phap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 11:44:27.000000 phap-2.2.1b8/src/phap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-26 11:44:27.000000 phap-2.2.1b8/src/phap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 11:44:27.666654 phap-2.2.1b8/src/stralgo/
--rw-rw-rw-   0        0        0       55 2023-05-26 11:28:00.000000 phap-2.2.1b8/src/stralgo/__init__.py
--rw-rw-rw-   0        0        0      972 2023-02-20 00:51:10.000000 phap-2.2.1b8/src/stralgo/base.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:44:27.669654 phap-2.2.1b8/src/stralgo/hash/
--rw-rw-rw-   0        0        0      251 2023-05-26 11:43:14.000000 phap-2.2.1b8/src/stralgo/hash/__init__.py
--rw-rw-rw-   0        0        0      460 2023-02-20 00:51:14.000000 phap-2.2.1b8/src/stralgo/hash/sha.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:44:27.672654 phap-2.2.1b8/src/stralgo/hash/sm/
--rw-rw-rw-   0        0        0       26 2023-05-26 09:54:41.000000 phap-2.2.1b8/src/stralgo/hash/sm/__init__.py
--rw-rw-rw-   0        0        0     6937 2023-05-26 09:54:41.000000 phap-2.2.1b8/src/stralgo/hash/sm/sm3libs.py
--rw-rw-rw-   0        0        0      175 2023-05-25 04:35:10.000000 phap-2.2.1b8/src/stralgo/json.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:53:42.328446 phap-2.2.1rc1/
+-rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-2.2.1rc1/LICENSE
+-rw-rw-rw-   0        0        0     2048 2023-05-27 02:53:42.326449 phap-2.2.1rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-05-27 02:53:14.000000 phap-2.2.1rc1/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-2.2.1rc1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 02:53:42.328446 phap-2.2.1rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1686 2023-05-27 02:51:19.000000 phap-2.2.1rc1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:53:41.906673 phap-2.2.1rc1/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 02:53:41.920305 phap-2.2.1rc1/src/numalgo/
+-rw-rw-rw-   0        0        0       62 2023-05-26 11:43:30.000000 phap-2.2.1rc1/src/numalgo/__init__.py
+-rw-rw-rw-   0        0        0      450 2023-05-27 02:24:29.000000 phap-2.2.1rc1/src/numalgo/deskcheck.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:53:41.921304 phap-2.2.1rc1/src/phap/
+-rw-rw-rw-   0        0        0      881 2023-05-26 10:49:29.000000 phap-2.2.1rc1/src/phap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:53:42.298383 phap-2.2.1rc1/src/phap.egg-info/
+-rw-rw-rw-   0        0        0     2048 2023-05-27 02:53:41.000000 phap-2.2.1rc1/src/phap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-05-27 02:53:41.000000 phap-2.2.1rc1/src/phap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 02:53:41.000000 phap-2.2.1rc1/src/phap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-27 02:53:41.000000 phap-2.2.1rc1/src/phap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 02:53:42.304392 phap-2.2.1rc1/src/stralgo/
+-rw-rw-rw-   0        0        0       55 2023-05-26 11:28:00.000000 phap-2.2.1rc1/src/stralgo/__init__.py
+-rw-rw-rw-   0        0        0      972 2023-02-20 00:51:10.000000 phap-2.2.1rc1/src/stralgo/base.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:53:42.308389 phap-2.2.1rc1/src/stralgo/hash/
+-rw-rw-rw-   0        0        0      251 2023-05-26 11:43:14.000000 phap-2.2.1rc1/src/stralgo/hash/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-02-20 00:51:14.000000 phap-2.2.1rc1/src/stralgo/hash/sha.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:53:42.312400 phap-2.2.1rc1/src/stralgo/hash/sm/
+-rw-rw-rw-   0        0        0       26 2023-05-26 09:54:41.000000 phap-2.2.1rc1/src/stralgo/hash/sm/__init__.py
+-rw-rw-rw-   0        0        0     6937 2023-05-26 09:54:41.000000 phap-2.2.1rc1/src/stralgo/hash/sm/sm3libs.py
+-rw-rw-rw-   0        0        0      175 2023-05-25 04:35:10.000000 phap-2.2.1rc1/src/stralgo/json.py
```

### Comparing `phap-2.2.1b8/LICENSE` & `phap-2.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `phap-2.2.1b8/PKG-INFO` & `phap-2.2.1rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 2.2.1b8
+Version: 2.2.1rc1
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,39 +15,60 @@
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # phap
-### Programing Helpful Algorithm Package
+### *Programing Helpful Algorithm Package*
 ### Powered by Python 3.11
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 ### English  | [简体中文](README-zh-CN.md)
 
 # Links
 [Github](https://github.com/DashBing/phap/ "Github") | [Pypi](https://pypi.org/project/phap/ "Pypi") | [Pypi (stralgo)](https://pypi.org/project/stralgo/ "Pypi (stralgo)")
 
 # Versions
-## Stable
+## Stable Version
 + v0.1.0 (stralgo)
 + v1.1.1 (stralgo)
 + v2.1.2
 
+## Latest Available Version
++ v2.2.0
+
 ## Latest Version
-+ v2.2.1-beta8
+### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
++ v2.2.1-rc1
 
 # Build
 ## Precondition
 + Install git and make tools
 + Install Python(the version 3.9 or the version 3.11)
 + Clone source code from source repository
-#### ```git clone git@github.com:DashBing/phap.git```
-#### or
-#### ```git clone https://github.com/DashBing/phap.git```
+```
+git clone git@github.com:DashBing/phap.git
+```
+### or
+```
+git clone https://github.com/DashBing/phap.git
+```
 
 ## Initialize packaging environment
-```make init```
+```
+make init
+```
+#### or
+#### Try to install the package:
++ build
++ twine
+#### This is the example command on Windows:
+```
+python -m pip install build
+python -m pip install twine
+```
 
 ## Build release
-```make build```
+```
+make build
+```
```

### Comparing `phap-2.2.1b8/README.md` & `phap-2.2.1rc1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,54 @@
 # phap
-### Programing Helpful Algorithm Package
+### *Programing Helpful Algorithm Package*
 ### Powered by Python 3.11
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 ### English  | [简体中文](README-zh-CN.md)
 
 # Links
 [Github](https://github.com/DashBing/phap/ "Github") | [Pypi](https://pypi.org/project/phap/ "Pypi") | [Pypi (stralgo)](https://pypi.org/project/stralgo/ "Pypi (stralgo)")
 
 # Versions
-## Stable
+## Stable Version
 + v0.1.0 (stralgo)
 + v1.1.1 (stralgo)
 + v2.1.2
 
+## Latest Available Version
++ v2.2.0
+
 ## Latest Version
-+ v2.2.1-beta8
+### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
++ v2.2.1-rc1
 
 # Build
 ## Precondition
 + Install git and make tools
 + Install Python(the version 3.9 or the version 3.11)
 + Clone source code from source repository
-#### ```git clone git@github.com:DashBing/phap.git```
-#### or
-#### ```git clone https://github.com/DashBing/phap.git```
+```
+git clone git@github.com:DashBing/phap.git
+```
+### or
+```
+git clone https://github.com/DashBing/phap.git
+```
 
 ## Initialize packaging environment
-```make init```
+```
+make init
+```
+#### or
+#### Try to install the package:
++ build
++ twine
+#### This is the example command on Windows:
+```
+python -m pip install build
+python -m pip install twine
+```
 
 ## Build release
-```make build```
+```
+make build
+```
```

### Comparing `phap-2.2.1b8/setup.py` & `phap-2.2.1rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phap",
-    version="2.2.1b8",  #版本
+    version="2.2.1rc1",  #版本
     author="DashBing",
     author_email="mcbbkf@outlook.com",
     description="Programing Helpful Algorithm Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #scripts=[],
     url="https://github.com/DashBing/phap/",
```

### Comparing `phap-2.2.1b8/src/phap/__init__.py` & `phap-2.2.1rc1/src/phap/__init__.py`

 * *Files identical despite different names*

### Comparing `phap-2.2.1b8/src/phap.egg-info/PKG-INFO` & `phap-2.2.1rc1/src/phap.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 2.2.1b8
+Version: 2.2.1rc1
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,39 +15,60 @@
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # phap
-### Programing Helpful Algorithm Package
+### *Programing Helpful Algorithm Package*
 ### Powered by Python 3.11
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 ### English  | [简体中文](README-zh-CN.md)
 
 # Links
 [Github](https://github.com/DashBing/phap/ "Github") | [Pypi](https://pypi.org/project/phap/ "Pypi") | [Pypi (stralgo)](https://pypi.org/project/stralgo/ "Pypi (stralgo)")
 
 # Versions
-## Stable
+## Stable Version
 + v0.1.0 (stralgo)
 + v1.1.1 (stralgo)
 + v2.1.2
 
+## Latest Available Version
++ v2.2.0
+
 ## Latest Version
-+ v2.2.1-beta8
+### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
++ v2.2.1-rc1
 
 # Build
 ## Precondition
 + Install git and make tools
 + Install Python(the version 3.9 or the version 3.11)
 + Clone source code from source repository
-#### ```git clone git@github.com:DashBing/phap.git```
-#### or
-#### ```git clone https://github.com/DashBing/phap.git```
+```
+git clone git@github.com:DashBing/phap.git
+```
+### or
+```
+git clone https://github.com/DashBing/phap.git
+```
 
 ## Initialize packaging environment
-```make init```
+```
+make init
+```
+#### or
+#### Try to install the package:
++ build
++ twine
+#### This is the example command on Windows:
+```
+python -m pip install build
+python -m pip install twine
+```
 
 ## Build release
-```make build```
+```
+make build
+```
```

### Comparing `phap-2.2.1b8/src/stralgo/base.py` & `phap-2.2.1rc1/src/stralgo/base.py`

 * *Files identical despite different names*

### Comparing `phap-2.2.1b8/src/stralgo/hash/sm/sm3libs.py` & `phap-2.2.1rc1/src/stralgo/hash/sm/sm3libs.py`

 * *Files identical despite different names*

