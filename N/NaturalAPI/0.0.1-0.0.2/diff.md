# Comparing `tmp/NaturalAPI-0.0.1.tar.gz` & `tmp/NaturalAPI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NaturalAPI-0.0.1.tar", last modified: Sat May 27 09:08:01 2023, max compression
+gzip compressed data, was "NaturalAPI-0.0.2.tar", last modified: Sat May 27 09:21:55 2023, max compression
```

## Comparing `NaturalAPI-0.0.1.tar` & `NaturalAPI-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 09:08:01.807890 NaturalAPI-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-27 08:51:54.000000 NaturalAPI-0.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-27 09:08:01.793636 NaturalAPI-0.0.1/NaturalAPI.egg-info/
--rw-rw-rw-   0        0        0     1520 2023-05-27 09:08:01.000000 NaturalAPI-0.0.1/NaturalAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-05-27 09:08:01.000000 NaturalAPI-0.0.1/NaturalAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:08:01.000000 NaturalAPI-0.0.1/NaturalAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:08:01.000000 NaturalAPI-0.0.1/NaturalAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1520 2023-05-27 09:08:01.800839 NaturalAPI-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1101 2023-05-27 09:04:31.000000 NaturalAPI-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 09:08:01.807890 NaturalAPI-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-05-27 09:07:55.000000 NaturalAPI-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 09:21:55.769575 NaturalAPI-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-27 08:51:54.000000 NaturalAPI-0.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-27 09:21:55.749695 NaturalAPI-0.0.2/NaturalAPI.egg-info/
+-rw-rw-rw-   0        0        0     1521 2023-05-27 09:21:55.000000 NaturalAPI-0.0.2/NaturalAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-05-27 09:21:55.000000 NaturalAPI-0.0.2/NaturalAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 09:21:55.000000 NaturalAPI-0.0.2/NaturalAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 09:21:55.000000 NaturalAPI-0.0.2/NaturalAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1521 2023-05-27 09:21:55.769575 NaturalAPI-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2023-05-27 09:20:22.000000 NaturalAPI-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 09:21:55.769575 NaturalAPI-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-05-27 09:20:12.000000 NaturalAPI-0.0.2/setup.py
```

### Comparing `NaturalAPI-0.0.1/LICENSE` & `NaturalAPI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NaturalAPI-0.0.1/NaturalAPI.egg-info/PKG-INFO` & `NaturalAPI-0.0.2/NaturalAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NaturalAPI
-Version: 0.0.1
+Version: 0.0.2
 Summary: API for a small studio
 Home-page: https://github.com/Buelie/Natural
 Author: yydshmcl@outlook.com
 Author-email: yydshmcl@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,9 +18,9 @@
 
 # 安装 | Install
 
 **使用如下命令安装（注意：需要python3.7+版本）：**
 > **Install with the following command (Note: Python 3.7+ is required):**
 
 ```
-pip install NaturalQY
+pip install NaturalAPI
 ```
```

### Comparing `NaturalAPI-0.0.1/PKG-INFO` & `NaturalAPI-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NaturalAPI
-Version: 0.0.1
+Version: 0.0.2
 Summary: API for a small studio
 Home-page: https://github.com/Buelie/Natural
 Author: yydshmcl@outlook.com
 Author-email: yydshmcl@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,9 +18,9 @@
 
 # 安装 | Install
 
 **使用如下命令安装（注意：需要python3.7+版本）：**
 > **Install with the following command (Note: Python 3.7+ is required):**
 
 ```
-pip install NaturalQY
+pip install NaturalAPI
 ```
```

### Comparing `NaturalAPI-0.0.1/README.md` & `NaturalAPI-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 
 # 安装 | Install
 
 **使用如下命令安装（注意：需要python3.7+版本）：**
 > **Install with the following command (Note: Python 3.7+ is required):**
 
 ```
-pip install NaturalQY
+pip install NaturalAPI
 ```
```

### Comparing `NaturalAPI-0.0.1/setup.py` & `NaturalAPI-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name="NaturalAPI",
-  version="0.0.1",
+  version="0.0.2",
   author="yydshmcl@outlook.com",
   author_email="yydshmcl@outlook.com",
   description="API for a small studio",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Buelie/Natural",
   packages=setuptools.find_packages(),
```

