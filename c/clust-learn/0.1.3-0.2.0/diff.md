# Comparing `tmp/clust-learn-0.1.3.tar.gz` & `tmp/clust-learn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clust-learn-0.1.3.tar", last modified: Wed Apr 26 21:43:42 2023, max compression
+gzip compressed data, was "clust-learn-0.2.0.tar", last modified: Sat May 27 06:35:50 2023, max compression
```

## Comparing `clust-learn-0.1.3.tar` & `clust-learn-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.980054 clust-learn-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-26 21:43:25.000000 clust-learn-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-04-26 21:43:42.980054 clust-learn-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28377 2023-04-26 21:43:25.000000 clust-learn-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.976054 clust-learn-0.1.3/clearn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.976054 clust-learn-0.1.3/clearn/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/classifier/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/classifier/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/classifier/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.976054 clust-learn-0.1.3/clearn/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25489 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/clustering/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/clustering/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/clustering/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/clustering/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.976054 clust-learn-0.1.3/clearn/data_preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/data_preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/data_preprocessing/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/data_preprocessing/viz_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.980054 clust-learn-0.1.3/clearn/dimensionality_reduction/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/dimensionality_reduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/dimensionality_reduction/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/dimensionality_reduction/table_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/dimensionality_reduction/viz_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-04-26 21:43:25.000000 clust-learn-0.1.3/clearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.980054 clust-learn-0.1.3/clust_learn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29128 2023-04-26 21:43:42.000000 clust-learn-0.1.3/clust_learn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 21:43:42.000000 clust-learn-0.1.3/clust_learn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:43:42.000000 clust-learn-0.1.3/clust_learn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-26 21:43:42.000000 clust-learn-0.1.3/clust_learn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 21:43:42.000000 clust-learn-0.1.3/clust_learn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-26 21:43:25.000000 clust-learn-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:43:42.980054 clust-learn-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-26 21:43:25.000000 clust-learn-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:42.980054 clust-learn-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:43:25.000000 clust-learn-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 21:43:25.000000 clust-learn-0.1.3/tests/test_clearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-27 06:35:38.000000 clust-learn-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29230 2023-05-27 06:35:50.929186 clust-learn-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28377 2023-05-27 06:35:38.000000 clust-learn-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clearn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clearn/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/classifier/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/classifier/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/classifier/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clearn/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/clustering/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/clustering/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/clustering/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16269 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/clustering/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clearn/data_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/data_preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/data_preprocessing/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/data_preprocessing/viz_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clearn/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/dimensionality_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/dimensionality_reduction/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/dimensionality_reduction/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/dimensionality_reduction/viz_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-27 06:35:38.000000 clust-learn-0.2.0/clearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/clust_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29230 2023-05-27 06:35:50.000000 clust-learn-0.2.0/clust_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 06:35:50.000000 clust-learn-0.2.0/clust_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:35:50.000000 clust-learn-0.2.0/clust_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 06:35:50.000000 clust-learn-0.2.0/clust_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 06:35:50.000000 clust-learn-0.2.0/clust_learn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-27 06:35:38.000000 clust-learn-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 06:35:50.929186 clust-learn-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-27 06:35:38.000000 clust-learn-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:50.929186 clust-learn-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:35:38.000000 clust-learn-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-27 06:35:38.000000 clust-learn-0.2.0/tests/test_clearn.py
```

### Comparing `clust-learn-0.1.3/LICENSE` & `clust-learn-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/PKG-INFO` & `clust-learn-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: clust-learn
-Version: 0.1.3
+Version: 0.2.0
 Summary: A Python package for explainable cluster analysis
 Home-page: https://github.com/malgar/clust-learn
 Author: Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra
 Author-email: Miguel Alvarez-Garcia <malvarez.statistics@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/malgar/clust-learn
 Project-URL: Bug Tracker, https://github.com/malgar/clust-learn/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- title -->
 <div align="center">
   <h3>Clust-learn</h3>
@@ -102,15 +104,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.1.3
+* Version: 0.2.0
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.1.3/README.md` & `clust-learn-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.1.3
+* Version: 0.2.0
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.1.3/clearn/classifier/classifier.py` & `clust-learn-0.2.0/clearn/classifier/classifier.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/clearn/classifier/utils.py` & `clust-learn-0.2.0/clearn/classifier/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/clearn/classifier/viz_utils.py` & `clust-learn-0.2.0/clearn/classifier/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/clearn/clustering/clustering.py` & `clust-learn-0.2.0/clearn/clustering/clustering.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,83 +13,87 @@
 from .utils import *
 from .viz_utils import *
 
 __metrics__ = ['inertia', 'davies_bouldin_score', 'silhouette_score', 'calinski_harabasz_score']
 METRIC_NAMES = dict(zip(__metrics__,
                         ['Weighted Sum of Squared Distances', 'Davies Bouldin Score', 'Silhouette Score',
                          'Calinski and Harabasz score']))
-KMEANS = ['kmeans', 'kmeans++']
-HIERARCHICAL_WARD = ['ward', 'hierarchical', 'agglomerative']
 
 
 class Clustering:
     """
     Clustering class
 
     Parameters
     ----------
     df : `pandas:DatasFrame`
         DataFrame with main data
-    algorithms : str or list, default='kmeans'
-        Algorithm/s to be used for clustering.
+    algorithms : instance or list of instances, default=None
+        Algorithm instances to be used for clustering. They must implement the `fit` and `set_params` methods.
         By default, [K-Means++](https://scikit-learn.org/stable/modules/clustering.html#k-means)
     normalize : bool, default=True
         Whether to apply data normalization for fair comparisons between variables. By default it is applied. In case
         dimensionality reduction is applied beforehand, normalization should not be applied.
     """
     def __init__(self,
                  df,
-                 algorithms='kmeans',
+                 algorithms=None,
                  normalize=True):
 
         # Normalize variables for fair comparisons
         self.normalize = normalize
         self.df = df.copy()
         if normalize:
             mms = MinMaxScaler()
             self.df = pd.DataFrame(mms.fit_transform(df), columns=df.columns)
 
         self.dimensions_ = list(df.columns)
 
+        if algorithms is None:
+            algorithms = [KMeans(random_state=42)]
         if not isinstance(algorithms, list):
             algorithms = [algorithms]
-        self.algorithms = list(map(str.lower, algorithms))
+        self.algorithms = list()
 
         self.instances_ = dict()
         for algorithm in self.algorithms:
-            if algorithm in KMEANS:
-                self.instances_[algorithm] = KMeans(random_state=42)
-            elif algorithm in HIERARCHICAL_WARD:
-                self.instances_[algorithm] = AgglomerativeClustering()
+            if is_sklearn_compatible(algorithm):
+                self.algorithms.append(str(algorithm))
+                self.instances_[self.algorithms[-1]] = algorithm
             else:
-                raise RuntimeWarning(f'''Algorithm {algorithm} is not supported.
-                                     Supported algorithms are: KMeans and Hierarchical clustering''')
+                raise RuntimeWarning(f'Algorithm {str(algorithm)} does not comply with scikit-learn standard')
 
         self.scores_ = dict()
         self._initialize_scores()
 
         self.metric_ = 'inertia'
         self.optimal_config_ = None
+        self.weights_ = None
 
     def _initialize_scores(self):
         for algorithm in self.algorithms:
-            if algorithm in KMEANS + HIERARCHICAL_WARD:
-                self.scores_[algorithm] = []
+            self.scores_[algorithm] = []
 
-    def _compute_clusters(self, algorithm, n_clusters):
+    def _compute_clusters(self, algorithm, n_clusters, weights=None):
         self.instances_[algorithm].set_params(n_clusters=n_clusters)
-        self.instances_[algorithm].fit(self.df[self.dimensions_])
+        if accepts_param(self.instances_[algorithm].fit, 'sample_weight'):
+            self.instances_[algorithm].fit(self.df[self.dimensions_], sample_weight=weights)
+        else:
+            self.instances_[algorithm].fit(self.df[self.dimensions_])
         self.labels_ = self.instances_[algorithm].labels_
 
-    def _compute_optimal_clustering_config(self, metric, cluster_range, weights):
+    def _compute_optimal_clustering_config(self, metric, cluster_range, weights=None):
         optimal_list = []
         for algorithm in self.algorithms:
             for nc in range(*cluster_range):
                 self.instances_[algorithm].set_params(n_clusters=nc)
-                self.instances_[algorithm].fit(self.df[self.dimensions_])
+                if accepts_param(self.instances_[algorithm].fit, 'sample_weight'):
+                    self.instances_[algorithm].fit(self.df[self.dimensions_], sample_weight=weights)
+                else:
+                    self.instances_[algorithm].fit(self.df[self.dimensions_])
 
                 if metric == 'inertia':
                     self.scores_[algorithm].append(
                         weighted_sum_of_squared_distances(self.df[self.dimensions_], self.instances_[algorithm].labels_,
                                                           weights))
                 elif metric == 'davies_bouldin_score':
                     self.scores_[algorithm].append(
@@ -138,41 +142,41 @@
             'calinski_harabasz_score']
         max_clusters : int, default=10
             In case of optimal search, this parameter limits the maximum number of clusters allowed.
         prefix : str, default=None
             Used for cluster naming. Naming format: `f'{prefix}_{x}'`
         weights : `numpy.array`, default=None
             In case observations have different weights.
-            *Note this is not implemented yet.*
 
         Returns
         ----------
         labels_ : `numpy.array`
             Cluster label of each observation.
         """
         if metric not in __metrics__:
             raise RuntimeError(f'''Metric {metric} not supported.
                                Supported metrics: {__metrics__}''')
 
         self._initialize_scores()
         self.metric_ = metric
+        self.weights_ = weights
 
         # Compute optimal number of clusters
         cluster_range = []
         if n_clusters is not None:
             cluster_range = [n_clusters, n_clusters + 1]
         else:
             cluster_range = [1, max_clusters + 1]
 
         self.optimal_config_ = self._compute_optimal_clustering_config(metric, cluster_range, weights)
 
         if self.optimal_config_ is None:
             raise RuntimeError('Optimal cluster configuration not available')
 
-        self._compute_clusters(self.optimal_config_[0], self.optimal_config_[1])
+        self._compute_clusters(self.optimal_config_[0], self.optimal_config_[1], weights)
 
         # Might be interesting to only keep one
         self.df['cluster'] = self.labels_
         self.df['cluster_cat'] = self.labels_
         if prefix is not None:
             name_len = len(str(max(self.labels_)))
             self.df['cluster_cat'] = list(map(lambda x: f'{prefix}_{str.zfill(str(x), name_len)}', self.labels_))
@@ -195,14 +199,15 @@
             List of variables (internal or external) for describing clusters. This parameter is optional and should
             be used when only a subset of the variable is of interest.
         cluster_filter : str or list, default=None
             In case the descriptive statistics of interest only applies to a subset of the calculated clusters.
         statistics : str or list, default=['mean', 'median', 'std']
             Statistics to use for describing clusters.
             *Note any statistics supported by Pandas can be used. This includes the `describe` function*
+            If weights are used for clustering, 'wmean' and 'wstd' can be used for weighted mean and standard dev.
         output_path : str, default=None
             If an output_path is passed, the resulting DataFame is saved as a CSV file.
 
         Returns
         ----------
         res : `pandas.DataFrame`
             DataFrame with the cluster description.
@@ -222,47 +227,63 @@
             variables.remove('cluster')
 
         if cluster_filter is None:
             cluster_filter = list(df_ext['cluster'].unique())
         if not isinstance(cluster_filter, list):
             cluster_filter = [cluster_filter]
 
+        if 'wmean' in statistics:
+            def wmean(x): return weighted_mean(x, self.weights_[x.index])
+            statistics[statistics.index('wmean')] = wmean
+        if 'wstd' in statistics:
+            def wstd(x): return weighted_std(x, self.weights_[x.index])
+            statistics[statistics.index('wstd')] = wstd
+
         res = df_ext[df_ext['cluster'].isin(cluster_filter)].groupby('cluster').agg(
             dict(zip(list(variables), [statistics] * len(variables)))).reset_index()
 
         if output_path is not None:
             res.to_csv(output_path, index=False)
 
         return res
 
-    def describe_clusters_cat(self, cat_array, cat_name=None, order=None, normalize=False, output_path=None):
+    def describe_clusters_cat(self, cat_array, cat_name, order=None, normalize=False, use_weights=False,
+                              output_path=None):
         """
         Describes clusters based on  external *categorical* variables. The result is a contingency table.
         For continuous variables use `describe_clusters()`.
 
         Parameters
         ----------
         cat_array : `pandas.Series` or `numpy.array`
             Values of categorical variable.
             The order of the observations must be the same as that of the base DataFrame.
-        cat_name : str, default=None
+        cat_name : str
             Name of the categorical variable.
         order : list or `numpy.array`, default=None
             In case categories should be displayed in a specific order.
         normalize : boolean, default=False
             If True, results are row-normalized.
+        use_weights : boolean, default=False
+            If True, frequencies are computed using weights.
         output_path : str, default=None
             If an output_path is passed, the resulting DataFame is saved as a CSV file.
 
         Returns
         ----------
         freq : `pandas.DataFrame`
             DataFrame with a cluster description based on the passed categorical variable.
         """
         freq = pd.crosstab(index=self.df['cluster_cat'], columns=cat_array, rownames=['Clusters'], colnames=[cat_name])
+        if use_weights:
+            wcrosstab_df = pd.DataFrame(data=[self.df['cluster_cat'], cat_array, self.weights_],
+                                        index=['Clusters', cat_name, 'weights']).transpose()
+            freq = wcrosstab_df.groupby(['Clusters', cat_name]).agg({'weights': 'sum'}).reset_index()\
+                .pivot(index='Clusters', columns=cat_name, values='weights')
+
         if order is not None:
             freq = freq[order]
 
         if normalize:
             freq['total'] = freq.sum(1)
             for col in freq.columns[:-1]:
                 freq[col] = freq[col] / freq['total']
@@ -291,18 +312,18 @@
         df_agg_diff : `pandas.DataFrame`
             DataFrame with the comparison.
         """
         if df_original is not None:
             var_names = list(df_original.columns)
             df_original = df_original.copy()
             df_original['cluster'] = self.labels_
-            return compare_cluster_means_to_global_means(df_original, var_names, output_path=output_path)
+            return compare_cluster_means_to_global_means(df_original, var_names, self.weights_, output_path=output_path)
         else:
-            return compare_cluster_means_to_global_means(self.df, self.dimensions_, data_standardized=not self.normalize,
-                                                         output_path=output_path)
+            return compare_cluster_means_to_global_means(self.df, self.dimensions_, self.weights_,
+                                                         data_standardized=not self.normalize, output_path=output_path)
 
     def anova_tests(self, df_test=None, vars_test=None, cluster_filter=None, output_path=None):
         """
         Runs ANOVA tests for a given set of continuous variables (internal or external) to test dependency with
         clusters.
 
         Parameters
@@ -412,35 +433,42 @@
             plot_optimal_components_normalized(self.scores_[self.optimal_config_[0]],
                                                len(self.scores_[self.optimal_config_[0]]),
                                                METRIC_NAMES[self.metric_],
                                                output_path, savefig_kws)
         else:
             raise RuntimeError('This plot can only be used when `cluster_range` contains at least 2 values')
 
-    def plot_clustercount(self, output_path=None, savefig_kws=None):
+    def plot_clustercount(self, use_weights=False, output_path=None, savefig_kws=None):
         """
         Plots a bar plot with cluster counts.
 
         Parameters
         ----------
+        use_weights: bool
+            Whether to use sample weights.
         output_path : str, default=None
             Path to save figure as image.
         savefig_kws : dict, default=None
             Save figure options.
         """
-        plot_clustercount(self.df, output_path, savefig_kws)
+        if use_weights:
+            plot_clustercount(self.df, self.weights_, output_path, savefig_kws)
+        else:
+            plot_clustercount(self.df, output_path, savefig_kws)
 
-    def plot_cluster_means_to_global_means_comparison(self, df_original=None, xlabel=None, ylabel=None,
+    def plot_cluster_means_to_global_means_comparison(self, use_weights= False, df_original=None, xlabel=None, ylabel=None,
                                                       levels=[-0.50, -0.32, -0.17, -0.05, 0.05, 0.17, 0.32, 0.50],
                                                       output_path=None, savefig_kws=None):
         """
         Plots the normalized curve used for computing the optimal number of clusters.
 
         Parameters
         ----------
+        use_weights : bool, default=False
+            Whether to use sample weights.
         df_original : `pandas.DataFrame`, default=None
             In case the comparison wants to be made with the original variables and values. Note it is assumed that both
             the original dataframe and the one used for clustering have observations is the same order.
         xlabel : str, default=None
             x-label name/description.
         ylabel : str, default=None
             y-label name/description.
@@ -448,25 +476,28 @@
             Values to be used as cuts for color intensity.
             Default values: [-0.50, -0.32, -0.17, -0.05, 0.05, 0.17, 0.32, 0.50]
         output_path : str, default=None
             Path to save figure as image.
         savefig_kws : dict, default=None
             Save figure options.
         """
+        weights = None
+        if use_weights:
+            weights = self.weights_
 
         if df_original is not None:
             var_names = list(df_original.columns)
             df_original = df_original.copy()
             df_original['cluster'] = self.labels_
 
-            plot_cluster_means_to_global_means_comparison(df_original, var_names, xlabel, ylabel, levels,
+            plot_cluster_means_to_global_means_comparison(df_original, var_names, weights, xlabel, ylabel, levels,
                                                           data_standardized=False, output_path=output_path,
                                                           savefig_kws=savefig_kws)
         else:
-            plot_cluster_means_to_global_means_comparison(self.df, self.dimensions_, xlabel, ylabel, levels,
+            plot_cluster_means_to_global_means_comparison(self.df, self.dimensions_, weights, xlabel, ylabel, levels,
                                                           data_standardized=not self.normalize, output_path=output_path,
                                                           savefig_kws=savefig_kws)
 
     def plot_distribution_comparison_by_cluster(self, df_ext=None, xlabel=None, ylabel=None, output_path=None,
                                                 savefig_kws=None):
         """
         Plots the violin plots per cluster and *continuous* variables of interest to understand differences in their
@@ -491,15 +522,15 @@
             df_ext = self.df[self.dimensions_]
         else:
             sharey = False
 
         plot_distribution_by_cluster(df_ext, self.labels_, xlabel=xlabel, ylabel=ylabel, sharey=sharey,
                                      output_path=output_path, savefig_kws=savefig_kws)
 
-    def plot_clusters_2D(self, coor1, coor2, style_kwargs=dict(), output_path=None, savefig_kws=None):
+    def plot_clusters_2D(self, coor1, coor2, use_weights=False, style_kwargs=dict(), output_path=None, savefig_kws=None):
         """
         Plots two 2D plots:
          - A scatter plot styled by the categorical variable `hue`.
          - A 2D plot comparing cluster centroids and optionally the density area.
 
         Parameters
         ----------
@@ -507,18 +538,21 @@
             If int, it represents the id of the internal variable to be used.
             If str, it must be an internal variable name.
             If `pandas.Series`, it is assumed it is an external variable.
         coor2 : int, str, or `pandas.Series`
             If int, it represents the id of the internal variable to be used.
             If str, it must be an internal variable name.
             If `pandas.Series`, it is assumed it is an external variable.
+        use_weights : bool, default=False
+            Whether to use weights for centroid comparison.
         style_kwargs : dict, default=empty dict
             Dictionary with optional styling parameters.
             List of parameters:
              - palette : matplotlib palette to be used. default='gnuplot'
+             - alpha : the alpha blending value, between 0 (transparent) and 1 (opaque). default=0.3
              - vline_color : color to be used for vertical line (used for plotting x mean value). default='#11A579'
              - hline_color : color to be used for horizontal line (used for plotting y mean value). default='#332288'
              - kdeplot : boolean to display density area of points (using seabonr.kdeplot). default=True
         output_path : str, default=None
             Path to save figure as image.
         savefig_kws : dict, default=None
             Save figure options.
@@ -535,15 +569,18 @@
             df_ext = pd.DataFrame(data={coor1.name: coor1,
                                         coor2.name: coor2,
                                         'cluster_cat': self.df['cluster_cat'].values})
             coor1 = coor1.name
             coor2 = coor2.name
 
         hue = 'cluster_cat'
-        plot_clusters_2D(coor1, coor2, hue, df_ext, style_kwargs=style_kwargs, output_path=output_path,
+        weights = None
+        if use_weights:
+            weights = self.weights_
+        plot_clusters_2D(coor1, coor2, hue, df_ext, weights, style_kwargs=style_kwargs, output_path=output_path,
                          savefig_kws=savefig_kws)
 
     def plot_cat_distribution_by_cluster(self, cat_array, cat_label=None, cluster_label=None, output_path=None,
                                          savefig_kws=None):
         """
         Plots the relative contingency table of the clusters with a categorical variable as a stacked bar plot.
```

### Comparing `clust-learn-0.1.3/clearn/clustering/viz_utils.py` & `clust-learn-0.2.0/clearn/clustering/viz_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Utils for visualization"""
 # Author: Miguel Alvarez-Garcia
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
 import seaborn as sns
 
 from kneed import KneeLocator
 from .table_utils import compare_cluster_means_to_global_means
+from .utils import *
 from ..utils import get_axis, plot_optimal_normalized_elbow, savefig
 
 
 sns.set_style('whitegrid')
 
 CARTO_COLORS = ['#7F3C8D', '#11A579', '#3969AC', '#F2B701', '#E73F74', '#80BA5A', '#E68310',  '#008695', '#CF1C90',
                 '#f97b72', '#4b4b8f', '#A5AA99']
@@ -72,64 +74,74 @@
     fig, ax = plt.subplots(figsize=(8, 5))
     kl = KneeLocator(x=range(1, max_clusters + 1), y=scores, curve='convex', direction='decreasing')
     plot_optimal_normalized_elbow(scores, kl, ax, optimal_label='Optimal number of clusters',
                                   xlabel='Number of clusters', ylabel=f'Normalized {metric_name}')
     savefig(output_path=output_path, savefig_kws=savefig_kws)
 
 
-def plot_clustercount(df, output_path=None, savefig_kws=None):
+def plot_clustercount(df, weights=None, output_path=None, savefig_kws=None):
     """
     Plots a bar plot with cluster counts.
 
     Parameters
     ----------
     df : `pandas.DataFrame`
         DataFrame containing at least a column named 'cluster_cat' with the cluster labels.
+    weights: `numpy.array`, default=None
+        Sample weights
     output_path : str, default=None
         Path to save figure as image.
     savefig_kws : dict, default=None
         Save figure options.
     """
     plt.figure(figsize=(df['cluster_cat'].nunique(), 5))
-    sns.countplot(x='cluster_cat', data=df, color='#332288', alpha=0.9, order=np.sort(df['cluster_cat'].unique()))
+    if weights is None:
+        sns.countplot(x='cluster_cat', data=df, color='#332288', alpha=0.9, order=np.sort(df['cluster_cat'].unique()))
+    else:
+        bar_df = pd.concat([df['cluster_cat'], pd.Series(weights, name='weights')], axis=1).groupby(
+            'cluster_cat').agg({'weights': 'sum'}).reset_index()
+        sns.barplot(x='cluster_cat', y='weights', data=bar_df, color='#332288', alpha=0.9,
+                    order=np.sort(df['cluster_cat'].unique()))
     # plt.xticks(rotation=30)
     plt.ylabel('count', fontsize=12, labelpad=10)
     plt.xlabel('clusters', fontsize=12, labelpad=10)
     plt.tight_layout(pad=2)
     savefig(output_path=output_path, savefig_kws=savefig_kws)
 
 
-def plot_cluster_means_to_global_means_comparison(df, dimensions, xlabel=None, ylabel=None,
+def plot_cluster_means_to_global_means_comparison(df, dimensions, weights=None, xlabel=None, ylabel=None,
                                                   levels=[-0.50, -0.32, -0.17, -0.05, 0.05, 0.17, 0.32, 0.50],
                                                   data_standardized=False, output_path=None, savefig_kws=None):
     """
     Plots the normalized curve used for computing the optimal number of clusters.
 
     Parameters
     ----------
     df : `pandas.DataFrame`
         DataFrame containing the variables used for clustering.
     dimensions : list
         List of variables of interest.
         *Note these must be internal variables, ie, variables used for clustering*
+    weights: `np.array`, default=None
+        Sample weights.
     xlabel : str, default=None
         x-label name/description.
     ylabel : str, default=None
         y-label name/description.
     levels : list or `numpy.array`
         Values to be used as cuts for color intensity.
         Default values: [-0.50, -0.32, -0.17, -0.05, 0.05, 0.17, 0.32, 0.50]
     data_standardized : bool, default=False
         If data are standardized, comparison to global mean is based solely on the mean per cluster.
     output_path : str, default=None
         Path to save figure as image.
     savefig_kws : dict, default=None
         Save figure options.
     """
-    df_diff = compare_cluster_means_to_global_means(df, dimensions, data_standardized=data_standardized)
+    df_diff = compare_cluster_means_to_global_means(df, dimensions, weights, data_standardized=data_standardized)
     colors = sns.color_palette("BrBG", n_colors=9)
     cmap, norm = matplotlib.colors.from_levels_and_colors(levels, colors, extend="both")
     width = min(len(dimensions), 20)
     height = min(df['cluster'].nunique(), 8)
     fig, ax = plt.subplots(figsize=(width, height))
     im = ax.imshow(df_diff[dimensions].values, cmap=cmap, norm=norm)
     ax.set(xticks=range(len(dimensions)), yticks=range(df_diff.shape[0]),
@@ -211,15 +223,15 @@
         ax.axis('off')
         i += 1
 
     fig.tight_layout(pad=2)
     savefig(output_path=output_path, savefig_kws=savefig_kws)
 
 
-def plot_clusters_2D(x, y, hue, df, style_kwargs=dict(), output_path=None, savefig_kws=None):
+def plot_clusters_2D(x, y, hue, df, weights=None, style_kwargs=dict(), output_path=None, savefig_kws=None):
     """
     Plots two 2D plots:
      - A scatter plot styled by the categorical variable `hue`.
      - A 2D plot comparing cluster centroids and optionally the density area.
 
     Parameters
     ----------
@@ -227,75 +239,98 @@
         x-coordinate data.
     y : `numpy.array` or list
         y-coordinate data.
     hue : `numpy.array` or list
         Array with categorical values to be used for color styling.
     df : `pandas.DataFrame`
         DataFrame containing the data.
+    weights : `numpy.array`, default=None
+        Sample weights
     style_kwargs : dict, default=empty dict
         Dictionary with optional styling parameters.
         List of parameters:
          - palette : matplotlib palette to be used. default='gnuplot'
+         - alpha : the alpha blending value, between 0 (transparent) and 1 (opaque). default=0.3
          - vline_color : color to be used for vertical line (used for plotting x mean value). default='#11A579'
          - hline_color : color to be used for horizontal line (used for plotting y mean value). default='#332288'
          - kdeplot : boolean to display density area of points (using seabonr.kdeplot). default=True
     output_path : str, default=None
         Path to save figure as image.
     savefig_kws : dict, default=None
         Save figure options.
     """
     # Style params
     palette = 'gnuplot'
     if style_kwargs.get('palette'):
         palette = style_kwargs.get('palette')
 
+    alpha = 0.3
+    if style_kwargs.get('alpha'):
+        alpha = style_kwargs.get('alpha')
+
     vline_color = '#11A579'
     if style_kwargs.get('vline_color'):
         vline_color = style_kwargs.get('vline_color')
 
     hline_color = '#332288'
     if style_kwargs.get('hline_color'):
         vline_color = style_kwargs.get('hline_color')
 
     kdeplot = True
     if style_kwargs.get('kdeplot') is not None:
         kdeplot = style_kwargs.get('kdeplot')
 
     fig, axs = plt.subplots(1, 2, figsize=(14, 5), sharey=True, sharex=True)
 
+    xmean = df[x].mean()
+    xmean_label= f'Mean {x}'
+    if weights is not None:
+        xmean = weighted_mean(df[x], weights)
+        xmean_label = f'W. Mean {x}'
     x_range = df[x].max() - df[x].min()
     xmin = df[x].min() - x_range * 0.05
     xmax = df[x].max() + x_range * 0.05
+
+    ymean = df[y].mean()
+    ymean_label = f'Mean {y}'
+    if weights is not None:
+        ymean = weighted_mean(df[y], weights)
+        ymean_label = f'W. Mean {y}'
     y_range = df[y].max() - df[y].min()
     ymin = df[y].min() - y_range * 0.05
     ymax = df[y].max() + y_range * 0.05
 
     # Left-hand side plot: Scatter plot colored by cluster category
-    sns.scatterplot(x=x, y=y, hue=hue, data=df.sort_values(hue), alpha=0.3, palette=palette, linewidth=0, ax=axs[0])
-    axs[0].vlines(df[x].mean(), ymin=ymin, ymax=ymax, color=vline_color, linewidth=1.15, linestyles='--', label=f'Mean {x}')
-    axs[0].hlines(df[y].mean(), xmin=xmin, xmax=xmax, color=hline_color, linewidth=1.15, linestyles='--',
-                  label=f'Mean {y}')
+    sns.scatterplot(x=x, y=y, hue=hue, data=df.sort_values(hue), alpha=alpha, palette=palette, linewidth=0, ax=axs[0])
+    axs[0].vlines(xmean, ymin=ymin, ymax=ymax, color=vline_color, linewidth=1.15, linestyles='--', label=xmean_label)
+    axs[0].hlines(ymean, xmin=xmin, xmax=xmax, color=hline_color, linewidth=1.15, linestyles='--', label=ymean_label)
     axs[0].set_xlabel(x, fontsize=12)
     axs[0].set_ylabel(y, fontsize=12)
     axs[0].set_title('Scatter plot by cluster', fontsize=13)
     axs[0].set_xlim(xmin, xmax)
     axs[0].set_ylim(ymin, ymax)
 
     # Right-hand side plot: Cluster centroids with optional kernel density area
-    sns.scatterplot(x=x, y=y, hue=hue, data=df.groupby(hue).mean().reset_index(),
+
+    agg_method = 'mean'
+    if weights is not None:
+        def wmean(v): return weighted_mean(v, weights[v.index])
+        agg_method = wmean
+    scatter_df = df.groupby(hue).agg(dict(zip([x, y], [agg_method] * 2))).reset_index()
+
+    sns.scatterplot(x=x, y=y, hue=hue, data=scatter_df,
                     alpha=1, palette=palette, linewidth=0, marker='X', s=100, ax=axs[1])
 
     if kdeplot:
-        sns.kdeplot(x=x, y=y, hue=hue, data=df.sort_values(hue), levels=1, alpha=0.2, palette=palette,
-                    ax=axs[1])
+        hue_order = np.sort(df[hue].values)
+        sns.kdeplot(x=x, y=y, hue=hue, data=df, levels=1, alpha=0.2, palette=palette,
+                    weights=weights, hue_order=hue_order, ax=axs[1])
 
-    axs[1].vlines(df[x].mean(), ymin=ymin, ymax=ymax, color=vline_color, linewidth=1, linestyles='--',
-                  label=f'Mean {x}')
-    axs[1].hlines(df[y].mean(), xmin=xmin, xmax=xmax, color=hline_color, linewidth=1, linestyles='--',
-                  label=f'Mean {y}')
+    axs[1].vlines(xmean, ymin=ymin, ymax=ymax, color=vline_color, linewidth=1, linestyles='--', label=xmean_label)
+    axs[1].hlines(ymean, xmin=xmin, xmax=xmax, color=hline_color, linewidth=1, linestyles='--', label=ymean_label)
     axs[1].set_xlabel(x, fontsize=12)
     axs[1].set_ylabel(y, fontsize=12)
     axs[1].set_title('Cluster centroids', fontsize=13)
 
     axs[0].legend(fontsize=11, title='', title_fontsize=12, labelspacing=0.5,
                   loc=(0.93, 0.5 - 0.167 * (df[hue].nunique() // 4)))
     axs[1].legend(fontsize=11, title='', title_fontsize=12, labelspacing=0.5,
```

### Comparing `clust-learn-0.1.3/clearn/data_preprocessing/__init__.py` & `clust-learn-0.2.0/clearn/data_preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/clearn/data_preprocessing/data_preprocessing.py` & `clust-learn-0.2.0/clearn/data_preprocessing/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/clearn/data_preprocessing/viz_utils.py` & `clust-learn-0.2.0/clearn/data_preprocessing/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/clearn/dimensionality_reduction/dimensionality_reduction.py` & `clust-learn-0.2.0/clearn/dimensionality_reduction/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/clearn/dimensionality_reduction/table_utils.py` & `clust-learn-0.2.0/clearn/dimensionality_reduction/table_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/clearn/dimensionality_reduction/viz_utils.py` & `clust-learn-0.2.0/clearn/dimensionality_reduction/viz_utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/clearn/utils.py` & `clust-learn-0.2.0/clearn/utils.py`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/clust_learn.egg-info/PKG-INFO` & `clust-learn-0.2.0/clust_learn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: clust-learn
-Version: 0.1.3
+Version: 0.2.0
 Summary: A Python package for explainable cluster analysis
 Home-page: https://github.com/malgar/clust-learn
 Author: Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra
 Author-email: Miguel Alvarez-Garcia <malvarez.statistics@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/malgar/clust-learn
 Project-URL: Bug Tracker, https://github.com/malgar/clust-learn/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- title -->
 <div align="center">
   <h3>Clust-learn</h3>
@@ -102,15 +104,15 @@
 pip install clust-learn
 ```
 
 <h2 id="user-content-license">
 5. Version and license information
 </h2>
 
-* Version: 0.1.3
+* Version: 0.2.0
 * Author: Miguel Alvarez-Garcia (malvarez.statistics@gmail.com)
 * License: GPLv3 
 
 <h2 id="user-content-future">
 6. Bug reports and future work
 </h2>
```

### Comparing `clust-learn-0.1.3/clust_learn.egg-info/SOURCES.txt` & `clust-learn-0.2.0/clust_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clust-learn-0.1.3/setup.py` & `clust-learn-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,38 +5,41 @@
 
 with open(os.path.join(ROOT, 'README.md')) as f:
     README = f.read()
 
 
 setup(
     name='clust-learn',
-    version=1.0,
+    version="0.2.0",
     description="A Python package for explainable cluster analysis",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Miguel Alvarez-Garcia, Raquel Ibar-Alonso, Mar Arenas-Parra",
     author_email="@gmail.com",
     url="https://github.com/malgar/clust-learn",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         'Topic :: Scientific/Engineering',
-        'Programming Language :: Python :: 3.9'
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
     license='GPLv3',
     install_requires=[
-        "kneed==0.7.0",
-        "matplotlib==3.4.3",
-        "networkx==2.6.3",
-        "numpy==1.20.3",
-        "pandas==1.3.4",
-        "pingouin==0.5.1",
+        "kneed>=0.7.0",
+        "matplotlib>=3.4.3",
+        "networkx>=2.6.3",
+        "numpy>=1.20.3",
+        "pandas>=1.3.4",
+        "pingouin>=0.5.1",
         "prince==0.7.0",
-        "scikit-learn==1.0.2",
-        "scipy==1.7.1",
-        "seaborn==0.11.2",
-        "shap==0.40.0",
-        "statsmodels==0.13.2",
-        "xgboost==1.5.2"
-    ]
+        "scikit-learn>=1.0.2",
+        "scipy>=1.7.1",
+        "seaborn>=0.11.2",
+        "shap>=0.40.0",
+        "statsmodels>=0.13.2",
+        "xgboost>=1.5.2"
+    ],
+    python_requires='>=3.9'
 )
```

