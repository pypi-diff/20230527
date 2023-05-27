# Comparing `tmp/flowchain-0.0.5.tar.gz` & `tmp/flowchain-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchain-0.0.5.tar", last modified: Sat May 27 09:17:04 2023, max compression
+gzip compressed data, was "/home/runner/work/flowchain/flowchain/dist/.tmp-bjji9yil/flowchain-0.0.6.tar", last modified: Sat May 27 09:41:17 2023, max compression
```

## Comparing `flowchain-0.0.5.tar` & `flowchain-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:17:04.593980 flowchain-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 09:16:51.000000 flowchain-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-27 09:17:04.593980 flowchain-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-27 09:16:51.000000 flowchain-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:17:04.593980 flowchain-0.0.5/flowchain/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 09:16:51.000000 flowchain-0.0.5/flowchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-27 09:16:51.000000 flowchain-0.0.5/flowchain/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:17:04.593980 flowchain-0.0.5/flowchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-27 09:17:04.000000 flowchain-0.0.5/flowchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-27 09:17:04.000000 flowchain-0.0.5/flowchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:17:04.000000 flowchain-0.0.5/flowchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 09:17:04.000000 flowchain-0.0.5/flowchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:17:04.593980 flowchain-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-27 09:16:51.000000 flowchain-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:41:17.000000 flowchain-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 09:41:01.000000 flowchain-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-27 09:41:17.000000 flowchain-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-27 09:41:01.000000 flowchain-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 09:41:01.000000 flowchain-0.0.6/flowchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-27 09:41:01.000000 flowchain-0.0.6/flowchain/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 09:41:17.000000 flowchain-0.0.6/flowchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:41:17.000000 flowchain-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-27 09:41:01.000000 flowchain-0.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `flowchain-0.0.5/LICENSE` & `flowchain-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchain-0.0.5/flowchain/chain.py` & `flowchain-0.0.6/flowchain/chain.py`

 * *Files identical despite different names*

### Comparing `flowchain-0.0.5/setup.py` & `flowchain-0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flowchain',
     packages=find_packages(exclude=[]),
-    version='0.0.5',
+    version='0.0.6',
     license='MIT',
     description='Flowchain - Method Chaining for TensorFlow',
     author='OrigamiDream',
     author_email='hello@origamidream.me',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/OrigamiDream/flowchain',
-    python_requires='>=3.8.0',
+    python_requires='>=3.7.0',
     extra_require={
         'gpu': ['tensorflow>=2.4'],
         'cpu': ['tensorflow-cpu>=2.4']
     },
     install_requires=[],
     keywords=[
         'machine learning',
@@ -25,10 +25,10 @@
         'extension'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.8'
+        'Programming Language :: Python :: 3.7'
     ]
 )
```

