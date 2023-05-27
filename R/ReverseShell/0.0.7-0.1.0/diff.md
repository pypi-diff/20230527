# Comparing `tmp/ReverseShell-0.0.7.tar.gz` & `tmp/ReverseShell-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseShell-0.0.7.tar", last modified: Mon May  1 20:51:02 2023, max compression
+gzip compressed data, was "ReverseShell-0.1.0.tar", last modified: Sat May 27 15:22:36 2023, max compression
```

## Comparing `ReverseShell-0.0.7.tar` & `ReverseShell-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/
--rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-05-01 15:42:38.000000 ReverseShell-0.0.7/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      151 2023-05-01 23:24:14.000000 ReverseShell-0.0.7/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     6977 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     5915 2023-05-01 20:04:16.000000 ReverseShell-0.0.7/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/ReverseShell.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     6977 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      926 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-05-01 20:51:02.000000 ReverseShell-0.0.7/ReverseShell.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    28080 2023-05-01 20:50:35.000000 ReverseShell-0.0.7/ReverseShell.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/clients/
--rw-r--r--   0 kali      (1000) kali      (1000)     3258 2023-05-01 21:42:38.000000 ReverseShell-0.0.7/clients/shellclientdns.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3957 2023-05-02 02:07:58.000000 ReverseShell-0.0.7/clients/shellclienthttp_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4121 2023-05-02 02:05:50.000000 ReverseShell-0.0.7/clients/shellclienthttps_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4993 2023-05-02 02:05:58.000000 ReverseShell-0.0.7/clients/shellclienthttpsencrypt_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4609 2023-05-02 02:06:52.000000 ReverseShell-0.0.7/clients/shellclienthttpsencrypt_advanced2.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3126 2023-05-02 04:11:00.000000 ReverseShell-0.0.7/clients/shellclientsocketirc.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2334 2023-05-02 04:11:00.000000 ReverseShell-0.0.7/clients/shellclientsockettcp.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2295 2023-05-02 04:11:00.000000 ReverseShell-0.0.7/clients/shellclienttcp.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3384 2023-05-02 02:08:36.000000 ReverseShell-0.0.7/clients/shellclienttcp_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2176 2023-05-01 21:42:38.000000 ReverseShell-0.0.7/clients/shellclientudp.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/minifiers/
--rw-r--r--   0 kali      (1000) kali      (1000)     1751 2023-05-02 02:21:22.000000 ReverseShell-0.0.7/minifiers/shellclienthttpsencrypt_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1281 2023-05-02 02:21:02.000000 ReverseShell-0.0.7/minifiers/shellclienthttpsencrypt_advanced2.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/oneliners/
--rw-r--r--   0 kali      (1000) kali      (1000)     1779 2023-05-02 02:25:04.000000 ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2024 2023-05-02 02:36:58.000000 ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced.sh
--rw-r--r--   0 kali      (1000) kali      (1000)     1314 2023-05-02 02:23:44.000000 ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced2.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1483 2023-05-02 02:37:24.000000 ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced2.sh
--rw-r--r--   0 kali      (1000) kali      (1000)     1514 2023-05-01 15:42:38.000000 ReverseShell-0.0.7/server.crt
--rw-r--r--   0 kali      (1000) kali      (1000)     1732 2023-05-01 15:42:38.000000 ReverseShell-0.0.7/server.key
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-05-01 20:51:02.310286 ReverseShell-0.0.7/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1745 2023-05-01 20:50:48.000000 ReverseShell-0.0.7/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-27 15:22:36.276066 ReverseShell-0.1.0/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      151 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)    11937 2023-05-27 15:22:36.276066 ReverseShell-0.1.0/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)    10969 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-27 15:22:36.256056 ReverseShell-0.1.0/ReverseShell.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)    11937 2023-05-27 15:22:36.000000 ReverseShell-0.1.0/ReverseShell.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1102 2023-05-27 15:22:36.000000 ReverseShell-0.1.0/ReverseShell.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-27 15:22:36.000000 ReverseShell-0.1.0/ReverseShell.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-05-27 15:22:36.000000 ReverseShell-0.1.0/ReverseShell.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-05-27 15:22:36.000000 ReverseShell-0.1.0/ReverseShell.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-05-27 15:22:36.000000 ReverseShell-0.1.0/ReverseShell.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    52467 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/ReverseShell.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-27 15:22:36.276066 ReverseShell-0.1.0/clients/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3258 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/clients/shellclientdns.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3957 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/clients/shellclienthttp_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4121 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/clients/shellclienthttps_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4993 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/clients/shellclienthttpsencrypt_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4609 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/clients/shellclienthttpsencrypt_advanced2.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    16289 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/clients/shellclienthttpsencrypt_advanced_0_1_0.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3126 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/clients/shellclientsocketirc.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2334 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/clients/shellclientsockettcp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2295 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/clients/shellclienttcp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3384 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/clients/shellclienttcp_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2176 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/clients/shellclientudp.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      909 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/file_version_info.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-27 15:22:36.276066 ReverseShell-0.1.0/minifiers/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1751 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/minifiers/shellclienthttpsencrypt_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1281 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/minifiers/shellclienthttpsencrypt_advanced2.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     9436 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/minifiers/shellclienthttpsencrypt_advanced_0_1_0.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-27 15:22:36.276066 ReverseShell-0.1.0/oneliners/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1779 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/oneliners/shellclienthttpsencrypt_advanced.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2024 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/oneliners/shellclienthttpsencrypt_advanced.sh
+-rw-r--r--   0 kali      (1000) kali      (1000)     1314 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/oneliners/shellclienthttpsencrypt_advanced2.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1483 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/oneliners/shellclienthttpsencrypt_advanced2.sh
+-rw-r--r--   0 kali      (1000) kali      (1000)     4349 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/oneliners/shellclienthttpsencrypt_advanced_0_1_0.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1514 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/server.crt
+-rw-r--r--   0 kali      (1000) kali      (1000)     1732 2023-05-27 15:20:41.000000 ReverseShell-0.1.0/server.key
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-05-27 15:22:36.276066 ReverseShell-0.1.0/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1745 2023-05-27 15:22:26.000000 ReverseShell-0.1.0/setup.py
```

### Comparing `ReverseShell-0.0.7/LICENSE.txt` & `ReverseShell-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/ReverseShell.egg-info/SOURCES.txt` & `ReverseShell-0.1.0/ReverseShell.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 ReverseShell.py
+file_version_info.txt
 server.crt
 server.key
 setup.cfg
 setup.py
 ReverseShell.egg-info/PKG-INFO
 ReverseShell.egg-info/SOURCES.txt
 ReverseShell.egg-info/dependency_links.txt
@@ -13,18 +14,21 @@
 ReverseShell.egg-info/requires.txt
 ReverseShell.egg-info/top_level.txt
 clients/shellclientdns.py
 clients/shellclienthttp_advanced.py
 clients/shellclienthttps_advanced.py
 clients/shellclienthttpsencrypt_advanced.py
 clients/shellclienthttpsencrypt_advanced2.py
+clients/shellclienthttpsencrypt_advanced_0_1_0.py
 clients/shellclientsocketirc.py
 clients/shellclientsockettcp.py
 clients/shellclienttcp.py
 clients/shellclienttcp_advanced.py
 clients/shellclientudp.py
 minifiers/shellclienthttpsencrypt_advanced.py
 minifiers/shellclienthttpsencrypt_advanced2.py
+minifiers/shellclienthttpsencrypt_advanced_0_1_0.py
 oneliners/shellclienthttpsencrypt_advanced.py
 oneliners/shellclienthttpsencrypt_advanced.sh
 oneliners/shellclienthttpsencrypt_advanced2.py
-oneliners/shellclienthttpsencrypt_advanced2.sh
+oneliners/shellclienthttpsencrypt_advanced2.sh
+oneliners/shellclienthttpsencrypt_advanced_0_1_0.py
```

### Comparing `ReverseShell-0.0.7/clients/shellclientdns.py` & `ReverseShell-0.1.0/clients/shellclientdns.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/clients/shellclienthttp_advanced.py` & `ReverseShell-0.1.0/clients/shellclienthttp_advanced.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/clients/shellclienthttps_advanced.py` & `ReverseShell-0.1.0/clients/shellclienthttps_advanced.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/clients/shellclienthttpsencrypt_advanced.py` & `ReverseShell-0.1.0/clients/shellclienthttpsencrypt_advanced.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/clients/shellclienthttpsencrypt_advanced2.py` & `ReverseShell-0.1.0/clients/shellclienthttpsencrypt_advanced2.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/clients/shellclientsocketirc.py` & `ReverseShell-0.1.0/clients/shellclientsocketirc.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/clients/shellclientsockettcp.py` & `ReverseShell-0.1.0/clients/shellclientsockettcp.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/clients/shellclienttcp.py` & `ReverseShell-0.1.0/clients/shellclienttcp.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/clients/shellclienttcp_advanced.py` & `ReverseShell-0.1.0/clients/shellclienttcp_advanced.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/clients/shellclientudp.py` & `ReverseShell-0.1.0/clients/shellclientudp.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/minifiers/shellclienthttpsencrypt_advanced.py` & `ReverseShell-0.1.0/minifiers/shellclienthttpsencrypt_advanced.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/minifiers/shellclienthttpsencrypt_advanced2.py` & `ReverseShell-0.1.0/minifiers/shellclienthttpsencrypt_advanced2.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced.py` & `ReverseShell-0.1.0/oneliners/shellclienthttpsencrypt_advanced.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced.sh` & `ReverseShell-0.1.0/oneliners/shellclienthttpsencrypt_advanced.sh`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced2.py` & `ReverseShell-0.1.0/oneliners/shellclienthttpsencrypt_advanced2.py`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/oneliners/shellclienthttpsencrypt_advanced2.sh` & `ReverseShell-0.1.0/oneliners/shellclienthttpsencrypt_advanced2.sh`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/server.crt` & `ReverseShell-0.1.0/server.crt`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/server.key` & `ReverseShell-0.1.0/server.key`

 * *Files identical despite different names*

### Comparing `ReverseShell-0.0.7/setup.py` & `ReverseShell-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from glob import glob
 
 setup(
     name="ReverseShell",
-    version="0.0.7",
+    version="0.1.0",
     py_modules=["ReverseShell"],
     install_requires=["PythonToolsKit"],
     author="Maurice Lambert",
     author_email="mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
     description=(
```

