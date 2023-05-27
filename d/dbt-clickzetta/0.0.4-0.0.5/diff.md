# Comparing `tmp/dbt-clickzetta-0.0.4.tar.gz` & `tmp/dbt-clickzetta-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickzetta-0.0.4.tar", last modified: Sat May 27 18:40:20 2023, max compression
+gzip compressed data, was "dbt-clickzetta-0.0.5.tar", last modified: Sat May 27 19:25:34 2023, max compression
```

## Comparing `dbt-clickzetta-0.0.4.tar` & `dbt-clickzetta-0.0.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 18:40:20.966794 dbt-clickzetta-0.0.4/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.4/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-27 18:40:20.966644 dbt-clickzetta-0.0.4/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 06:42:15.000000 dbt-clickzetta-0.0.4/README.md
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 18:40:20.958713 dbt-clickzetta-0.0.4/dbt/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.4/dbt/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 18:40:20.958014 dbt-clickzetta-0.0.4/dbt/adapters/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 18:40:20.959931 dbt-clickzetta-0.0.4/dbt/adapters/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-26 10:45:40.000000 dbt-clickzetta-0.0.4/dbt/adapters/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-26 13:43:40.000000 dbt-clickzetta-0.0.4/dbt/adapters/clickzetta/__version__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1010 2023-05-26 08:09:45.000000 dbt-clickzetta-0.0.4/dbt/adapters/clickzetta/column.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7394 2023-05-27 18:40:18.000000 dbt-clickzetta-0.0.4/dbt/adapters/clickzetta/connections.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4882 2023-05-27 13:59:58.000000 dbt-clickzetta-0.0.4/dbt/adapters/clickzetta/impl.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      443 2023-05-27 13:59:58.000000 dbt-clickzetta-0.0.4/dbt/adapters/clickzetta/relation.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 18:40:20.958103 dbt-clickzetta-0.0.4/dbt/include/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 18:40:20.960557 dbt-clickzetta-0.0.4/dbt/include/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-26 12:03:31.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/dbt_project.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 18:40:20.960766 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 13:59:58.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/adapters.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 18:40:20.961582 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 18:40:20.962422 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/incremental/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2651 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/seed.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/snapshot.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/table.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/view.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 18:40:20.965806 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/any_value.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/array_append.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/array_concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/array_construct.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/assert_not_null.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/bool_or.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/dateadd.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/datediff.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/listagg.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/split_part.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/timestamps.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-26 12:08:15.000000 dbt-clickzetta-0.0.4/dbt/include/clickzetta/profile_template.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 18:40:20.966488 dbt-clickzetta-0.0.4/dbt_clickzetta.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-27 18:40:20.000000 dbt-clickzetta-0.0.4/dbt_clickzetta.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-05-27 18:40:20.000000 dbt-clickzetta-0.0.4/dbt_clickzetta.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-27 18:40:20.000000 dbt-clickzetta-0.0.4/dbt_clickzetta.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-27 18:40:20.000000 dbt-clickzetta-0.0.4/dbt_clickzetta.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-05-27 18:40:20.000000 dbt-clickzetta-0.0.4/dbt_clickzetta.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-05-27 18:40:20.000000 dbt-clickzetta-0.0.4/dbt_clickzetta.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-27 18:40:20.966831 dbt-clickzetta-0.0.4/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-05-27 18:40:18.000000 dbt-clickzetta-0.0.4/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 19:25:34.685172 dbt-clickzetta-0.0.5/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.5/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-27 19:25:34.685053 dbt-clickzetta-0.0.5/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 06:42:15.000000 dbt-clickzetta-0.0.5/README.md
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 19:25:34.678146 dbt-clickzetta-0.0.5/dbt/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.5/dbt/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 19:25:34.677450 dbt-clickzetta-0.0.5/dbt/adapters/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 19:25:34.679225 dbt-clickzetta-0.0.5/dbt/adapters/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-26 10:45:40.000000 dbt-clickzetta-0.0.5/dbt/adapters/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-26 13:43:40.000000 dbt-clickzetta-0.0.5/dbt/adapters/clickzetta/__version__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1183 2023-05-27 19:24:21.000000 dbt-clickzetta-0.0.5/dbt/adapters/clickzetta/column.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7394 2023-05-27 18:40:18.000000 dbt-clickzetta-0.0.5/dbt/adapters/clickzetta/connections.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7075 2023-05-27 19:24:21.000000 dbt-clickzetta-0.0.5/dbt/adapters/clickzetta/impl.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      441 2023-05-27 19:24:21.000000 dbt-clickzetta-0.0.5/dbt/adapters/clickzetta/relation.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 19:25:34.677542 dbt-clickzetta-0.0.5/dbt/include/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 19:25:34.679632 dbt-clickzetta-0.0.5/dbt/include/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-26 12:03:31.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/dbt_project.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 19:25:34.679838 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 13:59:58.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/adapters.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 19:25:34.680818 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 19:25:34.681645 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/incremental/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2651 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/seed.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/snapshot.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/table.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/view.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 19:25:34.684264 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/any_value.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/array_append.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/array_concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/array_construct.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/assert_not_null.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/bool_or.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/dateadd.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/datediff.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/listagg.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/split_part.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/timestamps.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-26 12:08:15.000000 dbt-clickzetta-0.0.5/dbt/include/clickzetta/profile_template.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 19:25:34.684906 dbt-clickzetta-0.0.5/dbt_clickzetta.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-27 19:25:34.000000 dbt-clickzetta-0.0.5/dbt_clickzetta.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-05-27 19:25:34.000000 dbt-clickzetta-0.0.5/dbt_clickzetta.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-27 19:25:34.000000 dbt-clickzetta-0.0.5/dbt_clickzetta.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-27 19:25:34.000000 dbt-clickzetta-0.0.5/dbt_clickzetta.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-05-27 19:25:34.000000 dbt-clickzetta-0.0.5/dbt_clickzetta.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-05-27 19:25:34.000000 dbt-clickzetta-0.0.5/dbt_clickzetta.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-27 19:25:34.685208 dbt-clickzetta-0.0.5/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-05-27 19:25:32.000000 dbt-clickzetta-0.0.5/setup.py
```

### Comparing `dbt-clickzetta-0.0.4/dbt/adapters/clickzetta/__init__.py` & `dbt-clickzetta-0.0.5/dbt/adapters/clickzetta/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/adapters/clickzetta/connections.py` & `dbt-clickzetta-0.0.5/dbt/adapters/clickzetta/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/adapters/clickzetta/impl.py` & `dbt-clickzetta-0.0.5/dbt/adapters/clickzetta/impl.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from typing import Mapping, Any, Optional, List, Union, Dict
 
 import agate
+import dbt.exceptions
 
 from dbt.adapters.base.impl import AdapterConfig, ConstraintSupport  # type: ignore
 from dbt.adapters.sql import SQLAdapter  # type: ignore
 from dbt.adapters.sql.impl import (
     LIST_SCHEMAS_MACRO_NAME,
     LIST_RELATIONS_MACRO_NAME,
 )
@@ -13,14 +14,33 @@
 from dbt.adapters.clickzetta import ClickZettaConnectionManager
 from dbt.adapters.clickzetta import ClickZettaRelation
 from dbt.adapters.clickzetta import ClickZettaColumn
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.graph.nodes import ConstraintType
 from dbt.contracts.relation import RelationType
 from dbt.exceptions import CompilationError, DbtDatabaseError, DbtRuntimeError
+from dbt.adapters.base import BaseRelation
+from dbt.clients.agate_helper import DEFAULT_TYPE_TESTER
+from dbt.contracts.connection import AdapterResponse
+from dbt.contracts.graph.nodes import ConstraintType
+from dbt.contracts.relation import RelationType
+from dbt.events import AdapterLogger
+from dbt.utils import executor, AttrDict
+
+GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME = "get_columns_in_relation_raw"
+LIST_SCHEMAS_MACRO_NAME = "list_schemas"
+LIST_RELATIONS_MACRO_NAME = "list_relations_without_caching"
+LIST_RELATIONS_SHOW_TABLES_MACRO_NAME = "list_relations_show_tables_without_caching"
+DESCRIBE_TABLE_EXTENDED_MACRO_NAME = "describe_table_extended_without_caching"
+
+TABLE_OR_VIEW_NOT_FOUND_MESSAGES = (
+    "[TABLE_OR_VIEW_NOT_FOUND]",
+    "Table or view not found",
+    "NoSuchTableException",
+)
 
 
 @dataclass
 class ClickZettaConfig(AdapterConfig):
     pass
 
 
@@ -53,14 +73,52 @@
         decimals = agate_table.aggregate(agate.MaxPrecision(col_idx))
         return 'FLOAT' if decimals else 'INT'
 
     @classmethod
     def convert_datetime_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return 'DATE'
 
+    def parse_describe_extended(
+            self, relation: BaseRelation, raw_rows: AttrDict
+    ) -> List[ClickZettaColumn]:
+        # Convert the Row to a dict
+        dict_rows = [dict(zip(row._keys, row._values)) for row in raw_rows]
+
+        rows = [row for row in dict_rows if not row["col_name"].startswith("#")]
+
+        return [
+            ClickZettaColumn(
+                table_database=None,
+                table_schema=relation.schema,
+                table_name=relation.name,
+                column=column["col_name"],
+                dtype=column["data_type"],
+            )
+            for idx, column in enumerate(rows)
+        ]
+
+    def get_columns_in_relation(self, relation: BaseRelation) -> List[ClickZettaColumn]:
+        columns = []
+        try:
+            rows: AttrDict = self.execute_macro(
+                GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME, kwargs={"relation": relation}
+            )
+            columns = self.parse_describe_extended(relation, rows)
+        except dbt.exceptions.DbtRuntimeError as e:
+            errmsg = getattr(e, "msg", "")
+            found_msgs = (msg in errmsg for msg in TABLE_OR_VIEW_NOT_FOUND_MESSAGES)
+            if any(found_msgs):
+                pass
+            else:
+                raise e
+
+        # strip hudi metadata columns.
+        columns = [x for x in columns]
+        return columns
+
     def list_schemas(self, database: str) -> List[str]:
         try:
             results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": database})
         except DbtDatabaseError as exc:
             msg = f"Database error while listing schemas in database " f'"{database}"\n{exc}'
             raise DbtRuntimeError(msg)
```

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/adapters.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/incremental/validate.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/seed.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/snapshot.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/materializations/table.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/dateadd.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/datediff.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/listagg.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt/include/clickzetta/macros/utils/split_part.sql` & `dbt-clickzetta-0.0.5/dbt/include/clickzetta/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/dbt_clickzetta.egg-info/SOURCES.txt` & `dbt-clickzetta-0.0.5/dbt_clickzetta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.4/setup.py` & `dbt-clickzetta-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-clickzetta"
-package_version = "0.0.4"
+package_version = "0.0.5"
 dbt_core_version = _get_dbt_core_version()
 description = """The ClickZetta adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

