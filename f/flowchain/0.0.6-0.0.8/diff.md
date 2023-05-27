# Comparing `tmp/flowchain-0.0.6.tar.gz` & `tmp/flowchain-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/flowchain/flowchain/dist/.tmp-bjji9yil/flowchain-0.0.6.tar", last modified: Sat May 27 09:41:17 2023, max compression
+gzip compressed data, was "/home/runner/work/flowchain/flowchain/dist/.tmp-3hl68tnw/flowchain-0.0.8.tar", last modified: Sat May 27 12:18:20 2023, max compression
```

## Comparing `flowchain-0.0.6.tar` & `flowchain-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:41:17.000000 flowchain-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 09:41:01.000000 flowchain-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-27 09:41:17.000000 flowchain-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-27 09:41:01.000000 flowchain-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 09:41:01.000000 flowchain-0.0.6/flowchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-27 09:41:01.000000 flowchain-0.0.6/flowchain/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:41:17.000000 flowchain-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-27 09:41:01.000000 flowchain-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:18:20.000000 flowchain-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 12:18:09.000000 flowchain-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-27 12:18:20.000000 flowchain-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-27 12:18:09.000000 flowchain-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:18:20.000000 flowchain-0.0.8/flowchain/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 12:18:09.000000 flowchain-0.0.8/flowchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-27 12:18:09.000000 flowchain-0.0.8/flowchain/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-27 12:18:09.000000 flowchain-0.0.8/flowchain/chain_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:18:20.000000 flowchain-0.0.8/flowchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-27 12:18:20.000000 flowchain-0.0.8/flowchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-27 12:18:20.000000 flowchain-0.0.8/flowchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:18:20.000000 flowchain-0.0.8/flowchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 12:18:20.000000 flowchain-0.0.8/flowchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 12:18:20.000000 flowchain-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-27 12:18:09.000000 flowchain-0.0.8/setup.py
```

### Comparing `flowchain-0.0.6/LICENSE` & `flowchain-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchain-0.0.6/PKG-INFO` & `flowchain-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchain
-Version: 0.0.6
+Version: 0.0.8
 Summary: Flowchain - Method Chaining for TensorFlow
 Home-page: https://github.com/OrigamiDream/flowchain
 Author: OrigamiDream
 Author-email: hello@origamidream.me
 License: MIT
 Keywords: machine learning,deep learning,tensorflow,method chaining,extension
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flowchain-0.0.6/README.md` & `flowchain-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `flowchain-0.0.6/flowchain/chain.py` & `flowchain-0.0.8/flowchain/chain.py`

 * *Files identical despite different names*

### Comparing `flowchain-0.0.6/flowchain.egg-info/PKG-INFO` & `flowchain-0.0.8/flowchain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchain
-Version: 0.0.6
+Version: 0.0.8
 Summary: Flowchain - Method Chaining for TensorFlow
 Home-page: https://github.com/OrigamiDream/flowchain
 Author: OrigamiDream
 Author-email: hello@origamidream.me
 License: MIT
 Keywords: machine learning,deep learning,tensorflow,method chaining,extension
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flowchain-0.0.6/setup.py` & `flowchain-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flowchain',
     packages=find_packages(exclude=[]),
-    version='0.0.6',
+    version='0.0.8',
     license='MIT',
     description='Flowchain - Method Chaining for TensorFlow',
     author='OrigamiDream',
     author_email='hello@origamidream.me',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/OrigamiDream/flowchain',
```

