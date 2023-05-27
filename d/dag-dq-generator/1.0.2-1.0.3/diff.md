# Comparing `tmp/dag-dq-generator-1.0.2.tar.gz` & `tmp/dag-dq-generator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dag-dq-generator-1.0.2.tar", last modified: Fri May 19 18:27:44 2023, max compression
+gzip compressed data, was "dist/dag-dq-generator-1.0.3.tar", last modified: Sat May 27 18:20:32 2023, max compression
```

## Comparing `dag-dq-generator-1.0.2.tar` & `dag-dq-generator-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.499572 dag-dq-generator-1.0.2/
--rw-r--r--   0 hnankam    (501) staff       (20)     1790 2023-05-19 18:23:03.000000 dag-dq-generator-1.0.2/CHANGELOG.md
--rw-r--r--   0 hnankam    (501) staff       (20)     1080 2022-08-03 15:58:08.000000 dag-dq-generator-1.0.2/LICENSE
--rw-r--r--   0 hnankam    (501) staff       (20)      133 2022-09-19 21:54:41.000000 dag-dq-generator-1.0.2/MANIFEST.in
--rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-05-19 18:27:44.498938 dag-dq-generator-1.0.2/PKG-INFO
--rw-r--r--   0 hnankam    (501) staff       (20)     1382 2023-05-10 03:45:14.000000 dag-dq-generator-1.0.2/README.md
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.480163 dag-dq-generator-1.0.2/dag_dq_generator/
--rw-r--r--   0 hnankam    (501) staff       (20)       74 2022-09-19 21:34:24.000000 dag-dq-generator-1.0.2/dag_dq_generator/__init__.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.485912 dag-dq-generator-1.0.2/dag_dq_generator/__pycache__/
--rw-r--r--   0 hnankam    (501) staff       (20)      226 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.2/dag_dq_generator/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 hnankam    (501) staff       (20)      154 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.2/dag_dq_generator/__pycache__/__version__.cpython-38.pyc
--rw-r--r--   0 hnankam    (501) staff       (20)       90 2023-05-19 16:59:44.000000 dag-dq-generator-1.0.2/dag_dq_generator/__version__.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.488755 dag-dq-generator-1.0.2/dag_dq_generator/configs/
--rw-r--r--   0 hnankam    (501) staff       (20)     6537 2022-11-09 02:56:39.000000 dag-dq-generator-1.0.2/dag_dq_generator/configs/sample.yml
--rw-r--r--   0 hnankam    (501) staff       (20)     3383 2022-11-04 20:33:28.000000 dag-dq-generator-1.0.2/dag_dq_generator/configs/stage_sample.yml
--rw-r--r--   0 hnankam    (501) staff       (20)    11149 2023-05-12 18:41:55.000000 dag-dq-generator-1.0.2/dag_dq_generator/dag_generator.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.491365 dag-dq-generator-1.0.2/dag_dq_generator/dags/
--rw-r--r--   0 hnankam    (501) staff       (20)    16788 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.2/dag_dq_generator/dags/demo-dev-01.py
--rw-r--r--   0 hnankam    (501) staff       (20)     8727 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.2/dag_dq_generator/dags/stage_test_001.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.496123 dag-dq-generator-1.0.2/dag_dq_generator/templates/
--rw-r--r--   0 hnankam    (501) staff       (20)     7482 2023-05-17 22:52:00.000000 dag-dq-generator-1.0.2/dag_dq_generator/templates/_global_macros.py
--rw-r--r--   0 hnankam    (501) staff       (20)    17900 2023-05-17 22:49:36.000000 dag-dq-generator-1.0.2/dag_dq_generator/templates/dag_template.py
--rw-r--r--   0 hnankam    (501) staff       (20)    16800 2023-05-09 23:28:44.000000 dag-dq-generator-1.0.2/dag_dq_generator/templates/dq_sql_template.sql
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.498269 dag-dq-generator-1.0.2/dag_dq_generator/tests/
--rw-r--r--   0 hnankam    (501) staff       (20)        0 2022-09-19 18:15:00.000000 dag-dq-generator-1.0.2/dag_dq_generator/tests/__init__.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.484387 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/
--rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/PKG-INFO
--rw-r--r--   0 hnankam    (501) staff       (20)      878 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/SOURCES.txt
--rw-r--r--   0 hnankam    (501) staff       (20)        1 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/dependency_links.txt
--rw-r--r--   0 hnankam    (501) staff       (20)       71 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/entry_points.txt
--rw-r--r--   0 hnankam    (501) staff       (20)        1 2022-09-20 16:35:26.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/not-zip-safe
--rw-r--r--   0 hnankam    (501) staff       (20)      125 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/requires.txt
--rw-r--r--   0 hnankam    (501) staff       (20)       17 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/top_level.txt
--rw-r--r--   0 hnankam    (501) staff       (20)      124 2023-05-13 17:36:49.000000 dag-dq-generator-1.0.2/requirements.txt
--rw-r--r--   0 hnankam    (501) staff       (20)       38 2023-05-19 18:27:44.499818 dag-dq-generator-1.0.2/setup.cfg
--rw-r--r--   0 hnankam    (501) staff       (20)     1632 2023-05-17 22:52:05.000000 dag-dq-generator-1.0.2/setup.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.841430 dag-dq-generator-1.0.3/
+-rw-r--r--   0 hnankam    (501) staff       (20)     1874 2023-05-27 18:18:39.000000 dag-dq-generator-1.0.3/CHANGELOG.md
+-rw-r--r--   0 hnankam    (501) staff       (20)     1080 2022-08-03 15:58:08.000000 dag-dq-generator-1.0.3/LICENSE
+-rw-r--r--   0 hnankam    (501) staff       (20)      133 2022-09-19 21:54:41.000000 dag-dq-generator-1.0.3/MANIFEST.in
+-rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-05-27 18:20:32.841167 dag-dq-generator-1.0.3/PKG-INFO
+-rw-r--r--   0 hnankam    (501) staff       (20)     1382 2023-05-10 03:45:14.000000 dag-dq-generator-1.0.3/README.md
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.835477 dag-dq-generator-1.0.3/dag_dq_generator/
+-rw-r--r--   0 hnankam    (501) staff       (20)       74 2022-09-19 21:34:24.000000 dag-dq-generator-1.0.3/dag_dq_generator/__init__.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.838253 dag-dq-generator-1.0.3/dag_dq_generator/__pycache__/
+-rw-r--r--   0 hnankam    (501) staff       (20)      226 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.3/dag_dq_generator/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 hnankam    (501) staff       (20)      154 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.3/dag_dq_generator/__pycache__/__version__.cpython-38.pyc
+-rw-r--r--   0 hnankam    (501) staff       (20)       90 2023-05-26 15:14:47.000000 dag-dq-generator-1.0.3/dag_dq_generator/__version__.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.838843 dag-dq-generator-1.0.3/dag_dq_generator/configs/
+-rw-r--r--   0 hnankam    (501) staff       (20)     6537 2022-11-09 02:56:39.000000 dag-dq-generator-1.0.3/dag_dq_generator/configs/sample.yml
+-rw-r--r--   0 hnankam    (501) staff       (20)     3383 2022-11-04 20:33:28.000000 dag-dq-generator-1.0.3/dag_dq_generator/configs/stage_sample.yml
+-rw-r--r--   0 hnankam    (501) staff       (20)    11298 2023-05-26 15:13:19.000000 dag-dq-generator-1.0.3/dag_dq_generator/dag_generator.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.839505 dag-dq-generator-1.0.3/dag_dq_generator/dags/
+-rw-r--r--   0 hnankam    (501) staff       (20)    16788 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.3/dag_dq_generator/dags/demo-dev-01.py
+-rw-r--r--   0 hnankam    (501) staff       (20)     8727 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.3/dag_dq_generator/dags/stage_test_001.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.840449 dag-dq-generator-1.0.3/dag_dq_generator/templates/
+-rw-r--r--   0 hnankam    (501) staff       (20)     7482 2023-05-17 22:52:00.000000 dag-dq-generator-1.0.3/dag_dq_generator/templates/_global_macros.py
+-rw-r--r--   0 hnankam    (501) staff       (20)    17900 2023-05-17 22:49:36.000000 dag-dq-generator-1.0.3/dag_dq_generator/templates/dag_template.py
+-rw-r--r--   0 hnankam    (501) staff       (20)    17835 2023-05-26 15:01:56.000000 dag-dq-generator-1.0.3/dag_dq_generator/templates/dq_sql_template.sql
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.840819 dag-dq-generator-1.0.3/dag_dq_generator/tests/
+-rw-r--r--   0 hnankam    (501) staff       (20)        0 2022-09-19 18:15:00.000000 dag-dq-generator-1.0.3/dag_dq_generator/tests/__init__.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.837655 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/
+-rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/PKG-INFO
+-rw-r--r--   0 hnankam    (501) staff       (20)      878 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)        1 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)       71 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/entry_points.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)        1 2022-09-20 16:35:26.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/not-zip-safe
+-rw-r--r--   0 hnankam    (501) staff       (20)      125 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/requires.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)       17 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/top_level.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)      124 2023-05-13 17:36:49.000000 dag-dq-generator-1.0.3/requirements.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)       38 2023-05-27 18:20:32.841522 dag-dq-generator-1.0.3/setup.cfg
+-rw-r--r--   0 hnankam    (501) staff       (20)     1632 2023-05-17 22:52:05.000000 dag-dq-generator-1.0.3/setup.py
```

### Comparing `dag-dq-generator-1.0.2/CHANGELOG.md` & `dag-dq-generator-1.0.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.3] - 2023-05-27
+
+### Major changes
+- Added DQ SQL support for struct types
+
 ## [1.0.2] - 2023-05-19
 
 ### Major changes
 - Enabled pip integration with Adobe Artifactory and PyPI. dag-generator can now be installed using `pip install dag-dq-generator`. Please visit the [documentation](https://wiki.corp.adobe.com/pages/viewpage.action?pageId=2849653154#Implementation&Use-Setup&Installation) for more information
 
 ### New features
 - Feature: Added support for `TableauOperator` for connecting to Tableau for data refresh. Please visit the [documentation](https://wiki.corp.adobe.com/pages/viewpage.action?pageId=2849653154#Implementation&Use-TableauOperator) for more information
```

### Comparing `dag-dq-generator-1.0.2/LICENSE` & `dag-dq-generator-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.2/PKG-INFO` & `dag-dq-generator-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dag-dq-generator
-Version: 1.0.2
+Version: 1.0.3
 Summary: DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator
 Home-page: https://git.corp.adobe.com/ccea/dag-dq-generator
 Author: CI DMe Data Engineering
 Author-email: ccea-data-engineering@adobe.com
 License: MIT
 Description: # dag-dq-generator
         DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator.
```

### Comparing `dag-dq-generator-1.0.2/README.md` & `dag-dq-generator-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.2/dag_dq_generator/configs/sample.yml` & `dag-dq-generator-1.0.3/dag_dq_generator/configs/sample.yml`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.2/dag_dq_generator/configs/stage_sample.yml` & `dag-dq-generator-1.0.3/dag_dq_generator/configs/stage_sample.yml`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.2/dag_dq_generator/dag_generator.py` & `dag-dq-generator-1.0.3/dag_dq_generator/dag_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,23 +145,23 @@
         # Create DQ sub directory
         sql_subdir = os.path.join(DQ_STORAGE_PATH, config['pipeline_settings']['dbx_base_path'].lstrip('/'))
         os.makedirs(sql_subdir, exist_ok=True)
         
         for dq in config['data_quality']:
 
             _dimensions = dq['key_dimensions']
-            _group_set = _dimensions
+            _group_set = [dimension.split('.')[-1] for dimension in _dimensions]
 
             if 'grouping_level' in dq and isinstance(dq['grouping_level'], int):
 
                 if dq['grouping_level'] == 2:
-                    _group_set = _group_set + [f'({_dimensions[i]}, {_dimensions[j]})' for i in range(0, len(_dimensions)) for j in range(i + 1, len(_dimensions))]
+                    _group_set = _group_set + [f"({_dimensions[i].split('.')[-1]}, {_dimensions[j].split('.')[-1]})" for i in range(0, len(_dimensions)) for j in range(i + 1, len(_dimensions))]
                 elif dq['grouping_level'] == 3:
-                    _group_set = _group_set + [f'({_dimensions[i]}, {_dimensions[j]})' for i in range(0, len(_dimensions)) for j in range(i + 1, len(_dimensions))] + \
-                                              [f'({_dimensions[i]}, {_dimensions[j]}, {_dimensions[k]})' for i in range(0, len(_dimensions)) for j in range(i + 1, len(_dimensions)) for k in range(j + 1, len(_dimensions))]
+                    _group_set = _group_set + [f"({_dimensions[i].split('.')[-1]}, {_dimensions[j].split('.')[-1]})" for i in range(0, len(_dimensions)) for j in range(i + 1, len(_dimensions))] + \
+                                              [f"({_dimensions[i].split('.')[-1]}, {_dimensions[j].split('.')[-1]}, {_dimensions[k].split('.')[-1]})" for i in range(0, len(_dimensions)) for j in range(i + 1, len(_dimensions)) for k in range(j + 1, len(_dimensions))]
                 
             dq['group_set'] = _group_set
 
             sql_filename = os.path.join(sql_subdir, config['pipeline_settings']['dag_name']+ '_' + dq['id'] + '_metric.sql')
             
             # Render template to file
             with open(sql_filename, "w") as f:  # Replaces file if already exists
```

### Comparing `dag-dq-generator-1.0.2/dag_dq_generator/dags/demo-dev-01.py` & `dag-dq-generator-1.0.3/dag_dq_generator/dags/demo-dev-01.py`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.2/dag_dq_generator/dags/stage_test_001.py` & `dag-dq-generator-1.0.3/dag_dq_generator/dags/stage_test_001.py`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.2/dag_dq_generator/templates/_global_macros.py` & `dag-dq-generator-1.0.3/dag_dq_generator/templates/_global_macros.py`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.2/dag_dq_generator/templates/dag_template.py` & `dag-dq-generator-1.0.3/dag_dq_generator/templates/dag_template.py`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.2/dag_dq_generator/templates/dq_sql_template.sql` & `dag-dq-generator-1.0.3/dag_dq_generator/templates/dq_sql_template.sql`

 * *Files 13% similar despite different names*

```diff
@@ -104,89 +104,89 @@
     {%- endif %}
 
 ), table_metrics AS (
 
               SELECT 1 ID, 'num_count'          AS metric_name
     -- Key dimension metrics
     {% for kd in key_dimensions -%}
-    UNION ALL SELECT 1 ID, 'num_dist_{{kd}}'    AS metric_name
-    UNION ALL SELECT 1 ID, 'count_null_{{kd}}'  AS metric_name
+    UNION ALL SELECT 1 ID, 'num_dist_{{kd.split('.')[-1]}}'    AS metric_name
+    UNION ALL SELECT 1 ID, 'count_null_{{kd.split('.')[-1]}}'  AS metric_name
     {% endfor %}
     -- Key measures metrics
     {% for km in key_measures -%}
-    UNION ALL SELECT 1 ID, 'sum_{{km}}'  AS metric_name
-    UNION ALL SELECT 1 ID, 'avg_{{km}}'  AS metric_name
-    UNION ALL SELECT 1 ID, 'max_{{km}}'  AS metric_name
-    UNION ALL SELECT 1 ID, 'min_{{km}}'  AS metric_name
-    UNION ALL SELECT 1 ID, 'std_{{km}}'  AS metric_name
+    UNION ALL SELECT 1 ID, 'sum_{{km.split('.')[-1]}}'  AS metric_name
+    UNION ALL SELECT 1 ID, 'avg_{{km.split('.')[-1]}}'  AS metric_name
+    UNION ALL SELECT 1 ID, 'max_{{km.split('.')[-1]}}'  AS metric_name
+    UNION ALL SELECT 1 ID, 'min_{{km.split('.')[-1]}}'  AS metric_name
+    UNION ALL SELECT 1 ID, 'std_{{km.split('.')[-1]}}'  AS metric_name
     {% endfor %}
 ), dim_metrics AS (
 
               SELECT 1 ID, 'num_count'   AS metric_name
     {% for km in key_measures -%}
-    UNION ALL SELECT 1 ID, 'sum_{{km}}'  AS metric_name
-    UNION ALL SELECT 1 ID, 'avg_{{km}}'  AS metric_name
-    UNION ALL SELECT 1 ID, 'max_{{km}}'  AS metric_name
-    UNION ALL SELECT 1 ID, 'min_{{km}}'  AS metric_name
-    UNION ALL SELECT 1 ID, 'std_{{km}}'  AS metric_name
+    UNION ALL SELECT 1 ID, 'sum_{{km.split('.')[-1]}}'  AS metric_name
+    UNION ALL SELECT 1 ID, 'avg_{{km.split('.')[-1]}}'  AS metric_name
+    UNION ALL SELECT 1 ID, 'max_{{km.split('.')[-1]}}'  AS metric_name
+    UNION ALL SELECT 1 ID, 'min_{{km.split('.')[-1]}}'  AS metric_name
+    UNION ALL SELECT 1 ID, 'std_{{km.split('.')[-1]}}'  AS metric_name
     {% endfor %}
 ), table_stats AS (
 
     SELECT 
         1           AS ID
         , COUNT(*)                                             AS num_count
         -- All the key dimensions
         {% for kd in key_dimensions -%}
-        , COUNT(DISTINCT({{kd}}))                             AS num_dist_{{kd}}
-        , SUM(CASE WHEN {{kd}} IS NULL THEN 1 ELSE 0 END)     AS count_null_{{kd}}
+        , COUNT(DISTINCT({{kd.split('.')[-1]}}))                             AS num_dist_{{kd.split('.')[-1]}}
+        , SUM(CASE WHEN {{kd.split('.')[-1]}} IS NULL THEN 1 ELSE 0 END)     AS count_null_{{kd.split('.')[-1]}}
         {% endfor %}
         -- All the key measures
         {% for km in key_measures -%}
-        , SUM({{km}}) AS sum_{{km}}
-        , AVG({{km}}) AS avg_{{km}}
-        , MAX({{km}}) AS max_{{km}}
-        , MIN({{km}}) AS min_{{km}}
-        , STDDEV({{km}}) AS std_{{km}}
+        , SUM({{km.split('.')[-1]}}) AS sum_{{km.split('.')[-1]}}
+        , AVG({{km.split('.')[-1]}}) AS avg_{{km.split('.')[-1]}}
+        , MAX({{km.split('.')[-1]}}) AS max_{{km.split('.')[-1]}}
+        , MIN({{km.split('.')[-1]}}) AS min_{{km.split('.')[-1]}}
+        , STDDEV({{km.split('.')[-1]}}) AS std_{{km.split('.')[-1]}}
         {% endfor %}
         {% if partition %}, {{partition.col_name}} {%- endif %}
     FROM source_data
     {% if partition %}GROUP BY {{partition.col_name}} {%- endif %}
 
 ), _clean_source_data AS (
 
     SELECT 
-          CASE WHEN {{key_dimensions[0]}} IS NULL THEN '__na__' ELSE STRING({{key_dimensions[0]}}) END AS {{key_dimensions[0]}}
+          CASE WHEN {{key_dimensions[0]}} IS NULL THEN '__na__' ELSE STRING({{key_dimensions[0]}}) END AS {{key_dimensions[0].split('.')[-1]}}
         {% for kd in key_dimensions[1:] -%}
-        , CASE WHEN {{kd}} IS NULL THEN '__na__' ELSE STRING({{kd}}) END AS {{kd}}
+        , CASE WHEN {{kd.split('.')[-1]}} IS NULL THEN '__na__' ELSE STRING({{kd.split('.')[-1]}}) END AS {{kd.split('.')[-1]}}
         {% endfor %}
         {%- for km in key_measures -%}
-        , {{km}}
+        , {{km.split('.')[-1]}}
         {% endfor %}
         {%- if partition %}, {{partition.col_name}} {%- endif %}
     FROM source_data
 
 ), dimensional_stats AS (
 
     SELECT 
         1                           AS ID
         , MAP_CONCAT( -- in reality, due to cleanup above, will dimensions will never be null
-            CASE WHEN {{key_dimensions[0]}} IS NOT NULL THEN MAP('{{key_dimensions[0]}}', {{key_dimensions[0]}}) ELSE MAP() END
+            CASE WHEN {{key_dimensions[0]}} IS NOT NULL THEN MAP('{{key_dimensions[0].split('.')[-1]}}', {{key_dimensions[0]}}) ELSE MAP() END
             {% for kd in key_dimensions[1:] -%}
-            , CASE WHEN {{kd}} IS NOT NULL THEN MAP('{{kd}}', {{kd}}) ELSE MAP() END
+            , CASE WHEN {{kd.split('.')[-1]}} IS NOT NULL THEN MAP('{{kd.split('.')[-1]}}', {{kd.split('.')[-1]}}) ELSE MAP() END
             {% endfor %}
         ) AS dim_val
         , COUNT(*) num_count
         
         -- All the key measures
         {% for km in key_measures -%}
-        , SUM({{km}}) AS sum_{{km}}
-        , AVG({{km}}) AS avg_{{km}}
-        , MAX({{km}}) AS max_{{km}}
-        , MIN({{km}}) AS min_{{km}}
-        , STDDEV({{km}}) AS std_{{km}}
+        , SUM({{km.split('.')[-1]}}) AS sum_{{km.split('.')[-1]}}
+        , AVG({{km.split('.')[-1]}}) AS avg_{{km.split('.')[-1]}}
+        , MAX({{km.split('.')[-1]}}) AS max_{{km.split('.')[-1]}}
+        , MIN({{km.split('.')[-1]}}) AS min_{{km.split('.')[-1]}}
+        , STDDEV({{km.split('.')[-1]}}) AS std_{{km.split('.')[-1]}}
         {% endfor %}
         {% if partition %}, {{partition.col_name}} {%- endif %}
     FROM _clean_source_data
     --GROUP BY CUBE({{', '.join(key_dimensions)}}){% if partition %}, {{partition.col_name}} {%- endif %}
     GROUP BY GROUPING SETS({{', '.join(group_set)}}){% if partition %}, {{partition.col_name}} {%- endif %}
 
 )
@@ -204,24 +204,24 @@
     SELECT
         '{{source_table}}'          AS metric_source_table,
         metric_name                         AS metric_name,
         CASE WHEN metric_name = 'num_count'                   THEN num_count
 
             -- All the key dimensions
             {%- for kd in key_dimensions %}
-            WHEN metric_name = 'num_dist_{{kd}}'     THEN num_dist_{{kd}}
-            WHEN metric_name = 'count_null_{{kd}}'   THEN count_null_{{kd}}
+            WHEN metric_name = 'num_dist_{{kd.split('.')[-1]}}'     THEN num_dist_{{kd.split('.')[-1]}}
+            WHEN metric_name = 'count_null_{{kd.split('.')[-1]}}'   THEN count_null_{{kd.split('.')[-1]}}
             {%- endfor %}
             -- All the key measures
             {%- for km in key_measures %}
-            WHEN metric_name = 'sum_{{km}}'          THEN sum_{{km}}
-            WHEN metric_name = 'avg_{{km}}'          THEN avg_{{km}}
-            WHEN metric_name = 'max_{{km}}'          THEN max_{{km}}
-            WHEN metric_name = 'min_{{km}}'          THEN min_{{km}}
-            WHEN metric_name = 'std_{{km}}'          THEN std_{{km}}
+            WHEN metric_name = 'sum_{{km.split('.')[-1]}}'          THEN sum_{{km.split('.')[-1]}}
+            WHEN metric_name = 'avg_{{km.split('.')[-1]}}'          THEN avg_{{km.split('.')[-1]}}
+            WHEN metric_name = 'max_{{km.split('.')[-1]}}'          THEN max_{{km.split('.')[-1]}}
+            WHEN metric_name = 'min_{{km.split('.')[-1]}}'          THEN min_{{km.split('.')[-1]}}
+            WHEN metric_name = 'std_{{km.split('.')[-1]}}'          THEN std_{{km.split('.')[-1]}}
             {%- endfor %}
 
         END                                 AS metric_value,
         NULL                                AS metric_dimensions,
         '{{period_type}}'                   AS metric_calc_period_type,
         CURRENT_TIMESTAMP                   AS metric_calc_dttm,
         {% if partition -%} 
@@ -242,19 +242,19 @@
     UNION ALL
 
     SELECT
         '{{source_table}}'          AS metric_source_table,
         metric_name                 AS metric_name,
         CASE WHEN metric_name = 'num_count'       THEN num_count
             {%- for km in key_measures %}
-            WHEN metric_name = 'sum_{{km}}'          THEN sum_{{km}}
-            WHEN metric_name = 'avg_{{km}}'          THEN avg_{{km}}
-            WHEN metric_name = 'max_{{km}}'          THEN max_{{km}}
-            WHEN metric_name = 'min_{{km}}'          THEN min_{{km}}
-            WHEN metric_name = 'std_{{km}}'          THEN std_{{km}}
+            WHEN metric_name = 'sum_{{km.split('.')[-1]}}'          THEN sum_{{km.split('.')[-1]}}
+            WHEN metric_name = 'avg_{{km.split('.')[-1]}}'          THEN avg_{{km.split('.')[-1]}}
+            WHEN metric_name = 'max_{{km.split('.')[-1]}}'          THEN max_{{km.split('.')[-1]}}
+            WHEN metric_name = 'min_{{km.split('.')[-1]}}'          THEN min_{{km.split('.')[-1]}}
+            WHEN metric_name = 'std_{{km.split('.')[-1]}}'          THEN std_{{km.split('.')[-1]}}
             {%- endfor %}
         END                                 AS metric_value,
         dim_val                             AS metric_dimensions,
         '{{period_type}}'                   AS metric_calc_period_type,
         CURRENT_TIMESTAMP                   AS metric_calc_dttm,
         {% if partition -%} 
         {{partition.col_name}}
```

### Comparing `dag-dq-generator-1.0.2/dag_dq_generator.egg-info/PKG-INFO` & `dag-dq-generator-1.0.3/dag_dq_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dag-dq-generator
-Version: 1.0.2
+Version: 1.0.3
 Summary: DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator
 Home-page: https://git.corp.adobe.com/ccea/dag-dq-generator
 Author: CI DMe Data Engineering
 Author-email: ccea-data-engineering@adobe.com
 License: MIT
 Description: # dag-dq-generator
         DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator.
```

### Comparing `dag-dq-generator-1.0.2/dag_dq_generator.egg-info/SOURCES.txt` & `dag-dq-generator-1.0.3/dag_dq_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.2/setup.py` & `dag-dq-generator-1.0.3/setup.py`

 * *Files identical despite different names*

