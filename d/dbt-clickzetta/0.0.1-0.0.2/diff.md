# Comparing `tmp/dbt-clickzetta-0.0.1.tar.gz` & `tmp/dbt-clickzetta-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickzetta-0.0.1.tar", last modified: Fri May 26 14:50:01 2023, max compression
+gzip compressed data, was "dbt-clickzetta-0.0.2.tar", last modified: Sat May 27 15:00:52 2023, max compression
```

## Comparing `dbt-clickzetta-0.0.1.tar` & `dbt-clickzetta-0.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-26 14:50:01.554717 dbt-clickzetta-0.0.1/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.1/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-26 14:50:01.554586 dbt-clickzetta-0.0.1/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 06:42:15.000000 dbt-clickzetta-0.0.1/README.md
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-26 14:50:01.547094 dbt-clickzetta-0.0.1/dbt/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.1/dbt/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-26 14:50:01.546360 dbt-clickzetta-0.0.1/dbt/adapters/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-26 14:50:01.548406 dbt-clickzetta-0.0.1/dbt/adapters/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-26 10:45:40.000000 dbt-clickzetta-0.0.1/dbt/adapters/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-26 13:43:40.000000 dbt-clickzetta-0.0.1/dbt/adapters/clickzetta/__version__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1010 2023-05-26 08:09:45.000000 dbt-clickzetta-0.0.1/dbt/adapters/clickzetta/column.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7004 2023-05-26 12:08:15.000000 dbt-clickzetta-0.0.1/dbt/adapters/clickzetta/connections.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4694 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/adapters/clickzetta/impl.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      417 2023-05-26 10:45:40.000000 dbt-clickzetta-0.0.1/dbt/adapters/clickzetta/relation.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-26 14:50:01.546452 dbt-clickzetta-0.0.1/dbt/include/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-26 14:50:01.549015 dbt-clickzetta-0.0.1/dbt/include/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-26 12:03:31.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/dbt_project.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-26 14:50:01.549282 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14304 2023-05-26 14:32:14.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/adapters.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-26 14:50:01.550164 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-26 14:50:01.551052 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/incremental/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2651 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/seed.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/snapshot.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/table.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/view.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-26 14:50:01.553710 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/any_value.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/array_append.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/array_concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/array_construct.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/assert_not_null.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/bool_or.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/dateadd.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/datediff.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/listagg.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/split_part.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/timestamps.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-26 12:08:15.000000 dbt-clickzetta-0.0.1/dbt/include/clickzetta/profile_template.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-26 14:50:01.554421 dbt-clickzetta-0.0.1/dbt_clickzetta.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-26 14:50:01.000000 dbt-clickzetta-0.0.1/dbt_clickzetta.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-05-26 14:50:01.000000 dbt-clickzetta-0.0.1/dbt_clickzetta.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-26 14:50:01.000000 dbt-clickzetta-0.0.1/dbt_clickzetta.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-26 14:50:01.000000 dbt-clickzetta-0.0.1/dbt_clickzetta.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-05-26 14:50:01.000000 dbt-clickzetta-0.0.1/dbt_clickzetta.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-05-26 14:50:01.000000 dbt-clickzetta-0.0.1/dbt_clickzetta.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-26 14:50:01.554759 dbt-clickzetta-0.0.1/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-05-26 12:00:41.000000 dbt-clickzetta-0.0.1/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 15:00:52.562471 dbt-clickzetta-0.0.2/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.2/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-27 15:00:52.562344 dbt-clickzetta-0.0.2/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 06:42:15.000000 dbt-clickzetta-0.0.2/README.md
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 15:00:52.555317 dbt-clickzetta-0.0.2/dbt/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.2/dbt/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 15:00:52.554610 dbt-clickzetta-0.0.2/dbt/adapters/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 15:00:52.556502 dbt-clickzetta-0.0.2/dbt/adapters/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-26 10:45:40.000000 dbt-clickzetta-0.0.2/dbt/adapters/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-26 13:43:40.000000 dbt-clickzetta-0.0.2/dbt/adapters/clickzetta/__version__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1010 2023-05-26 08:09:45.000000 dbt-clickzetta-0.0.2/dbt/adapters/clickzetta/column.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7152 2023-05-27 13:59:58.000000 dbt-clickzetta-0.0.2/dbt/adapters/clickzetta/connections.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4882 2023-05-27 13:59:58.000000 dbt-clickzetta-0.0.2/dbt/adapters/clickzetta/impl.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      443 2023-05-27 13:59:58.000000 dbt-clickzetta-0.0.2/dbt/adapters/clickzetta/relation.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 15:00:52.554701 dbt-clickzetta-0.0.2/dbt/include/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 15:00:52.557010 dbt-clickzetta-0.0.2/dbt/include/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-26 12:03:31.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/dbt_project.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 15:00:52.557110 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 13:59:58.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/adapters.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 15:00:52.557950 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 15:00:52.558789 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/incremental/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2651 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/seed.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/snapshot.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/table.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/view.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 15:00:52.561502 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/any_value.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/array_append.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/array_concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/array_construct.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/assert_not_null.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/bool_or.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/dateadd.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/datediff.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/listagg.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/split_part.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/timestamps.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-26 12:08:15.000000 dbt-clickzetta-0.0.2/dbt/include/clickzetta/profile_template.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 15:00:52.562184 dbt-clickzetta-0.0.2/dbt_clickzetta.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-27 15:00:52.000000 dbt-clickzetta-0.0.2/dbt_clickzetta.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-05-27 15:00:52.000000 dbt-clickzetta-0.0.2/dbt_clickzetta.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-27 15:00:52.000000 dbt-clickzetta-0.0.2/dbt_clickzetta.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-27 15:00:52.000000 dbt-clickzetta-0.0.2/dbt_clickzetta.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-05-27 15:00:52.000000 dbt-clickzetta-0.0.2/dbt_clickzetta.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-05-27 15:00:52.000000 dbt-clickzetta-0.0.2/dbt_clickzetta.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-27 15:00:52.562511 dbt-clickzetta-0.0.2/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-05-27 15:00:35.000000 dbt-clickzetta-0.0.2/setup.py
```

### Comparing `dbt-clickzetta-0.0.1/dbt/adapters/clickzetta/__init__.py` & `dbt-clickzetta-0.0.2/dbt/adapters/clickzetta/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/adapters/clickzetta/column.py` & `dbt-clickzetta-0.0.2/dbt/adapters/clickzetta/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/adapters/clickzetta/connections.py` & `dbt-clickzetta-0.0.2/dbt/adapters/clickzetta/connections.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,19 +37,19 @@
 @dataclass
 class ClickZettaAdapterResponse(AdapterResponse):
     query_id: str = ""
 
 
 @dataclass
 class ClickZettaCredentials(Credentials):
-    workspace: str
-    instance_name: str
-    vc_name: str
-    password: str
-    base_url: str
+    workspace: str = ""
+    instance_name: str = ""
+    vc_name: str = "default"
+    password: str = ""
+    base_url: str = ""
     user_name: str = ""
     schema: str = "public"
     connect_retries: int = 3
     reuse_connections: bool = True
 
     @property
     def type(self):
@@ -75,15 +75,16 @@
     TYPE = "clickzetta"
 
     @contextmanager
     def exception_handler(self, sql):
         try:
             yield
         except Exception as e:
-            logger.debug("Error running SQL: {}", sql)
+            logger.warning("Error running SQL: {}", sql)
+            logger.warning("Exception {}", e)
             logger.debug("Rolling back transaction.")
             self.rollback_if_open()
             if isinstance(e, DbtRuntimeError):
                 # during a sql query, an internal to dbt exception was raised.
                 # this sounds a lot like a signal handler and probably has
                 # useful information, so raise it without modification.
                 raise
@@ -101,15 +102,15 @@
             session_parameters = {}
             log_params = LoginParams(
                 username=creds.user_name,
                 password=creds.password,
                 instance_name=creds.instance_name,
             )
             client = Client(
-                log_params=log_params,
+                login_params=log_params,
                 workspace=creds.workspace,
                 vc_name=creds.vc_name,
                 instance_name=creds.instance_name,
                 schema=creds.schema,
                 base_url=creds.base_url,
             )
             handle = ClickZettaConnection(client=client)
@@ -121,23 +122,24 @@
 
         return cls.retry_connection(
             connection,
             connect=connect,
             logger=logger,
             retry_limit=creds.connect_retries,
             retry_timeout=exponential_backoff,
+            retryable_exceptions=[],
         )
 
     def cancel(self, connection):
         pass
 
     @classmethod
     def get_response(cls, cursor) -> ClickZettaAdapterResponse:
         code = cursor.rowcount
-
+        logger.info(f"code: {code}")
         if code is not None:
             code = "SUCCESS"
 
         return ClickZettaAdapterResponse(
             _message="{} {}".format(code, cursor.rowcount),
             rows_affected=cursor.rowcount,
             code=code,
@@ -176,15 +178,15 @@
 
     def execute(
             self, sql: str, auto_begin: bool = False, fetch: bool = False, limit: Optional[int] = None
     ) -> Tuple[AdapterResponse, agate.Table]:
         _, cursor = self.add_query(sql, auto_begin)
         response = self.get_response(cursor)
         if fetch:
-            table = self.get_result_from_cursor(cursor, limit)
+            table = self.get_result_from_cursor(cursor)
         else:
             table = dbt.clients.agate_helper.empty_table()
         return response, table
 
     def add_standard_query(self, sql: str, **kwargs) -> Tuple[Connection, Any]:
         return super().add_query(self._add_query_comment(sql), **kwargs)
```

### Comparing `dbt-clickzetta-0.0.1/dbt/adapters/clickzetta/impl.py` & `dbt-clickzetta-0.0.2/dbt/adapters/clickzetta/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 )
 
 from dbt.adapters.clickzetta import ClickZettaConnectionManager
 from dbt.adapters.clickzetta import ClickZettaRelation
 from dbt.adapters.clickzetta import ClickZettaColumn
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.graph.nodes import ConstraintType
+from dbt.contracts.relation import RelationType
 from dbt.exceptions import CompilationError, DbtDatabaseError, DbtRuntimeError
 
 
 @dataclass
 class ClickZettaConfig(AdapterConfig):
     pass
 
@@ -59,47 +60,51 @@
     def list_schemas(self, database: str) -> List[str]:
         try:
             results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": database})
         except DbtDatabaseError as exc:
             msg = f"Database error while listing schemas in database " f'"{database}"\n{exc}'
             raise DbtRuntimeError(msg)
 
-        return [row["name"] for row in results]
+        return [row["schema_name"] for row in results]
 
     def get_columns_in_relation(self, relation):
         try:
             return super().get_columns_in_relation(relation)
         except DbtDatabaseError as exc:
             if "does not exist or not authorized" in str(exc):
                 return []
             else:
                 raise
 
-    def list_relations_without_caching(self, schema_relation: ClickZettaRelation) -> List[
-        ClickZettaRelation]:  # type: ignore
+    def list_relations_without_caching(self, schema_relation: ClickZettaRelation) \
+            -> List[ClickZettaRelation]:  # type: ignore
         kwargs = {"schema_relation": schema_relation}
         try:
             results = self.execute_macro(LIST_RELATIONS_MACRO_NAME, kwargs=kwargs)
         except DbtDatabaseError as exc:
             if "Object does not exist" in str(exc):
                 return []
             raise
 
         relations = []
-        quote_policy = {"database": True, "schema": True, "identifier": True}
-
-        columns = ["database_name", "schema_name", "name", "kind"]
-        for _database, _schema, _identifier, _type in results.select(columns):  # type: ignore
+        quote_policy = {"database": False, "schema": True, "identifier": True}
+        for row in results:
+            _schema, _identifier, _is_view, _is_materialized_view = row
             try:
-                _type = self.Relation.get_relation_type(_type.lower())
+                if _is_view == 'true':
+                    _type = RelationType.View
+                elif _is_materialized_view == 'true':
+                    _type = RelationType.MaterializedView
+                else:
+                    _type = RelationType.Table
             except ValueError:
                 _type = self.Relation.External
             relations.append(
                 self.Relation.create(
-                    database=_database,
+                    database=None,
                     schema=_schema,
                     identifier=_identifier,
                     quote_policy=quote_policy,
                     type=_type,
                 )
             )
```

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/adapters.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/adapters.sql`

 * *Files 0% similar despite different names*

```diff
@@ -259,23 +259,23 @@
       describe extended {{ relation.include(schema=(schema is not none)) }}
   {% endcall %}
   {% do return(load_result('get_columns_in_relation').table) %}
 {% endmacro %}
 
 {% macro clickzetta__list_relations_without_caching(relation) %}
   {% call statement('list_relations_without_caching', fetch_result=True) -%}
-    show table extended in {{ relation }} like '*'
+    show tables in {{ relation }}
   {% endcall %}
 
   {% do return(load_result('list_relations_without_caching').table) %}
 {% endmacro %}
 
 {% macro list_relations_show_tables_without_caching(schema_relation) %}
   {% call statement('list_relations_without_caching_show_tables', fetch_result=True) -%}
-    show tables in {{ schema_relation }} like '*'
+    show tables in {{ schema_relation }}
   {% endcall %}
 
   {% do return(load_result('list_relations_without_caching_show_tables').table) %}
 {% endmacro %}
 
 {% macro describe_table_extended_without_caching(table_name) %}
   {% call statement('describe_table_extended_without_caching', fetch_result=True) -%}
```

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/incremental/validate.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/seed.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/snapshot.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/materializations/table.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/dateadd.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/datediff.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/listagg.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt/include/clickzetta/macros/utils/split_part.sql` & `dbt-clickzetta-0.0.2/dbt/include/clickzetta/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/dbt_clickzetta.egg-info/SOURCES.txt` & `dbt-clickzetta-0.0.2/dbt_clickzetta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.1/setup.py` & `dbt-clickzetta-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-clickzetta"
-package_version = "0.0.1"
+package_version = "0.0.2"
 dbt_core_version = _get_dbt_core_version()
 description = """The ClickZetta adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

