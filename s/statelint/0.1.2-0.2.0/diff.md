# Comparing `tmp/statelint-0.1.2.tar.gz` & `tmp/statelint-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statelint-0.1.2.tar", last modified: Mon Mar  7 04:21:21 2022, max compression
+gzip compressed data, was "statelint-0.2.0.tar", last modified: Sat May 27 00:27:37 2023, max compression
```

## Comparing `statelint-0.1.2.tar` & `statelint-0.2.0.tar`

### file list

```diff
@@ -1,65 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 04:21:21.515127 statelint-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-03-07 04:21:09.000000 statelint-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-03-07 04:21:21.515127 statelint-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-03-07 04:21:09.000000 statelint-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-03-07 04:21:21.515127 statelint-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-07 04:21:09.000000 statelint-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 04:21:21.507126 statelint-0.1.2/statelint/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 04:21:21.511126 statelint-0.1.2/statelint/fields/
--rw-r--r--   0 runner    (1001) docker     (121)     5057 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/any_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/bool_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/container.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/list_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     2238 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/num_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/object_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/pattern_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/str_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/fields/timestamp_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/linter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 04:21:21.511126 statelint-0.1.2/statelint/nodes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/choice_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     5346 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/container_state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 04:21:21.511126 statelint-0.1.2/statelint/nodes/factory/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/factory/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/fail_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/map_state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 04:21:21.511126 statelint-0.1.2/statelint/nodes/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/mixins/catcher_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5281 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/mixins/choices_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/mixins/payload_template_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/mixins/result_path_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/mixins/retrier_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4366 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/parallel_state.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/pass_state.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/state.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/succeed_state.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/task_state.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/unknown_state.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/nodes/wait_state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 04:21:21.515127 statelint-0.1.2/statelint/problem/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/problem/predicate.py
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/problem/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/problem/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 04:21:21.515127 statelint-0.1.2/statelint/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-03-07 04:21:09.000000 statelint-0.1.2/statelint/utils/re_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 04:21:21.507126 statelint-0.1.2/statelint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-03-07 04:21:21.000000 statelint-0.1.2/statelint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-03-07 04:21:21.000000 statelint-0.1.2/statelint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-07 04:21:21.000000 statelint-0.1.2/statelint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-03-07 04:21:21.000000 statelint-0.1.2/statelint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-03-07 04:21:21.000000 statelint-0.1.2/statelint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-07 04:21:21.000000 statelint-0.1.2/statelint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.045829 statelint-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-27 00:27:25.000000 statelint-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-27 00:27:37.045829 statelint-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-27 00:27:25.000000 statelint-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-27 00:27:37.045829 statelint-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 00:27:25.000000 statelint-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.037829 statelint-0.2.0/statelint/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.037829 statelint-0.2.0/statelint/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/any_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/bool_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/list_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/num_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/object_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/pattern_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/str_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/timestamp_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/linter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.041829 statelint-0.2.0/statelint/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/choice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/container_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.041829 statelint-0.2.0/statelint/nodes/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/factory/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/fail_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/map_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.041829 statelint-0.2.0/statelint/nodes/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/catcher_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/choices_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/payload_template_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/result_path_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/retrier_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/parallel_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/pass_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/succeed_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/unknown_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/wait_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.041829 statelint-0.2.0/statelint/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/problem/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/problem/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/problem/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.041829 statelint-0.2.0/statelint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/utils/re_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.037829 statelint-0.2.0/statelint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.045829 statelint-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_catcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_choice_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_choice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_map_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_parallel_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_pass_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_ref_pattern_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_retrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_task_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_terminal_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_wait_state.py
```

### Comparing `statelint-0.1.2/LICENSE` & `statelint-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/PKG-INFO` & `statelint-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: statelint
-Version: 0.1.2
+Version: 0.2.0
 Summary: command-line validator for Amazon States Language
 Home-page: https://github.com/taro-kayo/statelint
 Author: taro-kayo
 License: Apache License 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6.1
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: yaml
 License-File: LICENSE
 
 # statelint
 <a href="https://github.com/taro-kayo/statelint/actions"><img alt="Actions Status" src="https://github.com/taro-kayo/statelint/workflows/Test/badge.svg"></a>
 <a href="https://coveralls.io/github/taro-kayo/statelint?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/taro-kayo/statelint/badge.svg?branch=main"></a>
 <a href="https://github.com/taro-kayo/statelint/blob/main/LICENSE"><img alt="License: Apache License 2.0" src="https://img.shields.io/badge/License-Apache_2.0-blue.svg"></a>
 <a href="https://pypi.org/project/statelint/"><img alt="PyPI" src="https://img.shields.io/pypi/v/statelint"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 
-An PyPI package providing a validator for [Amazon States Language](https://states-language.net/spec.html) JSON/YAML files.
+A PyPI package providing a validator for [Amazon States Language](https://states-language.net/spec.html) JSON/YAML files.
 
 This package is based on Amazon Web Services Labs' [awslabs/statelint](https://github.com/awslabs/statelint).
 
 ## Installation
 
 ```shell
 pip install statelint
@@ -78,9 +76,7 @@
 ```
 
 ## TODO
 
 - [reference path with dash doesn't validate](https://github.com/awslabs/statelint/issues/17)
 - [Reference Path with unicode doesn't validate](https://github.com/awslabs/statelint/issues/23)
 - [Does not catch Duplicated State names](https://github.com/awslabs/statelint/issues/39)
-
-
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: statelint Version: 0.1.2 Summary: command-line
+Metadata-Version: 2.1 Name: statelint Version: 0.2.0 Summary: command-line
 validator for Amazon States Language Home-page: https://github.com/taro-kayo/
-statelint Author: taro-kayo License: Apache License 2.0 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.6.1
-Description-Content-Type: text/markdown Provides-Extra: yaml License-File:
-LICENSE # statelint [Actions_Status] [Coverage_Status] [License:_Apache_License
-2.0] [PyPI] [Code_style:_black] An PyPI package providing a validator for
-[Amazon States Language](https://states-language.net/spec.html) JSON/YAML
-files. This package is based on Amazon Web Services Labs' [awslabs/statelint]
-(https://github.com/awslabs/statelint). ## Installation ```shell pip install
-statelint ``` ## Usage ```shell statelint fancy-state-machine-spec.json ``` If
-you prefer YAML, you need to install [PyYaml](https://pypi.org/project/PyYAML/
-). ```shell pip install PyYAML ``` Then, run command with a `--yaml` parameter.
-```shell statelint --yaml fancy-state-machine-spec.yaml ``` If you don't like
-to be complained that `BackoffRate` doesn't end with ".0", pass a `--
-ignore=FLOAT` parameter. ```shell statelint --ignore=FLOAT fancy-state-machine-
-spec.json ``` If your `Resource` doesn't contain URI string, pass a `--
+statelint Author: taro-kayo License: Apache License 2.0 Classifier: Development
+Status :: 4 - Beta Classifier: Environment :: Console Classifier: Intended
+Audience :: Developers Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.8.0 Description-Content-Type: text/markdown Provides-Extra: yaml
+License-File: LICENSE # statelint [Actions_Status] [Coverage_Status] [License:
+Apache_License_2.0] [PyPI] [Code_style:_black] A PyPI package providing a
+validator for [Amazon States Language](https://states-language.net/spec.html)
+JSON/YAML files. This package is based on Amazon Web Services Labs' [awslabs/
+statelint](https://github.com/awslabs/statelint). ## Installation ```shell pip
+install statelint ``` ## Usage ```shell statelint fancy-state-machine-spec.json
+``` If you prefer YAML, you need to install [PyYaml](https://pypi.org/project/
+PyYAML/). ```shell pip install PyYAML ``` Then, run command with a `--yaml`
+parameter. ```shell statelint --yaml fancy-state-machine-spec.yaml ``` If you
+don't like to be complained that `BackoffRate` doesn't end with ".0", pass a `-
+-ignore=FLOAT` parameter. ```shell statelint --ignore=FLOAT fancy-state-
+machine-spec.json ``` If your `Resource` doesn't contain URI string, pass a `--
 ignore=URI` parameter. ```shell statelint --ignore=URI fancy-state-machine-
 spec.json ``` You can pass both parameters at the same time. ```shell statelint
 --ignore=FLOAT,URI fancy-state-machine-spec.json ``` ## TODO - [reference path
 with dash doesn't validate](https://github.com/awslabs/statelint/issues/17) -
 [Reference Path with unicode doesn't validate](https://github.com/awslabs/
 statelint/issues/23) - [Does not catch Duplicated State names](https://
 github.com/awslabs/statelint/issues/39)
```

### Comparing `statelint-0.1.2/README.md` & `statelint-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # statelint
 <a href="https://github.com/taro-kayo/statelint/actions"><img alt="Actions Status" src="https://github.com/taro-kayo/statelint/workflows/Test/badge.svg"></a>
 <a href="https://coveralls.io/github/taro-kayo/statelint?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/taro-kayo/statelint/badge.svg?branch=main"></a>
 <a href="https://github.com/taro-kayo/statelint/blob/main/LICENSE"><img alt="License: Apache License 2.0" src="https://img.shields.io/badge/License-Apache_2.0-blue.svg"></a>
 <a href="https://pypi.org/project/statelint/"><img alt="PyPI" src="https://img.shields.io/pypi/v/statelint"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 
-An PyPI package providing a validator for [Amazon States Language](https://states-language.net/spec.html) JSON/YAML files.
+A PyPI package providing a validator for [Amazon States Language](https://states-language.net/spec.html) JSON/YAML files.
 
 This package is based on Amazon Web Services Labs' [awslabs/statelint](https://github.com/awslabs/statelint).
 
 ## Installation
 
 ```shell
 pip install statelint
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # statelint [Actions_Status] [Coverage_Status] [License:_Apache_License_2.0]
-[PyPI] [Code_style:_black] An PyPI package providing a validator for [Amazon
+[PyPI] [Code_style:_black] A PyPI package providing a validator for [Amazon
 States Language](https://states-language.net/spec.html) JSON/YAML files. This
 package is based on Amazon Web Services Labs' [awslabs/statelint](https://
 github.com/awslabs/statelint). ## Installation ```shell pip install statelint
 ``` ## Usage ```shell statelint fancy-state-machine-spec.json ``` If you prefer
 YAML, you need to install [PyYaml](https://pypi.org/project/PyYAML/). ```shell
 pip install PyYAML ``` Then, run command with a `--yaml` parameter. ```shell
 statelint --yaml fancy-state-machine-spec.yaml ``` If you don't like to be
```

### Comparing `statelint-0.1.2/setup.cfg` & `statelint-0.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taro-kayo/statelint
 author = taro-kayo
 license = Apache License 2.0
 license_file = LICENSE
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = find:
 install_requires = 
 	python-dateutil>=2.8.2
-	regex>=2022.1.18
-python_requires = >=3.6.1
+	regex>=2023.5.5
+python_requires = >=3.8.0
 
 [options.packages.find]
 include = 
 	statelint*
 
 [options.entry_points]
 console_scripts =
```

### Comparing `statelint-0.1.2/statelint/cli.py` & `statelint-0.2.0/statelint/cli.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/fields/__init__.py` & `statelint-0.2.0/statelint/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/fields/base.py` & `statelint-0.2.0/statelint/fields/base.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/fields/common.py` & `statelint-0.2.0/statelint/fields/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import json
 from enum import Enum
 from typing import Any
 
 
 class Comparison(str, Enum):
+    def __str__(self) -> str:
+        return self.value
+
     STRING_EQUALS = "StringEquals"
     STRING_LESS_THAN = "StringLessThan"
     STRING_GREATER_THAN = "StringGreaterThan"
     STRING_LESS_THAN_EQUALS = "StringLessThanEquals"
     STRING_GREATER_THAN_EQUALS = "StringGreaterThanEquals"
     NUMERIC_EQUALS = "NumericEquals"
     NUMERIC_LESS_THAN = "NumericLessThan"
@@ -42,14 +45,17 @@
     IS_STRING = "IsString"
     IS_BOOLEAN = "IsBoolean"
     IS_TIMESTAMP = "IsTimestamp"
     STRING_MATCHES = "StringMatches"
 
 
 class StateType(str, Enum):
+    def __str__(self) -> str:
+        return self.value
+
     PASS = "Pass"
     SUCCEED = "Succeed"
     FAIL = "Fail"
     TASK = "Task"
     CHOICE = "Choice"
     WAIT = "Wait"
     PARALLEL = "Parallel"
```

### Comparing `statelint-0.1.2/statelint/fields/container.py` & `statelint-0.2.0/statelint/fields/container.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/fields/list_field.py` & `statelint-0.2.0/statelint/fields/list_field.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/fields/num_field.py` & `statelint-0.2.0/statelint/fields/num_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 
 class BaseNumericField(NonNullMixin, Field, ABC):
     _floor: Optional[int]
     _ceiling: Optional[int]
 
     def __init__(
-        self, name: str, floor: int = None, ceiling: int = None, inclusive: bool = True
+        self,
+        name: str,
+        floor: Optional[int] = None,
+        ceiling: Optional[int] = None,
+        inclusive: bool = True,
     ) -> None:
         super().__init__(name)
         self._floor = floor
         self._ceiling = ceiling
         self._inclusive = inclusive
 
     @property
```

### Comparing `statelint-0.1.2/statelint/fields/pattern_field.py` & `statelint-0.2.0/statelint/fields/pattern_field.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/fields/str_field.py` & `statelint-0.2.0/statelint/fields/str_field.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/fields/timestamp_field.py` & `statelint-0.2.0/statelint/fields/timestamp_field.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/linter.py` & `statelint-0.2.0/statelint/linter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os.path
-from typing import Any, Callable, Dict, List, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
 from .config import Config
 from .nodes.factory.factory import StateFactory
 from .nodes.state_machine import StateMachine
 
 
 class ParseError(ValueError):
@@ -12,15 +12,16 @@
         super().__init__()
         self.root_cause = root_cause
 
 
 class Linter:
     @staticmethod
     def validate(
-        json_str_or_dict_or_file_path: Union[str, Dict[str, Any]], config: Config = None
+        json_str_or_dict_or_file_path: Union[str, Dict[str, Any]],
+        config: Optional[Config] = None,
     ) -> List[str]:
         if not config:
             config = Config()
 
         parse_text = _parse_yaml if config.is_yaml else _parse_json
         try:
             parsed = _parse_to_dict(json_str_or_dict_or_file_path, parse_text)
```

### Comparing `statelint-0.1.2/statelint/nodes/container_state.py` & `statelint-0.2.0/statelint/nodes/container_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/factory/factory.py` & `statelint-0.2.0/statelint/nodes/factory/factory.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/map_state.py` & `statelint-0.2.0/statelint/nodes/map_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/mixins/__init__.py` & `statelint-0.2.0/statelint/nodes/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/mixins/catcher_mixin.py` & `statelint-0.2.0/statelint/nodes/mixins/catcher_mixin.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/mixins/choices_mixin.py` & `statelint-0.2.0/statelint/nodes/mixins/choices_mixin.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/mixins/payload_template_mixin.py` & `statelint-0.2.0/statelint/nodes/mixins/payload_template_mixin.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/mixins/retrier_mixin.py` & `statelint-0.2.0/statelint/nodes/mixins/retrier_mixin.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/node.py` & `statelint-0.2.0/statelint/nodes/node.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/parallel_state.py` & `statelint-0.2.0/statelint/nodes/parallel_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/state_machine.py` & `statelint-0.2.0/statelint/nodes/state_machine.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/task_state.py` & `statelint-0.2.0/statelint/nodes/task_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/nodes/wait_state.py` & `statelint-0.2.0/statelint/nodes/wait_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.1.2/statelint/utils/re_helper.py` & `statelint-0.2.0/statelint/utils/re_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 INITIAL_NAME_CLASSES = ["Lu", "Ll", "Lt", "Lm", "Lo", "Nl"]
 NON_INITIAL_NAME_CLASSES = ["Mn", "Mc", "Nd", "Pc"]
 FOLLOWING_NAME_CLASSES = [*INITIAL_NAME_CLASSES, *NON_INITIAL_NAME_CLASSES]
 DOT_SEPARATOR = r"\.\.?"
 
 INTRINSIC_INVOCATION_PATTERN = re.compile(
-    r"^States\.(JsonToString|Format|StringToJson|Array)\(.+\)$"
+    r"^States\.(JsonToString|Format|StringToJson|Array|ArrayPartition|ArrayContains"
+    r"|ArrayRange|ArrayGetItem|ArrayLength|ArrayUnique|Base64Encode|Base64Decode"
+    r"|Hash|JsonMerge|MathRandom|MathAdd|StringSplit|UUID)\(.*\)$"
 )
 
 
 def is_reference_path(value: str) -> bool:
     return bool(_compile_reference_path_pattern().match(value))
```

### Comparing `statelint-0.1.2/statelint.egg-info/PKG-INFO` & `statelint-0.2.0/statelint.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: statelint
-Version: 0.1.2
+Version: 0.2.0
 Summary: command-line validator for Amazon States Language
 Home-page: https://github.com/taro-kayo/statelint
 Author: taro-kayo
 License: Apache License 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6.1
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: yaml
 License-File: LICENSE
 
 # statelint
 <a href="https://github.com/taro-kayo/statelint/actions"><img alt="Actions Status" src="https://github.com/taro-kayo/statelint/workflows/Test/badge.svg"></a>
 <a href="https://coveralls.io/github/taro-kayo/statelint?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/taro-kayo/statelint/badge.svg?branch=main"></a>
 <a href="https://github.com/taro-kayo/statelint/blob/main/LICENSE"><img alt="License: Apache License 2.0" src="https://img.shields.io/badge/License-Apache_2.0-blue.svg"></a>
 <a href="https://pypi.org/project/statelint/"><img alt="PyPI" src="https://img.shields.io/pypi/v/statelint"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 
-An PyPI package providing a validator for [Amazon States Language](https://states-language.net/spec.html) JSON/YAML files.
+A PyPI package providing a validator for [Amazon States Language](https://states-language.net/spec.html) JSON/YAML files.
 
 This package is based on Amazon Web Services Labs' [awslabs/statelint](https://github.com/awslabs/statelint).
 
 ## Installation
 
 ```shell
 pip install statelint
@@ -78,9 +76,7 @@
 ```
 
 ## TODO
 
 - [reference path with dash doesn't validate](https://github.com/awslabs/statelint/issues/17)
 - [Reference Path with unicode doesn't validate](https://github.com/awslabs/statelint/issues/23)
 - [Does not catch Duplicated State names](https://github.com/awslabs/statelint/issues/39)
-
-
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: statelint Version: 0.1.2 Summary: command-line
+Metadata-Version: 2.1 Name: statelint Version: 0.2.0 Summary: command-line
 validator for Amazon States Language Home-page: https://github.com/taro-kayo/
-statelint Author: taro-kayo License: Apache License 2.0 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.6.1
-Description-Content-Type: text/markdown Provides-Extra: yaml License-File:
-LICENSE # statelint [Actions_Status] [Coverage_Status] [License:_Apache_License
-2.0] [PyPI] [Code_style:_black] An PyPI package providing a validator for
-[Amazon States Language](https://states-language.net/spec.html) JSON/YAML
-files. This package is based on Amazon Web Services Labs' [awslabs/statelint]
-(https://github.com/awslabs/statelint). ## Installation ```shell pip install
-statelint ``` ## Usage ```shell statelint fancy-state-machine-spec.json ``` If
-you prefer YAML, you need to install [PyYaml](https://pypi.org/project/PyYAML/
-). ```shell pip install PyYAML ``` Then, run command with a `--yaml` parameter.
-```shell statelint --yaml fancy-state-machine-spec.yaml ``` If you don't like
-to be complained that `BackoffRate` doesn't end with ".0", pass a `--
-ignore=FLOAT` parameter. ```shell statelint --ignore=FLOAT fancy-state-machine-
-spec.json ``` If your `Resource` doesn't contain URI string, pass a `--
+statelint Author: taro-kayo License: Apache License 2.0 Classifier: Development
+Status :: 4 - Beta Classifier: Environment :: Console Classifier: Intended
+Audience :: Developers Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.8.0 Description-Content-Type: text/markdown Provides-Extra: yaml
+License-File: LICENSE # statelint [Actions_Status] [Coverage_Status] [License:
+Apache_License_2.0] [PyPI] [Code_style:_black] A PyPI package providing a
+validator for [Amazon States Language](https://states-language.net/spec.html)
+JSON/YAML files. This package is based on Amazon Web Services Labs' [awslabs/
+statelint](https://github.com/awslabs/statelint). ## Installation ```shell pip
+install statelint ``` ## Usage ```shell statelint fancy-state-machine-spec.json
+``` If you prefer YAML, you need to install [PyYaml](https://pypi.org/project/
+PyYAML/). ```shell pip install PyYAML ``` Then, run command with a `--yaml`
+parameter. ```shell statelint --yaml fancy-state-machine-spec.yaml ``` If you
+don't like to be complained that `BackoffRate` doesn't end with ".0", pass a `-
+-ignore=FLOAT` parameter. ```shell statelint --ignore=FLOAT fancy-state-
+machine-spec.json ``` If your `Resource` doesn't contain URI string, pass a `--
 ignore=URI` parameter. ```shell statelint --ignore=URI fancy-state-machine-
 spec.json ``` You can pass both parameters at the same time. ```shell statelint
 --ignore=FLOAT,URI fancy-state-machine-spec.json ``` ## TODO - [reference path
 with dash doesn't validate](https://github.com/awslabs/statelint/issues/17) -
 [Reference Path with unicode doesn't validate](https://github.com/awslabs/
 statelint/issues/23) - [Does not catch Duplicated State names](https://
 github.com/awslabs/statelint/issues/39)
```

### Comparing `statelint-0.1.2/statelint.egg-info/SOURCES.txt` & `statelint-0.2.0/statelint.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -48,8 +48,24 @@
 statelint/nodes/mixins/result_path_mixin.py
 statelint/nodes/mixins/retrier_mixin.py
 statelint/problem/__init__.py
 statelint/problem/predicate.py
 statelint/problem/problem.py
 statelint/problem/problem_type.py
 statelint/utils/__init__.py
-statelint/utils/re_helper.py
+statelint/utils/re_helper.py
+tests/test_catcher.py
+tests/test_choice_rule.py
+tests/test_choice_state.py
+tests/test_cli.py
+tests/test_fields.py
+tests/test_linter.py
+tests/test_map_state.py
+tests/test_parallel_state.py
+tests/test_parameters.py
+tests/test_pass_state.py
+tests/test_ref_pattern_field.py
+tests/test_retrier.py
+tests/test_state_machine.py
+tests/test_task_state.py
+tests/test_terminal_state.py
+tests/test_wait_state.py
```

