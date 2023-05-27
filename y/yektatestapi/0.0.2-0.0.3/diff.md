# Comparing `tmp/yektatestapi-0.0.2.tar.gz` & `tmp/yektatestapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yektatestapi-0.0.2.tar", last modified: Mon Oct  4 16:18:07 2021, max compression
+gzip compressed data, was "yektatestapi-0.0.3.tar", last modified: Sat May 27 17:58:02 2023, max compression
```

## Comparing `yektatestapi-0.0.2.tar` & `yektatestapi-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 alireza    (501) staff       (20)        0 2021-10-04 16:18:07.125023 yektatestapi-0.0.2/
--rw-r--r--   0 alireza    (501) staff       (20)    11541 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/LICENSE
--rw-r--r--   0 alireza    (501) staff       (20)       19 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/MANIFEST.in
--rw-r--r--   0 alireza    (501) staff       (20)      234 2021-10-04 16:18:07.125197 yektatestapi-0.0.2/PKG-INFO
--rw-r--r--   0 alireza    (501) staff       (20)    24776 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/README.md
-drwxr-xr-x   0 alireza    (501) staff       (20)        0 2021-10-04 16:18:07.042033 yektatestapi-0.0.2/kaggle/
--rw-r--r--   0 alireza    (501) staff       (20)      796 2021-10-04 11:33:45.000000 yektatestapi-0.0.2/kaggle/__init__.py
-drwxr-xr-x   0 alireza    (501) staff       (20)        0 2021-10-04 16:18:07.045610 yektatestapi-0.0.2/kaggle/api/
--rw-r--r--   0 alireza    (501) staff       (20)      742 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/api/__init__.py
--rw-r--r--   0 alireza    (501) staff       (20)   125827 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/api/kaggle_api.py
--rw-r--r--   0 alireza    (501) staff       (20)   110616 2021-10-04 08:46:58.000000 yektatestapi-0.0.2/kaggle/api/kaggle_api_extended.py
--rw-r--r--   0 alireza    (501) staff       (20)    25458 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/api_client.py
--rw-r--r--   0 alireza    (501) staff       (20)    53449 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/cli.py
--rw-r--r--   0 alireza    (501) staff       (20)     8858 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/configuration.py
-drwxr-xr-x   0 alireza    (501) staff       (20)        0 2021-10-04 16:18:07.119767 yektatestapi-0.0.2/kaggle/models/
--rw-r--r--   0 alireza    (501) staff       (20)     1481 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/__init__.py
--rw-r--r--   0 alireza    (501) staff       (20)     4851 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/collaborator.py
--rw-r--r--   0 alireza    (501) staff       (20)     7424 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/dataset_column.py
--rw-r--r--   0 alireza    (501) staff       (20)    12317 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/dataset_new_request.py
--rw-r--r--   0 alireza    (501) staff       (20)    10027 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/dataset_new_version_request.py
--rw-r--r--   0 alireza    (501) staff       (20)    10114 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/dataset_update_settings_request.py
--rw-r--r--   0 alireza    (501) staff       (20)     5544 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/dataset_upload_file.py
--rw-r--r--   0 alireza    (501) staff       (20)     4342 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/error.py
--rw-r--r--   0 alireza    (501) staff       (20)    15321 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/file.py
--rw-r--r--   0 alireza    (501) staff       (20)     6193 2021-10-04 16:15:59.000000 yektatestapi-0.0.2/kaggle/models/kaggle_models_extended.py
--rw-r--r--   0 alireza    (501) staff       (20)    18059 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/kernel_push_request.py
--rw-r--r--   0 alireza    (501) staff       (20)     4077 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/license.py
--rw-r--r--   0 alireza    (501) staff       (20)     2895 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/models/result.py
--rw-r--r--   0 alireza    (501) staff       (20)    13927 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/rest.py
-drwxr-xr-x   0 alireza    (501) staff       (20)        0 2021-10-04 16:18:07.121389 yektatestapi-0.0.2/kaggle/tests/
--rw-r--r--   0 alireza    (501) staff       (20)      596 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/tests/__init__.py
--rw-r--r--   0 alireza    (501) staff       (20)     1780 2021-10-03 20:27:23.000000 yektatestapi-0.0.2/kaggle/tests/test_authenticate.py
--rw-r--r--   0 alireza    (501) staff       (20)       79 2021-10-04 16:18:07.125705 yektatestapi-0.0.2/setup.cfg
--rw-r--r--   0 alireza    (501) staff       (20)     1225 2021-10-04 16:16:57.000000 yektatestapi-0.0.2/setup.py
-drwxr-xr-x   0 alireza    (501) staff       (20)        0 2021-10-04 16:18:07.124744 yektatestapi-0.0.2/yektatestapi.egg-info/
--rw-r--r--   0 alireza    (501) staff       (20)      234 2021-10-04 16:18:06.000000 yektatestapi-0.0.2/yektatestapi.egg-info/PKG-INFO
--rw-r--r--   0 alireza    (501) staff       (20)      927 2021-10-04 16:18:06.000000 yektatestapi-0.0.2/yektatestapi.egg-info/SOURCES.txt
--rw-r--r--   0 alireza    (501) staff       (20)        1 2021-10-04 16:18:06.000000 yektatestapi-0.0.2/yektatestapi.egg-info/dependency_links.txt
--rw-r--r--   0 alireza    (501) staff       (20)       44 2021-10-04 16:18:06.000000 yektatestapi-0.0.2/yektatestapi.egg-info/entry_points.txt
--rw-r--r--   0 alireza    (501) staff       (20)       71 2021-10-04 16:18:06.000000 yektatestapi-0.0.2/yektatestapi.egg-info/requires.txt
--rw-r--r--   0 alireza    (501) staff       (20)        7 2021-10-04 16:18:06.000000 yektatestapi-0.0.2/yektatestapi.egg-info/top_level.txt
+drwxr-xr-x   0 alireza    (501) staff       (20)        0 2023-05-27 17:58:02.346026 yektatestapi-0.0.3/
+-rw-r--r--   0 alireza    (501) staff       (20)    11541 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/LICENSE
+-rw-r--r--   0 alireza    (501) staff       (20)       19 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/MANIFEST.in
+-rw-r--r--   0 alireza    (501) staff       (20)      206 2023-05-27 17:58:02.346207 yektatestapi-0.0.3/PKG-INFO
+-rw-r--r--   0 alireza    (501) staff       (20)    24776 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/README.md
+drwxr-xr-x   0 alireza    (501) staff       (20)        0 2023-05-27 17:58:02.321378 yektatestapi-0.0.3/kaggle/
+-rw-r--r--   0 alireza    (501) staff       (20)      796 2021-10-04 11:33:45.000000 yektatestapi-0.0.3/kaggle/__init__.py
+drwxr-xr-x   0 alireza    (501) staff       (20)        0 2023-05-27 17:58:02.325811 yektatestapi-0.0.3/kaggle/api/
+-rw-r--r--   0 alireza    (501) staff       (20)      742 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/api/__init__.py
+-rw-r--r--   0 alireza    (501) staff       (20)   125827 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/api/kaggle_api.py
+-rw-r--r--   0 alireza    (501) staff       (20)   110616 2023-05-27 17:48:27.000000 yektatestapi-0.0.3/kaggle/api/kaggle_api_extended.py
+-rw-r--r--   0 alireza    (501) staff       (20)    25458 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/api_client.py
+-rw-r--r--   0 alireza    (501) staff       (20)    53449 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/cli.py
+-rw-r--r--   0 alireza    (501) staff       (20)     8858 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/configuration.py
+drwxr-xr-x   0 alireza    (501) staff       (20)        0 2023-05-27 17:58:02.341397 yektatestapi-0.0.3/kaggle/models/
+-rw-r--r--   0 alireza    (501) staff       (20)     1481 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/__init__.py
+-rw-r--r--   0 alireza    (501) staff       (20)     4851 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/collaborator.py
+-rw-r--r--   0 alireza    (501) staff       (20)     7424 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/dataset_column.py
+-rw-r--r--   0 alireza    (501) staff       (20)    12317 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/dataset_new_request.py
+-rw-r--r--   0 alireza    (501) staff       (20)    10027 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/dataset_new_version_request.py
+-rw-r--r--   0 alireza    (501) staff       (20)    10114 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/dataset_update_settings_request.py
+-rw-r--r--   0 alireza    (501) staff       (20)     5544 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/dataset_upload_file.py
+-rw-r--r--   0 alireza    (501) staff       (20)     4342 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/error.py
+-rw-r--r--   0 alireza    (501) staff       (20)    15321 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/file.py
+-rw-r--r--   0 alireza    (501) staff       (20)     6193 2021-10-04 16:15:59.000000 yektatestapi-0.0.3/kaggle/models/kaggle_models_extended.py
+-rw-r--r--   0 alireza    (501) staff       (20)    18059 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/kernel_push_request.py
+-rw-r--r--   0 alireza    (501) staff       (20)     4077 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/license.py
+-rw-r--r--   0 alireza    (501) staff       (20)     2895 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/models/result.py
+-rw-r--r--   0 alireza    (501) staff       (20)    13927 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/rest.py
+drwxr-xr-x   0 alireza    (501) staff       (20)        0 2023-05-27 17:58:02.343359 yektatestapi-0.0.3/kaggle/tests/
+-rw-r--r--   0 alireza    (501) staff       (20)      596 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/tests/__init__.py
+-rw-r--r--   0 alireza    (501) staff       (20)     1780 2021-10-03 20:27:23.000000 yektatestapi-0.0.3/kaggle/tests/test_authenticate.py
+-rw-r--r--   0 alireza    (501) staff       (20)       79 2023-05-27 17:58:02.347006 yektatestapi-0.0.3/setup.cfg
+-rw-r--r--   0 alireza    (501) staff       (20)     1224 2023-05-27 17:54:53.000000 yektatestapi-0.0.3/setup.py
+drwxr-xr-x   0 alireza    (501) staff       (20)        0 2023-05-27 17:58:02.345755 yektatestapi-0.0.3/yektatestapi.egg-info/
+-rw-r--r--   0 alireza    (501) staff       (20)      206 2023-05-27 17:58:01.000000 yektatestapi-0.0.3/yektatestapi.egg-info/PKG-INFO
+-rw-r--r--   0 alireza    (501) staff       (20)      927 2023-05-27 17:58:02.000000 yektatestapi-0.0.3/yektatestapi.egg-info/SOURCES.txt
+-rw-r--r--   0 alireza    (501) staff       (20)        1 2023-05-27 17:58:01.000000 yektatestapi-0.0.3/yektatestapi.egg-info/dependency_links.txt
+-rw-r--r--   0 alireza    (501) staff       (20)       43 2023-05-27 17:58:01.000000 yektatestapi-0.0.3/yektatestapi.egg-info/entry_points.txt
+-rw-r--r--   0 alireza    (501) staff       (20)       71 2023-05-27 17:58:01.000000 yektatestapi-0.0.3/yektatestapi.egg-info/requires.txt
+-rw-r--r--   0 alireza    (501) staff       (20)        7 2023-05-27 17:58:01.000000 yektatestapi-0.0.3/yektatestapi.egg-info/top_level.txt
```

### Comparing `yektatestapi-0.0.2/LICENSE` & `yektatestapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/README.md` & `yektatestapi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/__init__.py` & `yektatestapi-0.0.3/kaggle/__init__.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/api/__init__.py` & `yektatestapi-0.0.3/kaggle/api/__init__.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/api/kaggle_api.py` & `yektatestapi-0.0.3/kaggle/api/kaggle_api.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/api/kaggle_api_extended.py` & `yektatestapi-0.0.3/kaggle/api/kaggle_api_extended.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 try:
     unicode  # Python 2
 except NameError:
     unicode = str  # Python 3
 
 
 class KaggleApi(KaggleApi):
-    __version__ = '1.5.12'
+    __version__ = '1.5.13'
 
     CONFIG_NAME_PROXY = 'proxy'
     CONFIG_NAME_COMPETITION = 'competition'
     CONFIG_NAME_PATH = 'path'
     CONFIG_NAME_USER = 'username'
     CONFIG_NAME_KEY = 'key'
     CONFIG_NAME_SSL_CA_CERT = 'ssl_ca_cert'
```

### Comparing `yektatestapi-0.0.2/kaggle/api_client.py` & `yektatestapi-0.0.3/kaggle/api_client.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/cli.py` & `yektatestapi-0.0.3/kaggle/cli.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/configuration.py` & `yektatestapi-0.0.3/kaggle/configuration.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/__init__.py` & `yektatestapi-0.0.3/kaggle/models/__init__.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/collaborator.py` & `yektatestapi-0.0.3/kaggle/models/collaborator.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/dataset_column.py` & `yektatestapi-0.0.3/kaggle/models/dataset_column.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/dataset_new_request.py` & `yektatestapi-0.0.3/kaggle/models/dataset_new_request.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/dataset_new_version_request.py` & `yektatestapi-0.0.3/kaggle/models/dataset_new_version_request.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/dataset_update_settings_request.py` & `yektatestapi-0.0.3/kaggle/models/dataset_update_settings_request.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/dataset_upload_file.py` & `yektatestapi-0.0.3/kaggle/models/dataset_upload_file.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/error.py` & `yektatestapi-0.0.3/kaggle/models/error.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/file.py` & `yektatestapi-0.0.3/kaggle/models/file.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/kaggle_models_extended.py` & `yektatestapi-0.0.3/kaggle/models/kaggle_models_extended.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/kernel_push_request.py` & `yektatestapi-0.0.3/kaggle/models/kernel_push_request.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/license.py` & `yektatestapi-0.0.3/kaggle/models/license.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/models/result.py` & `yektatestapi-0.0.3/kaggle/models/result.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/rest.py` & `yektatestapi-0.0.3/kaggle/rest.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/tests/__init__.py` & `yektatestapi-0.0.3/kaggle/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/kaggle/tests/test_authenticate.py` & `yektatestapi-0.0.3/kaggle/tests/test_authenticate.py`

 * *Files identical despite different names*

### Comparing `yektatestapi-0.0.2/setup.py` & `yektatestapi-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 # limitations under the License.
 
 # coding=utf-8
 from setuptools import setup, find_packages
 
 setup(
     name='yektatestapi',
-    version='0.0.2',
+    version='0.0.3',
     description='test API',
     long_description=
     ('my first python test API.'),
-    author='Kaggle',
+    author='yekta',
     author_email='yekta1@live.com',
     keywords=['test', 'API'],
     entry_points={'console_scripts': ['kaggle = kaggle.cli:main']},
     install_requires=[
         'six >= 1.10',
         'certifi',
         'python-dateutil',
```

### Comparing `yektatestapi-0.0.2/yektatestapi.egg-info/SOURCES.txt` & `yektatestapi-0.0.3/yektatestapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

