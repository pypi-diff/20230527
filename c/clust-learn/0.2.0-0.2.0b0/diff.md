# Comparing `tmp/clust-learn-0.2.0.tar.gz` & `tmp/clust-learn-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clust-learn-0.2.0.tar", last modified: Sat May 27 06:35:50 2023, max compression
+gzip compressed data, was "clust-learn-0.2.0b0.tar", last modified: Sat May 27 07:19:34 2023, max compression
```

## Comparing `clust-learn-0.2.0.tar` & `clust-learn-0.2.0b0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-27 06:35:38.000000 clust-learn-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29230 2023-05-27 06:35:50.929186 clust-learn-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28377 2023-05-27 06:35:38.000000 clust-learn-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clearn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clearn/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/classifier/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/classifier/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/classifier/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clearn/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/clustering/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/clustering/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/clustering/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16269 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/clustering/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clearn/data_preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/data_preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/data_preprocessing/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/data_preprocessing/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clearn/dimensionality_reduction/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/dimensionality_reduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/dimensionality_reduction/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/dimensionality_reduction/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/dimensionality_reduction/viz_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clust_learn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29230 2023-05-27 06:35:50.000000 clust-learn-0.2.0/clust_learn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 06:35:50.000000 clust-learn-0.2.0/clust_learn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:35:50.000000 clust-learn-0.2.0/clust_learn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 06:35:50.000000 clust-learn-0.2.0/clust_learn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 06:35:50.000000 clust-learn-0.2.0/clust_learn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-27 06:35:38.000000 clust-learn-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 06:35:50.929186 clust-learn-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-27 06:35:38.000000 clust-learn-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:38.000000 clust-learn-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-27 06:35:38.000000 clust-learn-0.2.0/tests/test_clearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/classifier/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27503 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16269 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/clustering/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/data_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/data_preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/data_preprocessing/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/data_preprocessing/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clearn/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/dimensionality_reduction/viz_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/clearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/clust_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 07:19:34.000000 clust-learn-0.2.0b0/clust_learn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:34.543653 clust-learn-0.2.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-27 07:19:22.000000 clust-learn-0.2.0b0/tests/test_clearn.py
```

### Comparing `clust-learn-0.2.0/LICENSE` & `clust-learn-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/PKG-INFO` & `clust-learn-0.2.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clust-learn
-Version: 0.2.0
+Version: 0.2.0b0
 Summary: A Python package for explainable cluster analysis
 Home-page: https://github.com/malgar/clust-learn
 Author: Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra
 Author-email: Miguel Alvarez-Garcia <malvarez.statistics@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/malgar/clust-learn
 Project-URL: Bug Tracker, https://github.com/malgar/clust-learn/issues
@@ -104,15 +104,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.2.0
+* Version: 0.2.0b
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.2.0/README.md` & `clust-learn-0.2.0b0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.2.0
+* Version: 0.2.0b
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.2.0/clearn/classifier/classifier.py` & `clust-learn-0.2.0b0/clearn/classifier/classifier.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/classifier/utils.py` & `clust-learn-0.2.0b0/clearn/classifier/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/classifier/viz_utils.py` & `clust-learn-0.2.0b0/clearn/classifier/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/clustering/clustering.py` & `clust-learn-0.2.0b0/clearn/clustering/clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         if algorithms is None:
             algorithms = [KMeans(random_state=42)]
         if not isinstance(algorithms, list):
             algorithms = [algorithms]
         self.algorithms = list()
 
         self.instances_ = dict()
-        for algorithm in self.algorithms:
+        for algorithm in algorithms:
             if is_sklearn_compatible(algorithm):
                 self.algorithms.append(str(algorithm))
                 self.instances_[self.algorithms[-1]] = algorithm
             else:
                 raise RuntimeWarning(f'Algorithm {str(algorithm)} does not comply with scikit-learn standard')
 
         self.scores_ = dict()
```

### Comparing `clust-learn-0.2.0/clearn/clustering/table_utils.py` & `clust-learn-0.2.0b0/clearn/clustering/table_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/clustering/utils.py` & `clust-learn-0.2.0b0/clearn/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/clustering/viz_utils.py` & `clust-learn-0.2.0b0/clearn/clustering/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/data_preprocessing/__init__.py` & `clust-learn-0.2.0b0/clearn/data_preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/data_preprocessing/data_preprocessing.py` & `clust-learn-0.2.0b0/clearn/data_preprocessing/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/data_preprocessing/viz_utils.py` & `clust-learn-0.2.0b0/clearn/data_preprocessing/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/dimensionality_reduction/dimensionality_reduction.py` & `clust-learn-0.2.0b0/clearn/dimensionality_reduction/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/dimensionality_reduction/table_utils.py` & `clust-learn-0.2.0b0/clearn/dimensionality_reduction/table_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/dimensionality_reduction/viz_utils.py` & `clust-learn-0.2.0b0/clearn/dimensionality_reduction/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clearn/utils.py` & `clust-learn-0.2.0b0/clearn/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/clust_learn.egg-info/PKG-INFO` & `clust-learn-0.2.0b0/clust_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clust-learn
-Version: 0.2.0
+Version: 0.2.0b0
 Summary: A Python package for explainable cluster analysis
 Home-page: https://github.com/malgar/clust-learn
 Author: Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra
 Author-email: Miguel Alvarez-Garcia <malvarez.statistics@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/malgar/clust-learn
 Project-URL: Bug Tracker, https://github.com/malgar/clust-learn/issues
@@ -104,15 +104,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.2.0
+* Version: 0.2.0b
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.2.0/clust_learn.egg-info/SOURCES.txt` & `clust-learn-0.2.0b0/clust_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clust-learn-0.2.0/pyproject.toml` & `clust-learn-0.2.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "clust-learn"
-version = "0.2.0"
+version = "0.2.0b"
 authors = [
   { name="Miguel Alvarez-Garcia", email="malvarez.statistics@gmail.com" },
 ]
 description = "A Python package for explainable cluster analysis"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `clust-learn-0.2.0/setup.py` & `clust-learn-0.2.0b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(os.path.join(ROOT, 'README.md')) as f:
     README = f.read()
 
 
 setup(
     name='clust-learn',
-    version="0.2.0",
+    version="0.2.0b",
     description="A Python package for explainable cluster analysis",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra",
     author_email="@gmail.com",
     url="https://github.com/malgar/clust-learn",
     packages=find_packages(),
```

