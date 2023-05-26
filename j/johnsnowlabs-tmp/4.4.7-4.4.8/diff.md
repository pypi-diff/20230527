# Comparing `tmp/johnsnowlabs_tmp-4.4.7.tar.gz` & `tmp/johnsnowlabs_tmp-4.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs_tmp-4.4.7.tar", last modified: Thu May 25 05:48:38 2023, max compression
+gzip compressed data, was "johnsnowlabs_tmp-4.4.8.tar", last modified: Fri May 26 06:24:33 2023, max compression
```

## Comparing `johnsnowlabs_tmp-4.4.7.tar` & `johnsnowlabs_tmp-4.4.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-25 05:48:38.447944 johnsnowlabs_tmp-4.4.7/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs_tmp-4.4.7/LICENSE
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9282 2023-05-25 05:48:38.447944 johnsnowlabs_tmp-4.4.7/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs_tmp-4.4.7/README.md
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-25 05:48:38.439944 johnsnowlabs_tmp-4.4.7/johnsnowlabs/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-25 05:48:38.439944 johnsnowlabs_tmp-4.4.7/johnsnowlabs/abstract_base/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/abstract_base/software_product.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-25 05:48:38.443944 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-25 05:48:38.443944 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-25 05:48:38.443944 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/jsl_home.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-25 05:48:38.443944 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-05-25 04:21:48.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-05-25 02:23:06.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/offline_install.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9133 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4710 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/finance.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/lab.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4639 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/legal.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4528 2023-05-25 02:41:08.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/medical.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/nlp.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-25 05:48:38.443944 johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2201 2023-05-25 05:48:08.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/settings.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-25 05:48:38.443944 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4253 2023-04-26 21:13:04.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8127 2023-05-21 06:35:03.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/sparksession_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-25 05:48:38.447944 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/testing/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/visual.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs/viz.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-25 05:48:38.447944 johnsnowlabs_tmp-4.4.7/johnsnowlabs_tmp.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9282 2023-05-25 05:48:38.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs_tmp.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2486 2023-05-25 05:48:38.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs_tmp.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-25 05:48:38.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs_tmp.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      111 2023-05-25 05:48:38.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs_tmp.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-05-25 05:48:38.000000 johnsnowlabs_tmp-4.4.7/johnsnowlabs_tmp.egg-info/top_level.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-05-25 05:48:38.447944 johnsnowlabs_tmp-4.4.7/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2045 2023-05-25 05:47:59.000000 johnsnowlabs_tmp-4.4.7/setup.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.630854 johnsnowlabs_tmp-4.4.8/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11356 2023-03-31 15:38:35.000000 johnsnowlabs_tmp-4.4.8/LICENSE
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9282 2023-05-26 06:24:33.630854 johnsnowlabs_tmp-4.4.8/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8307 2023-03-31 15:38:35.000000 johnsnowlabs_tmp-4.4.8/README.md
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      932 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      395 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9775 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      733 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9287 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/software_product.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2623 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12144 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6612 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      973 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      884 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2076 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3496 2023-03-30 22:32:50.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6935 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11362 2023-02-01 13:41:22.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12079 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/jsl_home.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      124 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2061 2023-05-25 04:21:48.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3187 2023-05-25 02:23:06.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2105 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9118 2023-05-16 20:30:52.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/offline_install.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9182 2023-05-26 06:23:57.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4710 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/finance.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      212 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/lab.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4639 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/legal.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4528 2023-05-25 02:41:08.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/medical.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1367 2023-04-13 01:03:52.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/nlp.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4826 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    31165 2023-03-26 01:30:02.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4168 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        2 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      128 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2077 2023-05-16 20:23:18.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2233 2023-05-26 06:24:30.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/settings.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.626854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:26:15.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6657 2023-03-31 10:39:36.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4253 2023-04-26 21:13:04.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      759 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1005 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3326 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10004 2023-03-19 17:22:02.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10654 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5856 2023-01-31 09:04:19.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      982 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4371 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8127 2023-05-21 06:35:03.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/sparksession_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.630854 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2022-12-09 17:29:40.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4050 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1778 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1132 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3460 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4353 2023-04-26 21:13:04.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1332 2023-04-26 14:30:28.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/visual.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      408 2023-01-31 08:59:14.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs/viz.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-26 06:24:33.630854 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9282 2023-05-26 06:24:33.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2486 2023-05-26 06:24:33.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-26 06:24:33.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      114 2023-05-26 06:24:33.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       13 2023-05-26 06:24:33.000000 johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/top_level.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-05-26 06:24:33.630854 johnsnowlabs_tmp-4.4.8/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2045 2023-05-25 05:47:59.000000 johnsnowlabs_tmp-4.4.8/setup.py
```

### Comparing `johnsnowlabs_tmp-4.4.7/LICENSE` & `johnsnowlabs_tmp-4.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/PKG-INFO` & `johnsnowlabs_tmp-4.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs_tmp
-Version: 4.4.7
+Version: 4.4.8
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs_tmp-4.4.7/README.md` & `johnsnowlabs_tmp-4.4.8/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/__init__.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/auto_install/softwares.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,18 @@
     hard_dependencies = {SparkNlpSoftware}
     licensed_dependencies = {SparkHcSoftware, SparkOcrSoftware}
     optional_dependencies = {
         NlpDisplaySoftware
     }  # Todo streamlit,sklearn,plotly, nlp-display
     latest_version = LatestCompatibleProductVersion.nlu.value
     py_module_name = "nlu"
-    pypi_name = "nlu"
+    # pypi_name = "nlu"
+    pypi_name = "nlu_tmp"
+    # nlu_tmp==
+
     install_deps = False
 
     @classmethod
     def get_installed_version_via_import(cls):
         try:
             import nlu
 
@@ -216,15 +219,15 @@
 
     hard_dependencies = {SparkNlpSoftware}
     licensed_dependencies = {SparkHcSoftware, SparkOcrSoftware}
     optional_dependencies = {NlpDisplaySoftware, NluSoftware}
     latest_version = LatestCompatibleProductVersion.jsl_lib.value
     py_module_name = "johnsnowlabs"
     pypi_name = "johnsnowlabs"
-    pypi_name_databricks = "johnsnowlabs_for_databricks"
+    pypi_name_databricks = "johnsnowlabs_for_databricks_tmp"
 
 
 class JslFullSoftware(AbstractSoftwareProduct):
     name = ProductName.jsl_full.value
     logo = ProductLogo.jsl_full.value
     slogan = ProductSlogan.jsl_full.value
```

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/finance.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/finance.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/legal.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/legal.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/medical.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/medical.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/nlp.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/settings.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from johnsnowlabs.utils.env_utils import (
     is_running_in_databricks,
     set_py4j_logger_to_error_on_databricks,
     env_required_license,
 )
 
 # These versions are used for auto-installs and version  checks
-raw_version_jsl_lib = "4.4.7"
+raw_version_jsl_lib = "4.4.8"
 raw_version_nlp = "4.4.1"
-raw_version_nlu = "4.2.0"
+# raw_version_nlu = "4.2.0"
+raw_version_nlu = "4.3.0rc3"
+
 raw_version_pyspark = "3.1.2"
 raw_version_nlp_display = "4.1"
 
 raw_version_medical = "4.4.2"
 raw_version_secret_medical = "4.4.2"
 
 raw_version_secret_ocr = "4.4.1"
```

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/enums.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/functional.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/py_process.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs/visual.py` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs_tmp.egg-info/PKG-INFO` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs-tmp
-Version: 4.4.7
+Version: 4.4.8
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `johnsnowlabs_tmp-4.4.7/johnsnowlabs_tmp.egg-info/SOURCES.txt` & `johnsnowlabs_tmp-4.4.8/johnsnowlabs_tmp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_tmp-4.4.7/setup.py` & `johnsnowlabs_tmp-4.4.8/setup.py`

 * *Files identical despite different names*

