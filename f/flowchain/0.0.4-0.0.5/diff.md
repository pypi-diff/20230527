# Comparing `tmp/flowchain-0.0.4.tar.gz` & `tmp/flowchain-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchain-0.0.4.tar", last modified: Fri May 26 18:02:20 2023, max compression
+gzip compressed data, was "flowchain-0.0.5.tar", last modified: Sat May 27 09:17:04 2023, max compression
```

## Comparing `flowchain-0.0.4.tar` & `flowchain-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:02:20.126978 flowchain-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 18:02:09.000000 flowchain-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-26 18:02:20.126978 flowchain-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-26 18:02:09.000000 flowchain-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:02:20.126978 flowchain-0.0.4/flowchain/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 18:02:09.000000 flowchain-0.0.4/flowchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-26 18:02:09.000000 flowchain-0.0.4/flowchain/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:02:20.126978 flowchain-0.0.4/flowchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-26 18:02:20.000000 flowchain-0.0.4/flowchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 18:02:20.000000 flowchain-0.0.4/flowchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:02:20.000000 flowchain-0.0.4/flowchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 18:02:20.000000 flowchain-0.0.4/flowchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 18:02:20.126978 flowchain-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-26 18:02:09.000000 flowchain-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:17:04.593980 flowchain-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 09:16:51.000000 flowchain-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-27 09:17:04.593980 flowchain-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-27 09:16:51.000000 flowchain-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:17:04.593980 flowchain-0.0.5/flowchain/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 09:16:51.000000 flowchain-0.0.5/flowchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-27 09:16:51.000000 flowchain-0.0.5/flowchain/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:17:04.593980 flowchain-0.0.5/flowchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-27 09:17:04.000000 flowchain-0.0.5/flowchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-27 09:17:04.000000 flowchain-0.0.5/flowchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:17:04.000000 flowchain-0.0.5/flowchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 09:17:04.000000 flowchain-0.0.5/flowchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:17:04.593980 flowchain-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-27 09:16:51.000000 flowchain-0.0.5/setup.py
```

### Comparing `flowchain-0.0.4/LICENSE` & `flowchain-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchain-0.0.4/PKG-INFO` & `flowchain-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchain
-Version: 0.0.4
+Version: 0.0.5
 Summary: Flowchain - Method Chaining for TensorFlow
 Home-page: https://github.com/OrigamiDream/flowchain
 Author: OrigamiDream
 Author-email: hello@origamidream.me
 License: MIT
 Keywords: machine learning,deep learning,tensorflow,method chaining,extension
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flowchain-0.0.4/README.md` & `flowchain-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `flowchain-0.0.4/flowchain/chain.py` & `flowchain-0.0.5/flowchain/chain.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,27 +53,31 @@
 
 
 def _retrieve_tf_func(obj: Any = tf, module_whitelist: Optional[List[str]] = None):
     def _tf_func_wrap(fn: Callable) -> Callable:
         def _invoke(*args, **kwargs):
             return fn(*args, **kwargs)
 
+        def _replace_parameter_to_self(signature: inspect.Signature):
+            parameters = signature.parameters
+            self_param = inspect.Parameter('self', kind=inspect.Parameter.POSITIONAL_OR_KEYWORD)
+            return signature.replace(parameters=(self_param,) + tuple(parameters.values())[1:])
+
         _invoke.__doc__ = fn.__doc__
         _invoke.__name__ = fn.__name__
-        _invoke.__signature__ = inspect.signature(fn)
+        _invoke.__signature__ = _replace_parameter_to_self(inspect.signature(fn))
+        _invoke.__qualname__ = fn.__qualname__
         return _invoke
 
     tf_funcs = getmembers(obj, isfunction)
     funcs = dict()
     for name, func in tf_funcs:
         if not _is_allowed(func, name, module_whitelist):
             continue
-
-        signature = inspect.signature(func)
-        if len(signature.parameters) == 0:
+        if len(inspect.signature(func).parameters) == 0:
             continue
         funcs[name] = _tf_func_wrap(func)
     return funcs
 
 
 def register_tensor_chaining(obj, mappings=None):
     global _TENSOR_FN_CACHE
```

### Comparing `flowchain-0.0.4/flowchain.egg-info/PKG-INFO` & `flowchain-0.0.5/flowchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchain
-Version: 0.0.4
+Version: 0.0.5
 Summary: Flowchain - Method Chaining for TensorFlow
 Home-page: https://github.com/OrigamiDream/flowchain
 Author: OrigamiDream
 Author-email: hello@origamidream.me
 License: MIT
 Keywords: machine learning,deep learning,tensorflow,method chaining,extension
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flowchain-0.0.4/setup.py` & `flowchain-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flowchain',
     packages=find_packages(exclude=[]),
-    version='0.0.4',
+    version='0.0.5',
     license='MIT',
     description='Flowchain - Method Chaining for TensorFlow',
     author='OrigamiDream',
     author_email='hello@origamidream.me',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/OrigamiDream/flowchain',
```

