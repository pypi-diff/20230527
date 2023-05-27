# Comparing `tmp/optimus-prime-transformers-1.1.4.tar.gz` & `tmp/optimus-prime-transformers-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimus-prime-transformers-1.1.4.tar", last modified: Sat May 27 05:49:51 2023, max compression
+gzip compressed data, was "optimus-prime-transformers-1.1.5.tar", last modified: Sat May 27 08:35:10 2023, max compression
```

## Comparing `optimus-prime-transformers-1.1.4.tar` & `optimus-prime-transformers-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:49:51.056208 optimus-prime-transformers-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-27 05:49:51.056208 optimus-prime-transformers-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    63442 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:49:51.056208 optimus-prime-transformers-1.1.4/optimus_prime/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/continuous_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/nonautoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/x_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/optimus_prime/xl_autoregressive_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:49:51.056208 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-27 05:49:51.000000 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-27 05:49:51.000000 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 05:49:51.000000 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 05:49:51.000000 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-27 05:49:51.000000 optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 05:49:51.056208 optimus-prime-transformers-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-27 05:49:36.000000 optimus-prime-transformers-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:35:10.965114 optimus-prime-transformers-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-27 08:35:10.965114 optimus-prime-transformers-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    63442 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:35:10.965114 optimus-prime-transformers-1.1.5/optimus_prime_transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/continuous_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/nonautoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54747 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/x_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/xl_autoregressive_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:35:10.965114 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-27 08:35:10.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-27 08:35:10.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:35:10.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 08:35:10.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 08:35:10.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:35:10.965114 optimus-prime-transformers-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/setup.py
```

### Comparing `optimus-prime-transformers-1.1.4/LICENSE` & `optimus-prime-transformers-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.4/PKG-INFO` & `optimus-prime-transformers-1.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.4
+Version: 1.1.5
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.4/README.md` & `optimus-prime-transformers-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.4/optimus_prime/attend.py` & `optimus-prime-transformers-1.1.5/optimus_prime_transformers/attend.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.4/optimus_prime/autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.5/optimus_prime_transformers/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.4/optimus_prime/continuous_autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.5/optimus_prime_transformers/continuous_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.4/optimus_prime/nonautoregressive_wrapper.py` & `optimus-prime-transformers-1.1.5/optimus_prime_transformers/nonautoregressive_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 
 from einops import rearrange, repeat, pack, unpack
 
-from optimus_prime.optimus_prime import TransformerWrapper
+# from optimus_prime_transformers.optimus_prime import TransformerWrapper
+from x_transformers import TransformerWrapper
 from typing import Optional
 
 # constants
 
 Losses = namedtuple('Losses', ['loss', 'generator_loss', 'critic_loss'])
 
 # helper functions
```

### Comparing `optimus-prime-transformers-1.1.4/optimus_prime/x_transformers.py` & `optimus-prime-transformers-1.1.5/optimus_prime_transformers/x_transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from collections import namedtuple
 from dataclasses import dataclass
 from typing import List
 
 from einops import rearrange, repeat, reduce
 from einops.layers.torch import Rearrange
 
-from optimus_prime.attend import Attend, Intermediates
-from optimus_prime.autoregressive_wrapper import AutoregressiveWrapper
+from optimus_prime_transformers.attend import Attend, Intermediates
+from optimus_prime_transformers.autoregressive_wrapper import AutoregressiveWrapper
 
 from abc import ABC, abstractmethod
 
 # constants
 
 DEFAULT_DIM_HEAD = 64
```

### Comparing `optimus-prime-transformers-1.1.4/optimus_prime/xl_autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.5/optimus_prime_transformers/xl_autoregressive_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from math import ceil
 
 import torch
 from torch import nn
 import torch.nn.functional as F
 
 from einops import rearrange, pack, unpack
-from optimus_prime.autoregressive_wrapper import top_p, top_k, eval_decorator
+from optimus_prime_transformers.autoregressive_wrapper import top_p, top_k, eval_decorator
 
 # helper functions
 
 def exists(val):
     return val is not None
 
 def divisible_by(numer, denom):
```

### Comparing `optimus-prime-transformers-1.1.4/optimus_prime_transformers.egg-info/PKG-INFO` & `optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.4
+Version: 1.1.5
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.4/setup.py` & `optimus-prime-transformers-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'optimus-prime-transformers',
   packages = find_packages(exclude=['examples']),
-  version = '1.1.4',
+  version = '1.1.5',
   license='MIT',
   description = 'optimus-prime - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/Optimus-Prime',
   long_description_content_type = 'text/markdown',
   keywords = [
```

