# Comparing `tmp/optimus-prime-transformers-1.1.3.tar.gz` & `tmp/optimus-prime-transformers-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimus-prime-transformers-1.1.3.tar", last modified: Thu May 25 03:49:10 2023, max compression
+gzip compressed data, was "optimus-prime-transformers-1.1.4.tar", last modified: Sat May 27 05:49:51 2023, max compression
```

## Comparing `optimus-prime-transformers-1.1.3.tar` & `optimus-prime-transformers-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:49:10.071202 optimus-prime-transformers-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 03:49:10.067202 optimus-prime-transformers-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    63442 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:49:10.067202 optimus-prime-transformers-1.1.3/optimus_prime/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/continuous_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/nonautoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/x_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/optimus_prime/xl_autoregressive_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:49:10.067202 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 03:49:10.000000 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-25 03:49:10.000000 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:49:10.000000 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 03:49:10.000000 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 03:49:10.000000 optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 03:49:10.071202 optimus-prime-transformers-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-25 03:48:59.000000 optimus-prime-transformers-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:49:51.056208 optimus-prime-transformers-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-27 05:49:51.056208 optimus-prime-transformers-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    63442 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:49:51.056208 optimus-prime-transformers-1.1.4/optimus_prime/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/continuous_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/nonautoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/x_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/xl_autoregressive_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:49:51.056208 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-27 05:49:51.000000 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-27 05:49:51.000000 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 05:49:51.000000 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 05:49:51.000000 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-27 05:49:51.000000 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 05:49:51.056208 optimus-prime-transformers-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/setup.py
```

### Comparing `optimus-prime-transformers-1.1.3/LICENSE` & `optimus-prime-transformers-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.3/PKG-INFO` & `optimus-prime-transformers-1.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.3
+Version: 1.1.4
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.3/README.md` & `optimus-prime-transformers-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.3/optimus_prime/__init__.py` & `optimus-prime-transformers-1.1.4/optimus_prime/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 from packaging import version
 
 if version.parse(torch.__version__) >= version.parse('2.0.0'):
     from einops._torch_specific import allow_ops_in_compiled_graph
     allow_ops_in_compiled_graph()
 
 from optimus_prime.x_transformers import XTransformer, Encoder, Decoder, CrossAttender, Attention, TransformerWrapper, ViTransformerWrapper, ContinuousTransformerWrapper
-
+#d
 from optimus_prime.autoregressive_wrapper import AutoregressiveWrapper
 from optimus_prime.nonautoregressive_wrapper import NonAutoregressiveWrapper
 from optimus_prime.continuous_autoregressive_wrapper import ContinuousAutoregressiveWrapper
 from optimus_prime.xl_autoregressive_wrapper import XLAutoregressiveWrapper
```

### Comparing `optimus-prime-transformers-1.1.3/optimus_prime/attend.py` & `optimus-prime-transformers-1.1.4/optimus_prime/attend.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.3/optimus_prime/autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.4/optimus_prime/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.3/optimus_prime/continuous_autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.4/optimus_prime/continuous_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.3/optimus_prime/nonautoregressive_wrapper.py` & `optimus-prime-transformers-1.1.4/optimus_prime/nonautoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.3/optimus_prime/x_transformers.py` & `optimus-prime-transformers-1.1.4/optimus_prime/x_transformers.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.3/optimus_prime/xl_autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.4/optimus_prime/xl_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/PKG-INFO` & `optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.3
+Version: 1.1.4
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.3/optimus_prime_transformers.egg-info/SOURCES.txt` & `optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.3/setup.py` & `optimus-prime-transformers-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'optimus-prime-transformers',
   packages = find_packages(exclude=['examples']),
-  version = '1.1.3',
+  version = '1.1.4',
   license='MIT',
   description = 'optimus-prime - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/Optimus-Prime',
   long_description_content_type = 'text/markdown',
   keywords = [
```

