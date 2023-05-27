# Comparing `tmp/SNPTMT-0.0.6.tar.gz` & `tmp/SNPTMT-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SNPTMT-0.0.6.tar", last modified: Sat May 27 08:59:38 2023, max compression
+gzip compressed data, was "SNPTMT-0.0.7.tar", last modified: Sat May 27 21:30:35 2023, max compression
```

## Comparing `SNPTMT-0.0.6.tar` & `SNPTMT-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:59:38.683927 SNPTMT-0.0.6/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-27 08:38:07.000000 SNPTMT-0.0.6/LICENSE
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:59:38.684007 SNPTMT-0.0.6/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.6/README.md
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:59:38.682875 SNPTMT-0.0.6/SNPTMT/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      332 2023-05-27 08:58:59.000000 SNPTMT-0.0.6/SNPTMT/__init__.py
--rw-r--r--   0 andrewshatalov   (501) staff       (20)     8692 2023-05-27 08:55:15.000000 SNPTMT-0.0.6/SNPTMT/snptmt.py
-drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 08:59:38.683567 SNPTMT-0.0.6/SNPTMT.egg-info/
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 08:59:38.000000 SNPTMT-0.0.6/SNPTMT.egg-info/PKG-INFO
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      312 2023-05-27 08:59:38.000000 SNPTMT-0.0.6/SNPTMT.egg-info/SOURCES.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-27 08:59:38.000000 SNPTMT-0.0.6/SNPTMT.egg-info/dependency_links.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)        7 2023-05-27 08:59:38.000000 SNPTMT-0.0.6/SNPTMT.egg-info/top_level.txt
--rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-27 08:59:38.684279 SNPTMT-0.0.6/setup.cfg
--rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-27 08:59:26.000000 SNPTMT-0.0.6/setup.py
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 21:30:35.475846 SNPTMT-0.0.7/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     1111 2023-05-27 08:38:07.000000 SNPTMT-0.0.7/LICENSE
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 21:30:35.475955 SNPTMT-0.0.7/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        8 2023-05-26 20:22:56.000000 SNPTMT-0.0.7/README.md
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 21:30:35.474664 SNPTMT-0.0.7/SNPTMT/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      332 2023-05-27 08:58:59.000000 SNPTMT-0.0.7/SNPTMT/__init__.py
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)     8733 2023-05-27 21:29:46.000000 SNPTMT-0.0.7/SNPTMT/snptmt.py
+drwxr-xr-x   0 andrewshatalov   (501) staff       (20)        0 2023-05-27 21:30:35.475415 SNPTMT-0.0.7/SNPTMT.egg-info/
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      571 2023-05-27 21:30:35.000000 SNPTMT-0.0.7/SNPTMT.egg-info/PKG-INFO
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      312 2023-05-27 21:30:35.000000 SNPTMT-0.0.7/SNPTMT.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        1 2023-05-27 21:30:35.000000 SNPTMT-0.0.7/SNPTMT.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)        7 2023-05-27 21:30:35.000000 SNPTMT-0.0.7/SNPTMT.egg-info/top_level.txt
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)       38 2023-05-27 21:30:35.476260 SNPTMT-0.0.7/setup.cfg
+-rw-r--r--   0 andrewshatalov   (501) staff       (20)      945 2023-05-27 21:29:56.000000 SNPTMT-0.0.7/setup.py
```

### Comparing `SNPTMT-0.0.6/LICENSE` & `SNPTMT-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SNPTMT-0.0.6/PKG-INFO` & `SNPTMT-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.6/SNPTMT/snptmt.py` & `SNPTMT-0.0.7/SNPTMT/snptmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
     for i in range(1, n_clusters + 1):
         cluster_messages = [df.iloc[j + start_message]['message'] for j in cluster_dict[i]]
         #print(f"Cluster {i}: {cluster_messages}")
     return cluster_dict
 
 
 def add_points(df, start_message, end_message, cluster_dict, nlp):
+    nlp = spacy.load("ru_core_news_sm")
     #take part of prev clusters
     half_cluster_dict = {}
     for key, value in cluster_dict.items():
         half_len = math.ceil(len(value)/2)
         half_cluster_dict[key] = random.sample(value, half_len)
     #this if we want to compare half_clusters
     ###global cluster_dict_prev 
@@ -229,15 +230,15 @@
                 base_cluster_id = old_cluster_id
         if base_cluster_id is not None and max_intersection:
             base_clusters.append((base_cluster_id, new_cluster_id, max_intersection))
     return base_clusters
 
 
 
-def remove_outdated_clusters(cluster_dict, cluster_dict_prev, base_clusters, cluster_counters, threshold, added_points):
+def remove_outdated_clusters(cluster_dict, cluster_dict_prev, base_clusters, cluster_counters, added_points, threshold=1):
     updated_cluster_counters = {key: 0 for key in cluster_dict.keys()}
     for base_cluster, new_cluster, common_elements in base_clusters:
         # If the base cluster and the new cluster have the same content, it means that no new points have been added
         if set(cluster_dict[new_cluster]) == set(cluster_dict_prev[base_cluster]):
             increment = 1 - 1/added_points
             updated_cluster_counters[new_cluster] = cluster_counters.get(base_cluster, 0) + increment
         else:
@@ -251,8 +252,7 @@
     return cluster_dict, updated_cluster_counters
 
 
 
 def initialize_cluster_counters(cluster_dict):
     cluster_counters = {cluster_id: 1 for cluster_id in cluster_dict}
     return cluster_counters
-
```

### Comparing `SNPTMT-0.0.6/SNPTMT.egg-info/PKG-INFO` & `SNPTMT-0.0.7/SNPTMT.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SNPTMT
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python module for searching for a new popular topics in the message threade
 Home-page: https://github.com/FIvER4IK/snptmt
 Download-URL: 
 Author: FIvER4IK
 Author-email: andrewshatalov3@gmail.com
 Keywords: clusters clustering short text search new popular topics message thread
 Classifier: Programming Language :: Python
```

### Comparing `SNPTMT-0.0.6/setup.py` & `SNPTMT-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
-version = '0.0.6'
+version = '0.0.7'
 
 setup(
     name='SNPTMT',
     version=version,
 
     author='FIvER4IK',
     author_email='andrewshatalov3@gmail.com',
```

