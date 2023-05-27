# Comparing `tmp/dare_datasets-0.1.3.tar.gz` & `tmp/dare_datasets-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dare_datasets-0.1.3.tar", max compression
+gzip compressed data, was "dare_datasets-0.1.4.tar", max compression
```

## Comparing `dare_datasets-0.1.3.tar` & `dare_datasets-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      178 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/dare_datasets/__init__.py
--rw-r--r--   0        0        0     2310 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/dare_datasets/dataset_abc.py
--rw-r--r--   0        0        0     1427 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/dare_datasets/qr2t_benchmark.py
--rw-r--r--   0        0        0        0 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/dare_datasets/utils/__init__.py
--rw-r--r--   0        0        0      459 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/dare_datasets/utils/downloader.py
--rw-r--r--   0        0        0      528 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 dare_datasets-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      178 2023-05-27 09:16:11.245474 dare_datasets-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.4/dare_datasets/__init__.py
+-rw-r--r--   0        0        0     2310 2023-05-27 09:16:11.245474 dare_datasets-0.1.4/dare_datasets/dataset_abc.py
+-rw-r--r--   0        0        0     1427 2023-05-27 09:16:11.245474 dare_datasets-0.1.4/dare_datasets/qr2t_benchmark.py
+-rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.4/dare_datasets/utils/__init__.py
+-rw-r--r--   0        0        0      459 2023-05-27 09:16:11.245474 dare_datasets-0.1.4/dare_datasets/utils/downloader.py
+-rw-r--r--   0        0        0      528 2023-05-27 09:16:11.305473 dare_datasets-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 dare_datasets-0.1.4/PKG-INFO
```

### Comparing `dare_datasets-0.1.3/dare_datasets/dataset_abc.py` & `dare_datasets-0.1.4/dare_datasets/dataset_abc.py`

 * *Files identical despite different names*

### Comparing `dare_datasets-0.1.3/dare_datasets/qr2t_benchmark.py` & `dare_datasets-0.1.4/dare_datasets/qr2t_benchmark.py`

 * *Files identical despite different names*

### Comparing `dare_datasets-0.1.3/pyproject.toml` & `dare_datasets-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dare-datasets"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["MikeXydas <mikexydas@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dare_datasets"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dare_datasets-0.1.3/PKG-INFO` & `dare_datasets-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dare-datasets
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: MikeXydas
 Author-email: mikexydas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gdown (>=4.7.1,<5.0.0)
```

