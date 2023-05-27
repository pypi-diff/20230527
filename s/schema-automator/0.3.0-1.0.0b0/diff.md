# Comparing `tmp/schema_automator-0.3.0.tar.gz` & `tmp/schema_automator-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema_automator-0.3.0.tar", max compression
+gzip compressed data, was "schema_automator-1.0.0b0.tar", last modified: Tue Apr 12 00:32:30 2022, max compression
```

## Comparing `schema_automator-0.3.0.tar` & `schema_automator-1.0.0b0.tar`

### file list

```diff
@@ -1,44 +1,14 @@
--rw-r--r--   0        0        0     1526 2023-05-27 01:44:34.257803 schema_automator-0.3.0/LICENSE
--rw-r--r--   0        0        0      595 2023-05-27 01:44:34.257803 schema_automator-0.3.0/README.md
--rw-r--r--   0        0        0     2061 2023-05-27 01:45:37.430069 schema_automator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      127 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/__init__.py
--rw-r--r--   0        0        0      145 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/annotators/__init__.py
--rw-r--r--   0        0        0     3505 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/annotators/curated_to_enums.py
--rw-r--r--   0        0        0    17752 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/annotators/enum_annotator.py
--rw-r--r--   0        0        0     1438 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/annotators/enums_to_curateable.py
--rw-r--r--   0        0        0     2630 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/annotators/jsonld_annotator.py
--rw-r--r--   0        0        0     8487 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/annotators/schema_annotator.py
--rw-r--r--   0        0        0    20084 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/cli.py
--rw-r--r--   0        0        0        0 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/enhancer/__init__.py
--rw-r--r--   0        0        0      253 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/enhancer/general_enhancer.py
--rw-r--r--   0        0        0      251 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/generalizers/__init__.py
--rw-r--r--   0        0        0    30065 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/generalizers/csv_data_generalizer.py
--rw-r--r--   0        0        0     1281 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/generalizers/generalizer.py
--rw-r--r--   0        0        0     7642 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/generalizers/json_instance_generalizer.py
--rw-r--r--   0        0        0     2450 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/generalizers/pandas_generalizer.py
--rw-r--r--   0        0        0     3798 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/generalizers/rdf_data_generalizer.py
--rw-r--r--   0        0        0     1068 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/generalizers/toml_instance_generalizer.py
--rw-r--r--   0        0        0      329 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/importers/__init__.py
--rw-r--r--   0        0        0     9053 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/importers/dosdp_import_engine.py
--rw-r--r--   0        0        0     4989 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/importers/frictionless_import_engine.py
--rw-r--r--   0        0        0      666 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/importers/import_engine.py
--rw-r--r--   0        0        0    10620 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/importers/infer_model_from_rdftab.py
--rw-r--r--   0        0        0    15538 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/importers/jsonschema_import_engine.py
--rw-r--r--   0        0        0    17568 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/importers/owl_import_engine.py
--rw-r--r--   0        0        0     8067 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/importers/rdfs_import_engine.py
--rw-r--r--   0        0        0     2690 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/importers/sql_import_engine.py
--rw-r--r--   0        0        0     1717 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/importers/tabular_import_engine.py
--rw-r--r--   0        0        0        1 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/jsonschema/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/metamodels/__init__.py
--rw-r--r--   0        0        0       54 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/metamodels/dosdp/__init__.py
--rw-r--r--   0        0        0    17419 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/metamodels/dosdp/dosdp_linkml.yaml
--rw-r--r--   0        0        0    62403 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/metamodels/dosdp/model.py
--rw-r--r--   0        0        0    21430 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/metamodels/frictionless.py
--rw-r--r--   0        0        0     3716 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/metamodels/frictionless.yaml
--rw-r--r--   0        0        0     6117 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/metamodels/jsonschema.py
--rw-r--r--   0        0        0       59 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/utils/__init__.py
--rw-r--r--   0        0        0     1082 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/utils/enums_pvs_tsv.py
--rw-r--r--   0        0        0     7718 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/utils/instance_extractor.py
--rw-r--r--   0        0        0     1944 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/utils/schema_extractor.py
--rw-r--r--   0        0        0     2667 2023-05-27 01:44:34.269803 schema_automator-0.3.0/schema_automator/utils/schemautils.py
--rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 schema_automator-0.3.0/PKG-INFO
+drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2022-04-12 00:32:30.710684 schema_automator-1.0.0b0/
+-rw-r--r--   0 SMoxon     (502) staff       (20)     1526 2022-04-11 23:41:03.000000 schema_automator-1.0.0b0/LICENSE
+-rw-r--r--   0 SMoxon     (502) staff       (20)     4995 2022-04-12 00:32:30.710432 schema_automator-1.0.0b0/PKG-INFO
+-rw-r--r--   0 SMoxon     (502) staff       (20)     4376 2022-04-12 00:15:42.000000 schema_automator-1.0.0b0/README.md
+-rw-r--r--   0 SMoxon     (502) staff       (20)     1261 2022-04-12 00:22:31.000000 schema_automator-1.0.0b0/pyproject.toml
+drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2022-04-12 00:32:30.710066 schema_automator-1.0.0b0/schema_automator.egg-info/
+-rw-r--r--   0 SMoxon     (502) staff       (20)     4995 2022-04-12 00:32:30.000000 schema_automator-1.0.0b0/schema_automator.egg-info/PKG-INFO
+-rw-r--r--   0 SMoxon     (502) staff       (20)      283 2022-04-12 00:32:30.000000 schema_automator-1.0.0b0/schema_automator.egg-info/SOURCES.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)        1 2022-04-12 00:32:30.000000 schema_automator-1.0.0b0/schema_automator.egg-info/dependency_links.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)      696 2022-04-12 00:32:30.000000 schema_automator-1.0.0b0/schema_automator.egg-info/entry_points.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)      253 2022-04-12 00:32:30.000000 schema_automator-1.0.0b0/schema_automator.egg-info/requires.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)        1 2022-04-12 00:32:30.000000 schema_automator-1.0.0b0/schema_automator.egg-info/top_level.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)       38 2022-04-12 00:32:30.710772 schema_automator-1.0.0b0/setup.cfg
+-rw-r--r--   0 SMoxon     (502) staff       (20)     2183 2022-04-12 00:15:41.000000 schema_automator-1.0.0b0/setup.py
```

### Comparing `schema_automator-0.3.0/LICENSE` & `schema_automator-1.0.0b0/LICENSE`

 * *Files identical despite different names*

