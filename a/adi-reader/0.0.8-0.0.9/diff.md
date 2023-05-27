# Comparing `tmp/adi-reader-0.0.8.tar.gz` & `tmp/adi-reader-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adi-reader-0.0.8.tar", last modified: Mon Nov  8 22:13:36 2021, max compression
+gzip compressed data, was "adi-reader-0.0.9.tar", last modified: Sat May 27 16:25:02 2023, max compression
```

## Comparing `adi-reader-0.0.8.tar` & `adi-reader-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxrwxrwx   0        0        0        0 2021-11-08 22:13:36.544494 adi-reader-0.0.8/
--rw-rw-rw-   0        0        0       17 2021-05-27 16:06:34.000000 adi-reader-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3814 2021-11-08 22:13:36.539507 adi-reader-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2666 2021-11-08 14:58:42.000000 adi-reader-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-11-08 22:13:36.500610 adi-reader-0.0.8/adi/
--rw-rw-rw-   0        0        0    25038 2021-05-27 19:53:12.000000 adi-reader-0.0.8/adi/ADIDatCAPI_mex.h
--rw-rw-rw-   0        0        0  1828864 2021-05-27 19:53:12.000000 adi-reader-0.0.8/adi/ADIDatIOWin64.dll
--rw-rw-rw-   0        0        0     8374 2021-05-27 19:53:12.000000 adi-reader-0.0.8/adi/ADIDatIOWin64.lib
--rw-rw-rw-   0        0        0       56 2021-05-26 17:42:20.000000 adi-reader-0.0.8/adi/__init__.py
--rw-rw-rw-   0        0        0    73282 2021-05-27 19:53:12.000000 adi-reader-0.0.8/adi/_adi_cffi.c
--rw-rw-rw-   0        0        0    26624 2021-11-08 14:53:55.000000 adi-reader-0.0.8/adi/_adi_cffi.cp36-win_amd64.pyd
--rw-rw-rw-   0        0        0    26624 2021-05-27 19:53:12.000000 adi-reader-0.0.8/adi/_adi_cffi.cp37-win_amd64.pyd
--rw-rw-rw-   0        0        0    30720 2021-08-05 22:25:38.000000 adi-reader-0.0.8/adi/_adi_cffi.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0    30720 2021-10-24 12:24:45.000000 adi-reader-0.0.8/adi/_adi_cffi.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0    73289 2021-08-05 20:14:34.000000 adi-reader-0.0.8/adi/_adi_cffi2.c
--rw-rw-rw-   0        0        0    22528 2021-08-05 20:14:34.000000 adi-reader-0.0.8/adi/_adi_cffi2.cp38-win32.pyd
--rw-rw-rw-   0        0        0    22528 2021-10-24 12:24:45.000000 adi-reader-0.0.8/adi/_adi_cffi2.cp39-win32.pyd
--rw-rw-rw-   0        0        0     5349 2021-05-26 17:42:20.000000 adi-reader-0.0.8/adi/cffi_build.py
--rw-rw-rw-   0        0        0     5348 2021-08-05 20:14:34.000000 adi-reader-0.0.8/adi/cffi_build_win32.py
--rw-rw-rw-   0        0        0    18658 2021-11-08 15:02:36.000000 adi-reader-0.0.8/adi/read.py
-drwxrwxrwx   0        0        0        0 2021-11-08 22:13:36.534520 adi-reader-0.0.8/adi_reader.egg-info/
--rw-rw-rw-   0        0        0     3814 2021-11-08 22:13:35.000000 adi-reader-0.0.8/adi_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2021-11-08 22:13:36.000000 adi-reader-0.0.8/adi_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-08 22:13:35.000000 adi-reader-0.0.8/adi_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2021-11-08 22:13:36.000000 adi-reader-0.0.8/adi_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2021-11-08 22:13:36.000000 adi-reader-0.0.8/adi_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-08 22:13:36.545492 adi-reader-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      821 2021-11-08 22:13:31.000000 adi-reader-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 16:25:02.354819 adi-reader-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2019-03-13 17:33:28.000000 adi-reader-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       17 2021-10-26 00:23:59.000000 adi-reader-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3147 2023-05-27 16:25:02.354819 adi-reader-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2666 2022-01-15 03:00:55.000000 adi-reader-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 16:25:02.338183 adi-reader-0.0.9/adi/
+-rw-rw-rw-   0        0        0    25038 2014-08-05 23:48:41.000000 adi-reader-0.0.9/adi/ADIDatCAPI_mex.h
+-rw-rw-rw-   0        0        0  1309184 2016-03-10 16:24:50.000000 adi-reader-0.0.9/adi/ADIDatIOWin.dll
+-rw-rw-rw-   0        0        0     8358 2016-03-10 16:24:36.000000 adi-reader-0.0.9/adi/ADIDatIOWin.lib
+-rw-rw-rw-   0        0        0  1828864 2019-03-25 13:34:24.000000 adi-reader-0.0.9/adi/ADIDatIOWin64.dll
+-rw-rw-rw-   0        0        0     8374 2019-03-25 13:34:24.000000 adi-reader-0.0.9/adi/ADIDatIOWin64.lib
+-rw-rw-rw-   0        0        0       56 2019-03-13 14:40:46.000000 adi-reader-0.0.9/adi/__init__.py
+-rw-rw-rw-   0        0        0    73282 2021-05-26 16:42:32.000000 adi-reader-0.0.9/adi/_adi_cffi.c
+-rw-rw-rw-   0        0        0    29184 2023-05-27 16:02:37.000000 adi-reader-0.0.9/adi/_adi_cffi.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0    29184 2023-05-27 16:05:47.000000 adi-reader-0.0.9/adi/_adi_cffi.cp311-win_amd64.pyd
+-rw-rw-rw-   0        0        0    26624 2019-10-28 21:15:23.000000 adi-reader-0.0.9/adi/_adi_cffi.cp36-win_amd64.pyd
+-rw-rw-rw-   0        0        0    26624 2019-10-28 21:19:22.000000 adi-reader-0.0.9/adi/_adi_cffi.cp37-win_amd64.pyd
+-rw-rw-rw-   0        0        0    30720 2021-08-05 22:10:39.000000 adi-reader-0.0.9/adi/_adi_cffi.cp38-win_amd64.pyd
+-rw-rw-rw-   0        0        0    30720 2021-10-23 14:58:24.000000 adi-reader-0.0.9/adi/_adi_cffi.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0    73289 2021-08-05 19:36:19.000000 adi-reader-0.0.9/adi/_adi_cffi2.c
+-rw-rw-rw-   0        0        0    22528 2021-08-05 19:36:21.000000 adi-reader-0.0.9/adi/_adi_cffi2.cp38-win32.pyd
+-rw-rw-rw-   0        0        0    22528 2021-10-23 14:53:01.000000 adi-reader-0.0.9/adi/_adi_cffi2.cp39-win32.pyd
+-rw-rw-rw-   0        0        0     5349 2019-03-25 15:10:46.000000 adi-reader-0.0.9/adi/cffi_build.py
+-rw-rw-rw-   0        0        0     5348 2021-08-05 19:35:43.000000 adi-reader-0.0.9/adi/cffi_build_win32.py
+-rw-rw-rw-   0        0        0     5349 2019-03-25 15:10:46.000000 adi-reader-0.0.9/adi/cffi_build_win32.py.bak
+-rw-rw-rw-   0        0        0    18658 2022-01-15 03:00:55.000000 adi-reader-0.0.9/adi/read.py
+drwxrwxrwx   0        0        0        0 2023-05-27 16:25:02.353819 adi-reader-0.0.9/adi_reader.egg-info/
+-rw-rw-rw-   0        0        0     3147 2023-05-27 16:25:01.000000 adi-reader-0.0.9/adi_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-05-27 16:25:01.000000 adi-reader-0.0.9/adi_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 16:25:01.000000 adi-reader-0.0.9/adi_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-27 16:25:01.000000 adi-reader-0.0.9/adi_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-27 16:25:01.000000 adi-reader-0.0.9/adi_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 16:25:02.355819 adi-reader-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      821 2023-05-27 16:18:38.000000 adi-reader-0.0.9/setup.py
```

### Comparing `adi-reader-0.0.8/README.md` & `adi-reader-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `adi-reader-0.0.8/adi/ADIDatCAPI_mex.h` & `adi-reader-0.0.9/adi/ADIDatCAPI_mex.h`

 * *Files identical despite different names*

### Comparing `adi-reader-0.0.8/adi/ADIDatIOWin64.dll` & `adi-reader-0.0.9/adi/ADIDatIOWin64.dll`

 * *Files identical despite different names*

### Comparing `adi-reader-0.0.8/adi/ADIDatIOWin64.lib` & `adi-reader-0.0.9/adi/ADIDatIOWin64.lib`

 * *Files identical despite different names*

### Comparing `adi-reader-0.0.8/adi/_adi_cffi.c` & `adi-reader-0.0.9/adi/_adi_cffi.c`

 * *Files identical despite different names*

### Comparing `adi-reader-0.0.8/adi/_adi_cffi2.c` & `adi-reader-0.0.9/adi/_adi_cffi2.c`

 * *Files identical despite different names*

### Comparing `adi-reader-0.0.8/adi/cffi_build.py` & `adi-reader-0.0.9/adi/cffi_build.py`

 * *Files identical despite different names*

### Comparing `adi-reader-0.0.8/adi/cffi_build_win32.py` & `adi-reader-0.0.9/adi/cffi_build_win32.py`

 * *Files identical despite different names*

### Comparing `adi-reader-0.0.8/adi/read.py` & `adi-reader-0.0.9/adi/read.py`

 * *Files identical despite different names*

### Comparing `adi-reader-0.0.8/setup.py` & `adi-reader-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adi-reader",
-    version="0.0.8",
+    version="0.0.9",
     author="Jim Hokanson",
     author_email="jim.hokanson@gmail.com",
     description="Reading LabChart recorded data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JimHokanson/adinstruments_sdk_python/",
     packages=setuptools.find_packages(),
     install_requires=['numpy', 'cffi'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows",
     ],
-    python_requires='>= 3.6, < 3.10',
+    python_requires='>= 3.6, < 3.12',
     include_package_data=True,
 )
```

