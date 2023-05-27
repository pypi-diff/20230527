# Comparing `tmp/autogluon.common-0.7.1b20230526.tar.gz` & `tmp/autogluon.common-0.7.1b20230527.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.common-0.7.1b20230526.tar", last modified: Fri May 26 09:03:43 2023, max compression
+gzip compressed data, was "autogluon.common-0.7.1b20230527.tar", last modified: Sat May 27 09:03:44 2023, max compression
```

## Comparing `autogluon.common-0.7.1b20230526.tar` & `autogluon.common-0.7.1b20230527.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:43.319340 autogluon.common-0.7.1b20230526/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-26 09:03:43.319340 autogluon.common-0.7.1b20230526/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:03:43.319340 autogluon.common-0.7.1b20230526/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:43.311339 autogluon.common-0.7.1b20230526/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:43.311339 autogluon.common-0.7.1b20230526/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:43.315340 autogluon.common-0.7.1b20230526/src/autogluon/common/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:43.315340 autogluon.common-0.7.1b20230526/src/autogluon/common/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/features/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/features/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/features/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:43.315340 autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:43.315340 autogluon.common-0.7.1b20230526/src/autogluon/common/savers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/savers/save_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/savers/save_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/savers/save_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/savers/save_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/savers/save_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:43.319340 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/deprecated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/distribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/nvutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/resource_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-26 09:03:32.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 09:03:42.000000 autogluon.common-0.7.1b20230526/src/autogluon/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:43.315340 autogluon.common-0.7.1b20230526/src/autogluon.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-26 09:03:43.000000 autogluon.common-0.7.1b20230526/src/autogluon.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-26 09:03:43.000000 autogluon.common-0.7.1b20230526/src/autogluon.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:03:43.000000 autogluon.common-0.7.1b20230526/src/autogluon.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 09:03:43.000000 autogluon.common-0.7.1b20230526/src/autogluon.common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 09:03:43.000000 autogluon.common-0.7.1b20230526/src/autogluon.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 09:03:43.000000 autogluon.common-0.7.1b20230526/src/autogluon.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:03:43.000000 autogluon.common-0.7.1b20230526/src/autogluon.common.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:44.391023 autogluon.common-0.7.1b20230527/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-27 09:03:44.387025 autogluon.common-0.7.1b20230527/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:03:44.391023 autogluon.common-0.7.1b20230527/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:44.383026 autogluon.common-0.7.1b20230527/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:44.383026 autogluon.common-0.7.1b20230527/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:44.387025 autogluon.common-0.7.1b20230527/src/autogluon/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:44.387025 autogluon.common-0.7.1b20230527/src/autogluon/common/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/features/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/features/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/features/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:44.387025 autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:44.387025 autogluon.common-0.7.1b20230527/src/autogluon/common/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/savers/save_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/savers/save_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/savers/save_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/savers/save_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/savers/save_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:44.387025 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/deprecated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/distribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/nvutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/resource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-27 09:03:34.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-27 09:03:44.000000 autogluon.common-0.7.1b20230527/src/autogluon/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:44.387025 autogluon.common-0.7.1b20230527/src/autogluon.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-27 09:03:44.000000 autogluon.common-0.7.1b20230527/src/autogluon.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-27 09:03:44.000000 autogluon.common-0.7.1b20230527/src/autogluon.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:03:44.000000 autogluon.common-0.7.1b20230527/src/autogluon.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 09:03:44.000000 autogluon.common-0.7.1b20230527/src/autogluon.common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-27 09:03:44.000000 autogluon.common-0.7.1b20230527/src/autogluon.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 09:03:44.000000 autogluon.common-0.7.1b20230527/src/autogluon.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:03:44.000000 autogluon.common-0.7.1b20230527/src/autogluon.common.egg-info/zip-safe
```

### Comparing `autogluon.common-0.7.1b20230526/LICENSE` & `autogluon.common-0.7.1b20230527/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/PKG-INFO` & `autogluon.common-0.7.1b20230527/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230526
+Version: 0.7.1b20230527
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230526/setup.py` & `autogluon.common-0.7.1b20230527/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/features/feature_metadata.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/features/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/features/infer_types.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/features/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/features/types.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/features/types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/_utils.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_pd.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_pkl.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_pointer.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_pointer.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_s3.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_s3.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_str.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/loaders/load_zip.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/loaders/load_zip.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/savers/save_json.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/savers/save_json.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/savers/save_pd.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/savers/save_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/savers/save_pkl.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/savers/save_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/savers/save_str.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/savers/save_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/space.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/compression_utils.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/compression_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/deprecated_utils.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/deprecated_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/distribute_utils.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/file_utils.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/log_utils.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/multiprocessing_utils.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/nvutil.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/nvutil.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/pandas_utils.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/resource_utils.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/resource_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,29 +27,15 @@
         return psutil.cpu_count(logical=logical)
 
     @staticmethod
     @disable_if_lite_mode(ret=0)
     def get_gpu_count_all():
         num_gpus = ResourceManager._get_gpu_count_cuda()
         if num_gpus == 0:
-            # Get num gpus from mxnet first because of https://github.com/autogluon/autogluon/issues/2042
-            # TODO: stop using mxnet to determine num gpus once mxnet is removed from AG
-            num_gpus = ResourceManager.get_gpu_count_mxnet()
-            if num_gpus == 0:
-                num_gpus = ResourceManager.get_gpu_count_torch()
-        return num_gpus
-
-    @staticmethod
-    def get_gpu_count_mxnet():
-        # TODO: Remove this once AG get rid off mxnet
-        try:
-            import mxnet
-            num_gpus = mxnet.context.num_gpus()
-        except Exception:
-            num_gpus = 0
+            num_gpus = ResourceManager.get_gpu_count_torch()
         return num_gpus
 
     @staticmethod
     def get_gpu_count_torch():
         try:
             import torch
             num_gpus = torch.cuda.device_count()
@@ -119,15 +105,15 @@
         Returns obj with variables `free`, `total`, `used`, representing bytes as integers.
         """
         return shutil.disk_usage(path=path)
 
     @staticmethod
     def _get_gpu_count_cuda():
         # FIXME: Sometimes doesn't detect GPU on Windows
-        # FIXME: Doesn't ensure the GPUs are actually usable by the model (MXNet, PyTorch, etc.)
+        # FIXME: Doesn't ensure the GPUs are actually usable by the model (PyTorch, etc.)
         from .nvutil import cudaInit, cudaDeviceGetCount, cudaShutdown
         if not cudaInit(): return 0
         gpu_count = cudaDeviceGetCount()
         cudaShutdown()
         return gpu_count
```

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/s3_utils.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/try_import.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/try_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from types import ModuleType
 
 from ..version import __version__
 
 __all__ = [
     'try_import_mxboard',
-    'try_import_mxnet',
     'try_import_catboost',
     'try_import_lightgbm',
     'try_import_xgboost',
     'try_import_faiss',
     'try_import_fastai',
     'try_import_torch',
     'try_import_d8',
@@ -28,35 +27,14 @@
     try:
         import mxboard
     except ImportError:
         raise ImportError(
             "Unable to import dependency mxboard. "
             "A quick tip is to install via `pip install mxboard`. ")
 
-
-def try_import_mxnet():
-    mx_version = '1.6.0'
-    try:
-        import mxnet as mx
-        from packaging import version
-
-        if version.parse(mx.__version__) < version.parse(mx_version):
-            msg = (
-                "Legacy mxnet=={} detected, some new modules will not work properly. "
-                "mxnet>={} is required. You can use pip to upgrade mxnet "
-                "`pip install mxnet --upgrade` "
-                "or `pip install mxnet_cu101 --upgrade`").format(mx.__version__, mx_version)
-            raise ValueError(msg)
-    except ImportError:
-        raise ImportError(
-            "Unable to import dependency mxnet. "
-            "A quick tip is to install via `pip install mxnet --upgrade`, "
-            "or `pip install mxnet_cu101 --upgrade`")
-
-
 def try_import_ray() -> ModuleType:
     RAY_MAX_VERSION = '2.4.0'
     ray_max_version_os_map = dict(
         Darwin=RAY_MAX_VERSION,
         Windows=RAY_MAX_VERSION,
         Linux=RAY_MAX_VERSION,
     )
```

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon/common/utils/utils.py` & `autogluon.common-0.7.1b20230527/src/autogluon/common/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon.common.egg-info/PKG-INFO` & `autogluon.common-0.7.1b20230527/src/autogluon.common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230526
+Version: 0.7.1b20230527
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230526/src/autogluon.common.egg-info/SOURCES.txt` & `autogluon.common-0.7.1b20230527/src/autogluon.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

