# Comparing `tmp/cachetools-5.3.0.tar.gz` & `tmp/cachetools-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetools-5.3.0.tar", last modified: Sun Jan 22 22:29:41 2023, max compression
+gzip compressed data, was "cachetools-5.3.1.tar", last modified: Sat May 27 20:36:33 2023, max compression
```

## Comparing `cachetools-5.3.0.tar` & `cachetools-5.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-01-22 22:29:41.295361 cachetools-5.3.0/
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     8975 2023-01-22 22:22:32.000000 cachetools-5.3.0/CHANGELOG.rst
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     1085 2022-05-15 20:40:40.000000 cachetools-5.3.0/LICENSE
--rw-rw-r--   0 tkem      (1000) tkem      (1000)      167 2021-12-19 08:48:13.000000 cachetools-5.3.0/MANIFEST.in
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     5187 2023-01-22 22:29:41.295361 cachetools-5.3.0/PKG-INFO
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     4254 2023-01-08 20:40:00.000000 cachetools-5.3.0/README.rst
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-01-22 22:29:41.291361 cachetools-5.3.0/docs/
--rw-rw-r--   0 tkem      (1000) tkem      (1000)        7 2021-09-27 19:32:46.000000 cachetools-5.3.0/docs/.gitignore
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     5580 2021-09-27 19:32:46.000000 cachetools-5.3.0/docs/Makefile
--rw-rw-r--   0 tkem      (1000) tkem      (1000)      418 2023-01-22 22:22:12.000000 cachetools-5.3.0/docs/conf.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)    23214 2023-01-22 22:22:12.000000 cachetools-5.3.0/docs/index.rst
--rw-rw-r--   0 tkem      (1000) tkem      (1000)      100 2021-12-19 08:48:13.000000 cachetools-5.3.0/pyproject.toml
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     1174 2023-01-22 22:29:41.295361 cachetools-5.3.0/setup.cfg
--rw-rw-r--   0 tkem      (1000) tkem      (1000)       38 2021-12-19 08:48:13.000000 cachetools-5.3.0/setup.py
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-01-22 22:29:41.291361 cachetools-5.3.0/src/
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-01-22 22:29:41.291361 cachetools-5.3.0/src/cachetools/
--rw-rw-r--   0 tkem      (1000) tkem      (1000)    24981 2023-01-22 22:22:12.000000 cachetools-5.3.0/src/cachetools/__init__.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     3616 2023-01-22 22:22:12.000000 cachetools-5.3.0/src/cachetools/func.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     1613 2022-05-29 20:40:29.000000 cachetools-5.3.0/src/cachetools/keys.py
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-01-22 22:29:41.291361 cachetools-5.3.0/src/cachetools.egg-info/
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     5187 2023-01-22 22:29:41.000000 cachetools-5.3.0/src/cachetools.egg-info/PKG-INFO
--rw-rw-r--   0 tkem      (1000) tkem      (1000)      620 2023-01-22 22:29:41.000000 cachetools-5.3.0/src/cachetools.egg-info/SOURCES.txt
--rw-rw-r--   0 tkem      (1000) tkem      (1000)        1 2023-01-22 22:29:41.000000 cachetools-5.3.0/src/cachetools.egg-info/dependency_links.txt
--rw-rw-r--   0 tkem      (1000) tkem      (1000)       11 2023-01-22 22:29:41.000000 cachetools-5.3.0/src/cachetools.egg-info/top_level.txt
-drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-01-22 22:29:41.295361 cachetools-5.3.0/tests/
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     9744 2021-12-21 20:17:15.000000 cachetools-5.3.0/tests/__init__.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)      149 2021-12-19 08:48:13.000000 cachetools-5.3.0/tests/test_cache.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     8383 2023-01-22 22:22:12.000000 cachetools-5.3.0/tests/test_cached.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     6975 2022-05-29 20:40:29.000000 cachetools-5.3.0/tests/test_cachedmethod.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     1377 2021-12-19 08:48:13.000000 cachetools-5.3.0/tests/test_fifo.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     5101 2021-12-19 08:48:13.000000 cachetools-5.3.0/tests/test_func.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     2660 2021-12-19 08:48:13.000000 cachetools-5.3.0/tests/test_keys.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     1198 2021-12-19 08:48:13.000000 cachetools-5.3.0/tests/test_lfu.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     1371 2021-12-19 08:48:13.000000 cachetools-5.3.0/tests/test_lru.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     1253 2021-12-19 08:48:13.000000 cachetools-5.3.0/tests/test_mru.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)      832 2021-12-19 08:48:13.000000 cachetools-5.3.0/tests/test_rr.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     7938 2021-12-21 20:17:15.000000 cachetools-5.3.0/tests/test_tlru.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)     5667 2021-12-21 20:17:15.000000 cachetools-5.3.0/tests/test_ttl.py
--rw-rw-r--   0 tkem      (1000) tkem      (1000)      770 2021-12-19 11:39:54.000000 cachetools-5.3.0/tox.ini
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-05-27 20:36:33.982085 cachetools-5.3.1/
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     9045 2023-05-27 20:34:14.000000 cachetools-5.3.1/CHANGELOG.rst
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     1085 2022-05-15 20:40:40.000000 cachetools-5.3.1/LICENSE
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)      167 2021-12-19 08:48:13.000000 cachetools-5.3.1/MANIFEST.in
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     5187 2023-05-27 20:36:33.982085 cachetools-5.3.1/PKG-INFO
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     4254 2023-01-08 20:40:00.000000 cachetools-5.3.1/README.rst
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-05-27 20:36:33.982085 cachetools-5.3.1/docs/
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)        7 2021-09-27 19:32:46.000000 cachetools-5.3.1/docs/.gitignore
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     5580 2021-09-27 19:32:46.000000 cachetools-5.3.1/docs/Makefile
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)      418 2023-01-22 22:22:12.000000 cachetools-5.3.1/docs/conf.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)    23214 2023-01-22 22:22:12.000000 cachetools-5.3.1/docs/index.rst
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)      100 2021-12-19 08:48:13.000000 cachetools-5.3.1/pyproject.toml
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     1174 2023-05-27 20:36:33.982085 cachetools-5.3.1/setup.cfg
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)       38 2021-12-19 08:48:13.000000 cachetools-5.3.1/setup.py
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-05-27 20:36:33.978085 cachetools-5.3.1/src/
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-05-27 20:36:33.982085 cachetools-5.3.1/src/cachetools/
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)    24981 2023-05-27 20:32:14.000000 cachetools-5.3.1/src/cachetools/__init__.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     3616 2023-01-22 22:22:12.000000 cachetools-5.3.1/src/cachetools/func.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     1613 2022-05-29 20:40:29.000000 cachetools-5.3.1/src/cachetools/keys.py
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-05-27 20:36:33.982085 cachetools-5.3.1/src/cachetools.egg-info/
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     5187 2023-05-27 20:36:33.000000 cachetools-5.3.1/src/cachetools.egg-info/PKG-INFO
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)      620 2023-05-27 20:36:33.000000 cachetools-5.3.1/src/cachetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)        1 2023-05-27 20:36:33.000000 cachetools-5.3.1/src/cachetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)       11 2023-05-27 20:36:33.000000 cachetools-5.3.1/src/cachetools.egg-info/top_level.txt
+drwxrwxr-x   0 tkem      (1000) tkem      (1000)        0 2023-05-27 20:36:33.982085 cachetools-5.3.1/tests/
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     9744 2023-03-17 20:55:31.000000 cachetools-5.3.1/tests/__init__.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)      149 2023-03-17 20:55:31.000000 cachetools-5.3.1/tests/test_cache.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     8383 2023-01-22 22:22:12.000000 cachetools-5.3.1/tests/test_cached.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     6975 2022-05-29 20:40:29.000000 cachetools-5.3.1/tests/test_cachedmethod.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     1377 2023-03-17 20:55:31.000000 cachetools-5.3.1/tests/test_fifo.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     5101 2023-03-17 20:55:31.000000 cachetools-5.3.1/tests/test_func.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     2660 2021-12-19 08:48:13.000000 cachetools-5.3.1/tests/test_keys.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     1198 2023-03-17 20:55:31.000000 cachetools-5.3.1/tests/test_lfu.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     1371 2023-03-17 20:55:31.000000 cachetools-5.3.1/tests/test_lru.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     1253 2023-03-17 20:55:31.000000 cachetools-5.3.1/tests/test_mru.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)      832 2023-03-17 20:55:31.000000 cachetools-5.3.1/tests/test_rr.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     7938 2023-03-17 20:55:31.000000 cachetools-5.3.1/tests/test_tlru.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)     5667 2023-03-17 20:55:31.000000 cachetools-5.3.1/tests/test_ttl.py
+-rw-rw-r--   0 tkem      (1000) tkem      (1000)      823 2023-03-17 21:03:01.000000 cachetools-5.3.1/tox.ini
```

### Comparing `cachetools-5.3.0/CHANGELOG.rst` & `cachetools-5.3.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v5.3.1 (2023-05-27)
+===================
+
+- Depend on Python >= 3.7.
+
+
 v5.3.0 (2023-01-22)
 ===================
 
 - Add ``cache_info()`` function to ``@cached`` decorator.
 
 
 v5.2.1 (2023-01-08)
```

### Comparing `cachetools-5.3.0/LICENSE` & `cachetools-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/PKG-INFO` & `cachetools-5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetools
-Version: 5.3.0
+Version: 5.3.1
 Summary: Extensible memoizing collections and decorators
 Home-page: https://github.com/tkem/cachetools/
 Author: Thomas Kemmer
 Author-email: tkemmer@computer.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: ~=3.7
+Requires-Python: >=3.7
 License-File: LICENSE
 
 cachetools
 ========================================================================
 
 .. image:: https://img.shields.io/pypi/v/cachetools
    :target: https://pypi.org/project/cachetools/
```

### Comparing `cachetools-5.3.0/README.rst` & `cachetools-5.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/docs/Makefile` & `cachetools-5.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/docs/index.rst` & `cachetools-5.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/setup.cfg` & `cachetools-5.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = ~= 3.7
+python_requires = >= 3.7
 
 [options.packages.find]
 where = src
 
 [flake8]
 max-line-length = 80
 exclude = .git, .tox, build
```

### Comparing `cachetools-5.3.0/src/cachetools/__init__.py` & `cachetools-5.3.1/src/cachetools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "RRCache",
     "TLRUCache",
     "TTLCache",
     "cached",
     "cachedmethod",
 )
 
-__version__ = "5.3.0"
+__version__ = "5.3.1"
 
 import collections
 import collections.abc
 import functools
 import heapq
 import random
 import time
```

### Comparing `cachetools-5.3.0/src/cachetools/func.py` & `cachetools-5.3.1/src/cachetools/func.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/src/cachetools/keys.py` & `cachetools-5.3.1/src/cachetools/keys.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/src/cachetools.egg-info/PKG-INFO` & `cachetools-5.3.1/src/cachetools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetools
-Version: 5.3.0
+Version: 5.3.1
 Summary: Extensible memoizing collections and decorators
 Home-page: https://github.com/tkem/cachetools/
 Author: Thomas Kemmer
 Author-email: tkemmer@computer.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: ~=3.7
+Requires-Python: >=3.7
 License-File: LICENSE
 
 cachetools
 ========================================================================
 
 .. image:: https://img.shields.io/pypi/v/cachetools
    :target: https://pypi.org/project/cachetools/
```

### Comparing `cachetools-5.3.0/src/cachetools.egg-info/SOURCES.txt` & `cachetools-5.3.1/src/cachetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/__init__.py` & `cachetools-5.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/test_cached.py` & `cachetools-5.3.1/tests/test_cached.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/test_cachedmethod.py` & `cachetools-5.3.1/tests/test_cachedmethod.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/test_fifo.py` & `cachetools-5.3.1/tests/test_fifo.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/test_func.py` & `cachetools-5.3.1/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/test_keys.py` & `cachetools-5.3.1/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/test_lfu.py` & `cachetools-5.3.1/tests/test_lfu.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/test_lru.py` & `cachetools-5.3.1/tests/test_lru.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/test_mru.py` & `cachetools-5.3.1/tests/test_mru.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/test_rr.py` & `cachetools-5.3.1/tests/test_rr.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/test_tlru.py` & `cachetools-5.3.1/tests/test_tlru.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tests/test_ttl.py` & `cachetools-5.3.1/tests/test_ttl.py`

 * *Files identical despite different names*

### Comparing `cachetools-5.3.0/tox.ini` & `cachetools-5.3.1/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -28,12 +28,13 @@
 commands =
      sphinx-build -W -b doctest -d {envtmpdir}/doctrees docs {envtmpdir}/doctest
 
 [testenv:flake8]
 deps =
     flake8
     flake8-black; implementation_name == "cpython"
+    black==22.12.0; implementation_name == "cpython"
     flake8-bugbear
     flake8-import-order
 commands =
     flake8
 skip_install = true
```

