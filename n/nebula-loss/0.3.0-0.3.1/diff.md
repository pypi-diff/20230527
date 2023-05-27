# Comparing `tmp/nebula-loss-0.3.0.tar.gz` & `tmp/nebula-loss-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nebula-loss-0.3.0.tar", last modified: Sat May  6 01:55:46 2023, max compression
+gzip compressed data, was "nebula-loss-0.3.1.tar", last modified: Sat May 27 06:37:23 2023, max compression
```

## Comparing `nebula-loss-0.3.0.tar` & `nebula-loss-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:55:46.210139 nebula-loss-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-06 01:55:28.000000 nebula-loss-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-06 01:55:46.210139 nebula-loss-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-06 01:55:28.000000 nebula-loss-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:55:46.210139 nebula-loss-0.3.0/nebula_loss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-06 01:55:46.000000 nebula-loss-0.3.0/nebula_loss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-06 01:55:46.000000 nebula-loss-0.3.0/nebula_loss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:55:46.000000 nebula-loss-0.3.0/nebula_loss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 01:55:46.000000 nebula-loss-0.3.0/nebula_loss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:55:46.000000 nebula-loss-0.3.0/nebula_loss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:55:46.210139 nebula-loss-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-06 01:55:28.000000 nebula-loss-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:37:23.151839 nebula-loss-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-27 06:37:10.000000 nebula-loss-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-27 06:37:23.151839 nebula-loss-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-27 06:37:10.000000 nebula-loss-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:37:23.151839 nebula-loss-0.3.1/nebula/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 06:37:10.000000 nebula-loss-0.3.1/nebula/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-27 06:37:10.000000 nebula-loss-0.3.1/nebula/nebulav2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:37:23.151839 nebula-loss-0.3.1/nebula_loss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-27 06:37:23.000000 nebula-loss-0.3.1/nebula_loss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-27 06:37:23.000000 nebula-loss-0.3.1/nebula_loss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:37:23.000000 nebula-loss-0.3.1/nebula_loss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 06:37:23.000000 nebula-loss-0.3.1/nebula_loss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 06:37:23.000000 nebula-loss-0.3.1/nebula_loss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 06:37:23.151839 nebula-loss-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-27 06:37:10.000000 nebula-loss-0.3.1/setup.py
```

### Comparing `nebula-loss-0.3.0/LICENSE` & `nebula-loss-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebula-loss-0.3.0/PKG-INFO` & `nebula-loss-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebula-loss
-Version: 0.3.0
+Version: 0.3.1
 Summary: 1 Loss Function to rule them all!
 Home-page: https://github.com/kyegomez/nebula
 Author: Agora
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,jax,loss ffunction,Multi-Modality AI
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nebula-loss-0.3.0/README.md` & `nebula-loss-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,23 @@
 ### Requirements
 - Python 3.7 or higher
 - PyTorch 1.9 or higher
 - NumPy
 
 ### Installation
 ```sh
-pip install nebula
+pip install nebula-loss'
 ```
 
 ### Usage
 
 ```python
 import torch
 from nebula_loss import Nebula
+from nebula_loss.nebulav3 import Nebula
 
 # Instantiate the Nebula loss function
 loss_function = Nebula()
 
 # Define your model, dataset, and other components here
 
 # Calculate loss using the Nebula loss function
```

### Comparing `nebula-loss-0.3.0/nebula_loss.egg-info/PKG-INFO` & `nebula-loss-0.3.1/nebula_loss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebula-loss
-Version: 0.3.0
+Version: 0.3.1
 Summary: 1 Loss Function to rule them all!
 Home-page: https://github.com/kyegomez/nebula
 Author: Agora
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,jax,loss ffunction,Multi-Modality AI
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nebula-loss-0.3.0/setup.py` & `nebula-loss-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'nebula-loss',
   packages = find_packages(exclude=[]),
-  version = '0.3.0',
+  version = '0.3.1',
   license='MIT',
   description = '1 Loss Function to rule them all!',
   author = 'Agora',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/nebula',
   keywords = [
```

