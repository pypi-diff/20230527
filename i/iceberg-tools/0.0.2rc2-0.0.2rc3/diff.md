# Comparing `tmp/iceberg_tools-0.0.2rc2.tar.gz` & `tmp/iceberg_tools-0.0.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceberg_tools-0.0.2rc2.tar", last modified: Fri May 26 00:30:26 2023, max compression
+gzip compressed data, was "iceberg_tools-0.0.2rc3.tar", last modified: Fri May 26 23:16:19 2023, max compression
```

## Comparing `iceberg_tools-0.0.2rc2.tar` & `iceberg_tools-0.0.2rc3.tar`

### file list

```diff
@@ -1,73 +1,77 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.309278 iceberg_tools-0.0.2rc2/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2862 2023-05-26 00:30:26.308979 iceberg_tools-0.0.2rc2/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     2126 2023-05-26 00:28:26.000000 iceberg_tools-0.0.2rc2/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.170302 iceberg_tools-0.0.2rc2/iceberg_tools/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-12 16:19:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.175709 iceberg_tools-0.0.2rc2/iceberg_tools/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142      482 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc2/iceberg_tools/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4423 2023-05-25 22:36:19.000000 iceberg_tools-0.0.2rc2/iceberg_tools/cli/data.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5607 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc2/iceberg_tools/cli/schema.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.192399 iceberg_tools-0.0.2rc2/iceberg_tools/data/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-25 15:58:53.000000 iceberg_tools-0.0.2rc2/iceberg_tools/data/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.192783 iceberg_tools-0.0.2rc2/iceberg_tools/data/migrator/
--rw-r--r--   0 walsbr   (320923486) 1971611142    12270 2023-05-25 22:13:53.000000 iceberg_tools-0.0.2rc2/iceberg_tools/data/migrator/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6137 2023-05-25 19:18:02.000000 iceberg_tools-0.0.2rc2/iceberg_tools/data/pfb.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.193969 iceberg_tools-0.0.2rc2/iceberg_tools/data/simplifier/
--rw-r--r--   0 walsbr   (320923486) 1971611142    25714 2023-05-25 22:21:05.000000 iceberg_tools-0.0.2rc2/iceberg_tools/data/simplifier/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142   123504 2023-05-23 18:08:13.000000 iceberg_tools-0.0.2rc2/iceberg_tools/data/simplifier/oid_lookup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.196129 iceberg_tools-0.0.2rc2/iceberg_tools/schema/
--rw-r--r--   0 walsbr   (320923486) 1971611142     9512 2023-05-25 19:25:02.000000 iceberg_tools-0.0.2rc2/iceberg_tools/schema/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1348 2023-05-13 22:22:19.000000 iceberg_tools-0.0.2rc2/iceberg_tools/schema/bmeg.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    19847 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc2/iceberg_tools/schema/gen3.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4157 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc2/iceberg_tools/schema/gen3_validator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6840 2023-05-25 15:57:02.000000 iceberg_tools-0.0.2rc2/iceberg_tools/util.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.174693 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2862 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     2140 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       84 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      146 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       20 2023-05-26 00:30:26.000000 iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-05-26 00:30:26.309360 iceberg_tools-0.0.2rc2/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5751 2023-05-26 00:29:56.000000 iceberg_tools-0.0.2rc2/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.157916 iceberg_tools-0.0.2rc2/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.196574 iceberg_tools-0.0.2rc2/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-13 20:01:03.000000 iceberg_tools-0.0.2rc2/tests/integration/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.282095 iceberg_tools-0.0.2rc2/tests/integration/bmeg/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1834 2023-05-15 20:39:46.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      967 2023-05-15 20:24:40.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      782 2023-05-15 20:39:22.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_edge_load_granular_reference.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2736 2023-05-15 20:39:04.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_edge_validator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1449 2023-05-15 20:38:41.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_invalid_edges.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      255 2023-05-15 20:24:59.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_lathe_lint.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      662 2023-05-15 20:38:23.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_negative_trivial_vertex_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      829 2023-05-23 20:22:18.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_schema.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      330 2023-05-13 20:02:59.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_schema_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1140 2023-05-15 20:38:10.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_spot_check_embedded_type.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      731 2023-05-15 20:37:50.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_trivial_edge_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      888 2023-05-15 20:37:28.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_trivial_vertex_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      340 2023-05-13 20:02:59.000000 iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_yaml_anonymous_schemas.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.288288 iceberg_tools-0.0.2rc2/tests/integration/data/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-23 23:15:41.000000 iceberg_tools-0.0.2rc2/tests/integration/data/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4897 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc2/tests/integration/data/test_pfb.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.306702 iceberg_tools-0.0.2rc2/tests/integration/gen3/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-12 18:03:42.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      616 2023-05-18 20:08:55.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      911 2023-05-15 20:20:57.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_codeable_concept.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      451 2023-05-15 20:17:07.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_embedded_types.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-14 12:07:10.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_identifiers.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      171 2023-05-12 18:57:49.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_individual_yaml.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      275 2023-05-12 18:56:56.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_keys.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      979 2023-05-23 19:23:34.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_primitive.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      469 2023-05-15 20:06:10.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_quantities.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      517 2023-05-18 20:10:27.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_research_study_has_project.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      155 2023-05-24 00:59:54.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_schema.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1832 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_simplify_medication.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1744 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_simplify_task.py
--rw-r--r--   0 walsbr   (320923486) 1971611142       34 2023-05-18 20:08:09.000000 iceberg_tools-0.0.2rc2/tests/integration/gen3/test_task.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 00:30:26.308466 iceberg_tools-0.0.2rc2/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-13 20:01:24.000000 iceberg_tools-0.0.2rc2/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      176 2023-05-15 20:40:27.000000 iceberg_tools-0.0.2rc2/tests/unit/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 iceberg_tools-0.0.2rc2/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3144 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc2/tests/unit/test_schema.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1080 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc2/tests/unit/test_simplify.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.065983 iceberg_tools-0.0.2rc3/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2940 2023-05-26 23:16:19.065744 iceberg_tools-0.0.2rc3/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2204 2023-05-26 23:14:20.000000 iceberg_tools-0.0.2rc3/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.021742 iceberg_tools-0.0.2rc3/iceberg_tools/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-12 16:19:26.000000 iceberg_tools-0.0.2rc3/iceberg_tools/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.034784 iceberg_tools-0.0.2rc3/iceberg_tools/cli/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      482 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc3/iceberg_tools/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6024 2023-05-26 23:00:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools/cli/data.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5048 2023-05-26 23:02:49.000000 iceberg_tools-0.0.2rc3/iceberg_tools/cli/schema.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.036178 iceberg_tools-0.0.2rc3/iceberg_tools/data/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-25 15:58:53.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.036641 iceberg_tools-0.0.2rc3/iceberg_tools/data/migrator/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13714 2023-05-26 19:23:29.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/migrator/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6137 2023-05-25 19:18:02.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/pfb.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3530 2023-05-26 23:02:01.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/report.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.037595 iceberg_tools-0.0.2rc3/iceberg_tools/data/simplifier/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    26369 2023-05-26 21:11:37.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/simplifier/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142   123504 2023-05-23 18:08:13.000000 iceberg_tools-0.0.2rc3/iceberg_tools/data/simplifier/oid_lookup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.039401 iceberg_tools-0.0.2rc3/iceberg_tools/schema/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11116 2023-05-26 16:55:34.000000 iceberg_tools-0.0.2rc3/iceberg_tools/schema/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1348 2023-05-13 22:22:19.000000 iceberg_tools-0.0.2rc3/iceberg_tools/schema/bmeg.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    20425 2023-05-26 15:19:47.000000 iceberg_tools-0.0.2rc3/iceberg_tools/schema/gen3.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4157 2023-05-25 21:03:15.000000 iceberg_tools-0.0.2rc3/iceberg_tools/schema/gen3_validator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6840 2023-05-25 15:57:02.000000 iceberg_tools-0.0.2rc3/iceberg_tools/util.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.027235 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2940 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2263 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       84 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      146 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       20 2023-05-26 23:16:18.000000 iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-05-26 23:16:19.066059 iceberg_tools-0.0.2rc3/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5751 2023-05-26 23:06:27.000000 iceberg_tools-0.0.2rc3/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.008616 iceberg_tools-0.0.2rc3/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.039748 iceberg_tools-0.0.2rc3/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-13 20:01:03.000000 iceberg_tools-0.0.2rc3/tests/integration/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.058505 iceberg_tools-0.0.2rc3/tests/integration/bmeg/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1834 2023-05-15 20:39:46.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      967 2023-05-15 20:24:40.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      782 2023-05-15 20:39:22.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_edge_load_granular_reference.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2736 2023-05-15 20:39:04.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_edge_validator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1449 2023-05-15 20:38:41.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_invalid_edges.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      255 2023-05-15 20:24:59.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_lathe_lint.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      662 2023-05-15 20:38:23.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_negative_trivial_vertex_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      829 2023-05-23 20:22:18.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_schema.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      330 2023-05-13 20:02:59.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_schema_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1140 2023-05-15 20:38:10.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_spot_check_embedded_type.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      731 2023-05-15 20:37:50.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_trivial_edge_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      888 2023-05-15 20:37:28.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_trivial_vertex_load.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      340 2023-05-13 20:02:59.000000 iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_yaml_anonymous_schemas.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.060159 iceberg_tools-0.0.2rc3/tests/integration/data/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-23 23:15:41.000000 iceberg_tools-0.0.2rc3/tests/integration/data/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      305 2023-05-26 22:58:19.000000 iceberg_tools-0.0.2rc3/tests/integration/data/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5374 2023-05-26 22:55:04.000000 iceberg_tools-0.0.2rc3/tests/integration/data/test_pfb.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.063699 iceberg_tools-0.0.2rc3/tests/integration/gen3/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-12 18:03:42.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      616 2023-05-18 20:08:55.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      911 2023-05-15 20:20:57.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_codeable_concept.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      451 2023-05-15 20:17:07.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_embedded_types.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-14 12:07:10.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_identifiers.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      171 2023-05-12 18:57:49.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_individual_yaml.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      275 2023-05-12 18:56:56.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_keys.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      979 2023-05-23 19:23:34.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_primitive.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      469 2023-05-15 20:06:10.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_quantities.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      517 2023-05-18 20:10:27.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_research_study_has_project.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      155 2023-05-24 00:59:54.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_schema.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1832 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_simplify_medication.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1744 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_simplify_task.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142       34 2023-05-18 20:08:09.000000 iceberg_tools-0.0.2rc3/tests/integration/gen3/test_task.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.064178 iceberg_tools-0.0.2rc3/tests/integration/simplifier/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-26 14:08:42.000000 iceberg_tools-0.0.2rc3/tests/integration/simplifier/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1080 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc3/tests/integration/simplifier/test_simplify.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-26 23:16:19.065384 iceberg_tools-0.0.2rc3/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-13 20:01:24.000000 iceberg_tools-0.0.2rc3/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      176 2023-05-15 20:40:27.000000 iceberg_tools-0.0.2rc3/tests/unit/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 iceberg_tools-0.0.2rc3/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3144 2023-05-25 23:13:19.000000 iceberg_tools-0.0.2rc3/tests/unit/test_schema.py
```

### Comparing `iceberg_tools-0.0.2rc2/PKG-INFO` & `iceberg_tools-0.0.2rc3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceberg_tools
-Version: 0.0.2rc2
+Version: 0.0.2rc3
 Summary: FHIR schemas tools for bioinformatics.
 Home-page: https://github.com/bmeg/iceberg-schema-tools
 Author: https://ellrottlab.org/
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bmeg/iceberg-schema-tools/issues
 Project-URL: Source, https://github.com/bmeg/iceberg-schema-tools
 Keywords: FHIR PFB gen3 bioinformatics graph
@@ -18,15 +18,16 @@
 Description-Content-Type: text/markdown
 
 # iceberg-schema-tools
 Create and maintain central iceberg schema.  Render and validate FHIR data.
 
 ## Overview
 
-![image](docs/figure-5.png)
+![image](https://github.com/bmeg/iceberg-schema-tools/assets/47808/cf5f544c-081f-470f-b1d8-27f16ad21b67)
+
 
 
 Code that generates the base schema from FHIR goes here.  Additional tools are provided to lints, validates and visualize the schema.
 
 Note: The actual schemas are stored in [iceberg](https://github.com/bmeg/iceberg)
```

### Comparing `iceberg_tools-0.0.2rc2/README.md` & `iceberg_tools-0.0.2rc3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # iceberg-schema-tools
 Create and maintain central iceberg schema.  Render and validate FHIR data.
 
 ## Overview
 
-![image](docs/figure-5.png)
+![image](https://github.com/bmeg/iceberg-schema-tools/assets/47808/cf5f544c-081f-470f-b1d8-27f16ad21b67)
+
 
 
 Code that generates the base schema from FHIR goes here.  Additional tools are provided to lints, validates and visualize the schema.
 
 Note: The actual schemas are stored in [iceberg](https://github.com/bmeg/iceberg)
```

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools/cli/data.py` & `iceberg_tools-0.0.2rc3/iceberg_tools/cli/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import logging
 import pathlib
 import threading
 import uuid
 
 import click
+import yaml
 from fhir.resources import FHIRAbstractModel  # noqa
+from yaml import SafeLoader
 
+from iceberg_tools.data.report import aggregate_edges
 from iceberg_tools.data.migrator import migrate_directory
 from iceberg_tools.data.pfb import SimplePFBWriter
 from iceberg_tools.data.simplifier import cli as simplifier
 from iceberg_tools.schema.gen3_validator import directory_reader as gen3_directory_reader
 from iceberg_tools.util import NaturalOrderGroup, directory_reader
 
 LINKS = threading.local()
@@ -81,24 +84,41 @@
 @click.argument('path')
 @click.argument('output_path')
 @click.option('--schema_path', required=True,
               default='iceberg/schemas/gen3/aced.json',
               show_default=True,
               help='Path to gen3 schema json, a file path or url'
               )
-def pfb(path, output_path, schema_path):
+@click.option('--config_path',
+              default='config.yaml',
+              show_default=True,
+              help='Path to config file.')
+def pfb(path, output_path, schema_path, config_path):
 
     """Write simplified FHIR files to a PFB.
 
     \b
-    PATH: Path to simplified FHIR ndjson files.
-    OUTPUT_PATH: Path where to the PFB
+    PATH: Directory path to simplified FHIR ndjson files.
+    OUTPUT_PATH: File path where to write the PFB.
     """
+    path = pathlib.Path(path)
+    output_path = pathlib.Path(output_path)
+    config_path = pathlib.Path(config_path)
+    assert output_path.is_dir(), f"Path {output_path} is not a directory"
+    assert config_path.is_file(), f"Path {config_path} is not a file"
+    assert path.is_file(), f"Path {path} is not a file"
+
+    with open(config_path) as fp:
+        gen3_config = yaml.load(fp, SafeLoader)
+    dependency_order = gen3_config['dependency_order']
+
     pfb_writer = SimplePFBWriter(schema_path=schema_path,
-                                 output_path=output_path)
+                                 output_path=output_path,
+                                 dependency_order=dependency_order
+                                 )
 
     # this is a generator, needs to be consumed
     [_ for _ in pfb_writer.transform_directory(path)]
 
     inspection = pfb_writer.inspect()
     if len(inspection.errors) > 0:
         logger.error(inspection.warnings)
@@ -108,17 +128,19 @@
         for _ in inspection.info:
             logger.info(_)
 
 
 @cli.command('migrate')
 @click.argument('path')
 @click.argument('output_path')
-@click.option('--validate', default=True, is_flag=True, show_default=True,
+@click.option('--validate/--no-validate', default=True, is_flag=True, show_default=True,
               help="Validate after migration")
-def migrate(path, output_path, validate):
+@click.option('--pattern', required=True, default="**/*.*json", show_default=True,
+              help='File name pattern')
+def migrate(path, output_path, validate, pattern):
     """Migrate from FHIR R4B to R5.0.
 
 
     We solely focus on migrating the necessary migrations for the encountered data, without undertaking a comprehensive migration process.
     Please refer to repository for more details: https://github.com/bmeg/iceberg-schema-tools
 
     PATH: Path containing bundles (*.json) or resources (*.ndjson)
@@ -130,12 +152,28 @@
     assert path.is_dir(), f"Path {path} is not a directory"
 
     if not output_path.exists():
         output_path.mkdir(parents=True, exist_ok=True)
 
     assert output_path.is_dir(), f"Path {output_path} is not a directory"
 
-    migrate_directory(path, output_path, validate)
+    migrate_directory(path, output_path, validate, pattern)
+
+
+@cli.command()
+@click.argument('path')
+@click.argument('output_path')
+@click.option('--pattern', default='**/*.avro', help='Search pattern', show_default=True)
+def report(path: str,  output_path: str,  pattern: str):
+    """Aggregate avro pfb files into a cytoscape friendly tsv.
+
+    \b
+    PATH: Directory path to search for pfb files
+    OUTPUT_PATH: Directory path to write the report TSVs
+    """
+    assert pathlib.Path(path).is_dir(), f"Path {path} is not a directory"
+    assert pathlib.Path(output_path).is_dir(), f"Path {output_path} is not a directory"
+    aggregate_edges(path, output_path, pattern)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools/cli/schema.py` & `iceberg_tools-0.0.2rc3/iceberg_tools/cli/schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,25 +32,27 @@
               show_default=True,
               help='Path to generated schema files'
               )
 @click.option('--config_path',
               default='config.yaml',
               show_default=True,
               help='Path to config file.')
-def generate_bmeg(output_path, config_path):
+@click.option('--stats/--no-stats', default=True, is_flag=True, show_default=True,
+              help="Log statistics about the FHIR classes found.")
+def generate_bmeg(output_path, config_path, stats):
     """Create BMEG schemas."""
 
     output_path = pathlib.Path(output_path)
     config_path = pathlib.Path(config_path)
     assert output_path.is_dir()
     assert config_path.is_file()
     with open(config_path) as fp:
         gen3_config = yaml.load(fp, SafeLoader)
 
-    classes = _find_fhir_classes(gen3_config)
+    classes = _find_fhir_classes(gen3_config, log_stats=stats)
     schemas = _extract_schemas(classes, BASE_URI)
 
     output_path.mkdir(parents=True, exist_ok=True)
 
     for klass, schema in schemas.items():
         with open(output_path / pathlib.Path(klass + ".yaml"), "w") as fp:
             yaml.dump(schema, fp)
@@ -70,38 +72,40 @@
               default='config.yaml',
               show_default=True,
               help='Path to config file.')
 @click.option('--gen3_fixtures',
               default='resources/static_gen3_fixtures',
               show_default=True,
               help='Path to gen3 static data dictionary files.')
+@click.option('--stats/--no-stats', default=True, is_flag=True, show_default=True,
+              help="Log statistics about the FHIR classes found.")
 # @click.option('--cytoscape_output_path', required=True,
 #               default='iceberg/docs',
 #               show_default=True,
 #               help='Path to generated docs'
 #               )
 # @click.option('--generate_edge_schemas',
 #               default=False,
 #               show_default=True,
 #               help='Generate specialized Edge schemas.')
-def generate_gen3(output_path, config_path, gen3_fixtures):
+def generate_gen3(output_path, config_path, gen3_fixtures, stats):
     """Create Gen3 schemas."""
 
     output_path = pathlib.Path(output_path)
     config_path = pathlib.Path(config_path)
     gen3_fixtures = pathlib.Path(gen3_fixtures)
     assert gen3_fixtures.is_dir()
     assert output_path.is_dir()
     assert config_path.is_file()
     with open(config_path) as fp:
         gen3_config = yaml.load(fp, SafeLoader)
 
-    classes = _find_fhir_classes(gen3_config)
+    classes = _find_fhir_classes(gen3_config, log_stats=stats)
     schemas = _extract_schemas(classes, BASE_URI)
-    schemas = _simplify_schemas(gen3_config, gen3_fixtures, schemas)
+    schemas = _simplify_schemas(gen3_config, gen3_fixtures, schemas, log_stats=stats)
 
     # also write out yaml files
     for k, v in schemas.items():
 
         fn = k
         if not k.startswith('_') and 'id' in v:
             fn = v['id']
@@ -139,28 +143,7 @@
               help='Path to generated schema files'
               )
 def compile_gen3(output_path):
     """Compile Gen3 schemas."""
     output_path = pathlib.Path(output_path)
     compile_gen3_schemas(output_path)
     logger.info(f'Gen3 schemas written to {output_path / pathlib.Path("aced.json")}')
-
-
-@cli.command(name='publish')
-@click.argument('dictionary_path', default='iceberg/schemas/gen3/aced.json')
-@click.option('--bucket', default="s3://aced-public", help="Bucket target", show_default=True)
-@click.option('--production', default=False, is_flag=True, show_default=True,
-              help="Write to aced.json, otherwise aced-test.json")
-def schema_publish(dictionary_path, bucket, production):
-    """Copy dictionary to s3 (note:aws cli dependency)"""
-
-    dictionary_path = pathlib.Path(dictionary_path)
-    assert dictionary_path.is_file(), f"{dictionary_path} should be a path"
-    click.echo(f"Writing schema into {bucket}")
-    import subprocess
-    if production:
-        cmd = f"aws s3 cp {dictionary_path} {bucket}".split(' ')
-    else:
-        cmd = f"aws s3 cp {dictionary_path} {bucket}/aced-test.json".split(' ')
-    s3_cp = subprocess.run(cmd)
-    assert s3_cp.returncode == 0, s3_cp
-    print("OK")
```

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools/data/migrator/__init__.py` & `iceberg_tools-0.0.2rc3/iceberg_tools/data/migrator/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,18 +37,33 @@
     migrate_observation(resource, resource_type)
     migrate_medication_administration(resource, resource_type)
     migrate_research_subject(resource, resource_type)
     migrate_research_study(resource, resource_type)
     migrate_practitioner_role(resource, resource_type)
     migrate_specimen(resource, resource_type)
     migrate_organization(resource, resource_type)
+    migrate_location(resource, resource_type)
 
     return resource
 
 
+def migrate_location(resource, resource_type):
+    """Migrate Location resource to 5.0"""
+    if resource_type == "Location":
+        contact_0 = {}
+        if 'address' in resource:
+            contact_0['address'] = resource['address']
+            del resource['address']
+        if 'telecom' in resource:
+            contact_0['telecom'] = resource['telecom']
+            del resource['telecom']
+        if len(contact_0.keys()) > 0:
+            resource['contact'] = [contact_0]
+
+
 def migrate_organization(resource, resource_type):
     """Migrate Organization resource to 5.0"""
     if resource_type == "Organization":
         contact_0 = {}
         if 'address' in resource:
             contact_0['address'] = resource['address'][0]
             del resource['address']
@@ -83,18 +98,22 @@
     if resource_type == "Encounter":
         resource['class'] = [
             {
                 'coding': [resource['class']]
             }
         ]
         for _ in resource['participant']:
-            _['actor'] = _['individual']
-            del _['individual']
-        resource['actualPeriod'] = resource['period']
-        del resource['period']
+            if 'individual' in _:
+                _['actor'] = _['individual']
+                del _['individual']
+
+        if 'period' in resource:
+            resource['actualPeriod'] = resource['period']
+            del resource['period']
+
         if 'reasonCode' in resource:
             resource['reason'] = [{'use': resource['reasonCode']}]
             del resource['reasonCode']
         if 'hospitalization' in resource:
             resource['admission'] = resource['hospitalization']
             del resource['hospitalization']
 
@@ -114,34 +133,38 @@
 
 
 def migrate_observation(resource, resource_type):
     """Migrate Observation resource to 5.0"""
     if resource_type == "Observation":
         _ = resource.get('valueSampledData', None)
         if _:
-            _['intervalUnit'] = '/s'
-            _['interval'] = _['period']
-            del _['period']
+            if 'period' in _:
+                _['intervalUnit'] = '/s'
+                _['interval'] = _['period']
+                del _['period']
         if 'status' not in resource:
             resource['status'] = 'final'
 
 
 def migrate_medication_administration(resource, resource_type):
     """Migrate MedicationAdministration resource to 5.0"""
     if resource_type == "MedicationAdministration":
-        resource['occurenceDateTime'] = resource['effectiveDateTime']
-        del resource['effectiveDateTime']
-
-        resource['medication'] = {
-            'concept': resource['medicationCodeableConcept']
-        }
-        del resource['medicationCodeableConcept']
+        if 'effectiveDateTime' in resource:
+            resource['occurenceDateTime'] = resource['effectiveDateTime']
+            del resource['effectiveDateTime']
+
+        if 'medicationCodeableConcept' in resource:
+            resource['medication'] = {
+                'concept': resource['medicationCodeableConcept']
+            }
+            del resource['medicationCodeableConcept']
 
-        resource['encounter'] = resource['context']
-        del resource['context']
+        if 'context' in resource:
+            resource['encounter'] = resource['context']
+            del resource['context']
 
         if 'reasonReference' in resource:
             resource['reason'] = [{'reference': _} for _ in resource['reasonReference']]
             del resource['reasonReference']
 
 
 def migrate_research_subject(resource, resource_type):
@@ -233,85 +256,97 @@
 
 
 def _is_resource(resource):
     """Return True if resource is a FHIR resource."""
     return 'resourceType' in resource
 
 
-def migrate_bundles(output_path, path, validate):
+def migrate_bundles(output_path, path, validate, pattern='**/*.json'):
     """Migrate bundles."""
-    for input_file in path.glob('**/*.json'):   # TODO: see util directory_reader
+    for input_file in path.glob(pattern):   # TODO: see util directory_reader
         with open(input_file, "rb") as fp:
             resource = orjson.loads(fp.read())
             if not _is_resource(resource):
                 logger.warning(f"Not a FHIR resource {input_file}")
                 continue
             if not _is_bundle(resource):
+                logger.warning(f"Not a bundle {input_file}")
                 continue
             bundle_ = resource
             if 'entry' not in bundle_:
-                print(f"No 'entry' in bundle {input_file} ")
+                logger.warning(f"No 'entry' in bundle {input_file} ")
                 continue
         for entry in bundle_['entry']:
             resource = entry['resource']
             _ = migrate_resource(resource)
             logging_validator(_, input_file, validate)
 
         output_file = output_path / input_file.name
+
         with open(output_file, "wb") as fp:
             fp.write(orjson.dumps(bundle_))
-        logger.info(f'Migrated {input_file} to {output_file}')
+        logger.info(f"Migrated bundle {input_file} to {output_file} entry_count:{len(bundle_['entry'])}")
 
 
-def migrate_resources(output_path, path, validate):
+def migrate_resources(output_path, path, validate, pattern='**/*.json'):
     """Migrate single resource per file."""
-    for input_file in path.glob('**/*.json'):  # TODO: see util directory_reader
+    for input_file in path.glob(pattern):  # TODO: see util directory_reader
         with open(input_file, "rb") as fp:
             resource = orjson.loads(fp.read())
             if not _is_resource(resource):
                 logger.warning(f"Not a FHIR resource {input_file}")
                 continue
             if _is_bundle(resource):
                 continue
             _ = migrate_resource(resource)
             logging_validator(_, input_file, validate)
 
         output_file = output_path / input_file.name
         with open(output_file, "wb") as fp:
             fp.write(orjson.dumps(_))
-        logger.info(f'Migrated {input_file} to {output_file}')
+        logger.info(f'Migrated resource {input_file} to {output_file}')
 
 
 def logging_validator(_, input_file, validate):
     """Log validation errors."""
     if validate:
         parse_result = parse_obj(_)
         if parse_result.exception is not None:
             if 'resourceType' not in str(parse_result.exception):
                 logger.warning(f"{input_file} has exception {parse_result.exception}")
 
 
-def migrate_ndjson(output_path, path, validate):
+def migrate_ndjson(output_path, path, validate, pattern='**/*.json'):
     """Migrate ndjson files, not expecting bundles."""
-    for input_file in path.glob('**/*.ndjson'):  # TODO: see util directory_reader
-        with open(input_file, "r") as fp:
-            output_file = output_path / input_file.name
-            with open(output_file, "wb") as out_fp:
+    for input_file in path.glob(pattern):  # TODO: see util directory_reader
+        out_fp = None
+        try:
+            with open(input_file, "r") as fp:
+                output_file = output_path / input_file.name
                 for line in fp.readlines():
                     resource = orjson.loads(line)
                     _ = migrate_resource(resource)
+                    if out_fp is None:
+                        out_fp = open(output_file, "wb")
                     logging_validator(_, input_file, validate)
-
                     out_fp.write(orjson.dumps(_, option=orjson.OPT_APPEND_NEWLINE))
-        logger.info(f'Migrated {input_file} to {output_file}')
+            logger.info(f'Migrated {input_file} to {output_file}')
+        except orjson.JSONDecodeError as e:
+            if 'unexpected end of data' not in str(e):
+                logger.warning(f"{input_file} has exception {e}")
+        finally:
+            if out_fp is not None:
+                out_fp.close()
 
 
-def migrate_json_gz(output_path, path, validate):
+def migrate_json_gz(output_path, path, validate, pattern='**/*.json'):
     """Migrate *json.gz files."""
-    for input_file in path.glob('*.*json.gz'):  # TODO: see util directory_reader
+    if 'gz' not in pattern:
+        pattern += ".gz"
+    for input_file in path.glob(pattern):  # TODO: see util directory_reader
 
         with io.TextIOWrapper(io.BufferedReader(gzip.GzipFile(input_file))) as fp:
             output_file = output_path / input_file.name
             with gzip.open(output_file, 'wb') as out_fp:
                 for line in fp.readlines():
                     resource = orjson.loads(line)
                     try:
@@ -321,16 +356,16 @@
                         out_fp.write(orjson.dumps(_, option=orjson.OPT_APPEND_NEWLINE))
                     except Exception as e:
                         print('\t', str(e))
                         break
         logger.info(f'Migrated {input_file} to {output_file}')
 
 
-def migrate_directory(path, output_path, validate):
+def migrate_directory(path, output_path, validate, pattern):
     """Migrate all files in a directory."""
     # single resources per file
-    migrate_bundles(output_path, path, validate)
-    migrate_resources(output_path, path, validate)
+    migrate_bundles(output_path, path, validate, pattern)
+    migrate_resources(output_path, path, validate, pattern)
 
     # multiple resources per file
-    migrate_ndjson(output_path, path, validate)
-    migrate_json_gz(output_path, path, validate)
+    migrate_ndjson(output_path, path, validate, pattern)
+    migrate_json_gz(output_path, path, validate, pattern)
```

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools/data/pfb.py` & `iceberg_tools-0.0.2rc3/iceberg_tools/data/pfb.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools/data/simplifier/__init__.py` & `iceberg_tools-0.0.2rc3/iceberg_tools/data/simplifier/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 import threading
 from typing import Dict, List
 
 import click
 import inflection
 import orjson
 import requests
+import yaml
 from fhir.resources import FHIRAbstractModel  # noqa
 from fhir.resources.attachment import Attachment
 from fhir.resources.codeableconcept import CodeableConcept
 from fhir.resources.codeablereference import CodeableReference
 from fhir.resources.coding import Coding
 from fhir.resources.core.utils import is_primitive_type
 from fhir.resources.documentreference import DocumentReferenceContent, DocumentReference
 from fhir.resources.extension import Extension
 from fhir.resources.identifier import Identifier
 from fhir.resources.observation import Observation
 from fhir.resources.reference import Reference
 from fhir.resources.task import Task
+from yaml import SafeLoader
 
 from iceberg_tools.util import EmitterContextManager, directory_reader
 from iceberg_tools.data.simplifier.oid_lookup import get_oid
 
 # Latest FHIR version by default
 FHIR_CLASSES = importlib.import_module('fhir.resources')
 
@@ -476,30 +478,36 @@
     """
     if dialect != 'GEN3':
         return simplified
     simplified = _gen3_scaffolding_document_reference(simplified, resource)
     return simplified
 
 
-def _render_dialect(simplified: dict, references: List[str], dialect: str, schemas) -> dict:
+def _render_dialect(simplified: dict, references: List[str], dialect: str, schemas: dict, limit_links: dict) -> dict:
     """Render as Gen3 record ready for import
     """
     if dialect != 'GEN3':
         return simplified
 
     labels = [_['title'] for _ in schemas.values() if 'title' in _]
 
+    permitted_destinations = None
+    if simplified['resourceType'] in limit_links:
+        permitted_destinations = limit_links[simplified['resourceType']]
+
     gen3_links = []
     for _ in references:
         if len(_.split('/')) != 2:
             logger.warning(f"Unexpected reference format {_} in {simplified['resourceType']} {simplified['id']}")
             continue
         label, id_ = _.split('/')
         if label not in labels:
             continue
+        if permitted_destinations is not None and label not in permitted_destinations:
+            continue
         gen3_links.append({"dst_id": id_, "dst_name": inflection.underscore(label)})
 
     return {'id': simplified['id'], 'name': inflection.underscore(simplified['resourceType']), 'relations': gen3_links, 'object': simplified}
 
 
 def simplify(resource: FHIRAbstractModel, dialect: str) -> (Dict, List[str]):
     """Create a Gen3 friendly resource. Returns simplified resource and associated references."""
@@ -571,28 +579,32 @@
         # DocumentReference.dict = self.orig_document_reference_dict
         Observation.dict = self.orig_observation_dict
         CodeableConcept.dict = self.orig_codeable_concept_dict
         CodeableReference.dict = self.orig_codeable_reference_dict
         Task.dict = self.orig_task_dict
 
 
-def simplify_directory(input_path, pattern, output_path, schema_path, dialect):
+def simplify_directory(input_path, pattern, output_path, schema_path, dialect, config_path):
     """Reads directory of FHIR, renders simple, data frame friendly flattened records."""
 
     input_path = pathlib.Path(input_path)
     assert input_path.is_dir(), f"{input_path} not a directory"
     dialect = dialect.upper()
 
     if pathlib.Path(schema_path).is_file():
         with open(schema_path, "rb") as fp_:
             schemas = orjson.loads(fp_.read())
     else:
         schemas = requests.get(schema_path).json()
     assert schemas, f"No schema found at {schema_path}"
 
+    with open(config_path) as fp:
+        gen3_config = yaml.load(fp, SafeLoader)
+    limit_links = gen3_config['limit_links']
+
     with SimplifierContextManager():
         with EmitterContextManager(output_path) as emitter:
             for parse_result in directory_reader(directory_path=input_path, pattern=pattern,
                                                  validate=False):
                 if parse_result.exception is not None:
                     if 'resourceType' not in str(parse_result.exception):
                         logger.error(f"{parse_result.path} has exception {parse_result.exception}")
@@ -605,15 +617,15 @@
                 except (TypeError, AssertionError) as e:
                     _debug_once(str(e))
 
                 assert simplified, ("Should have simplified", resource.resource_type, resource.id)
                 all_ok = all([validate_simplified_value(_) for _ in simplified.values()])
                 _assert_all_ok(all_ok, parse_result, resource, simplified)
 
-                simplified = _render_dialect(simplified, references, dialect, schemas)
+                simplified = _render_dialect(simplified, references, dialect, schemas, limit_links)
                 fp = emitter.emit(resource.resource_type)
                 fp.write(orjson.dumps(simplified, default=_default_json_serializer,
                                       option=orjson.OPT_APPEND_NEWLINE).decode())
 
 
 def _debug_once(msg):
     if msg not in LOGGED_ALREADY:
@@ -642,19 +654,23 @@
               help='Path to gen3 schema json.  (Accepts file path for schema development)'
               )
 @click.option('--dialect',
               default='GEN3',
               type=click.Choice(['FHIR', 'GEN3'], case_sensitive=False),
               help='GEN3: adds common properties, FHIR: passthrough'
               )
-def cli(path, pattern, output_path, schema_path, dialect):
+@click.option('--config_path',
+              default='config.yaml',
+              show_default=True,
+              help='Path to config file.')
+def cli(path, pattern, output_path, schema_path, dialect, config_path):
     """Renders Gen3 friendly flattened records.
 
     PATH: Path containing bundles (*.json) or resources (*.ndjson)
     OUTPUT_PATH: Path where simplified resources will be stored
     """
-    simplify_directory(path, pattern, output_path, schema_path, dialect)
+    simplify_directory(path, pattern, output_path, schema_path, dialect, config_path)
 
 
 if __name__ == '__main__':
     logging.basicConfig(level=logging.INFO)
     cli()
```

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools/data/simplifier/oid_lookup.py` & `iceberg_tools-0.0.2rc3/iceberg_tools/data/simplifier/oid_lookup.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools/schema/__init__.py` & `iceberg_tools-0.0.2rc3/iceberg_tools/schema/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,38 +20,87 @@
 
 ELEMENT_DB = sqlite3.connect(path)
 BASE_URI = 'http://bmeg.io/schema/0.0.2'
 
 logger = logging.getLogger(__name__)
 
 
-def _find_fhir_classes(gen3_config) -> List[type]:
+def _find_fhir_classes(gen3_config, log_stats=True) -> List[type]:
     """Based on config, expand dependencies."""
+
     class_names = [c for c in gen3_config['dependency_order'] if not c.startswith('_')]
     class_names = [c for c in class_names if c not in ['Program', 'Project']]
+
+    subclass_depth = gen3_config.get('subclass_depth', 3)
+
     mod = importlib.import_module('fhir.resources')
     classes = set()
     for class_name in class_names:
         classes.add(mod.get_fhir_model_class(class_name))
-    # find subclasses 3 levels deep
-    for _ in range(3):
+
+    # find subclasses N levels deep
+    # maintain statistics
+    stats = defaultdict(int)
+
+    for _ in range(subclass_depth):
         embedded_classes = set()
         for klass in classes:
+
             for p in klass.element_properties():
-                mod = importlib.import_module('fhir.resources')
                 try:
+
                     embedded_class = mod.get_fhir_model_class(get_fhir_type_name(p.type_))
                     embedded_classes.add(embedded_class)
+
+                    _update_stats(stats, klass, embedded_class)
+
                 except KeyError:
                     pass
+
         classes.update(embedded_classes)
-        classes.add(FHIRPrimitiveExtension)
+    classes.add(FHIRPrimitiveExtension)
+
+    if log_stats:
+        logger.info(f"Class statistics number of nested objects:\n{_summarize_stats(stats)}")
+
     return classes
 
 
+def _summarize_stats(stats: dict) -> str:
+    """Summarize stats, counts of subclasses."""
+    summary = {}
+    for _ in stats:
+        parts = _.split('.')
+        klass_name = parts[0]
+        if klass_name in ['Meta', 'Extension']:
+            continue
+        nested_class_count = len(parts[1:])
+        total_property_counts = stats[_]
+        summary[klass_name] = {'nested_class_count': nested_class_count, 'total_property_counts': total_property_counts}
+
+    stats_table = '\n  '.join(sorted([f'{k}: {v}' for k, v in summary.items()]))
+    return '  ' + stats_table
+
+
+def _update_stats(stats: dict, klass, embedded_class):
+    """Update stats for class and embedded class."""
+    if embedded_class.__name__ in ['Meta', 'Extension']:
+        return
+    stat_property = f"{klass.__name__}.{embedded_class.__name__}"
+    existing_stat_property = next(iter([k for k in stats.keys() if klass.__name__ in k]), None)
+    if existing_stat_property:
+        if embedded_class.__name__ not in existing_stat_property:
+            property_count = stats[existing_stat_property]
+            del stats[existing_stat_property]
+            existing_stat_property += f".{embedded_class.__name__}"
+            stats[existing_stat_property] = property_count + len(list(embedded_class.element_properties()))
+    else:
+        stats[stat_property] += 1
+
+
 def _extract_schemas(classes: List[type], base_uri: str) -> dict:
     """Get json schema for all classes."""
     schemas = {}
     for klass in classes:
         schema = klass.schema()
 
         assert 'title' in schema, schema
```

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools/schema/bmeg.py` & `iceberg_tools-0.0.2rc3/iceberg_tools/schema/bmeg.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools/schema/gen3.py` & `iceberg_tools-0.0.2rc3/iceberg_tools/schema/gen3.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,29 @@
     "date": 'string',
     "dateTime": 'string',
     "instant": 'string',
     "time": 'string'
 }
 
 
-def _simplify_schemas(gen3_config, gen3_fixtures, schemas):  # , edge_schemas
+def _summarize_stats(gen3_schema) -> str:
+    """Summarize the stats of the schema."""
+    summary = {}
+    for schema in gen3_schema.values():
+        if 'title' not in schema or 'properties' not in schema:
+            continue
+        summary[schema['title']] = {'total_property_counts': len(schema['properties'])}
+    stats_table = '\n  '.join(sorted([f'{k}: {v}' for k, v in summary.items()]))
+    return '  ' + stats_table
+
+
+def _simplify_schemas(gen3_config, gen3_fixtures, schemas, log_stats=True):
     """Make the schema Gen3 (data-frame) friendly."""
 
-    # config_paths = gen3_config['paths']
+    # extract expected configurations
     config_categories = gen3_config['categories']
     ignored_properties = gen3_config['ignored_properties']
     dependency_order = gen3_config['dependency_order']
     extra_properties = gen3_config['extra_properties']
     renamed_properties = gen3_config['renamed_properties']
     limit_links = gen3_config['limit_links']
     extensions = gen3_config['extensions']
@@ -82,14 +93,17 @@
 
     # save gen3 schema in order
     dependency_order.extend(k for k in schemas if k not in dependency_order)
 
     # change to lowercase for gen3
     gen3_schema = {inflection.underscore(k).replace('.yaml', ''): schemas[k] for k in dependency_order if k in schemas}
 
+    if log_stats:
+        logger.info(f"Class statistics number of simplified objects:\n{_summarize_stats(gen3_schema)}")
+
     return gen3_schema
 
 
 def _add_gen3_static_dependencies(gen3_fixtures, schemas):
     # add gen3 dependencies
     for fn in ["_definitions.yaml", "_terms.yaml", "_program.yaml", "_project.yaml", "_core_metadata_collection.yaml",
                "_settings.yaml"]:
@@ -316,14 +330,15 @@
 #             print()
 #         codings = _scalar_of_type(schema, 'Coding')
 #         if len(codings) > 0:
 #             print()
 
 def _simplify_embedded_types(schemas):
     """Any remaining embedded types are simply rendered as strings."""
+    # TODO - implement "PLUCK"
     for schema in schemas.values():
         lists_of_any = _list_of_any_type(schema)
         for name, property_ in lists_of_any.items():
             property_['description'] = f"[Text representation of {property_['items']['$ref'].replace('.yaml', '')}] {property_['description']}"
             property_['items']['type'] = 'string'
             del property_['items']['$ref']
         scalars_of_any = _scalar_of_any_type(schema)
```

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools/schema/gen3_validator.py` & `iceberg_tools-0.0.2rc3/iceberg_tools/schema/gen3_validator.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools/util.py` & `iceberg_tools-0.0.2rc3/iceberg_tools/util.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/PKG-INFO` & `iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceberg-tools
-Version: 0.0.2rc2
+Version: 0.0.2rc3
 Summary: FHIR schemas tools for bioinformatics.
 Home-page: https://github.com/bmeg/iceberg-schema-tools
 Author: https://ellrottlab.org/
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bmeg/iceberg-schema-tools/issues
 Project-URL: Source, https://github.com/bmeg/iceberg-schema-tools
 Keywords: FHIR PFB gen3 bioinformatics graph
@@ -18,15 +18,16 @@
 Description-Content-Type: text/markdown
 
 # iceberg-schema-tools
 Create and maintain central iceberg schema.  Render and validate FHIR data.
 
 ## Overview
 
-![image](docs/figure-5.png)
+![image](https://github.com/bmeg/iceberg-schema-tools/assets/47808/cf5f544c-081f-470f-b1d8-27f16ad21b67)
+
 
 
 Code that generates the base schema from FHIR goes here.  Additional tools are provided to lints, validates and visualize the schema.
 
 Note: The actual schemas are stored in [iceberg](https://github.com/bmeg/iceberg)
```

### Comparing `iceberg_tools-0.0.2rc2/iceberg_tools.egg-info/SOURCES.txt` & `iceberg_tools-0.0.2rc3/iceberg_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 iceberg_tools.egg-info/requires.txt
 iceberg_tools.egg-info/top_level.txt
 iceberg_tools/cli/__init__.py
 iceberg_tools/cli/data.py
 iceberg_tools/cli/schema.py
 iceberg_tools/data/__init__.py
 iceberg_tools/data/pfb.py
+iceberg_tools/data/report.py
 iceberg_tools/data/migrator/__init__.py
 iceberg_tools/data/simplifier/__init__.py
 iceberg_tools/data/simplifier/oid_lookup.py
 iceberg_tools/schema/__init__.py
 iceberg_tools/schema/bmeg.py
 iceberg_tools/schema/gen3.py
 iceberg_tools/schema/gen3_validator.py
@@ -31,14 +32,15 @@
 tests/integration/bmeg/test_schema.py
 tests/integration/bmeg/test_schema_load.py
 tests/integration/bmeg/test_spot_check_embedded_type.py
 tests/integration/bmeg/test_trivial_edge_load.py
 tests/integration/bmeg/test_trivial_vertex_load.py
 tests/integration/bmeg/test_yaml_anonymous_schemas.py
 tests/integration/data/__init__.py
+tests/integration/data/conftest.py
 tests/integration/data/test_pfb.py
 tests/integration/gen3/__init__.py
 tests/integration/gen3/conftest.py
 tests/integration/gen3/test_codeable_concept.py
 tests/integration/gen3/test_embedded_types.py
 tests/integration/gen3/test_identifiers.py
 tests/integration/gen3/test_individual_yaml.py
@@ -46,12 +48,13 @@
 tests/integration/gen3/test_primitive.py
 tests/integration/gen3/test_quantities.py
 tests/integration/gen3/test_research_study_has_project.py
 tests/integration/gen3/test_schema.py
 tests/integration/gen3/test_simplify_medication.py
 tests/integration/gen3/test_simplify_task.py
 tests/integration/gen3/test_task.py
+tests/integration/simplifier/__init__.py
+tests/integration/simplifier/test_simplify.py
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/test_coding_conventions.py
-tests/unit/test_schema.py
-tests/unit/test_simplify.py
+tests/unit/test_schema.py
```

### Comparing `iceberg_tools-0.0.2rc2/setup.py` & `iceberg_tools-0.0.2rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='iceberg_tools',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2rc2',  # Required
+    version='0.0.2rc3',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='FHIR schemas tools for bioinformatics.',
     # Optional
```

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/bmeg/__init__.py` & `iceberg_tools-0.0.2rc3/tests/integration/bmeg/__init__.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/bmeg/conftest.py` & `iceberg_tools-0.0.2rc3/tests/integration/bmeg/conftest.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_edge_load_granular_reference.py` & `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_edge_load_granular_reference.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_edge_validator.py` & `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_edge_validator.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_invalid_edges.py` & `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_invalid_edges.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_negative_trivial_vertex_load.py` & `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_negative_trivial_vertex_load.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_schema.py` & `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_schema.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_spot_check_embedded_type.py` & `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_spot_check_embedded_type.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_trivial_edge_load.py` & `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_trivial_edge_load.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/bmeg/test_trivial_vertex_load.py` & `iceberg_tools-0.0.2rc3/tests/integration/bmeg/test_trivial_vertex_load.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/data/test_pfb.py` & `iceberg_tools-0.0.2rc3/tests/integration/data/test_pfb.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,123 +1,126 @@
 from iceberg_tools.data.pfb import SimplePFBWriter
 from iceberg_tools.data.simplifier import simplify_directory
 
 
-def test_studies(caplog):
+def test_studies(caplog, dependency_order):
     """Ensure we can create a pfb file from a synthetic study."""
     simplify_directory('tests/fixtures/simplify/study/', '**/*.*', 'tmp/study/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3')
+                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
 
     pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
-                                 output_path='tmp/study/extractions/simplified-study.avro')
-    for _ in pfb_writer.transform_directory('tmp/study/extractions'):
-        print(_)
+                                 output_path='tmp/CohesiveDataSet.avro',
+                                 dependency_order=dependency_order)
+
+    list(pfb_writer.transform_directory('tmp/study/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
     if len(inspection.warnings) > 0:
         print(inspection.warnings)
 
 
-def test_synthea(caplog):
+def test_synthea(caplog, dependency_order):
     """Ensure we can create a pfb file from a synthetic study."""
     simplify_directory('tests/fixtures/simplify/synthea', '**/*.*', 'tmp/synthea/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3')
+                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
 
     pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
-                                 output_path='tmp/synthea/simplified-synthea.avro')
-    for _ in pfb_writer.transform_directory('tmp/synthea/extractions'):
-        print(_)
+                                 output_path='tmp/Synthea.avro',
+                                 dependency_order=dependency_order)
+
+    list(pfb_writer.transform_directory('tmp/synthea/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
     if len(inspection.warnings) > 0:
         print(inspection.warnings)
 
 
-def test_kf(caplog):
+def test_kf(caplog, dependency_order):
     """Ensure we can create a pfb file from a Kids first study."""
     simplify_directory('tests/fixtures/simplify/kf', '**/*.*', 'tmp/kf/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3')
+                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
 
     pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
-                                 output_path='tmp/kf/simplified-kf.avro')
+                                 output_path='tmp/KidsFirst.avro',
+                                 dependency_order=dependency_order)
 
-    for _ in pfb_writer.transform_directory('tmp/kf/extractions'):
-        print(_)
+    list(pfb_writer.transform_directory('tmp/kf/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
     if len(inspection.warnings) > 0:
         print(inspection.warnings)
 
 
-def test_ncpi(caplog):
+def test_ncpi(caplog, dependency_order):
     """Ensure we can create a pfb file from a NCPI IG examples."""
 
     simplify_directory('tests/fixtures/simplify/ncpi/examples-5.0', '*.*', 'tmp/ncpi/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3')
+                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
 
     pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
-                                 output_path='tmp/ncpi/simplified-ncpi.avro')
+                                 output_path='tmp/NCPI.avro',
+                                 dependency_order=dependency_order)
 
-    for _ in pfb_writer.transform_directory('tmp/ncpi/extractions'):
-        print(_)
+    list(pfb_writer.transform_directory('tmp/ncpi/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
     if len(inspection.warnings) > 0:
         print(inspection.warnings)
 
 
-def test_genomics_reporting(caplog):
+def test_genomics_reporting(caplog, dependency_order):
     """Ensure we can create a pfb file from a Genomics Reporting IG examples."""
 
-    simplify_directory('tests/fixtures/simplify/genomics-reporting/examples-5.0', '*.*', 'tmp/genomics-reporting/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3')
+    simplify_directory('tests/fixtures/simplify/genomics-reporting/examples-5.0',
+                       '*.*', 'tmp/genomics-reporting/extractions',
+                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
 
     pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
-                                 output_path='tmp/genomics-reporting/simplified-ncpi.avro')
+                                 output_path='tmp/GenomicsReporting.avro',
+                                 dependency_order=dependency_order)
 
-    for _ in pfb_writer.transform_directory('tmp/genomics-reporting/extractions'):
-        print(_)
+    list(pfb_writer.transform_directory('tmp/genomics-reporting/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
     if len(inspection.warnings) > 0:
         print(inspection.warnings)
 
 
-def test_dbgap(caplog):
+def test_dbgap(caplog, dependency_order):
     """Ensure we can create a pfb file from dbGAP examples."""
 
     simplify_directory('tests/fixtures/simplify/dbgap/examples-5.0', '*.*', 'tmp/dbgap/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3')
+                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
 
     pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
-                                 output_path='tmp/dbgap/simplified-dbgap.avro')
+                                 output_path='tmp/dbGap.avro',
+                                 dependency_order=dependency_order)
 
-    for _ in pfb_writer.transform_directory('tmp/dbgap/extractions'):
-        print(_)
+    list(pfb_writer.transform_directory('tmp/dbgap/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
     if len(inspection.warnings) > 0:
         print(inspection.warnings)
 
 
-def test_anvil(caplog):
+def test_anvil(caplog, dependency_order):
     """Ensure we can create a pfb file from AnVIL examples."""
 
-    simplify_directory('tests/fixtures/simplify/anvil/fhir/', '**/*.*', 'tmp/anvil/extractions',
-                       'iceberg/schemas/gen3/aced.json', 'GEN3')
+    simplify_directory('tests/fixtures/simplify/anvil/fhir-5.0/', '**/*.*', 'tmp/anvil/extractions',
+                       'iceberg/schemas/gen3/aced.json', 'GEN3', 'config.yaml')
 
     pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/gen3/aced.json',
-                                 output_path='tmp/anvil/simplified-anvil.avro')
+                                 output_path='tmp/AnVIL.avro',
+                                 dependency_order=dependency_order)
 
-    for _ in pfb_writer.transform_directory('tmp/anvil/extractions'):
-        print(_)
+    list(pfb_writer.transform_directory('tmp/anvil/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
     if len(inspection.warnings) > 0:
         print(inspection.warnings)
```

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/gen3/conftest.py` & `iceberg_tools-0.0.2rc3/tests/integration/gen3/conftest.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/gen3/test_codeable_concept.py` & `iceberg_tools-0.0.2rc3/tests/integration/gen3/test_codeable_concept.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/gen3/test_primitive.py` & `iceberg_tools-0.0.2rc3/tests/integration/gen3/test_primitive.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/gen3/test_research_study_has_project.py` & `iceberg_tools-0.0.2rc3/tests/integration/gen3/test_research_study_has_project.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/gen3/test_simplify_medication.py` & `iceberg_tools-0.0.2rc3/tests/integration/gen3/test_simplify_medication.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/integration/gen3/test_simplify_task.py` & `iceberg_tools-0.0.2rc3/tests/integration/gen3/test_simplify_task.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/unit/test_coding_conventions.py` & `iceberg_tools-0.0.2rc3/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/unit/test_schema.py` & `iceberg_tools-0.0.2rc3/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.2rc2/tests/unit/test_simplify.py` & `iceberg_tools-0.0.2rc3/tests/integration/simplifier/test_simplify.py`

 * *Files identical despite different names*

