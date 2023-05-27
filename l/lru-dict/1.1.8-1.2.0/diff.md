# Comparing `tmp/lru-dict-1.1.8.tar.gz` & `tmp/lru-dict-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lru-dict-1.1.8.tar", last modified: Sat Jul  9 06:59:37 2022, max compression
+gzip compressed data, was "lru-dict-1.2.0.tar", last modified: Sat May 27 00:55:49 2023, max compression
```

## Comparing `lru-dict-1.1.8.tar` & `lru-dict-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 06:59:37.578906 lru-dict-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-07-09 06:59:30.000000 lru-dict-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-07-09 06:59:30.000000 lru-dict-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4598 2022-07-09 06:59:37.578906 lru-dict-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3566 2022-07-09 06:59:30.000000 lru-dict-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    23036 2022-07-09 06:59:30.000000 lru-dict-1.1.8/lru.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 06:59:37.574905 lru-dict-1.1.8/lru_dict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4598 2022-07-09 06:59:37.000000 lru-dict-1.1.8/lru_dict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-07-09 06:59:37.000000 lru-dict-1.1.8/lru_dict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-09 06:59:37.000000 lru-dict-1.1.8/lru_dict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-09 06:59:37.000000 lru-dict-1.1.8/lru_dict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-09 06:59:37.000000 lru-dict-1.1.8/lru_dict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-09 06:59:37.578906 lru-dict-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-07-09 06:59:30.000000 lru-dict-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 06:59:37.574905 lru-dict-1.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)    11368 2022-07-09 06:59:30.000000 lru-dict-1.1.8/test/test_lru.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:49.876415 lru-dict-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-27 00:55:42.000000 lru-dict-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 00:55:42.000000 lru-dict-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-27 00:55:49.876415 lru-dict-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-27 00:55:42.000000 lru-dict-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23024 2023-05-27 00:55:42.000000 lru-dict-1.2.0/lru.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:49.872415 lru-dict-1.2.0/lru_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-27 00:55:49.000000 lru-dict-1.2.0/lru_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-27 00:55:49.000000 lru-dict-1.2.0/lru_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:55:49.000000 lru-dict-1.2.0/lru_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-27 00:55:49.000000 lru-dict-1.2.0/lru_dict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-27 00:55:49.000000 lru-dict-1.2.0/lru_dict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 00:55:49.876415 lru-dict-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-27 00:55:42.000000 lru-dict-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:55:49.872415 lru-dict-1.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-27 00:55:42.000000 lru-dict-1.2.0/test/test_lru.py
```

### Comparing `lru-dict-1.1.8/LICENSE` & `lru-dict-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lru-dict-1.1.8/PKG-INFO` & `lru-dict-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: lru-dict
-Version: 1.1.8
+Version: 1.2.0
 Summary: An Dict like LRU container.
 Home-page: https://github.com/amitdev/lru-dict
 Author: Amit Dev
 License: MIT
 Keywords: lru,dict
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
-.. image:: https://travis-ci.com/amitdev/lru-dict.svg?branch=master
-    :target: https://travis-ci.com/amitdev/lru-dict
-
 .. image:: https://github.com/amitdev/lru-dict/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/amitdev/lru-dict/actions/workflows/tests.yml
 
 .. image:: https://github.com/amitdev/lru-dict/actions/workflows/build-and-deploy.yml/badge.svg
     :target: https://github.com/amitdev/lru-dict/actions/workflows/build-and-deploy.yml
 
 LRU Dict
```

### Comparing `lru-dict-1.1.8/README.rst` & `lru-dict-1.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-.. image:: https://travis-ci.com/amitdev/lru-dict.svg?branch=master
-    :target: https://travis-ci.com/amitdev/lru-dict
-
 .. image:: https://github.com/amitdev/lru-dict/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/amitdev/lru-dict/actions/workflows/tests.yml
 
 .. image:: https://github.com/amitdev/lru-dict/actions/workflows/build-and-deploy.yml/badge.svg
     :target: https://github.com/amitdev/lru-dict/actions/workflows/build-and-deploy.yml
 
 LRU Dict
```

### Comparing `lru-dict-1.1.8/lru.c` & `lru-dict-1.2.0/lru.c`

 * *Files 0% similar despite different names*

```diff
@@ -622,15 +622,15 @@
                     PyDoc_STR("L.has_key(key) -> Check if key is there in L")},
     {"get",	(PyCFunction)LRU_get, METH_VARARGS,
                     PyDoc_STR("L.get(key, instead) -> If L has key return its value, otherwise instead")},
     {"setdefault", (PyCFunction)LRU_setdefault, METH_VARARGS,
                     PyDoc_STR("L.setdefault(key, default=None) -> If L has key return its value, otherwise insert key with a value of default and return default")},
     {"pop", (PyCFunction)LRU_pop, METH_VARARGS,
                     PyDoc_STR("L.pop(key[, default]) -> If L has key return its value and remove it from L, otherwise return default. If default is not given and key is not in L, a KeyError is raised.")},
-    {"popitem", (PyCFunctionWithKeywords)LRU_popitem, METH_VARARGS | METH_KEYWORDS,
+    {"popitem", (PyCFunction)LRU_popitem, METH_VARARGS | METH_KEYWORDS,
                     PyDoc_STR("L.popitem([least_recent=True]) -> Returns and removes a (key, value) pair. The pair returned is the least-recently used if least_recent is true, or the most-recently used if false.")},
     {"set_size", (PyCFunction)LRU_set_size, METH_VARARGS,
                     PyDoc_STR("L.set_size() -> set size of LRU")},
     {"get_size", (PyCFunction)LRU_get_size, METH_NOARGS,
                     PyDoc_STR("L.get_size() -> get size of LRU")},
     {"clear", (PyCFunction)LRU_clear, METH_NOARGS,
                     PyDoc_STR("L.clear() -> clear LRU")},
```

### Comparing `lru-dict-1.1.8/lru_dict.egg-info/PKG-INFO` & `lru-dict-1.2.0/lru_dict.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: lru-dict
-Version: 1.1.8
+Version: 1.2.0
 Summary: An Dict like LRU container.
 Home-page: https://github.com/amitdev/lru-dict
 Author: Amit Dev
 License: MIT
 Keywords: lru,dict
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
-.. image:: https://travis-ci.com/amitdev/lru-dict.svg?branch=master
-    :target: https://travis-ci.com/amitdev/lru-dict
-
 .. image:: https://github.com/amitdev/lru-dict/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/amitdev/lru-dict/actions/workflows/tests.yml
 
 .. image:: https://github.com/amitdev/lru-dict/actions/workflows/build-and-deploy.yml/badge.svg
     :target: https://github.com/amitdev/lru-dict/actions/workflows/build-and-deploy.yml
 
 LRU Dict
```

### Comparing `lru-dict-1.1.8/setup.py` & `lru-dict-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, Extension
 
 module1 = Extension('lru',
                     sources = ['lru.c'])
 
 setup (name = 'lru-dict',
-       version = '1.1.8',
+       version = '1.2.0',
        description = 'An Dict like LRU container.',
        long_description = open('README.rst').read(),
        long_description_content_type="text/x-rst",
        author='Amit Dev',
        url='https://github.com/amitdev/lru-dict',
        license='MIT',
        keywords='lru, dict',
@@ -16,21 +16,20 @@
        classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Operating System :: POSIX',
         'Programming Language :: C',
-        'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Software Development :: Libraries :: Python Modules',
         ],
         extras_require={
             'test': ['pytest'],
         },
 )
```

### Comparing `lru-dict-1.1.8/test/test_lru.py` & `lru-dict-1.2.0/test/test_lru.py`

 * *Files identical despite different names*

