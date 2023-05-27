# Comparing `tmp/apache-airflow-providers-ftp-3.4.1.tar.gz` & `tmp/apache-airflow-providers-ftp-3.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-ftp-3.4.1.tar", last modified: Wed May 24 07:13:58 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-ftp-3.4.1rc1.tar", last modified: Wed May 24 07:20:26 2023, max compression
```

## Comparing `apache-airflow-providers-ftp-3.4.1.tar` & `apache-airflow-providers-ftp-3.4.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:13:58.000000 apache-airflow-providers-ftp-3.4.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:13:55.000000 apache-airflow-providers-ftp-3.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9966 2023-05-24 07:13:58.000000 apache-airflow-providers-ftp-3.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8400 2023-05-24 07:13:55.000000 apache-airflow-providers-ftp-3.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:13:57.000000 apache-airflow-providers-ftp-3.4.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:13:57.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:13:57.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/
--rw-r--r--   0 root         (0) root         (0)     1528 2023-05-24 07:09:22.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-05-24 07:13:55.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:13:58.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9842 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/hooks/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:13:58.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6093 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/operators/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:13:58.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/sensors/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:13:58.000000 apache-airflow-providers-ftp-3.4.1/apache_airflow_providers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9966 2023-05-24 07:13:57.000000 apache-airflow-providers-ftp-3.4.1/apache_airflow_providers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-24 07:13:57.000000 apache-airflow-providers-ftp-3.4.1/apache_airflow_providers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:13:57.000000 apache-airflow-providers-ftp-3.4.1/apache_airflow_providers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-24 07:13:57.000000 apache-airflow-providers-ftp-3.4.1/apache_airflow_providers_ftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:13:57.000000 apache-airflow-providers-ftp-3.4.1/apache_airflow_providers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 07:13:57.000000 apache-airflow-providers-ftp-3.4.1/apache_airflow_providers_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:13:57.000000 apache-airflow-providers-ftp-3.4.1/apache_airflow_providers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1842 2023-05-24 07:13:58.000000 apache-airflow-providers-ftp-3.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1620 2023-05-24 07:13:55.000000 apache-airflow-providers-ftp-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9972 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8403 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-05-24 07:09:22.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9842 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6093 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9972 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-ftp-3.4.1/LICENSE` & `apache-airflow-providers-ftp-3.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/MANIFEST.in` & `apache-airflow-providers-ftp-3.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/PKG-INFO` & `apache-airflow-providers-ftp-3.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.4.1
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-ftp-3.4.1/README.rst` & `apache-airflow-providers-ftp-3.4.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/__init__.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/get_provider_info.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/hooks/__init__.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/hooks/ftp.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/operators/__init__.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/operators/ftp.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/sensors/__init__.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/airflow/providers/ftp/sensors/ftp.py` & `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/apache_airflow_providers_ftp.egg-info/PKG-INFO` & `apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.4.1
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-ftp-3.4.1/apache_airflow_providers_ftp.egg-info/SOURCES.txt` & `apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/pyproject.toml` & `apache-airflow-providers-ftp-3.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1/setup.cfg` & `apache-airflow-providers-ftp-3.4.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.ftp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.ftp
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-ftp-3.4.1/setup.py` & `apache-airflow-providers-ftp-3.4.1rc1/setup.py`

 * *Files identical despite different names*

