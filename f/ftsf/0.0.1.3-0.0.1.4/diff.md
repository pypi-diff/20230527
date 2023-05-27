# Comparing `tmp/ftsf-0.0.1.3.tar.gz` & `tmp/ftsf-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftsf-0.0.1.3.tar", last modified: Sat May 27 02:31:37 2023, max compression
+gzip compressed data, was "ftsf-0.0.1.4.tar", last modified: Sat May 27 02:33:04 2023, max compression
```

## Comparing `ftsf-0.0.1.3.tar` & `ftsf-0.0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 02:31:37.924658 ftsf-0.0.1.3/
-drwxrwxrwx   0        0        0        0 2023-05-27 02:31:37.899966 ftsf-0.0.1.3/FTSF.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-05-27 02:31:37.000000 ftsf-0.0.1.3/FTSF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-05-27 02:31:37.000000 ftsf-0.0.1.3/FTSF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 02:31:37.000000 ftsf-0.0.1.3/FTSF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-27 02:31:37.000000 ftsf-0.0.1.3/FTSF.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-27 02:31:37.000000 ftsf-0.0.1.3/FTSF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1100 2023-05-26 02:11:38.000000 ftsf-0.0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1120 2023-05-27 02:31:37.923122 ftsf-0.0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-05-26 23:32:26.000000 ftsf-0.0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 02:31:37.916090 ftsf-0.0.1.3/ftsf/
--rw-rw-rw-   0        0        0        0 2023-05-25 02:03:02.000000 ftsf-0.0.1.3/ftsf/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-05-27 01:28:45.000000 ftsf-0.0.1.3/ftsf/backtest.py
--rw-rw-rw-   0        0        0     7484 2023-05-27 02:13:28.000000 ftsf-0.0.1.3/ftsf/evaluation.py
--rw-rw-rw-   0        0        0     7962 2023-05-27 02:00:08.000000 ftsf-0.0.1.3/ftsf/model.py
--rw-rw-rw-   0        0        0     4486 2023-05-26 04:29:45.000000 ftsf-0.0.1.3/ftsf/preprocessing.py
--rw-rw-rw-   0        0        0     1646 2023-05-27 01:35:41.000000 ftsf-0.0.1.3/ftsf/scaler.py
-drwxrwxrwx   0        0        0        0 2023-05-27 02:31:37.921100 ftsf-0.0.1.3/ftsf/tests/
--rw-rw-rw-   0        0        0      629 2023-05-25 02:40:23.000000 ftsf-0.0.1.3/ftsf/tests/test_scaler.py
--rw-rw-rw-   0        0        0     5321 2023-05-27 02:11:47.000000 ftsf-0.0.1.3/ftsf/utils.py
--rw-rw-rw-   0        0        0      812 2023-05-26 06:33:01.000000 ftsf-0.0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 02:31:37.924658 ftsf-0.0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 02:33:04.814004 ftsf-0.0.1.4/
+drwxrwxrwx   0        0        0        0 2023-05-27 02:33:04.794993 ftsf-0.0.1.4/FTSF.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-05-27 02:33:04.000000 ftsf-0.0.1.4/FTSF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-05-27 02:33:04.000000 ftsf-0.0.1.4/FTSF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 02:33:04.000000 ftsf-0.0.1.4/FTSF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-27 02:33:04.000000 ftsf-0.0.1.4/FTSF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-27 02:33:04.000000 ftsf-0.0.1.4/FTSF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1100 2023-05-26 02:11:38.000000 ftsf-0.0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-05-27 02:33:04.812494 ftsf-0.0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-05-26 23:32:26.000000 ftsf-0.0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 02:33:04.807492 ftsf-0.0.1.4/ftsf/
+-rw-rw-rw-   0        0        0        0 2023-05-25 02:03:02.000000 ftsf-0.0.1.4/ftsf/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-05-27 01:28:45.000000 ftsf-0.0.1.4/ftsf/backtest.py
+-rw-rw-rw-   0        0        0     7484 2023-05-27 02:13:28.000000 ftsf-0.0.1.4/ftsf/evaluation.py
+-rw-rw-rw-   0        0        0     7962 2023-05-27 02:00:08.000000 ftsf-0.0.1.4/ftsf/model.py
+-rw-rw-rw-   0        0        0     4486 2023-05-26 04:29:45.000000 ftsf-0.0.1.4/ftsf/preprocessing.py
+-rw-rw-rw-   0        0        0     1646 2023-05-27 01:35:41.000000 ftsf-0.0.1.4/ftsf/scaler.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:33:04.810508 ftsf-0.0.1.4/ftsf/tests/
+-rw-rw-rw-   0        0        0      629 2023-05-25 02:40:23.000000 ftsf-0.0.1.4/ftsf/tests/test_scaler.py
+-rw-rw-rw-   0        0        0     5321 2023-05-27 02:11:47.000000 ftsf-0.0.1.4/ftsf/utils.py
+-rw-rw-rw-   0        0        0      812 2023-05-27 02:32:39.000000 ftsf-0.0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 02:33:04.815520 ftsf-0.0.1.4/setup.cfg
```

### Comparing `ftsf-0.0.1.3/FTSF.egg-info/PKG-INFO` & `ftsf-0.0.1.4/FTSF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftsf
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: Package for financial time series forecasting.
 Author-email: Nikita Safonov <sixxio@yandex.ru>
 Project-URL: Homepage, https://github.com/sixxio/ftsf
 Project-URL: Documentation, https://sixxio.github.io/ftsf/
 Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ftsf-0.0.1.3/LICENSE` & `ftsf-0.0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.1.3/PKG-INFO` & `ftsf-0.0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftsf
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: Package for financial time series forecasting.
 Author-email: Nikita Safonov <sixxio@yandex.ru>
 Project-URL: Homepage, https://github.com/sixxio/ftsf
 Project-URL: Documentation, https://sixxio.github.io/ftsf/
 Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ftsf-0.0.1.3/ftsf/backtest.py` & `ftsf-0.0.1.4/ftsf/backtest.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.1.3/ftsf/evaluation.py` & `ftsf-0.0.1.4/ftsf/evaluation.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.1.3/ftsf/model.py` & `ftsf-0.0.1.4/ftsf/model.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.1.3/ftsf/preprocessing.py` & `ftsf-0.0.1.4/ftsf/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.1.3/ftsf/scaler.py` & `ftsf-0.0.1.4/ftsf/scaler.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.1.3/ftsf/tests/test_scaler.py` & `ftsf-0.0.1.4/ftsf/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.1.3/ftsf/utils.py` & `ftsf-0.0.1.4/ftsf/utils.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.1.3/pyproject.toml` & `ftsf-0.0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ftsf"
-version = "0.0.1.3"
+version = "0.0.1.4"
 authors = [{ name="Nikita Safonov", email="sixxio@yandex.ru" }]
 description = "Package for financial time series forecasting."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
```

