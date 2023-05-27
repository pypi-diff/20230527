# Comparing `tmp/jupyter-converter-0.0.1.tar.gz` & `tmp/jupyter-converter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-converter-0.0.1.tar", last modified: Sat May 27 19:35:32 2023, max compression
+gzip compressed data, was "jupyter-converter-0.0.2.tar", last modified: Sat May 27 19:44:45 2023, max compression
```

## Comparing `jupyter-converter-0.0.1.tar` & `jupyter-converter-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 teddy      (501) staff       (20)        0 2023-05-27 19:35:32.812689 jupyter-converter-0.0.1/
--rw-r--r--   0 teddy      (501) staff       (20)      518 2023-05-27 19:35:32.812597 jupyter-converter-0.0.1/PKG-INFO
-drwxr-xr-x   0 teddy      (501) staff       (20)        0 2023-05-27 19:35:32.811693 jupyter-converter-0.0.1/jupyter-converter/
--rw-r--r--   0 teddy      (501) staff       (20)       21 2023-05-27 19:33:50.000000 jupyter-converter-0.0.1/jupyter-converter/__init__.py
--rw-------   0 teddy      (501) staff       (20)     8663 2023-05-27 19:29:12.000000 jupyter-converter-0.0.1/jupyter-converter/cells.py
--rw-------   0 teddy      (501) staff       (20)     3400 2023-05-27 19:29:17.000000 jupyter-converter-0.0.1/jupyter-converter/converter.py
-drwxr-xr-x   0 teddy      (501) staff       (20)        0 2023-05-27 19:35:32.812466 jupyter-converter-0.0.1/jupyter_converter.egg-info/
--rw-r--r--   0 teddy      (501) staff       (20)      518 2023-05-27 19:35:32.000000 jupyter-converter-0.0.1/jupyter_converter.egg-info/PKG-INFO
--rw-r--r--   0 teddy      (501) staff       (20)      340 2023-05-27 19:35:32.000000 jupyter-converter-0.0.1/jupyter_converter.egg-info/SOURCES.txt
--rw-r--r--   0 teddy      (501) staff       (20)        1 2023-05-27 19:35:32.000000 jupyter-converter-0.0.1/jupyter_converter.egg-info/dependency_links.txt
--rw-r--r--   0 teddy      (501) staff       (20)        1 2023-05-27 19:35:32.000000 jupyter-converter-0.0.1/jupyter_converter.egg-info/not-zip-safe
--rw-r--r--   0 teddy      (501) staff       (20)       12 2023-05-27 19:35:32.000000 jupyter-converter-0.0.1/jupyter_converter.egg-info/requires.txt
--rw-r--r--   0 teddy      (501) staff       (20)       18 2023-05-27 19:35:32.000000 jupyter-converter-0.0.1/jupyter_converter.egg-info/top_level.txt
--rw-r--r--   0 teddy      (501) staff       (20)       38 2023-05-27 19:35:32.812717 jupyter-converter-0.0.1/setup.cfg
--rw-r--r--   0 teddy      (501) staff       (20)      749 2023-05-27 19:35:26.000000 jupyter-converter-0.0.1/setup.py
+drwxr-xr-x   0 teddy      (501) staff       (20)        0 2023-05-27 19:44:45.761101 jupyter-converter-0.0.2/
+-rw-r--r--   0 teddy      (501) staff       (20)      518 2023-05-27 19:44:45.761005 jupyter-converter-0.0.2/PKG-INFO
+drwxr-xr-x   0 teddy      (501) staff       (20)        0 2023-05-27 19:44:45.759968 jupyter-converter-0.0.2/jupyter_converter/
+-rw-r--r--   0 teddy      (501) staff       (20)       21 2023-05-27 19:44:37.000000 jupyter-converter-0.0.2/jupyter_converter/__init__.py
+-rw-------   0 teddy      (501) staff       (20)     8663 2023-05-27 19:29:12.000000 jupyter-converter-0.0.2/jupyter_converter/cells.py
+-rw-------   0 teddy      (501) staff       (20)     3400 2023-05-27 19:29:17.000000 jupyter-converter-0.0.2/jupyter_converter/converter.py
+drwxr-xr-x   0 teddy      (501) staff       (20)        0 2023-05-27 19:44:45.760872 jupyter-converter-0.0.2/jupyter_converter.egg-info/
+-rw-r--r--   0 teddy      (501) staff       (20)      518 2023-05-27 19:44:45.000000 jupyter-converter-0.0.2/jupyter_converter.egg-info/PKG-INFO
+-rw-r--r--   0 teddy      (501) staff       (20)      340 2023-05-27 19:44:45.000000 jupyter-converter-0.0.2/jupyter_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 teddy      (501) staff       (20)        1 2023-05-27 19:44:45.000000 jupyter-converter-0.0.2/jupyter_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 teddy      (501) staff       (20)        1 2023-05-27 19:35:32.000000 jupyter-converter-0.0.2/jupyter_converter.egg-info/not-zip-safe
+-rw-r--r--   0 teddy      (501) staff       (20)       12 2023-05-27 19:44:45.000000 jupyter-converter-0.0.2/jupyter_converter.egg-info/requires.txt
+-rw-r--r--   0 teddy      (501) staff       (20)       18 2023-05-27 19:44:45.000000 jupyter-converter-0.0.2/jupyter_converter.egg-info/top_level.txt
+-rw-r--r--   0 teddy      (501) staff       (20)       38 2023-05-27 19:44:45.761132 jupyter-converter-0.0.2/setup.cfg
+-rw-r--r--   0 teddy      (501) staff       (20)      750 2023-05-27 19:44:32.000000 jupyter-converter-0.0.2/setup.py
```

### Comparing `jupyter-converter-0.0.1/PKG-INFO` & `jupyter-converter-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-converter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Jupyter Notebook exam generator written by TeddyNote
 Home-page: https://github.com/teddylee777
 Author: teddylee777
 Author-email: teddylee777@gmail.com
 Keywords: teddynote,teddylee777,jupyter notebook converter,exam generator
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `jupyter-converter-0.0.1/jupyter-converter/cells.py` & `jupyter-converter-0.0.2/jupyter_converter/cells.py`

 * *Files identical despite different names*

### Comparing `jupyter-converter-0.0.1/jupyter-converter/converter.py` & `jupyter-converter-0.0.2/jupyter_converter/converter.py`

 * *Files identical despite different names*

### Comparing `jupyter-converter-0.0.1/jupyter_converter.egg-info/PKG-INFO` & `jupyter-converter-0.0.2/jupyter_converter.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-converter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Jupyter Notebook exam generator written by TeddyNote
 Home-page: https://github.com/teddylee777
 Author: teddylee777
 Author-email: teddylee777@gmail.com
 Keywords: teddynote,teddylee777,jupyter notebook converter,exam generator
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `jupyter-converter-0.0.1/setup.py` & `jupyter-converter-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup, find_packages
 
+
 setup(
     name='jupyter-converter',
-    version='0.0.1',
+    version='0.0.2',
     description='Jupyter Notebook exam generator written by TeddyNote',
     author='teddylee777',
     author_email='teddylee777@gmail.com',
     url='https://github.com/teddylee777',
     install_requires=['json', 'codecs'],
     packages=find_packages(exclude=[]),
     keywords=['teddynote', 'teddylee777', 'jupyter notebook converter', 'exam generator'],
```

