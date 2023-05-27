# Comparing `tmp/lokii-0.1.8.tar.gz` & `tmp/lokii-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokii-0.1.8.tar", last modified: Fri Mar 25 11:43:42 2022, max compression
+gzip compressed data, was "lokii-1.0.0.tar", last modified: Sat May 27 12:40:34 2023, max compression
```

## Comparing `lokii-0.1.8.tar` & `lokii-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,64 @@
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2022-03-25 11:43:42.326325 lokii-0.1.8/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      695 2022-03-25 11:43:42.326325 lokii-0.1.8/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1451 2022-03-25 11:13:55.000000 lokii-0.1.8/README.md
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2022-03-25 11:43:42.322325 lokii-0.1.8/lokii/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       25 2021-03-01 13:39:35.000000 lokii-0.1.8/lokii/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     5214 2021-10-18 10:29:56.000000 lokii-0.1.8/lokii/lokii.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     7702 2022-03-25 11:43:22.000000 lokii-0.1.8/lokii/table.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      487 2021-03-01 15:18:09.000000 lokii-0.1.8/lokii/utils.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2022-03-25 11:43:42.326325 lokii-0.1.8/lokii.egg-info/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      695 2022-03-25 11:43:42.000000 lokii-0.1.8/lokii.egg-info/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      311 2022-03-25 11:43:42.000000 lokii-0.1.8/lokii.egg-info/SOURCES.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2022-03-25 11:43:42.000000 lokii-0.1.8/lokii.egg-info/dependency_links.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-0.1.8/lokii.egg-info/not-zip-safe
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       14 2022-03-25 11:43:42.000000 lokii-0.1.8/lokii.egg-info/requires.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2022-03-25 11:43:42.000000 lokii-0.1.8/lokii.egg-info/top_level.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       38 2022-03-25 11:43:42.326325 lokii-0.1.8/setup.cfg
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      899 2022-03-25 11:43:39.000000 lokii-0.1.8/setup.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2022-03-25 11:43:42.326325 lokii-0.1.8/tests/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2020-11-25 07:53:42.000000 lokii-0.1.8/tests/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     8210 2021-10-18 10:41:50.000000 lokii-0.1.8/tests/test_lokii.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      877 2021-03-08 12:40:31.000000 lokii-0.1.8/tests/test_table.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-26 20:12:04.000000 lokii-1.0.0/LICENSE
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     5858 2023-05-27 12:40:34.816118 lokii-1.0.0/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4748 2023-05-27 12:36:19.000000 lokii-1.0.0/README.md
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        5 2023-05-26 20:12:04.000000 lokii-1.0.0/VERSION
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.812118 lokii-1.0.0/lokii/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       55 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       78 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/__main__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3224 2023-05-27 12:02:33.000000 lokii-1.0.0/lokii/cli.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2084 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/config.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.812118 lokii-1.0.0/lokii/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2679 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/exec/gen_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.812118 lokii-1.0.0/lokii/logger/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/logger/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1238 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/logger/color.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1756 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/logger/context.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      662 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/logger/formatter.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      639 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/logger/progress.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4201 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/main.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.812118 lokii-1.0.0/lokii/model/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/model/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1514 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/model/gen_module.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/lokii/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      985 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/parse/graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3451 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/parse/node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/lokii/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4330 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/storage/data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      844 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/storage/temp_storage.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/lokii/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1279 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/util/module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      610 2023-05-26 20:12:04.000000 lokii-1.0.0/lokii/util/perf_timer_context.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.812118 lokii-1.0.0/lokii.egg-info/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     5858 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1190 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/SOURCES.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/dependency_links.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       45 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/entry_points.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-1.0.0/lokii.egg-info/not-zip-safe
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      110 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/requires.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2023-05-27 12:40:34.000000 lokii-1.0.0/lokii.egg-info/top_level.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       38 2023-05-27 12:40:34.816118 lokii-1.0.0/setup.cfg
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1852 2023-05-27 12:39:37.000000 lokii-1.0.0/setup.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/tests/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1815 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/conftest.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/tests/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1142 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/exec/test_gen_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/tests/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1474 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/parse/test_graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3920 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/parse/test_node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/tests/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3844 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/storage/test_data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      369 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/storage/test_temp_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4841 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/test_cli.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-05-27 12:40:34.816118 lokii-1.0.0/tests/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1007 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/util/test_module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      629 2023-05-26 20:12:04.000000 lokii-1.0.0/tests/util/test_perf_timer_context.py
```

