# Comparing `tmp/gpt_json-0.1.8.tar.gz` & `tmp/gpt_json-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_json-0.1.8.tar", max compression
+gzip compressed data, was "gpt_json-0.1.9.tar", max compression
```

## Comparing `gpt_json-0.1.8.tar` & `gpt_json-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-05-19 18:17:05.455002 gpt_json-0.1.8/LICENSE
--rw-r--r--   0        0        0     8963 2023-05-19 18:17:05.455002 gpt_json-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/enums.py
--rw-r--r--   0        0        0      135 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/exceptions.py
--rw-r--r--   0        0        0    11997 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/gpt.py
--rw-r--r--   0        0        0      783 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/models.py
--rw-r--r--   0        0        0     1535 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/parsers.py
--rw-r--r--   0        0        0     2005 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/prompts.py
--rw-r--r--   0        0        0        0 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/__init__.py
--rw-r--r--   0        0        0      355 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/conftest.py
--rw-r--r--   0        0        0      256 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/shared.py
--rw-r--r--   0        0        0      292 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_fixtures.py
--rw-r--r--   0        0        0     8987 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_gpt.py
--rw-r--r--   0        0        0      830 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_models.py
--rw-r--r--   0        0        0     1273 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_parsers.py
--rw-r--r--   0        0        0     1208 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_prompts.py
--rw-r--r--   0        0        0     4078 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/tests/test_transformations.py
--rw-r--r--   0        0        0     2822 2023-05-19 18:17:05.455002 gpt_json-0.1.8/gpt_json/transformations.py
--rw-r--r--   0        0        0      628 2023-05-19 18:17:05.459003 gpt_json-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     9515 1970-01-01 00:00:00.000000 gpt_json-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-19 18:58:38.927164 gpt_json-0.1.9/LICENSE
+-rw-r--r--   0        0        0     8963 2023-05-19 18:58:38.927164 gpt_json-0.1.9/README.md
+-rw-r--r--   0        0        0       79 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/enums.py
+-rw-r--r--   0        0        0      135 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/exceptions.py
+-rw-r--r--   0        0        0    11997 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/gpt.py
+-rw-r--r--   0        0        0      783 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/models.py
+-rw-r--r--   0        0        0     1535 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/parsers.py
+-rw-r--r--   0        0        0     2005 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/prompts.py
+-rw-r--r--   0        0        0        0 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/__init__.py
+-rw-r--r--   0        0        0      355 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/conftest.py
+-rw-r--r--   0        0        0      256 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/shared.py
+-rw-r--r--   0        0        0      381 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_api.py
+-rw-r--r--   0        0        0      292 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_fixtures.py
+-rw-r--r--   0        0        0     8987 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_gpt.py
+-rw-r--r--   0        0        0      830 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_models.py
+-rw-r--r--   0        0        0     1273 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_parsers.py
+-rw-r--r--   0        0        0     1208 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_prompts.py
+-rw-r--r--   0        0        0     4078 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/tests/test_transformations.py
+-rw-r--r--   0        0        0     2822 2023-05-19 18:58:38.931164 gpt_json-0.1.9/gpt_json/transformations.py
+-rw-r--r--   0        0        0      628 2023-05-19 18:58:38.935164 gpt_json-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     9515 1970-01-01 00:00:00.000000 gpt_json-0.1.9/PKG-INFO
```

### Comparing `gpt_json-0.1.8/LICENSE` & `gpt_json-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/README.md` & `gpt_json-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/gpt_json/gpt.py` & `gpt_json-0.1.9/gpt_json/gpt.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/gpt_json/models.py` & `gpt_json-0.1.9/gpt_json/models.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/gpt_json/parsers.py` & `gpt_json-0.1.9/gpt_json/parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/gpt_json/prompts.py` & `gpt_json-0.1.9/gpt_json/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/gpt_json/tests/test_gpt.py` & `gpt_json-0.1.9/gpt_json/tests/test_gpt.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/gpt_json/tests/test_models.py` & `gpt_json-0.1.9/gpt_json/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/gpt_json/tests/test_parsers.py` & `gpt_json-0.1.9/gpt_json/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/gpt_json/tests/test_prompts.py` & `gpt_json-0.1.9/gpt_json/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/gpt_json/tests/test_transformations.py` & `gpt_json-0.1.9/gpt_json/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/gpt_json/transformations.py` & `gpt_json-0.1.9/gpt_json/transformations.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.8/PKG-INFO` & `gpt_json-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-json
-Version: 0.1.8
+Version: 0.1.9
 Summary: Structured and typehinted GPT responses in Python.
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

