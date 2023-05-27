# Comparing `tmp/dare_datasets-0.1.5.tar.gz` & `tmp/dare_datasets-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dare_datasets-0.1.5.tar", max compression
+gzip compressed data, was "dare_datasets-0.1.6.tar", max compression
```

## Comparing `dare_datasets-0.1.5.tar` & `dare_datasets-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      178 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/dare_datasets/__init__.py
--rw-r--r--   0        0        0     2310 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/dare_datasets/dataset_abc.py
--rw-r--r--   0        0        0     1427 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/dare_datasets/qr2t_benchmark.py
--rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/dare_datasets/utils/__init__.py
--rw-r--r--   0        0        0      459 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/dare_datasets/utils/downloader.py
--rw-r--r--   0        0        0      588 2023-05-27 09:22:09.076489 dare_datasets-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 dare_datasets-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      178 2023-05-27 09:16:11.245474 dare_datasets-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.6/dare_datasets/__init__.py
+-rw-r--r--   0        0        0     2310 2023-05-27 09:16:11.245474 dare_datasets-0.1.6/dare_datasets/dataset_abc.py
+-rw-r--r--   0        0        0     1427 2023-05-27 09:16:11.245474 dare_datasets-0.1.6/dare_datasets/qr2t_benchmark.py
+-rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.6/dare_datasets/utils/__init__.py
+-rw-r--r--   0        0        0      459 2023-05-27 09:16:11.245474 dare_datasets-0.1.6/dare_datasets/utils/downloader.py
+-rw-r--r--   0        0        0      795 2023-05-27 16:26:39.896449 dare_datasets-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 dare_datasets-0.1.6/PKG-INFO
```

### Comparing `dare_datasets-0.1.5/dare_datasets/dataset_abc.py` & `dare_datasets-0.1.6/dare_datasets/dataset_abc.py`

 * *Files identical despite different names*

### Comparing `dare_datasets-0.1.5/dare_datasets/qr2t_benchmark.py` & `dare_datasets-0.1.6/dare_datasets/qr2t_benchmark.py`

 * *Files identical despite different names*

### Comparing `dare_datasets-0.1.5/PKG-INFO` & `dare_datasets-0.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: dare-datasets
-Version: 0.1.5
+Version: 0.1.6
 Summary: A quick and easy way to download datasets from the DARE lab.
 Author: MikeXydas
 Author-email: mikexydas@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gdown (>=4.7.1,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Darelab Datasets
```

