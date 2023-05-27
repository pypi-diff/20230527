# Comparing `tmp/feloopy-0.2.4.tar.gz` & `tmp/feloopy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feloopy-0.2.4.tar", last modified: Sun Apr 16 18:25:12 2023, max compression
+gzip compressed data, was "feloopy-0.2.5.tar", last modified: Sat May 27 17:33:22 2023, max compression
```

## Comparing `feloopy-0.2.4.tar` & `feloopy-0.2.5.tar`

### file list

```diff
@@ -1,126 +1,170 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.945277 feloopy-0.2.4/
--rw-rw-rw-   0        0        0     1092 2023-03-25 08:57:31.000000 feloopy-0.2.4/LICENSE
--rw-rw-rw-   0        0        0    12389 2023-04-16 18:25:11.944282 feloopy-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    11764 2023-04-16 18:24:34.000000 feloopy-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.713287 feloopy-0.2.4/feloopy/
--rw-rw-rw-   0        0        0     9884 2023-04-16 13:41:04.000000 feloopy-0.2.4/feloopy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.727268 feloopy-0.2.4/feloopy/algorithms/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.728264 feloopy-0.2.4/feloopy/algorithms/constraint/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/constraint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.731265 feloopy-0.2.4/feloopy/algorithms/exact/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/exact/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.742262 feloopy-0.2.4/feloopy/algorithms/heuristic/
--rw-rw-rw-   0        0        0     2812 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/DE.py
--rw-rw-rw-   0        0        0     3096 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/GA.py
--rw-rw-rw-   0        0        0     2347 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/GWO.py
--rw-rw-rw-   0        0        0     3658 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/SA.py
--rw-rw-rw-   0        0        0     1794 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/TS.py
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/algorithms/heuristic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.745262 feloopy-0.2.4/feloopy/classes/
--rw-rw-rw-   0        0        0        0 2023-04-11 13:35:08.000000 feloopy-0.2.4/feloopy/classes/__init__.py
--rw-rw-rw-   0        0        0     1295 2023-04-11 13:36:26.000000 feloopy-0.2.4/feloopy/classes/empty.py
--rw-rw-rw-   0        0        0    77008 2023-04-16 18:12:48.000000 feloopy-0.2.4/feloopy/feloopy.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.760262 feloopy-0.2.4/feloopy/functions/
--rw-rw-rw-   0        0        0        0 2023-04-11 13:45:00.000000 feloopy-0.2.4/feloopy/functions/__init__.py
--rw-rw-rw-   0        0        0      488 2023-04-16 13:41:27.000000 feloopy-0.2.4/feloopy/functions/count_operators.py
--rw-rw-rw-   0        0        0      229 2023-04-16 18:06:45.000000 feloopy-0.2.4/feloopy/functions/fix_operators.py
--rw-rw-rw-   0        0        0     3029 2023-04-11 13:51:06.000000 feloopy-0.2.4/feloopy/functions/heuristic_operators.py
--rw-rw-rw-   0        0        0       38 2023-04-11 13:49:57.000000 feloopy-0.2.4/feloopy/functions/math_operators.py
--rw-rw-rw-   0        0        0      185 2023-04-11 13:50:07.000000 feloopy-0.2.4/feloopy/functions/random_operators.py
--rw-rw-rw-   0        0        0      305 2023-04-11 13:50:17.000000 feloopy-0.2.4/feloopy/functions/set_operators.py
--rw-rw-rw-   0        0        0     1669 2023-04-11 13:50:36.000000 feloopy-0.2.4/feloopy/functions/update_operators.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.771258 feloopy-0.2.4/feloopy/generators/
--rw-rw-rw-   0        0        0      129 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.814776 feloopy-0.2.4/feloopy/generators/model/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/model/__init__.py
--rw-rw-rw-   0        0        0      156 2023-04-11 11:47:49.000000 feloopy-0.2.4/feloopy/generators/model/cplex_cp_model_generator.py
--rw-rw-rw-   0        0        0      153 2023-04-11 11:48:02.000000 feloopy-0.2.4/feloopy/generators/model/cplex_model_generator.py
--rw-rw-rw-   0        0        0      136 2023-04-16 12:06:27.000000 feloopy-0.2.4/feloopy/generators/model/cvxpy_model_generator.py
--rw-rw-rw-   0        0        0      155 2023-04-11 11:48:21.000000 feloopy-0.2.4/feloopy/generators/model/cylp_model_generator.py
--rw-rw-rw-   0        0        0     1572 2023-04-05 08:38:53.000000 feloopy-0.2.4/feloopy/generators/model/feloopy_model_generator.py
--rw-rw-rw-   0        0        0      146 2023-04-11 11:49:14.000000 feloopy-0.2.4/feloopy/generators/model/gekko_model_generator.py
--rw-rw-rw-   0        0        0      133 2023-04-11 11:49:40.000000 feloopy-0.2.4/feloopy/generators/model/gurobi_model_generator.py
--rw-rw-rw-   0        0        0      104 2023-04-11 11:49:51.000000 feloopy-0.2.4/feloopy/generators/model/linopy_model_generator.py
--rw-rw-rw-   0        0        0    26710 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/model/mealpy_model_generator.py
--rw-rw-rw-   0        0        0      140 2023-04-11 11:50:27.000000 feloopy-0.2.4/feloopy/generators/model/mip_model_generator.py
--rw-rw-rw-   0        0        0      139 2023-04-11 11:50:43.000000 feloopy-0.2.4/feloopy/generators/model/ortools_cp_model_generator.py
--rw-rw-rw-   0        0        0      156 2023-04-11 11:51:10.000000 feloopy-0.2.4/feloopy/generators/model/ortools_model_generator.py
--rw-rw-rw-   0        0        0      135 2023-04-11 11:51:26.000000 feloopy-0.2.4/feloopy/generators/model/picos_model_generator.py
--rw-rw-rw-   0        0        0      156 2023-04-11 11:51:37.000000 feloopy-0.2.4/feloopy/generators/model/pulp_model_generator.py
--rw-rw-rw-   0        0        0      127 2023-04-11 11:51:46.000000 feloopy-0.2.4/feloopy/generators/model/pymprog_model_generator.py
--rw-rw-rw-   0        0        0      149 2023-04-11 11:52:04.000000 feloopy-0.2.4/feloopy/generators/model/pyomo_model_generator.py
--rw-rw-rw-   0        0        0      133 2023-04-11 11:52:21.000000 feloopy-0.2.4/feloopy/generators/model/xpress_model_generator.py
--rw-rw-rw-   0        0        0     2474 2023-04-11 11:47:11.000000 feloopy-0.2.4/feloopy/generators/model_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.848770 feloopy-0.2.4/feloopy/generators/result/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/result/__init__.py
--rw-rw-rw-   0        0        0      385 2023-04-11 17:07:27.000000 feloopy-0.2.4/feloopy/generators/result/cplex_cp_result_generator.py
--rw-rw-rw-   0        0        0      453 2023-04-11 17:07:23.000000 feloopy-0.2.4/feloopy/generators/result/cplex_result_generator.py
--rw-rw-rw-   0        0        0      452 2023-04-16 12:04:52.000000 feloopy-0.2.4/feloopy/generators/result/cvxpy_result_generator.py
--rw-rw-rw-   0        0        0      504 2023-04-05 08:40:40.000000 feloopy-0.2.4/feloopy/generators/result/cylp_result_generator.py
--rw-rw-rw-   0        0        0      576 2023-04-05 08:40:56.000000 feloopy-0.2.4/feloopy/generators/result/gekko_result_generator.py
--rw-rw-rw-   0        0        0     1183 2023-04-05 08:41:25.000000 feloopy-0.2.4/feloopy/generators/result/gurobi_result_generator.py
--rw-rw-rw-   0        0        0      452 2023-04-05 08:41:37.000000 feloopy-0.2.4/feloopy/generators/result/linopy_result_generator.py
--rw-rw-rw-   0        0        0      391 2023-04-05 08:41:43.000000 feloopy-0.2.4/feloopy/generators/result/mip_result_generator.py
--rw-rw-rw-   0        0        0      548 2023-04-05 08:41:48.000000 feloopy-0.2.4/feloopy/generators/result/ortools_cp_result_generator.py
--rw-rw-rw-   0        0        0      622 2023-04-05 08:41:53.000000 feloopy-0.2.4/feloopy/generators/result/ortools_result_generator.py
--rw-rw-rw-   0        0        0      414 2023-04-05 08:41:58.000000 feloopy-0.2.4/feloopy/generators/result/picos_result_generator.py
--rw-rw-rw-   0        0        0      507 2023-04-05 08:42:04.000000 feloopy-0.2.4/feloopy/generators/result/pulp_result_generator.py
--rw-rw-rw-   0        0        0      500 2023-04-05 08:42:10.000000 feloopy-0.2.4/feloopy/generators/result/pymprog_result_generator.py
--rw-rw-rw-   0        0        0      469 2023-04-05 08:42:16.000000 feloopy-0.2.4/feloopy/generators/result/pyomo_result_generator.py
--rw-rw-rw-   0        0        0      417 2023-04-05 08:42:22.000000 feloopy-0.2.4/feloopy/generators/result/xpress_result_generator.py
--rw-rw-rw-   0        0        0     6254 2023-04-04 11:50:22.000000 feloopy-0.2.4/feloopy/generators/result_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.876770 feloopy-0.2.4/feloopy/generators/solution/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/solution/__init__.py
--rw-rw-rw-   0        0        0     2446 2023-04-11 11:29:12.000000 feloopy-0.2.4/feloopy/generators/solution/cplex_cp_solution_generator.py
--rw-rw-rw-   0        0        0     3968 2023-04-11 11:29:46.000000 feloopy-0.2.4/feloopy/generators/solution/cplex_solution_generator.py
--rw-rw-rw-   0        0        0     2929 2023-04-16 12:52:44.000000 feloopy-0.2.4/feloopy/generators/solution/cvxpy_solution_generator.py
--rw-rw-rw-   0        0        0     1998 2023-04-11 11:30:29.000000 feloopy-0.2.4/feloopy/generators/solution/cylp_solution_generator.py
--rw-rw-rw-   0        0        0     2947 2023-03-31 08:00:48.000000 feloopy-0.2.4/feloopy/generators/solution/feloopy_solution_generator.py
--rw-rw-rw-   0        0        0     2740 2023-04-16 13:02:36.000000 feloopy-0.2.4/feloopy/generators/solution/gekko_solution_generator.py
--rw-rw-rw-   0        0        0     2728 2023-04-11 11:31:20.000000 feloopy-0.2.4/feloopy/generators/solution/gurobi_solution_generator.py
--rw-rw-rw-   0        0        0     2136 2023-04-11 11:31:33.000000 feloopy-0.2.4/feloopy/generators/solution/linopy_solution_generator.py
--rw-rw-rw-   0        0        0     4315 2023-04-11 11:31:52.000000 feloopy-0.2.4/feloopy/generators/solution/mealpy_solution_generator.py
--rw-rw-rw-   0        0        0     1901 2023-04-11 11:32:13.000000 feloopy-0.2.4/feloopy/generators/solution/mip_solution_generator.py
--rw-rw-rw-   0        0        0     2758 2023-04-11 11:32:29.000000 feloopy-0.2.4/feloopy/generators/solution/ortools_cp_solution_generator.py
--rw-rw-rw-   0        0        0     3091 2023-04-11 11:32:41.000000 feloopy-0.2.4/feloopy/generators/solution/ortools_solution_generator.py
--rw-rw-rw-   0        0        0     2278 2023-04-11 11:32:52.000000 feloopy-0.2.4/feloopy/generators/solution/picos_solution_generator.py
--rw-rw-rw-   0        0        0     3322 2023-04-11 11:33:06.000000 feloopy-0.2.4/feloopy/generators/solution/pulp_solution_generator.py
--rw-rw-rw-   0        0        0     2054 2023-04-12 06:39:22.000000 feloopy-0.2.4/feloopy/generators/solution/pymprog_solution_generator.py
--rw-rw-rw-   0        0        0     5576 2023-04-12 06:19:57.000000 feloopy-0.2.4/feloopy/generators/solution/pyomo_solution_generator.py
--rw-rw-rw-   0        0        0     1935 2023-04-11 15:44:52.000000 feloopy-0.2.4/feloopy/generators/solution/xpress_solution_generator.py
--rw-rw-rw-   0        0        0     2674 2023-04-11 11:23:04.000000 feloopy-0.2.4/feloopy/generators/solution_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.927279 feloopy-0.2.4/feloopy/generators/variable/
--rw-rw-rw-   0        0        0        0 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/generators/variable/__init__.py
--rw-rw-rw-   0        0        0     2677 2023-04-04 08:02:30.000000 feloopy-0.2.4/feloopy/generators/variable/cplex_cp_variable_generator.py
--rw-rw-rw-   0        0        0     2967 2023-04-11 15:32:22.000000 feloopy-0.2.4/feloopy/generators/variable/cplex_variable_generator.py
--rw-rw-rw-   0        0        0     6460 2023-04-16 12:18:37.000000 feloopy-0.2.4/feloopy/generators/variable/cvxpy_variable_generator.py
--rw-rw-rw-   0        0        0     2783 2023-03-31 08:38:56.000000 feloopy-0.2.4/feloopy/generators/variable/cylp_variable_generator.py
--rw-rw-rw-   0        0        0     2621 2023-03-31 08:39:01.000000 feloopy-0.2.4/feloopy/generators/variable/gekko_variable_generator.py
--rw-rw-rw-   0        0        0     7602 2023-04-16 18:11:55.000000 feloopy-0.2.4/feloopy/generators/variable/gurobi_variable_generator.py
--rw-rw-rw-   0        0        0     2123 2023-03-31 08:39:06.000000 feloopy-0.2.4/feloopy/generators/variable/linopy_variable_generator.py
--rw-rw-rw-   0        0        0     2657 2023-03-31 09:21:12.000000 feloopy-0.2.4/feloopy/generators/variable/mip_variable_generator.py
--rw-rw-rw-   0        0        0     3756 2023-04-04 13:36:46.000000 feloopy-0.2.4/feloopy/generators/variable/ortools_cp_variable_generator.py
--rw-rw-rw-   0        0        0     3997 2023-03-31 08:36:53.000000 feloopy-0.2.4/feloopy/generators/variable/ortools_variable_generator.py
--rw-rw-rw-   0        0        0     2888 2023-03-31 08:39:12.000000 feloopy-0.2.4/feloopy/generators/variable/picos_variable_generator.py
--rw-rw-rw-   0        0        0     3544 2023-03-31 08:39:15.000000 feloopy-0.2.4/feloopy/generators/variable/pulp_variable_generator.py
--rw-rw-rw-   0        0        0     3048 2023-03-31 08:39:17.000000 feloopy-0.2.4/feloopy/generators/variable/pymprog_variable_generator.py
--rw-rw-rw-   0        0        0     2326 2023-03-31 08:39:19.000000 feloopy-0.2.4/feloopy/generators/variable/pyomo_variable_generator.py
--rw-rw-rw-   0        0        0     4552 2023-03-31 08:39:21.000000 feloopy-0.2.4/feloopy/generators/variable/xpress_variable_generator.py
--rw-rw-rw-   0        0        0     2814 2023-04-04 07:53:39.000000 feloopy-0.2.4/feloopy/generators/variable_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.936279 feloopy-0.2.4/feloopy/operators/
--rw-rw-rw-   0        0        0       69 2023-03-25 08:57:31.000000 feloopy-0.2.4/feloopy/operators/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-04-11 17:03:29.000000 feloopy-0.2.4/feloopy/operators/common.py
--rw-rw-rw-   0        0        0       89 2023-04-05 08:20:05.000000 feloopy-0.2.4/feloopy/operators/exact.py
--rw-rw-rw-   0        0        0      187 2023-04-05 08:19:38.000000 feloopy-0.2.4/feloopy/operators/heuristic.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.726265 feloopy-0.2.4/feloopy.egg-info/
--rw-rw-rw-   0        0        0    12389 2023-04-16 18:25:11.000000 feloopy-0.2.4/feloopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4869 2023-04-16 18:25:11.000000 feloopy-0.2.4/feloopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 18:25:11.000000 feloopy-0.2.4/feloopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-04-16 18:25:11.000000 feloopy-0.2.4/feloopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 18:25:11.000000 feloopy-0.2.4/feloopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 18:25:11.945277 feloopy-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-04-16 18:02:29.000000 feloopy-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 18:25:11.943277 feloopy-0.2.4/tests/
--rw-rw-rw-   0        0        0     1029 2023-04-16 17:34:01.000000 feloopy-0.2.4/tests/test_exact_kp.py
--rw-rw-rw-   0        0        0     1277 2023-04-12 07:11:14.000000 feloopy-0.2.4/tests/test_exact_tsp.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.083867 feloopy-0.2.5/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1094 2023-05-11 14:53:22.000000 feloopy-0.2.5/LICENSE
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)    10791 2023-05-27 17:33:22.079867 feloopy-0.2.5/PKG-INFO
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)    10001 2023-05-27 17:30:23.000000 feloopy-0.2.5/README.md
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:21.999867 feloopy-0.2.5/feloopy/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     9762 2023-05-26 17:18:32.000000 feloopy-0.2.5/feloopy/__init__.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:21.999867 feloopy-0.2.5/feloopy/algorithms/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-17 08:47:59.000000 feloopy-0.2.5/feloopy/algorithms/__init__.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:21.999867 feloopy-0.2.5/feloopy/algorithms/constraint/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 18:18:46.000000 feloopy-0.2.5/feloopy/algorithms/constraint/__init__.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:21.999867 feloopy-0.2.5/feloopy/algorithms/exact/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:22:32.000000 feloopy-0.2.5/feloopy/algorithms/exact/__init__.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.003867 feloopy-0.2.5/feloopy/algorithms/heuristic/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3302 2023-05-17 08:43:08.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/DE.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3471 2023-05-17 08:43:29.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/GA.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2644 2023-05-12 20:25:18.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/GWO.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4030 2023-05-12 20:25:25.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/SA.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2085 2023-05-12 20:25:30.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/TS.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:22:42.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/__init__.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.015867 feloopy-0.2.5/feloopy/algorithms/mcdm/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      957 2023-05-15 18:09:12.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1861 2023-05-26 15:27:35.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/ahp.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2666 2023-05-26 15:29:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/aras.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2366 2023-05-26 15:31:12.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/borda.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2620 2023-05-26 15:35:07.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/bwm.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2821 2023-05-26 15:37:07.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/codas.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2670 2023-05-26 15:39:44.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/copras.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1989 2023-05-26 15:42:38.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/critic.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3512 2023-05-26 15:48:36.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/dematel.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1192 2023-05-15 17:53:51.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/edas.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3349 2023-05-26 16:25:52.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/elecre_i.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2215 2023-05-15 17:48:22.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_i_s.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3438 2023-05-15 17:48:29.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_i_v.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3029 2023-05-15 17:48:33.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_ii.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3518 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_iii.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2145 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_iv.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3047 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_tri.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2273 2023-05-15 17:49:03.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/fahp.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2828 2023-05-15 17:56:01.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/fdematel.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1341 2023-05-15 17:54:40.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/fedeas.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1180 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/ftopsis.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2647 2023-05-15 17:52:09.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/fvikor.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1381 2023-05-15 17:50:08.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/gra.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1478 2023-05-15 17:55:13.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/idocriw.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1247 2023-05-15 17:55:23.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/mabac.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1648 2023-05-15 17:55:33.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/maut.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1668 2023-05-15 17:55:40.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/moora.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2252 2023-05-15 17:50:26.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/moosra.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2049 2023-05-15 17:49:15.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/multimoora.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1905 2023-05-15 17:52:20.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_gaia.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1329 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_i.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3258 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_ii.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3141 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_iii.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3000 2023-05-15 18:23:05.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_iv.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2878 2023-05-15 17:57:18.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_v.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2398 2023-05-15 17:57:13.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_vi.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1356 2023-05-15 17:57:05.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/saw.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1664 2023-05-15 17:56:55.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/smart.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1468 2023-05-15 17:56:48.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/topsis.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2277 2023-05-15 17:56:41.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/vikor.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2628 2023-05-15 17:51:32.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/waspas.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2193 2023-05-15 17:51:36.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/wings.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)   150152 2023-05-27 15:34:30.000000 feloopy-0.2.5/feloopy/feloopy.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.019867 feloopy-0.2.5/feloopy/generators/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      421 2023-05-12 17:33:41.000000 feloopy-0.2.5/feloopy/generators/__init__.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.031867 feloopy-0.2.5/feloopy/generators/model/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:24:04.000000 feloopy-0.2.5/feloopy/generators/model/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      431 2023-05-17 15:20:21.000000 feloopy-0.2.5/feloopy/generators/model/cplex_cp_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      426 2023-05-26 16:26:32.000000 feloopy-0.2.5/feloopy/generators/model/cplex_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      420 2023-05-12 17:24:33.000000 feloopy-0.2.5/feloopy/generators/model/cvxpy_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      440 2023-05-12 17:24:39.000000 feloopy-0.2.5/feloopy/generators/model/cylp_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3717 2023-05-27 17:31:47.000000 feloopy-0.2.5/feloopy/generators/model/feloopy_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      435 2023-05-12 17:25:19.000000 feloopy-0.2.5/feloopy/generators/model/gekko_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      421 2023-05-12 17:25:23.000000 feloopy-0.2.5/feloopy/generators/model/gurobi_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      392 2023-05-12 17:25:27.000000 feloopy-0.2.5/feloopy/generators/model/linopy_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)    26915 2023-05-12 17:29:08.000000 feloopy-0.2.5/feloopy/generators/model/mealpy_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      427 2023-05-26 16:28:01.000000 feloopy-0.2.5/feloopy/generators/model/mip_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      425 2023-05-26 16:28:05.000000 feloopy-0.2.5/feloopy/generators/model/ortools_cp_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      447 2023-05-26 16:28:10.000000 feloopy-0.2.5/feloopy/generators/model/ortools_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      423 2023-05-12 17:29:23.000000 feloopy-0.2.5/feloopy/generators/model/picos_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      444 2023-05-12 17:29:28.000000 feloopy-0.2.5/feloopy/generators/model/pulp_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      415 2023-05-12 17:29:36.000000 feloopy-0.2.5/feloopy/generators/model/pymprog_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      437 2023-05-12 17:29:40.000000 feloopy-0.2.5/feloopy/generators/model/pyomo_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      421 2023-05-12 17:29:44.000000 feloopy-0.2.5/feloopy/generators/model/xpress_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2687 2023-05-26 10:39:58.000000 feloopy-0.2.5/feloopy/generators/model_generator.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.047867 feloopy-0.2.5/feloopy/generators/result/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:29:52.000000 feloopy-0.2.5/feloopy/generators/result/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      680 2023-05-12 17:29:58.000000 feloopy-0.2.5/feloopy/generators/result/cplex_cp_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      745 2023-05-12 17:30:09.000000 feloopy-0.2.5/feloopy/generators/result/cplex_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      751 2023-05-12 17:30:13.000000 feloopy-0.2.5/feloopy/generators/result/cvxpy_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      751 2023-05-12 17:30:17.000000 feloopy-0.2.5/feloopy/generators/result/cylp_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      860 2023-05-12 17:30:22.000000 feloopy-0.2.5/feloopy/generators/result/gekko_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1448 2023-05-12 17:30:26.000000 feloopy-0.2.5/feloopy/generators/result/gurobi_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      736 2023-05-12 17:30:31.000000 feloopy-0.2.5/feloopy/generators/result/linopy_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      674 2023-05-12 17:30:34.000000 feloopy-0.2.5/feloopy/generators/result/mip_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      855 2023-05-12 17:30:38.000000 feloopy-0.2.5/feloopy/generators/result/ortools_cp_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      930 2023-05-12 17:30:46.000000 feloopy-0.2.5/feloopy/generators/result/ortools_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      692 2023-05-12 17:30:50.000000 feloopy-0.2.5/feloopy/generators/result/picos_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      796 2023-05-12 17:30:55.000000 feloopy-0.2.5/feloopy/generators/result/pulp_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      778 2023-05-12 17:30:58.000000 feloopy-0.2.5/feloopy/generators/result/pymprog_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      747 2023-05-12 17:31:02.000000 feloopy-0.2.5/feloopy/generators/result/pyomo_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      711 2023-05-12 17:31:06.000000 feloopy-0.2.5/feloopy/generators/result/xpress_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     6520 2023-05-12 17:33:49.000000 feloopy-0.2.5/feloopy/generators/result_generator.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.051867 feloopy-0.2.5/feloopy/generators/solution/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:31:12.000000 feloopy-0.2.5/feloopy/generators/solution/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2294 2023-05-26 16:32:33.000000 feloopy-0.2.5/feloopy/generators/solution/cplex_cp_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4247 2023-05-12 17:31:21.000000 feloopy-0.2.5/feloopy/generators/solution/cplex_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3241 2023-05-12 17:31:26.000000 feloopy-0.2.5/feloopy/generators/solution/cvxpy_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2255 2023-05-12 17:31:30.000000 feloopy-0.2.5/feloopy/generators/solution/cylp_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3182 2023-05-12 17:31:34.000000 feloopy-0.2.5/feloopy/generators/solution/feloopy_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2935 2023-05-12 17:31:37.000000 feloopy-0.2.5/feloopy/generators/solution/gekko_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2984 2023-05-12 17:31:41.000000 feloopy-0.2.5/feloopy/generators/solution/gurobi_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2372 2023-05-12 17:31:45.000000 feloopy-0.2.5/feloopy/generators/solution/linopy_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4607 2023-05-26 22:10:18.000000 feloopy-0.2.5/feloopy/generators/solution/mealpy_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2186 2023-05-12 17:31:54.000000 feloopy-0.2.5/feloopy/generators/solution/mip_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2976 2023-05-12 17:31:58.000000 feloopy-0.2.5/feloopy/generators/solution/ortools_cp_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3311 2023-05-12 17:32:03.000000 feloopy-0.2.5/feloopy/generators/solution/ortools_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2570 2023-05-12 17:32:06.000000 feloopy-0.2.5/feloopy/generators/solution/picos_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3558 2023-05-12 20:06:11.000000 feloopy-0.2.5/feloopy/generators/solution/pulp_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2349 2023-05-12 17:32:17.000000 feloopy-0.2.5/feloopy/generators/solution/pymprog_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     5347 2023-05-27 17:00:58.000000 feloopy-0.2.5/feloopy/generators/solution/pymultiobjective_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     5733 2023-05-12 17:32:27.000000 feloopy-0.2.5/feloopy/generators/solution/pyomo_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2240 2023-05-12 17:32:31.000000 feloopy-0.2.5/feloopy/generators/solution/xpress_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3090 2023-05-17 15:57:15.000000 feloopy-0.2.5/feloopy/generators/solution_generator.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.059867 feloopy-0.2.5/feloopy/generators/variable/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:32:36.000000 feloopy-0.2.5/feloopy/generators/variable/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3123 2023-05-27 16:01:05.000000 feloopy-0.2.5/feloopy/generators/variable/cplex_cp_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3433 2023-05-12 17:32:45.000000 feloopy-0.2.5/feloopy/generators/variable/cplex_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     6293 2023-05-19 19:26:03.000000 feloopy-0.2.5/feloopy/generators/variable/cvxpy_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3158 2023-05-12 17:32:53.000000 feloopy-0.2.5/feloopy/generators/variable/cylp_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3072 2023-05-12 17:32:57.000000 feloopy-0.2.5/feloopy/generators/variable/gekko_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     8216 2023-05-12 17:33:01.000000 feloopy-0.2.5/feloopy/generators/variable/gurobi_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2420 2023-05-12 17:33:04.000000 feloopy-0.2.5/feloopy/generators/variable/linopy_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2955 2023-05-12 17:33:08.000000 feloopy-0.2.5/feloopy/generators/variable/mip_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3742 2023-05-12 17:33:12.000000 feloopy-0.2.5/feloopy/generators/variable/ortools_cp_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3957 2023-05-12 17:33:17.000000 feloopy-0.2.5/feloopy/generators/variable/ortools_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3295 2023-05-12 17:33:21.000000 feloopy-0.2.5/feloopy/generators/variable/picos_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3661 2023-05-12 17:33:25.000000 feloopy-0.2.5/feloopy/generators/variable/pulp_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3508 2023-05-12 17:33:30.000000 feloopy-0.2.5/feloopy/generators/variable/pymprog_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2705 2023-05-12 17:33:34.000000 feloopy-0.2.5/feloopy/generators/variable/pyomo_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4232 2023-05-12 17:33:37.000000 feloopy-0.2.5/feloopy/generators/variable/xpress_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3022 2023-05-12 17:34:00.000000 feloopy-0.2.5/feloopy/generators/variable_generator.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.063867 feloopy-0.2.5/feloopy/helpers/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:34:12.000000 feloopy-0.2.5/feloopy/helpers/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1494 2023-05-12 17:34:17.000000 feloopy-0.2.5/feloopy/helpers/empty.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)       49 2023-05-27 11:55:10.000000 feloopy-0.2.5/feloopy/helpers/error.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      132 2023-05-27 14:39:24.000000 feloopy-0.2.5/feloopy/helpers/formatter.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.079867 feloopy-0.2.5/feloopy/operators/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      384 2023-05-12 20:17:53.000000 feloopy-0.2.5/feloopy/operators/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)    11270 2023-05-12 17:54:44.000000 feloopy-0.2.5/feloopy/operators/common.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      772 2023-05-12 17:34:37.000000 feloopy-0.2.5/feloopy/operators/count_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)        0 2023-05-12 20:47:21.000000 feloopy-0.2.5/feloopy/operators/epsilon.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      380 2023-05-12 17:34:41.000000 feloopy-0.2.5/feloopy/operators/exact.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      560 2023-05-26 22:23:23.000000 feloopy-0.2.5/feloopy/operators/fix_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      474 2023-05-12 17:34:53.000000 feloopy-0.2.5/feloopy/operators/heuristic.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3656 2023-05-12 17:34:49.000000 feloopy-0.2.5/feloopy/operators/heuristic_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1569 2023-05-25 13:29:00.000000 feloopy-0.2.5/feloopy/operators/math_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)    15154 2023-05-26 16:39:30.000000 feloopy-0.2.5/feloopy/operators/metric_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)        0 2023-05-26 10:16:57.000000 feloopy-0.2.5/feloopy/operators/pareto.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      476 2023-05-12 17:35:00.000000 feloopy-0.2.5/feloopy/operators/random_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      576 2023-05-26 16:39:45.000000 feloopy-0.2.5/feloopy/operators/set_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1932 2023-05-26 16:39:50.000000 feloopy-0.2.5/feloopy/operators/update_operators.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:21.999867 feloopy-0.2.5/feloopy.egg-info/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)    10791 2023-05-27 17:33:21.000000 feloopy-0.2.5/feloopy.egg-info/PKG-INFO
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     6493 2023-05-27 17:33:21.000000 feloopy-0.2.5/feloopy.egg-info/SOURCES.txt
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)        1 2023-05-27 17:33:21.000000 feloopy-0.2.5/feloopy.egg-info/dependency_links.txt
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      270 2023-05-27 17:33:21.000000 feloopy-0.2.5/feloopy.egg-info/requires.txt
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)        8 2023-05-27 17:33:21.000000 feloopy-0.2.5/feloopy.egg-info/top_level.txt
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)       38 2023-05-27 17:33:22.083867 feloopy-0.2.5/setup.cfg
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1809 2023-05-17 08:50:20.000000 feloopy-0.2.5/setup.py
```

### Comparing `feloopy-0.2.4/LICENSE` & `feloopy-0.2.5/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Keivan Tafakkori
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Keivan Tafakkori. All rights reserved.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `feloopy-0.2.4/feloopy/algorithms/heuristic/DE.py` & `feloopy-0.2.5/feloopy/algorithms/heuristic/DE.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,80 @@
-import numpy as np
-import warnings as wn
-
-wn.filterwarnings("ignore")
-
-class DE:
-
-    def __init__(self, f: int, d: list, s: int, t: int, cr: float, mu: float):
-
-        self.d = np.asarray([1 if item == 'max' else -1 for item in d])
-        self.r = 0 if len(d) == 1 else len(d)
-        self.f = f
-        self.s = s
-        self.t = t
-        self.cr = cr
-        self.mu = mu
-        self.new_features_cols = [0, self.f]
-        self.old_features_cols = [self.f, 2*self.f]
-        self.status_col = [-2]
-        self.new_reward_col = [-1]
-        self.old_reward_col = [-3] if self.r==0 else [-3-self.r]
-        self.single_objective_tot = self.f + self.f + 1 + 1 + 1
-        self.solve = self.run
-
-    def run(self, evaluate):
-
-        self.evaluate = evaluate
-        self.initialize()
-        for self.it_no in range(0, self.s):
-            self.update()
-            self.vary()
-        return self.report()
-    
-    def initialize(self):
-
-        if self.r == 0:
-            self.pie = np.random.rand(self.t, self.single_objective_tot)
-            self.pie[:, self.new_reward_col] = - np.inf * self.d
-            self.pie[:, self.old_reward_col] = - np.inf * self.d
-            self.pie[:, self.status_col] = 0
-            self.best_index = -1*(1+self.d[0])//2
-            self.bad_status = -1
-        self.best = self.pie[-1].copy()
-
-    def update(self):
-
-        self.pie = self.evaluate(self.pie)
-        if self.r == 0:
-            self.pie[:,self.old_features_cols[0]:self.old_features_cols[1]] = np.where(np.reshape(self.d[0]*self.pie[:,self.new_reward_col[0]]>self.d[0]*self.pie[:,self.old_reward_col[0]], [self.t, 1]), self.pie[:,self.new_features_cols[0]:self.new_features_cols[1]], self.pie[:,self.old_features_cols[0]:self.old_features_cols[1]])
-            self.pie[:,self.old_reward_col[0]] = np.where(self.d[0]*self.pie[:,self.new_reward_col[0]]>self.d[0]*self.pie[:,self.old_reward_col[0]], self.pie[:,self.new_reward_col[0]], self.pie[:,self.old_reward_col[0]])
-            self.pie = self.pie[np.argsort(self.pie[:, self.old_reward_col[0]])]
-            if self.d[0]*self.pie[self.best_index][self.old_reward_col[0]] > self.d[0]*self.best[self.old_reward_col[0]]: self.best = self.pie[self.best_index].copy()
-
-    def vary(self):
-        
-        indices = np.array([np.random.randint(0,self.t, 3) for t in range(self.t)])
-        self.pie[:, :self.f] = np.where(np.random.rand(self.f) < self.cr, np.clip(self.pie[indices[:,0], :self.f] + self.mu * (self.pie[indices[:,1], :self.f] - self.pie[indices[:,2], :self.f]), 0, 1), self.pie[:, :self.f])
-
-    def report(self):
-
-        if self.r == 0: return self.best[self.old_features_cols[0]:self.old_features_cols[1]], self.best[self.old_reward_col[0]], self.best[self.status_col]
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+
+import numpy as np
+import warnings as wn
+
+wn.filterwarnings("ignore")
+
+
+class DE:
+
+    def __init__(self, f: int, d: list, s: int, t: int, cr: float, mu: float, **kwargs):
+
+        self.d = np.asarray([1 if item == 'max' else -1 for item in d])
+        self.r = 0 if len(d) == 1 else len(d)
+        self.f = f
+        self.s = s
+        self.t = t
+        self.cr = cr
+        self.mu = mu
+        self.new_features_cols = [0, self.f]
+        self.old_features_cols = [self.f, 2*self.f]
+        self.status_col = [-2]
+        self.new_reward_col = [-1]
+        self.old_reward_col = [-3] if self.r == 0 else [-3-self.r]
+        self.single_objective_tot = self.f + self.f + 1 + 1 + 1
+        self.solve = self.run
+
+    def run(self, evaluate):
+
+        self.evaluate = evaluate
+        self.initialize()
+        for self.it_no in range(0, self.s):
+            self.update()
+            self.vary()
+        return self.report()
+
+    def initialize(self):
+
+        if self.r == 0:
+            self.pie = np.random.rand(self.t, self.single_objective_tot)
+            self.pie[:, self.new_reward_col] = - np.inf * self.d
+            self.pie[:, self.old_reward_col] = - np.inf * self.d
+            self.pie[:, self.status_col] = 0
+            self.best_index = -1*(1+self.d[0])//2
+            self.bad_status = -1
+        self.best = self.pie[-1].copy()
+
+    def update(self):
+
+        self.pie = self.evaluate(self.pie)
+        if self.r == 0:
+            self.pie[:, self.old_features_cols[0]:self.old_features_cols[1]] = np.where(np.reshape(self.d[0]*self.pie[:, self.new_reward_col[0]] > self.d[0]*self.pie[:, self.old_reward_col[0]], [
+                                                                                        self.t, 1]), self.pie[:, self.new_features_cols[0]:self.new_features_cols[1]], self.pie[:, self.old_features_cols[0]:self.old_features_cols[1]])
+            self.pie[:, self.old_reward_col[0]] = np.where(self.d[0]*self.pie[:, self.new_reward_col[0]] > self.d[0] *
+                                                           self.pie[:, self.old_reward_col[0]], self.pie[:, self.new_reward_col[0]], self.pie[:, self.old_reward_col[0]])
+            self.pie = self.pie[np.argsort(
+                self.pie[:, self.old_reward_col[0]])]
+            if self.d[0]*self.pie[self.best_index][self.old_reward_col[0]] > self.d[0]*self.best[self.old_reward_col[0]]:
+                self.best = self.pie[self.best_index].copy()
+
+    def vary(self):
+
+        indices = np.array([np.random.randint(0, self.t, 3)
+                           for t in range(self.t)])
+        self.pie[:, :self.f] = np.where(np.random.rand(self.f) < self.cr, np.clip(self.pie[indices[:, 0], :self.f] + self.mu * (
+            self.pie[indices[:, 1], :self.f] - self.pie[indices[:, 2], :self.f]), 0, 1), self.pie[:, :self.f])
+
+    def report(self):
+
+        if self.r == 0:
+            return self.best[self.old_features_cols[0]:self.old_features_cols[1]], self.best[self.old_reward_col[0]], self.best[self.status_col]
```

### Comparing `feloopy-0.2.4/feloopy/algorithms/heuristic/GWO.py` & `feloopy-0.2.5/feloopy/algorithms/heuristic/GA.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,84 @@
-import numpy as np
-import warnings as wn
-
-wn.filterwarnings("ignore")
-
-class GWO:
-    
-    def __init__(self, f: int, d: list, s: int, t: int):
-
-        self.d = np.asarray([1 if item == 'max' else -1 for item in d])
-        self.r = 0 if len(d) == 1 else len(d)
-        self.f = f
-        self.it = s
-        self.t = t
-        self.features_cols = [0, self.f]
-        self.status_col = [-2]
-        self.reward_col = [-1]
-        self.single_objective_tot = self.f + 1 + 1
-        self.solve = self.run
-
-    def run(self, evaluate):
-
-        self.evaluate = evaluate
-        self.initialize()
-        for self.it_no in range(0, self.it):
-            self.update()
-            self.vary()
-        return self.report()
-
-    def initialize(self):
-
-        if self.r == 0:
-            self.pie = np.random.rand(self.t, self.single_objective_tot)
-            self.pie[:, self.reward_col] = - np.inf * self.d
-            self.pie[:, self.status_col] = 0
-            self.bad_status = -1
-            self.best_index = -1*(1+self.d[0])//2
-        self.alpha, self.beta, self.delta = np.copy(self.pie[-1]), np.copy(self.pie[-2]), np.copy(self.pie[-3])
-        self.best = self.pie[-1].copy()
-
-    def update(self):
-
-        self.pie = self.evaluate(self.pie)
-        if self.r == 0:
-            self.pie = self.pie[np.argsort(self.pie[:, self.reward_col[0]])]
-            if self.d[0]*self.pie[self.best_index][-1] > self.d[0]*self.best[-1]: self.best = self.pie[self.best_index].copy() 
-            self.alpha = self.pie[:, -1].copy()
-            self.beta = self.pie[:, -2].copy()
-            self.delta = self.pie[:, -3].copy()
-
-    def vary(self):
-
-        a = 2*(1 - self.it_no/self.it)*(2*np.random.rand(self.t, self.f, 3)-1)
-        c = 2*np.random.rand(self.t, self.f, 3)
-        self.pie[:, :self.f] = np.clip((self.alpha[:self.f] - a[:, :, 0] * abs(c[:, :, 0] * self.alpha[:self.f] - self.pie[:, :self.f]))/3 + (self.beta[:self.f] - a[:, :, 1] * abs(c[:, :, 1] * self.beta[:self.f] - self.pie[:, :self.f]))/3 + (self.delta[:self.f] - a[:, :, 2] * abs(c[:, :, 2] * self.delta[:self.f] - self.pie[:, :self.f]))/3, 0, 1)
-
-    def report(self):
-
-        if self.r == 0: return self.best[self.features_cols[0]:self.features_cols[1]], self.best[self.reward_col[0]], self.best[self.status_col]
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+
+import numpy as np
+import warnings as wn
+
+wn.filterwarnings("ignore")
+
+
+class GA:
+
+    def __init__(self, f: int, d: list, s: int, t: int, cr: float, mu: float, sfl: float, sfu: float, **kwargs):
+
+        self.d = np.asarray([1 if item == 'max' else -1 for item in d])
+        self.r = 0 if len(d) == 1 else len(d)
+        self.f = f
+        self.s = s
+        self.t = t
+        self.cr = cr
+        self.mu = mu
+        self.features_cols = [0, self.f]
+        self.status_col = [-2]
+        self.reward_col = [-1]
+        self.single_objective_tot = self.f + 1 + 1
+        self.survival_of_the_fittest_lb = sfl
+        self.survival_of_the_fittest_ub = sfu
+        self.solve = self.run
+
+    def run(self, evaluate):
+
+        self.evaluate = evaluate
+        self.initialize()
+        for self.it_no in range(0, self.s):
+            self.update()
+            self.vary()
+        return self.report()
+
+    def initialize(self):
+
+        if self.r == 0:
+            self.pie = np.random.rand(self.t, self.single_objective_tot)
+            self.pie[:, self.reward_col] = - np.inf * self.d
+            self.pie[:, self.status_col] = 0
+            self.best_index = -1*(1+self.d[0])//2
+            self.bad_status = -1
+        self.best = self.pie[-1].copy()
+
+    def update(self):
+
+        self.pie = self.evaluate(self.pie)
+        if self.r == 0:
+            self.pie = self.pie[np.argsort(self.pie[:, self.reward_col[0]])]
+            if self.d[0]*self.pie[self.best_index][self.reward_col[0]] > self.d[0]*self.best[self.reward_col[0]]:
+                self.best = self.pie[self.best_index].copy()
+            cut = int(np.random.uniform(self.survival_of_the_fittest_lb,
+                      self.survival_of_the_fittest_ub)*self.t)
+            if self.d[0] == 1:
+                self.pie[:cut] = self.pie[np.random.choice(self.t, cut)]
+            else:
+                self.pie[cut:] = self.pie[np.random.choice(self.t, self.t-cut)]
+
+    def vary(self):
+
+        pool = np.asarray([np.array([t, np.random.randint(0, self.t)]) if np.random.rand(
+        ) < self.cr else np.array([t, t]) for t in range(0, self.t)], dtype=np.int64)
+        self.pie[:, self.features_cols[0]:self.features_cols[1]] = np.where(np.random.randint(0, 2, size=(self.t, self.f)) == 1, self.pie[pool.T[1], self.features_cols[0]:self.features_cols[1]] + np.random.uniform(-1, 1, size=(
+            self.t, self.f))*(self.pie[pool.T[1], self.features_cols[0]:self.features_cols[1]]-self.pie[pool.T[0], self.features_cols[0]:self.features_cols[1]]), self.pie[pool.T[0], self.features_cols[0]:self.features_cols[1]])
+        self.pie[:, self.features_cols[0]:self.features_cols[1]] = np.where((np.random.rand(
+            self.t, self.f) < self.mu), 1-self.pie[:, self.features_cols[0]:self.features_cols[1]], self.pie[:, self.features_cols[0]:self.features_cols[1]])
+        self.pie[:, self.features_cols[0]:self.features_cols[1]] = np.clip(
+            self.pie[:, self.features_cols[0]:self.features_cols[1]], 0, 1)
+
+    def report(self):
+
+        if self.r == 0:
+            return self.best[self.features_cols[0]:self.features_cols[1]], self.best[self.reward_col[0]], self.best[self.status_col]
```

### Comparing `feloopy-0.2.4/feloopy/algorithms/heuristic/SA.py` & `feloopy-0.2.5/feloopy/algorithms/heuristic/SA.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,81 @@
-import numpy as np
-import warnings as wn
-
-wn.filterwarnings("ignore")
-
-class SA:
-
-    def __init__(self, f: int, d: list, s: int, t: int, cc: int, mt: int):
- 
-        self.d = np.asarray([1 if item == 'max' else -1 for item in d])
-        self.r = 0 if len(d) == 1 else len(d)
-        self.f = f
-        self.s = s
-        self.t = t
-        self.cc = cc
-        self.mt = mt
-        self.new_features_cols = [0, self.f]
-        self.old_features_cols = [self.f, 2*self.f]
-        self.status_col = [-2]
-        self.new_reward_col = [-1]
-        self.old_reward_col = [-3] if self.r==0 else [-3-self.r]
-        self.single_objective_tot = self.f + self.f + 1 + 1 + 1
-        self.solve = self.run
-
-    def run(self, evaluate):
-
-        self.evaluate = evaluate
-        self.initialize()
-        for self.it_no in range(0, self.s):
-            for self.c in range(0, self.cc):
-                self.update()
-                self.vary()
-        return self.report()
-    
-    def initialize(self):
-
-        if self.r == 0:
-            self.pie = np.random.rand(1, self.single_objective_tot)
-            self.pie[:, self.new_reward_col] = - np.inf * self.d
-            self.pie[:, self.old_reward_col] = - np.inf * self.d
-            self.pie[:, self.status_col] = 0
-            self.best_index = -1*(1+self.d[0])//2
-            self.bad_status = -1
-        self.best = self.pie[-1].copy()
-
-    def update(self):
-        
-        self.pie = self.evaluate(self.pie)
-        Accept = np.random.rand()
-        if self.r == 0:
-            self.pie[:,self.new_features_cols[0]:self.new_features_cols[1]] = np.where(self.d[0]*self.pie[:,self.new_reward_col[0]] > self.d[0]*self.pie[:,self.old_reward_col[0]] or Accept < np.exp(-abs(self.pie[:,self.old_reward_col[0]] -self.pie[:,self.new_reward_col[0]])/(((self.s-self.it_no)/self.s)*self.mt)), self.pie[:,self.new_features_cols[0]:self.new_features_cols[1]], self.pie[:,self.old_features_cols[0]:self.old_features_cols[1]])
-            self.pie[:,self.new_reward_col[0]] = np.where(self.d[0]*self.pie[:,self.new_reward_col[0]] > self.d[0]*self.pie[:,self.old_reward_col[0]] or Accept < np.exp(-abs(self.pie[:,self.old_reward_col[0]] -self.pie[:,self.new_reward_col[0]])/(((self.s-self.it_no)/self.s)*self.mt)), self.pie[:,self.new_reward_col[0]], self.pie[:,self.old_reward_col[0]])
-            self.pie[:,self.old_features_cols[0]:self.old_features_cols[1]] = np.where(self.d[0]*self.pie[:,self.new_reward_col[0]] > self.d[0]*self.pie[:,self.old_reward_col[0]] or Accept < np.exp(-abs(self.pie[:,self.old_reward_col[0]] -self.pie[:,self.new_reward_col[0]])/(((self.s-self.it_no)/self.s)*self.mt)), self.pie[:,self.new_features_cols[0]:self.new_features_cols[1]], self.pie[:,self.old_features_cols[0]:self.old_features_cols[1]])
-            self.pie[:,self.old_reward_col[0]] = np.where(self.d[0]*self.pie[:,self.new_reward_col[0]] > self.d[0]*self.pie[:,self.old_reward_col[0]] or Accept < np.exp(-abs(self.pie[:,self.old_reward_col[0]] -self.pie[:,self.new_reward_col[0]])/(((self.s-self.it_no)/self.s)*self.mt)), self.pie[:,self.new_reward_col[0]], self.pie[:,self.old_reward_col[0]])
-            if self.d[0]*self.pie[self.best_index][self.old_reward_col[0]] > self.d[0]*self.best[self.old_reward_col[0]]: self.best = self.pie[self.best_index].copy()
-
-    def vary(self):
-
-        self.pie[:, :self.f] = np.clip(self.pie[:, :self.f] + 2*np.random.rand(self.f)-1, 0, 1)
-
-    def report(self):
-
-        if self.r == 0: return self.best[self.old_features_cols[0]:self.old_features_cols[1]], self.best[self.old_reward_col[0]], self.best[self.status_col]
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+import numpy as np
+import warnings as wn
+
+wn.filterwarnings("ignore")
+
+
+class SA:
+
+    def __init__(self, f: int, d: list, s: int, t: int, cc: int, mt: int, **kwargs):
+
+        self.d = np.asarray([1 if item == 'max' else -1 for item in d])
+        self.r = 0 if len(d) == 1 else len(d)
+        self.f = f
+        self.s = s
+        self.t = t
+        self.cc = cc
+        self.mt = mt
+        self.new_features_cols = [0, self.f]
+        self.old_features_cols = [self.f, 2*self.f]
+        self.status_col = [-2]
+        self.new_reward_col = [-1]
+        self.old_reward_col = [-3] if self.r == 0 else [-3-self.r]
+        self.single_objective_tot = self.f + self.f + 1 + 1 + 1
+        self.solve = self.run
+
+    def run(self, evaluate):
+
+        self.evaluate = evaluate
+        self.initialize()
+        for self.it_no in range(0, self.s):
+            for self.c in range(0, self.cc):
+                self.update()
+                self.vary()
+        return self.report()
+
+    def initialize(self):
+
+        if self.r == 0:
+            self.pie = np.random.rand(1, self.single_objective_tot)
+            self.pie[:, self.new_reward_col] = - np.inf * self.d
+            self.pie[:, self.old_reward_col] = - np.inf * self.d
+            self.pie[:, self.status_col] = 0
+            self.best_index = -1*(1+self.d[0])//2
+            self.bad_status = -1
+        self.best = self.pie[-1].copy()
+
+    def update(self):
+
+        self.pie = self.evaluate(self.pie)
+        Accept = np.random.rand()
+        if self.r == 0:
+            self.pie[:, self.new_features_cols[0]:self.new_features_cols[1]] = np.where(self.d[0]*self.pie[:, self.new_reward_col[0]] > self.d[0]*self.pie[:, self.old_reward_col[0]] or Accept < np.exp(-abs(
+                self.pie[:, self.old_reward_col[0]] - self.pie[:, self.new_reward_col[0]])/(((self.s-self.it_no)/self.s)*self.mt)), self.pie[:, self.new_features_cols[0]:self.new_features_cols[1]], self.pie[:, self.old_features_cols[0]:self.old_features_cols[1]])
+            self.pie[:, self.new_reward_col[0]] = np.where(self.d[0]*self.pie[:, self.new_reward_col[0]] > self.d[0]*self.pie[:, self.old_reward_col[0]] or Accept < np.exp(-abs(
+                self.pie[:, self.old_reward_col[0]] - self.pie[:, self.new_reward_col[0]])/(((self.s-self.it_no)/self.s)*self.mt)), self.pie[:, self.new_reward_col[0]], self.pie[:, self.old_reward_col[0]])
+            self.pie[:, self.old_features_cols[0]:self.old_features_cols[1]] = np.where(self.d[0]*self.pie[:, self.new_reward_col[0]] > self.d[0]*self.pie[:, self.old_reward_col[0]] or Accept < np.exp(-abs(
+                self.pie[:, self.old_reward_col[0]] - self.pie[:, self.new_reward_col[0]])/(((self.s-self.it_no)/self.s)*self.mt)), self.pie[:, self.new_features_cols[0]:self.new_features_cols[1]], self.pie[:, self.old_features_cols[0]:self.old_features_cols[1]])
+            self.pie[:, self.old_reward_col[0]] = np.where(self.d[0]*self.pie[:, self.new_reward_col[0]] > self.d[0]*self.pie[:, self.old_reward_col[0]] or Accept < np.exp(-abs(
+                self.pie[:, self.old_reward_col[0]] - self.pie[:, self.new_reward_col[0]])/(((self.s-self.it_no)/self.s)*self.mt)), self.pie[:, self.new_reward_col[0]], self.pie[:, self.old_reward_col[0]])
+            if self.d[0]*self.pie[self.best_index][self.old_reward_col[0]] > self.d[0]*self.best[self.old_reward_col[0]]:
+                self.best = self.pie[self.best_index].copy()
+
+    def vary(self):
+
+        self.pie[:, :self.f] = np.clip(
+            self.pie[:, :self.f] + 2*np.random.rand(self.f)-1, 0, 1)
+
+    def report(self):
+
+        if self.r == 0:
+            return self.best[self.old_features_cols[0]:self.old_features_cols[1]], self.best[self.old_reward_col[0]], self.best[self.status_col]
```

### Comparing `feloopy-0.2.4/feloopy/functions/update_operators.py` & `feloopy-0.2.5/feloopy/operators/update_operators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,45 @@
-
-from .count_operators import *
-
-def update_variable_features(name, variable_dim, variable_bound, variable_counter_type, features):
-    """ For hierarchical updating the features of the problem.
-    """
-    match features['solution_method']:
-
-        case 'exact':
-
-            features['total_variable_counter'], features['variable_counter_type'] = count_variable(
-                variable_dim, features['total_variable_counter'], features[variable_counter_type])
-
-        case 'heuristic':
-
-            if features['agent_status'] == 'idle':
-
-                features['variable_spread'][name] = [
-                    features['total_variable_counter'][1], 0]
-                features['total_variable_counter'], features[variable_counter_type] = count_variable(
-                    variable_dim, features['total_variable_counter'], features[variable_counter_type])
-                features['variable_spread'][name][1] = features['total_variable_counter'][1]
-                if variable_counter_type == 'free_variable_counter':
-                    features['variable_type'][name] = 'fvar'
-                if variable_counter_type == 'binary_variable_counter':
-                    features['variable_type'][name] = 'bvar'
-                if variable_counter_type == 'integer_variable_counter':
-                    features['variable_type'][name] = 'ivar'
-                if variable_counter_type == 'positive_variable_counter':
-                    features['variable_type'][name] = 'pvar'
-                features['variable_bound'][name] = variable_bound
-                features['variable_dim'][name] = variable_dim
-
-    return features
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+
+from .count_operators import *
+
+
+def update_variable_features(name, variable_dim, variable_bound, variable_counter_type, features):
+    """ For hierarchical updating the features of the problem.
+    """
+    match features['solution_method']:
+
+        case 'exact':
+
+            features['total_variable_counter'], features['variable_counter_type'] = count_variable(
+                variable_dim, features['total_variable_counter'], features[variable_counter_type])
+
+        case 'heuristic':
+
+            if features['agent_status'] == 'idle':
+
+                features['variable_spread'][name] = [
+                    features['total_variable_counter'][1], 0]
+                features['total_variable_counter'], features[variable_counter_type] = count_variable(
+                    variable_dim, features['total_variable_counter'], features[variable_counter_type])
+                features['variable_spread'][name][1] = features['total_variable_counter'][1]
+                if variable_counter_type == 'free_variable_counter':
+                    features['variable_type'][name] = 'fvar'
+                if variable_counter_type == 'binary_variable_counter':
+                    features['variable_type'][name] = 'bvar'
+                if variable_counter_type == 'integer_variable_counter':
+                    features['variable_type'][name] = 'ivar'
+                if variable_counter_type == 'positive_variable_counter':
+                    features['variable_type'][name] = 'pvar'
+                features['variable_bound'][name] = variable_bound
+                features['variable_dim'][name] = variable_dim
+
+    return features
```

### Comparing `feloopy-0.2.4/feloopy/generators/model/mealpy_model_generator.py` & `feloopy-0.2.5/feloopy/generators/model/mealpy_model_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,708 +1,806 @@
-
-def generate_model(solver_name,solver_options):
-
-        match solver_name:
-
-            #============ Evolutionary
-
-            case 'OriginalEP':
-                from mealpy.evolutionary_based import EP
-                model_object = EP.OriginalEP(**solver_options)
-            
-            case 'LevyEP':
-                from mealpy.evolutionary_based import EP
-                model_object = EP.LevyEP(**solver_options)
-
-            case 'OriginalES':
-                from mealpy.evolutionary_based import ES
-                model_object = ES.OriginalES(**solver_options)
-            
-            case 'LevyES':
-                from mealpy.evolutionary_based import ES
-                model_object = ES.LevyES(**solver_options)
-            
-            case 'OriginalMA':
-                from mealpy.evolutionary_based import MA
-                model_object = MA.OriginalMA(**solver_options)
-            
-            case 'BaseGA':
-                from mealpy.evolutionary_based import GA
-                model_object = GA.BaseGA(**solver_options)
-
-            case 'SingleGA':
-                from mealpy.evolutionary_based import GA
-                model_object = GA.SingleGA(**solver_options)
-            
-            case 'MultiGA':
-                from mealpy.evolutionary_based import GA
-                model_object = GA.MultiGA(**solver_options)
-
-            case 'EliteSingleGA':
-                from mealpy.evolutionary_based import GA
-                model_object = GA.EliteSingleGA(**solver_options)
-
-            case 'EliteMultiGA':
-                from mealpy.evolutionary_based import GA
-                model_object = GA.EliteMultiGA(**solver_options)
-
-            case 'BaseDE':
-                from mealpy.evolutionary_based import DE
-                model_object = DE.BaseDE(**solver_options)
-
-            case 'JADE':
-                from mealpy.evolutionary_based import DE
-                model_object = DE.JADE(**solver_options)
-
-            case 'SADE':
-                from mealpy.evolutionary_based import DE
-                model_object = DE.SADE(**solver_options)
-            
-            case 'SHADE':
-                from mealpy.evolutionary_based import DE
-                model_object = DE.SHADE(**solver_options)
-
-            case 'L_SHADE':
-                from mealpy.evolutionary_based import DE
-                model_object = DE.L_SHADE(**solver_options)
-
-            case 'SAP_DE':
-                from mealpy.evolutionary_based import DE
-                model_object = DE.SAP_DE(**solver_options)
-
-            case 'OriginalFPA':
-                from mealpy.evolutionary_based import FPA
-                model_object = FPA.OriginalFPA(**solver_options)
-
-            case 'OriginalCRO':
-                from mealpy.evolutionary_based import CRO
-                model_object = CRO.OriginalCRO(**solver_options)
-
-            case 'OCRO':
-                from mealpy.evolutionary_based import CRO
-                model_object = CRO.OCRO(**solver_options)
-
-            #============ Swarm
-
-            case 'OriginalPSO':
-                from mealpy.swarm_based import PSO
-                model_object = PSO.OriginalPSO(**solver_options)
-
-            case 'PPSO':
-                from mealpy.swarm_based import PSO
-                model_object = PSO.PPSO(**solver_options)
-
-            case 'HPSO_TVAC':
-                from mealpy.swarm_based import PSO
-                model_object = PSO.HPSO_TVAC(**solver_options)
-
-            case 'C_PSO':
-                from mealpy.swarm_based import PSO
-                model_object = PSO.C_PSO(**solver_options)
-
-            case 'CL_PSO':
-                from mealpy.swarm_based import PSO
-                model_object = PSO.CL_PSO(**solver_options)
-
-            case 'OriginalBFO':
-                from mealpy.swarm_based import BFO
-                model_object = BFO.OriginalBFO(**solver_options)
-
-            case 'ABFO':
-                from mealpy.swarm_based import BFO
-                model_object = BFO.OriginalBFO(**solver_options)
-
-            case 'OriginalBeesA':
-                from mealpy.swarm_based import BeesA
-                model_object = BeesA.OriginalBeesA(**solver_options)
-
-            case 'ProbBeesA':
-                from mealpy.swarm_based import BeesA
-                model_object = BeesA.ProbBeesA(**solver_options)
-
-            case 'OriginalCSO':
-                from mealpy.swarm_based import CSO
-                model_object = CSO.OriginalCSO(**solver_options)
-                
-            case 'OriginalABC':
-                from mealpy.swarm_based import ABC
-                model_object = ABC.OriginalABC(**solver_options)
-
-            case 'OriginalACOR':
-                from mealpy.swarm_based import ACOR
-                model_object = ACOR.OriginalACOR(**solver_options)
-
-            case 'OriginalCSA':
-                from mealpy.swarm_based import CSA
-                model_object = CSA.OriginalCSA(**solver_options)
-
-            case 'OriginalFFA':
-                from mealpy.swarm_based import FFA
-                model_object = FFA.OriginalFFA(**solver_options)
-
-            case 'OriginalFA':
-                from mealpy.swarm_based import FA
-                model_object = FA.OriginalFA(**solver_options)
-
-            case 'OriginalBA':
-                from mealpy.swarm_based import BA
-                model_object = BA.OriginalBA(**solver_options)
-
-            case 'AdaptiveBA':
-                from mealpy.swarm_based import BA
-                model_object = BA.AdaptiveBA(**solver_options)
-
-            case 'ModifiedBA':
-                from mealpy.swarm_based import BA
-                model_object = BA.ModifiedBA(**solver_options)
-
-            case 'OriginalFOA':
-                from mealpy.swarm_based import FOA
-                model_object = FOA.OriginalFOA(**solver_options)
-
-            case 'BaseFOA':
-                from mealpy.swarm_based import FOA
-                model_object = FOA.BaseFOA(**solver_options)
-
-            case 'WhaleFOA':
-                from mealpy.swarm_based import FOA
-                model_object = FOA.WhaleFOA(**solver_options)
-
-            case 'OriginalSSpiderO':
-                from mealpy.swarm_based import SSpiderO
-                model_object = SSpiderO.OriginalSSpiderO(**solver_options)
-
-            case 'OriginalGWO':
-                from mealpy.swarm_based import GWO
-                model_object = GWO.OriginalGWO(**solver_options)
-
-            case 'RW_GWO':
-                from mealpy.swarm_based import GWO
-                model_object = GWO.RW_GWO(**solver_options)
-
-            case 'OriginalSSpiderA':
-                from mealpy.swarm_based import SSpiderA
-                model_object = SSpiderA.OriginalSSpiderA(**solver_options)
-
-            case 'OriginalALO':
-                from mealpy.swarm_based import ALO
-                model_object = ALO.OriginalALO(**solver_options)
-
-            case 'BaseALO':
-                from mealpy.swarm_based import ALO
-                model_object = ALO.BaseALO(**solver_options)
-
-            case 'OriginalMFO':
-                from mealpy.swarm_based import MFO
-                model_object = MFO.OriginalMFO(**solver_options)
-
-            case 'BaseMFO':
-                from mealpy.swarm_based import MFO
-                model_object = MFO.BaseMFO(**solver_options)
-
-            case 'OriginalEHO':
-                from mealpy.swarm_based import EHO
-                model_object = EHO.OriginalEHO(**solver_options)
-
-            case 'OriginalJA':
-                from mealpy.swarm_based import JA
-                model_object = JA.OriginalJA(**solver_options)
-
-            case 'BaseJA':
-                from mealpy.swarm_based import JA
-                model_object = JA.BaseJA(**solver_options)
-
-            case 'LevyJA':
-                from mealpy.swarm_based import JA
-                model_object = JA.LevyJA(**solver_options)
-
-            case 'OriginalWOA':
-                from mealpy.swarm_based import WOA
-                model_object = WOA.OriginalWOA(**solver_options)
-
-            case 'HI_WOA':
-                from mealpy.swarm_based import WOA
-                model_object = WOA.HI_WOA(**solver_options)
-
-            case 'OriginalDO':
-                from mealpy.swarm_based import DO
-                model_object = DO.OriginalDO(**solver_options)
-
-            case 'OriginalBSA':
-                from mealpy.swarm_based import BSA
-                model_object = BSA.OriginalBSA(**solver_options)
-
-            case 'OriginalSHO':
-                from mealpy.swarm_based import SHO
-                model_object = SHO.OriginalSHO(**solver_options)
-
-            case 'OriginalSSO':
-                from mealpy.swarm_based import SSO
-                model_object = SSO.OriginalSSO(**solver_options)
-
-            case 'OriginalSRSR':
-                from mealpy.swarm_based import SRSR
-                model_object = SRSR.OriginalSRSR(**solver_options)
-
-            case 'OriginalGOA':
-                from mealpy.swarm_based import GOA
-                model_object = GOA.OriginalGOA(**solver_options)
-
-            case 'OriginalCOA':
-                from mealpy.swarm_based import COA
-                model_object = COA.OriginalCOA(**solver_options)
-
-            case 'OriginalMSA':
-                from mealpy.swarm_based import MSA
-                model_object = MSA.OriginalMSA(**solver_options)
-
-            case 'OriginalSLO':
-                from mealpy.swarm_based import SLO
-                model_object = SLO.OriginalSLO(**solver_options)
-
-            case 'ModifiedSLO':
-                from mealpy.swarm_based import SLO
-                model_object = SLO.ModifiedSLO(**solver_options)
-
-            case 'ImprovedSLO':
-                from mealpy.swarm_based import SLO
-                model_object = SLO.ImprovedSLO(**solver_options)
-
-            case 'OriginalNMRA':
-                from mealpy.swarm_based import NMRA
-                model_object = NMRA.OriginalNMRA(**solver_options)
-
-            case 'ImprovedNMRA':
-                from mealpy.swarm_based import NMRA
-                model_object = NMRA.ImprovedNMRA(**solver_options)
-
-            case 'OriginalPFA':
-                from mealpy.swarm_based import PFA
-                model_object = PFA.OriginalPFA(**solver_options)
-
-            case 'OriginalSFO':
-                from mealpy.swarm_based import SFO
-                model_object = SFO.OriginalSFO(**solver_options)
-
-            case 'ImprovedSFO':
-                from mealpy.swarm_based import SFO
-                model_object = SFO.ImprovedSFO(**solver_options)
-                
-            case 'OriginalHHO':
-                from mealpy.swarm_based import HHO
-                model_object = HHO.OriginalHHO(**solver_options)
-
-            case 'OriginalMRFO':
-                from mealpy.swarm_based import MRFO
-                model_object = MRFO.OriginalMRFO(**solver_options)
-
-            case 'OriginalBES':
-                from mealpy.swarm_based import BES
-                model_object = BES.OriginalBES(**solver_options)
-
-            case 'OriginalSSA':
-                from mealpy.swarm_based import SSA
-                model_object = SSA.OriginalSSA(**solver_options)
-
-            case 'BaseSSA':
-                from mealpy.swarm_based import SSA
-                model_object = SSA.BaseSSA(**solver_options)
-
-            case 'OriginalHGS':
-                from mealpy.swarm_based import HGS
-                model_object = HGS.OriginalHGS(**solver_options)
-
-            case 'OriginalAO':
-                from mealpy.swarm_based import AO
-                model_object = AO.OriginalAO(**solver_options)
-
-            case 'GWO_WOA':
-                from mealpy.swarm_based import GWO
-                model_object = GWO.OriginalGWO(**solver_options)
-
-            case 'OriginalMPA':
-                from mealpy.swarm_based import MPA
-                model_object = MPA.OriginalMPA(**solver_options)
-
-            case 'OriginalHBA':
-                from mealpy.swarm_based import HBA
-                model_object = HBA.OriginalHBA(**solver_options)
-
-            case 'OriginalSCSO':
-                from mealpy.swarm_based import SCSO
-                model_object = SCSO.OriginalSCSO(**solver_options)
-
-            case 'OriginalTSO':
-                from mealpy.swarm_based import TSO
-                model_object = TSO.OriginalTSO(**solver_options)
-
-            case 'OriginalAVOA':
-                from mealpy.swarm_based import AVOA
-                model_object = AVOA.OriginalAVOA(**solver_options)
-
-            case 'OriginalAGTO':
-                from mealpy.swarm_based import AGTO
-                model_object = AGTO.OriginalAGTO(**solver_options)
-
-            case 'OriginalARO':
-                from mealpy.swarm_based import ARO
-                model_object = ARO.OriginalARO(**solver_options)
-
-            #============ Physics
-
-            case 'OriginalSA':
-                from mealpy.physics_based import SA
-                model_object = SA.OriginalSA(**solver_options)
-
-            case 'OriginalWDO':
-                from mealpy.physics_based import WDO
-                model_object = WDO.OriginalWDO(**solver_options)
-
-            case 'OriginalMVO':
-                from mealpy.physics_based import MVO
-                model_object = MVO.OriginalMVO(**solver_options)
-
-            case 'BaseMVO':
-                from mealpy.physics_based import MVO
-                model_object = MVO.BaseMVO(**solver_options)
-
-            case 'OriginalTWO':
-                from mealpy.physics_based import TWO
-                model_object = TWO.OriginalTWO(**solver_options)
-
-            case 'OppoTWO':
-                from mealpy.physics_based import TWO
-                model_object = TWO.OppoTWO(**solver_options)
-
-            case 'LevyTWO':
-                from mealpy.physics_based import TWO
-                model_object = TWO.LevyTWO(**solver_options)
-
-            case 'EnhancedTWO':
-                from mealpy.physics_based import TWO
-                model_object = TWO.EnhancedTWO(**solver_options)
-
-            case 'OriginalEFO':
-                from mealpy.physics_based import EFO
-                model_object = EFO.OriginalEFO(**solver_options)
-
-            case 'BaseEFO':
-                from mealpy.physics_based import EFO
-                model_object = EFO.BaseEFO(**solver_options)
-
-            case 'OriginalNRO':
-                from mealpy.physics_based import NRO
-                model_object = NRO.OriginalNRO(**solver_options)
-
-            case 'OriginalHGSO':
-                from mealpy.physics_based import HGSO
-                model_object = HGSO.OriginalHGSO(**solver_options)
-
-            case 'OriginalASO':
-                from mealpy.physics_based import ASO
-                model_object = ASO.OriginalASO(**solver_options)
-
-            case 'OriginalEO':
-                from mealpy.physics_based import EO
-                model_object = EO.OriginalEO(**solver_options)
-
-            case 'ModifiedEO':
-                from mealpy.physics_based import EO
-                model_object = EO.ModifiedEO(**solver_options)
-
-            case 'AdaptiveEO':
-                from mealpy.physics_based import EO
-                model_object = EO.AdaptiveEO(**solver_options)
-
-            case 'OriginalArchOA':
-                from mealpy.physics_based import ArchOA
-                model_object = ArchOA.OriginalArchOA(**solver_options)
-
-            #============ Human
-
-            case 'OriginalCA':
-                from mealpy.human_based import CA
-                model_object = CA.OriginalCA(**solver_options)
-
-            case 'OriginalICA':
-                from mealpy.human_based import ICA
-                model_object = ICA.OriginalICA(**solver_options)
-
-            case 'OriginalTLO':
-                from mealpy.human_based import TLO
-                model_object = TLO.OriginalTLO(**solver_options)
-            
-            case 'BaseTLO':
-                from mealpy.human_based import TLO
-                model_object = TLO.BaseTLO(**solver_options)
-
-            case 'ITLO':
-                from mealpy.human_based import TLO
-                model_object = TLO.ImprovedTLO(**solver_options)
-
-            case 'OriginalBSO':
-                from mealpy.human_based import BSO
-                model_object = BSO.OriginalBSO(**solver_options)
-
-            case 'ImprovedBSO':
-                from mealpy.human_based import BSO
-                model_object = BSO.ImprovedBSO(**solver_options)
-
-            case 'OriginalQSA':
-                from mealpy.human_based import QSA
-                model_object = QSA.OriginalQSA(**solver_options)
-
-            case 'BaseQSA':
-                from mealpy.human_based import QSA
-                model_object = QSA.BaseQSA(**solver_options)
-
-            case 'OppoQSA':
-                from mealpy.human_based import QSA
-                model_object = QSA.OppoQSA(**solver_options)
-
-            case 'LevyQSA':
-                from mealpy.human_based import QSA
-                model_object = QSA.LevyQSA(**solver_options)
-
-            case 'ImprovedQSA':
-                from mealpy.human_based import QSA
-                model_object = QSA.ImprovedQSA(**solver_options)
-
-            case 'OriginalSARO':
-                from mealpy.human_based import SARO
-                model_object = SARO.OriginalSARO(**solver_options)
-
-            case 'BaseSARO':
-                from mealpy.human_based import SARO
-                model_object = SARO.BaseSARO(**solver_options)
-
-            case 'OriginalLCO':
-                from mealpy.human_based import LCO
-                model_object = LCO.OriginalLCO(**solver_options)
-                
-            case 'BaseLCO':
-                from mealpy.human_based import LCO
-                model_object = LCO.BaseLCO(**solver_options)
-
-            case 'ImprovedLCO':
-                from mealpy.human_based import LCO
-                model_object = LCO.ImprovedLCO(**solver_options)
-
-            case 'OriginalSSDO':
-                from mealpy.human_based import SSDO
-                model_object = SSDO.OriginalSSDO(**solver_options)
-
-            case 'OriginalGSKA':
-                from mealpy.human_based import GSKA
-                model_object = GSKA.OriginalGSKA(**solver_options)
-
-            case 'BaseGSKA':
-                from mealpy.human_based import GSKA
-                model_object = GSKA.BaseGSKA(**solver_options)
-
-            case 'OriginalCHIO':
-                from mealpy.human_based import CHIO
-                model_object = CHIO.OriginalCHIO(**solver_options)
-
-            case 'BaseCHIO':
-                from mealpy.human_based import CHIO
-                model_object = CHIO.BaseCHIO(**solver_options)
-
-            case 'OriginalFBIO':
-                from mealpy.human_based import FBIO
-                model_object = FBIO.OriginalFBIO(**solver_options)
-
-            case 'BaseFBIO':
-                from mealpy.human_based import FBIO
-                model_object = FBIO.BaseFBIO(**solver_options)
-
-            case 'OriginalBRO':
-                from mealpy.human_based import BRO
-                model_object = BRO.OriginalBRO(**solver_options)
-            
-            case 'BaseBRO':
-                from mealpy.human_based import BRO
-                model_object = BRO.BaseBRO(**solver_options)
-
-            case 'OriginalSPBO':
-                from mealpy.human_based import SPBO
-                model_object = SPBO.OriginalSPBO(**solver_options)
-
-            case 'DevSPBO':
-                from mealpy.human_based import SPBO
-                model_object = SPBO.DevSPBO(**solver_options)
-
-            case 'OriginalDMOA':
-                print('OriginalDMOA: Not supported yet. Using SPBO instead')
-                # from mealpy.human_based import DMOA
-                # model_object = DMOA.OriginalDMOA(**solver_options)
-                from mealpy.human_based import SPBO
-                model_object = SPBO.DevSPBO(**solver_options)
-
-            case 'DevDMOA':
-                print('DevDMOA: Not supported yet. Using SPBO instead')
-                # from mealpy.human_based import DMOA
-                # model_object = DMOA.DevDMOA(**solver_options)
-                from mealpy.human_based import SPBO
-                model_object = SPBO.DevSPBO(**solver_options)
-
-            #============ Bio
-
-            case 'OriginalIWO':
-                from mealpy.bio_based import IWO
-                model_object = IWO.OriginalIWO(**solver_options)
-
-            case 'OriginalBBO':
-                from mealpy.bio_based import BBO
-                model_object = BBO.OriginalBBO(**solver_options)
-
-            case 'BaseBBO':
-                from mealpy.bio_based import BBO
-                model_object = BBO.BaseBBO(**solver_options)
-
-            case 'OriginalVCS':
-                from mealpy.bio_based import VCS
-                model_object = VCS.OriginalVCS(**solver_options)
-
-            case 'BaseVCS':
-                from mealpy.bio_based import VCS
-                model_object = VCS.BaseVCS(**solver_options)
-
-            case 'OriginalSBO':
-                from mealpy.bio_based import SBO
-                model_object = SBO.OriginalSBO(**solver_options)
-
-            case 'BaseSBO':
-                from mealpy.bio_based import SBO
-                model_object = SBO.BaseSBO(**solver_options)
-
-            case 'OriginalEOA':
-                from mealpy.bio_based import EOA
-                model_object = EOA.OriginalEOA(**solver_options)
-
-            case 'OriginalWHO':
-                from mealpy.bio_based import WHO
-                model_object = WHO.OriginalWHO(**solver_options)
-
-            case 'OriginalSMA':
-                from mealpy.bio_based import SMA
-                model_object = SMA.OriginalSMA(**solver_options)
-
-            case 'BaseSMA':
-                from mealpy.bio_based import SMA
-                model_object = SMA.BaseSMA(**solver_options)
-
-            case 'OriginalBMO':
-                from mealpy.bio_based import BMO
-                model_object = BMO.OriginalBMO(**solver_options)
-
-            case 'OriginalTSA':
-                from mealpy.bio_based import TSA
-                model_object = TSA.OriginalTSA(**solver_options)
-
-            case 'OriginalSOS':
-                from mealpy.bio_based import SOS
-                model_object = SOS.OriginalSOS(**solver_options)
-
-            case 'OriginalSOA':
-                from mealpy.bio_based import SOA
-                model_object = SOA.OriginalSOA(**solver_options)
-
-            case 'DevSOA':
-                from mealpy.bio_based import SOA
-                model_object = SOA.DevSOA(**solver_options)
-
-            #============ System
-
-            case 'OriginalGCO':
-                from mealpy.system_based import GCO
-                model_object = GCO.OriginalGCO(**solver_options)
-
-            case 'BaseGCO':
-                from mealpy.system_based import GCO
-                model_object = GCO.BaseGCO(**solver_options)
-
-            case 'OriginalWCA':
-                from mealpy.system_based import WCA
-                model_object = WCA.OriginalWCA(**solver_options)
-
-            case 'OriginalAEO':
-                from mealpy.system_based import AEO
-                model_object = AEO.OriginalAEO(**solver_options)
-
-            case 'EnhancedAEO':
-                from mealpy.system_based import AEO
-                model_object = AEO.EnhancedAEO(**solver_options)
-
-            case 'ModifiedAEO':
-                from mealpy.system_based import AEO
-                model_object = AEO.ModifiedAEO(**solver_options)
-
-            case 'ImprovedAEO':
-                from mealpy.system_based import AEO
-                model_object = AEO.ImprovedAEO(**solver_options)
-
-            case 'AdaptiveAEO':
-                from mealpy.system_based import AEO
-                model_object = AEO.AdaptiveAEO(**solver_options)
-
-            #============ Math
-
-            case 'OriginalHC':
-                from mealpy.math_based import HC
-                model_object = HC.OriginalHC(**solver_options)
-
-            case 'SwarmHC':
-                from mealpy.math_based import HC
-                model_object = HC.SwarmHC(**solver_options)
-
-            case 'OriginalCEM':
-                from mealpy.math_based import CEM
-                model_object = CEM.OriginalCEM(**solver_options)
-
-            case 'OriginalSCA':
-                from mealpy.math_based import SCA
-                model_object = SCA.OriginalSCA(**solver_options)
-
-            case 'BaseSCA':
-                from mealpy.math_based import SCA
-                model_object = SCA.BaseSCA(**solver_options)
-
-            case 'OriginalGBO':
-                from mealpy.math_based import GBO
-                model_object = GBO.OriginalGBO(**solver_options)
-
-            case 'OrginalAOA':
-                from mealpy.math_based import AOA
-                model_object = AOA.OriginalAOA(**solver_options)
-
-            case 'OriginalCGO':
-                from mealpy.math_based import CGO
-                model_object = CGO.OriginalCGO(**solver_options)
-
-            case 'OriginalPSS':
-                from mealpy.math_based import PSS
-                model_object = PSS.OriginalPSS(**solver_options)
-
-            case 'OriginalINFO':
-                from mealpy.math_based import INFO
-                model_object = INFO.OriginalINFO(**solver_options)
-
-            case 'OriginalRUN':
-                from mealpy.math_based import RUN
-                model_object = RUN.OriginalRUN(**solver_options)
-
-            case 'OriginalCircleSA':
-                from mealpy.math_based import CircleSA
-                model_object = CircleSA.OriginalCircleSA(**solver_options)
-            
-            #============ Music
-            
-            case 'OriginalHS':
-                from mealpy.music_based import HS
-                model_object = HS.OriginalHS(**solver_options)
-
-            case 'BaseHS':
-                from mealpy.music_based import HS
-                model_object = HS.BaseHS(**solver_options)
-        
-        return model_object
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+
+def generate_model(solver_name, solver_options):
+
+    match solver_name:
+
+        # Evolution-Inspired Heuristic Optimization Algorithms
+
+        case 'orig-ep':
+            from mealpy.evolutionary_based import EP
+            model_object = EP.OriginalEP(**solver_options)
+
+        case 'levy-ep':
+            from mealpy.evolutionary_based import EP
+            model_object = EP.LevyEP(**solver_options)
+
+        case 'orig-es':
+            from mealpy.evolutionary_based import ES
+            model_object = ES.OriginalES(**solver_options)
+
+        case 'levy-es':
+            from mealpy.evolutionary_based import ES
+            model_object = ES.LevyES(**solver_options)
+
+        case 'orig-ma':
+            from mealpy.evolutionary_based import MA
+            model_object = MA.OriginalMA(**solver_options)
+
+        case 'base-ga':
+            from mealpy.evolutionary_based import GA
+            model_object = GA.BaseGA(**solver_options)
+
+        case 'single-ga':
+            from mealpy.evolutionary_based import GA
+            model_object = GA.SingleGA(**solver_options)
+
+        case 'multi-ga':
+            from mealpy.evolutionary_based import GA
+            model_object = GA.MultiGA(**solver_options)
+
+        case 'elite-single-ga':
+            from mealpy.evolutionary_based import GA
+            model_object = GA.EliteSingleGA(**solver_options)
+
+        case 'elite-multi-ga':
+            from mealpy.evolutionary_based import GA
+            model_object = GA.EliteMultiGA(**solver_options)
+
+        case 'base-de':
+            from mealpy.evolutionary_based import DE
+            model_object = DE.BaseDE(**solver_options)
+
+        case 'ja-de':
+            from mealpy.evolutionary_based import DE
+            model_object = DE.JADE(**solver_options)
+
+        case 'sa-de':
+            from mealpy.evolutionary_based import DE
+            model_object = DE.SADE(**solver_options)
+
+        case 'sha-de':
+            from mealpy.evolutionary_based import DE
+            model_object = DE.SHADE(**solver_options)
+
+        case 'l-sha-de':
+            from mealpy.evolutionary_based import DE
+            model_object = DE.L_SHADE(**solver_options)
+
+        case 'sap-de':
+            from mealpy.evolutionary_based import DE
+            model_object = DE.SAP_DE(**solver_options)
+
+        case 'orig-fpa':
+            from mealpy.evolutionary_based import FPA
+            model_object = FPA.OriginalFPA(**solver_options)
+
+        case 'orig-cro':
+            from mealpy.evolutionary_based import CRO
+            model_object = CRO.OriginalCRO(**solver_options)
+
+        case 'o-cro':
+            from mealpy.evolutionary_based import CRO
+            model_object = CRO.OCRO(**solver_options)
+
+        case 'cma-es':
+            from mealpy.evolutionary_based import ES
+            model_object = ES.CMA_ES(**solver_options)
+
+        case 'simp-cma-es':
+            from mealpy.evolutionary_based import ES
+            model_object = ES.Simple_CMA_ES(**solver_options)
+
+        # Swarm-Inspired Heuristic Optimization Algorithms
+
+        case 'orig-pso':
+            from mealpy.swarm_based import PSO
+            model_object = PSO.OriginalPSO(**solver_options)
+
+        case 'p-pso':
+            from mealpy.swarm_based import PSO
+            model_object = PSO.PPSO(**solver_options)
+
+        case 'h-pso-tvac':
+            from mealpy.swarm_based import PSO
+            model_object = PSO.HPSO_TVAC(**solver_options)
+
+        case 'c-pso':
+            from mealpy.swarm_based import PSO
+            model_object = PSO.C_PSO(**solver_options)
+
+        case 'cl-pso':
+            from mealpy.swarm_based import PSO
+            model_object = PSO.CL_PSO(**solver_options)
+
+        case 'orig-bfo':
+            from mealpy.swarm_based import BFO
+            model_object = BFO.OriginalBFO(**solver_options)
+
+        case 'orig-beesa':
+            from mealpy.swarm_based import BeesA
+            model_object = BeesA.OriginalBeesA(**solver_options)
+
+        case 'a-bfo':
+            from mealpy.swarm_based import BFO
+            model_object = BFO.OriginalBFO(**solver_options)
+
+        case 'prob-beesa':
+            from mealpy.swarm_based import BeesA
+            model_object = BeesA.ProbBeesA(**solver_options)
+
+        case 'orig-cso':
+            from mealpy.swarm_based import CSO
+            model_object = CSO.OriginalCSO(**solver_options)
+
+        case 'orig-abc':
+            from mealpy.swarm_based import ABC
+            model_object = ABC.OriginalABC(**solver_options)
+
+        case 'orig-acor':
+            from mealpy.swarm_based import ACOR
+            model_object = ACOR.orig_acor(**solver_options)
+
+        case 'orig-csa':
+            from mealpy.swarm_based import CSA
+            model_object = CSA.OriginalCSA(**solver_options)
+
+        case 'orig-ffa':
+            from mealpy.swarm_based import FFA
+            model_object = FFA.OriginalFFA(**solver_options)
+
+        case 'orig-fa':
+            from mealpy.swarm_based import FA
+            model_object = FA.OriginalFA(**solver_options)
+
+        case 'orig-ba':
+            from mealpy.swarm_based import BA
+            model_object = BA.OriginalBA(**solver_options)
+
+        case 'adap-ba':
+            from mealpy.swarm_based import BA
+            model_object = BA.AdaptiveBA(**solver_options)
+
+        case 'modi-ba':
+            from mealpy.swarm_based import BA
+            model_object = BA.ModifiedBA(**solver_options)
+
+        case 'orig-foa':
+            from mealpy.swarm_based import FOA
+            model_object = FOA.OriginalFOA(**solver_options)
+
+        case 'base-foa':
+            from mealpy.swarm_based import FOA
+            model_object = FOA.BaseFOA(**solver_options)
+
+        case 'whale-foa':
+            from mealpy.swarm_based import FOA
+            model_object = FOA.WhaleFOA(**solver_options)
+
+        case 'orig-sspidero':
+            from mealpy.swarm_based import SSpiderO
+            model_object = SSpiderO.OriginalSSpiderO(**solver_options)
+
+        case 'orig-gwo':
+            from mealpy.swarm_based import GWO
+            model_object = GWO.OriginalGWO(**solver_options)
+
+        case 'rw-gwo':
+            from mealpy.swarm_based import GWO
+            model_object = GWO.RW_GWO(**solver_options)
+
+        case 'orig-sspidera':
+            from mealpy.swarm_based import SSpiderA
+            model_object = SSpiderA.OriginalSSpiderA(**solver_options)
+
+        case 'orig-alo':
+            from mealpy.swarm_based import ALO
+            model_object = ALO.OriginalALO(**solver_options)
+
+        case 'base-alo':
+            from mealpy.swarm_based import ALO
+            model_object = ALO.BaseALO(**solver_options)
+
+        case 'orig-mfo':
+            from mealpy.swarm_based import MFO
+            model_object = MFO.OriginalMFO(**solver_options)
+
+        case 'base-mfo':
+            from mealpy.swarm_based import MFO
+            model_object = MFO.BaseMFO(**solver_options)
+
+        case 'orig-eho':
+            from mealpy.swarm_based import EHO
+            model_object = EHO.OriginalEHO(**solver_options)
+
+        case 'orig-ja':
+            from mealpy.swarm_based import JA
+            model_object = JA.OriginalJA(**solver_options)
+
+        case 'base-ja':
+            from mealpy.swarm_based import JA
+            model_object = JA.BaseJA(**solver_options)
+
+        case 'levy-ja':
+            from mealpy.swarm_based import JA
+            model_object = JA.LevyJA(**solver_options)
+
+        case 'orig-woa':
+            from mealpy.swarm_based import WOA
+            model_object = WOA.OriginalWOA(**solver_options)
+
+        case 'hi-woa':
+            from mealpy.swarm_based import WOA
+            model_object = WOA.HI_WOA(**solver_options)
+
+        case 'orig-do':
+            from mealpy.swarm_based import DO
+            model_object = DO.OriginalDO(**solver_options)
+
+        case 'orig-bsa':
+            from mealpy.swarm_based import BSA
+            model_object = BSA.OriginalBSA(**solver_options)
+
+        case 'orig-sho':
+            from mealpy.swarm_based import SHO
+            model_object = SHO.OriginalSHO(**solver_options)
+
+        case 'orig-sso':
+            from mealpy.swarm_based import SSO
+            model_object = SSO.OriginalSSO(**solver_options)
+
+        case 'orig-srsr':
+            from mealpy.swarm_based import SRSR
+            model_object = SRSR.OriginalSRSR(**solver_options)
+
+        case 'orig-goa':
+            from mealpy.swarm_based import GOA
+            model_object = GOA.OriginalGOA(**solver_options)
+
+        case 'orig-coa':
+            from mealpy.swarm_based import COA
+            model_object = COA.OriginalCOA(**solver_options)
+
+        case 'orig-msa':
+            from mealpy.swarm_based import MSA
+            model_object = MSA.OriginalMSA(**solver_options)
+
+        case 'orig-slo':
+            from mealpy.swarm_based import SLO
+            model_object = SLO.OriginalSLO(**solver_options)
+
+        case 'modi-slo':
+            from mealpy.swarm_based import SLO
+            model_object = SLO.ModifiedSLO(**solver_options)
+
+        case 'impr-slo':
+            from mealpy.swarm_based import SLO
+            model_object = SLO.ImprovedSLO(**solver_options)
+
+        case 'orig-nmra':
+            from mealpy.swarm_based import NMRA
+            model_object = NMRA.OriginalNMRA(**solver_options)
+
+        case 'impr-nmra':
+            from mealpy.swarm_based import NMRA
+            model_object = NMRA.ImprovedNMRA(**solver_options)
+
+        case 'orig-pfa':
+            from mealpy.swarm_based import PFA
+            model_object = PFA.OriginalPFA(**solver_options)
+
+        case 'orig-sfo':
+            from mealpy.swarm_based import SFO
+            model_object = SFO.OriginalSFO(**solver_options)
+
+        case 'impr-sfo':
+            from mealpy.swarm_based import SFO
+            model_object = SFO.ImprovedSFO(**solver_options)
+
+        case 'orig-hho':
+            from mealpy.swarm_based import HHO
+            model_object = HHO.OriginalHHO(**solver_options)
+
+        case 'orig-mrfo':
+            from mealpy.swarm_based import MRFO
+            model_object = MRFO.OriginalMRFO(**solver_options)
+
+        case 'orig-bes':
+            from mealpy.swarm_based import BES
+            model_object = BES.OriginalBES(**solver_options)
+
+        case 'orig-ssa':
+            from mealpy.swarm_based import SSA
+            model_object = SSA.OriginalSSA(**solver_options)
+
+        case 'base-ssa':
+            from mealpy.swarm_based import SSA
+            model_object = SSA.BaseSSA(**solver_options)
+
+        case 'orig-hgs':
+            from mealpy.swarm_based import HGS
+            model_object = HGS.OriginalHGS(**solver_options)
+
+        case 'orig-ao':
+            from mealpy.swarm_based import AO
+            model_object = AO.OriginalAO(**solver_options)
+
+        case 'gwo-woa':
+            from mealpy.swarm_based import GWO
+            model_object = GWO.OriginalGWO(**solver_options)
+
+        case 'orig-mpa':
+            from mealpy.swarm_based import MPA
+            model_object = MPA.OriginalMPA(**solver_options)
+
+        case 'orig-hba':
+            from mealpy.swarm_based import HBA
+            model_object = HBA.OriginalHBA(**solver_options)
+
+        case 'orig-scso':
+            from mealpy.swarm_based import SCSO
+            model_object = SCSO.OriginalSCSO(**solver_options)
+
+        case 'orig-tso':
+            from mealpy.swarm_based import TSO
+            model_object = TSO.OriginalTSO(**solver_options)
+
+        case 'orig-avoa':
+            from mealpy.swarm_based import AVOA
+            model_object = AVOA.OriginalAVOA(**solver_options)
+
+        case 'orig-agto':
+            from mealpy.swarm_based import AGTO
+            model_object = AGTO.OriginalAGTO(**solver_options)
+
+        case 'orig-aro':
+            from mealpy.swarm_based import ARO
+            model_object = ARO.OriginalARO(**solver_options)
+
+        case 'levy-aro':
+            from mealpy.swarm_based import ARO
+            model_object = ARO.LARO(**solver_options)
+
+        case 'selec-aro':
+            from mealpy.swarm_based import ARO
+            model_object = ARO.IARO(**solver_options)
+
+        case 'wmqi-mrfo':
+            from mealpy.swarm_based import MRFO
+            model_object = MRFO.WMQIMRFO(**solver_options)
+
+        case 'orig-esoa':
+            from mealpy.swarm_based import ESOA
+            model_object = ESOA.OriginalESOA(**solver_options)
+
+        case 'sea-ho':
+            from mealpy.swarm_based import SeaHO
+            model_object = SeaHO.OriginalSeaHO(**solver_options)
+
+        case 'orig-mgo':
+            from mealpy.swarm_based import MGO
+            model_object = MGO.OriginalMGO(**solver_options)
+
+        case 'orig-gjo':
+            from mealpy.swarm_based import GJO
+            model_object = GJO.OriginalGJO(**solver_options)
+
+        case 'orig-fox':
+            from mealpy.swarm_based import FOX
+            model_object = FOX.OriginalFOX(**solver_options)
+
+        case 'orig-gto':
+            from mealpy.swarm_based import GTO
+            model_object = GTO.OriginalGTO(**solver_options)
+
+        case 'modi101-gto':
+            from mealpy.swarm_based import GTO
+            model_object = GTO.Matlab101GTO(**solver_options)
+
+        case 'modi102-gto':
+            from mealpy.swarm_based import GTO
+            model_object = GTO.Matlab102GTO(**solver_options)
+
+        # Physics-Inspired Heuristic Optimization Algorithms
+
+        case 'orig-sa':
+            from mealpy.physics_based import SA
+            model_object = SA.OriginalSA(**solver_options)
+
+        case 'orig-wdo':
+            from mealpy.physics_based import WDO
+            model_object = WDO.OriginalWDO(**solver_options)
+
+        case 'orig-mvo':
+            from mealpy.physics_based import MVO
+            model_object = MVO.OriginalMVO(**solver_options)
+
+        case 'base-mvo':
+            from mealpy.physics_based import MVO
+            model_object = MVO.BaseMVO(**solver_options)
+
+        case 'orig-two':
+            from mealpy.physics_based import TWO
+            model_object = TWO.OriginalTWO(**solver_options)
+
+        case 'oppo-two':
+            from mealpy.physics_based import TWO
+            model_object = TWO.OppoTWO(**solver_options)
+
+        case 'levy-two':
+            from mealpy.physics_based import TWO
+            model_object = TWO.LevyTWO(**solver_options)
+
+        case 'enha-two':
+            from mealpy.physics_based import TWO
+            model_object = TWO.EnhancedTWO(**solver_options)
+
+        case 'orig-efo':
+            from mealpy.physics_based import EFO
+            model_object = EFO.OriginalEFO(**solver_options)
+
+        case 'base-efo':
+            from mealpy.physics_based import EFO
+            model_object = EFO.BaseEFO(**solver_options)
+
+        case 'orig-nro':
+            from mealpy.physics_based import NRO
+            model_object = NRO.OriginalNRO(**solver_options)
+
+        case 'orig-hgso':
+            from mealpy.physics_based import HGSO
+            model_object = HGSO.OriginalHGSO(**solver_options)
+
+        case 'orig-aso':
+            from mealpy.physics_based import ASO
+            model_object = ASO.OriginalASO(**solver_options)
+
+        case 'orig-eo':
+            from mealpy.physics_based import EO
+            model_object = EO.OriginalEO(**solver_options)
+
+        case 'modi-eo':
+            from mealpy.physics_based import EO
+            model_object = EO.ModifiedEO(**solver_options)
+
+        case 'adap-eo':
+            from mealpy.physics_based import EO
+            model_object = EO.AdaptiveEO(**solver_options)
+
+        case 'orig-archoa':
+            from mealpy.physics_based import ArchOA
+            model_object = ArchOA.OriginalArchOA(**solver_options)
+
+        case 'orig-rime':
+            from mealpy.physics_based import RIME
+            model_object = RIME.OriginalRIME(**solver_options)
+
+        case 'orig-evo':
+            from mealpy.physics_based import EVO
+            model_object = EVO.OriginalEVO(**solver_options)
+
+        case 'orig-cdo':
+            from mealpy.physics_based import CDO
+            model_object = CDO.OriginalCDO
+
+        case 'orig-fla':
+            from mealpy.physics_based import FLA
+            model_object = FLA.OriginalFLA
+
+        # Human-Inspired Heuristic Optimization Algorithms
+
+        case 'orig-ca':
+            from mealpy.human_based import CA
+            model_object = CA.OriginalCA(**solver_options)
+
+        case 'orig-ica':
+            from mealpy.human_based import ICA
+            model_object = ICA.OriginalICA(**solver_options)
+
+        case 'orig-tlo':
+            from mealpy.human_based import TLO
+            model_object = TLO.OriginalTLO(**solver_options)
+
+        case 'base-tlo':
+            from mealpy.human_based import TLO
+            model_object = TLO.BaseTLO(**solver_options)
+
+        case 'itlo':
+            from mealpy.human_based import TLO
+            model_object = TLO.ImprovedTLO(**solver_options)
+
+        case 'orig-bso':
+            from mealpy.human_based import BSO
+            model_object = BSO.OriginalBSO(**solver_options)
+
+        case 'impr-bso':
+            from mealpy.human_based import BSO
+            model_object = BSO.ImprovedBSO(**solver_options)
+
+        case 'orig-qsa':
+            from mealpy.human_based import QSA
+            model_object = QSA.OriginalQSA(**solver_options)
+
+        case 'base-qsa':
+            from mealpy.human_based import QSA
+            model_object = QSA.BaseQSA(**solver_options)
+
+        case 'oppo-qsa':
+            from mealpy.human_based import QSA
+            model_object = QSA.OppoQSA(**solver_options)
+
+        case 'levy-qsa':
+            from mealpy.human_based import QSA
+            model_object = QSA.LevyQSA(**solver_options)
+
+        case 'impr-qsa':
+            from mealpy.human_based import QSA
+            model_object = QSA.ImprovedQSA(**solver_options)
+
+        case 'orig-saro':
+            from mealpy.human_based import SARO
+            model_object = SARO.OriginalSARO(**solver_options)
+
+        case 'base-saro':
+            from mealpy.human_based import SARO
+            model_object = SARO.BaseSARO(**solver_options)
+
+        case 'orig-lco':
+            from mealpy.human_based import LCO
+            model_object = LCO.OriginalLCO(**solver_options)
+
+        case 'base-lco':
+            from mealpy.human_based import LCO
+            model_object = LCO.BaseLCO(**solver_options)
+
+        case 'impr-lco':
+            from mealpy.human_based import LCO
+            model_object = LCO.ImprovedLCO(**solver_options)
+
+        case 'orig-ssdo':
+            from mealpy.human_based import SSDO
+            model_object = SSDO.OriginalSSDO(**solver_options)
+
+        case 'orig-gska':
+            from mealpy.human_based import GSKA
+            model_object = GSKA.OriginalGSKA(**solver_options)
+
+        case 'base-gska':
+            from mealpy.human_based import GSKA
+            model_object = GSKA.BaseGSKA(**solver_options)
+
+        case 'orig-chio':
+            from mealpy.human_based import CHIO
+            model_object = CHIO.OriginalCHIO(**solver_options)
+
+        case 'base-chio':
+            from mealpy.human_based import CHIO
+            model_object = CHIO.BaseCHIO(**solver_options)
+
+        case 'orig-fbio':
+            from mealpy.human_based import FBIO
+            model_object = FBIO.OriginalFBIO(**solver_options)
+
+        case 'base-fbio':
+            from mealpy.human_based import FBIO
+            model_object = FBIO.BaseFBIO(**solver_options)
+
+        case 'orig-bro':
+            from mealpy.human_based import BRO
+            model_object = BRO.OriginalBRO(**solver_options)
+
+        case 'base-bro':
+            from mealpy.human_based import BRO
+            model_object = BRO.BaseBRO(**solver_options)
+
+        case 'orig-spbo':
+            from mealpy.human_based import SPBO
+            model_object = SPBO.OriginalSPBO(**solver_options)
+
+        case 'dev-spbo':
+            from mealpy.human_based import SPBO
+            model_object = SPBO.DevSPBO(**solver_options)
+
+        case 'orig-dmoa':
+            print('OriginalDMOA: Not supported yet. Using SPBO instead')
+            # from mealpy.human_based import DMOA
+            # model_object = DMOA.OriginalDMOA(**solver_options)
+            from mealpy.human_based import SPBO
+            model_object = SPBO.DevSPBO(**solver_options)
+
+        case 'dev-dmoa':
+            print('DevDMOA: Not supported yet. Using SPBO instead')
+            # from mealpy.human_based import DMOA
+            # model_object = DMOA.DevDMOA(**solver_options)
+            from mealpy.human_based import SPBO
+            model_object = SPBO.DevSPBO(**solver_options)
+
+        case 'orig-huco':
+            from mealpy.human_based import HCO
+            model_object = HCO.OriginalHCO(**solver_options)
+
+        case 'orig-warso':
+            from mealpy.human_based import WarSO
+            model_object = WarSO.OriginalWarSO(**solver_options)
+
+        case 'orig-hbo':
+            from mealpy.human_based import HBO
+            model_object = HBO.OriginalHBO(**solver_options)
+
+        # Bio-Inspired Heuristic Optimization Algorithms
+
+        case 'orig-iwo':
+            from mealpy.bio_based import IWO
+            model_object = IWO.OriginalIWO(**solver_options)
+
+        case 'orig-bboa':
+            from mealpy.bio_based import BBO
+            model_object = BBO.OriginalBBO(**solver_options)
+
+        case 'base-bbo':
+            from mealpy.bio_based import BBO
+            model_object = BBO.BaseBBO(**solver_options)
+
+        case 'orig-vcs':
+            from mealpy.bio_based import VCS
+            model_object = VCS.OriginalVCS(**solver_options)
+
+        case 'base-vcs':
+            from mealpy.bio_based import VCS
+            model_object = VCS.BaseVCS(**solver_options)
+
+        case 'orig-sbo':
+            from mealpy.bio_based import SBO
+            model_object = SBO.OriginalSBO(**solver_options)
+
+        case 'base-sbo':
+            from mealpy.bio_based import SBO
+            model_object = SBO.BaseSBO(**solver_options)
+
+        case 'orig-eoa':
+            from mealpy.bio_based import EOA
+            model_object = EOA.OriginalEOA(**solver_options)
+
+        case 'orig-who':
+            from mealpy.bio_based import WHO
+            model_object = WHO.OriginalWHO(**solver_options)
+
+        case 'orig-sma':
+            from mealpy.bio_based import SMA
+            model_object = SMA.OriginalSMA(**solver_options)
+
+        case 'base-sma':
+            from mealpy.bio_based import SMA
+            model_object = SMA.BaseSMA(**solver_options)
+
+        case 'orig-bmo':
+            from mealpy.bio_based import BMO
+            model_object = BMO.OriginalBMO(**solver_options)
+
+        case 'orig-tsa':
+            from mealpy.bio_based import TSA
+            model_object = TSA.OriginalTSA(**solver_options)
+
+        case 'orig-sos':
+            from mealpy.bio_based import SOS
+            model_object = SOS.OriginalSOS(**solver_options)
+
+        case 'orig-soa':
+            from mealpy.bio_based import SOA
+            model_object = SOA.OriginalSOA(**solver_options)
+
+        case 'dev-soa':
+            from mealpy.bio_based import SOA
+            model_object = SOA.DevSOA(**solver_options)
+
+        # System-Inspired Heuristic Optimization Algorithms
+
+        case 'orig-gco':
+            from mealpy.system_based import GCO
+            model_object = GCO.OriginalGCO(**solver_options)
+
+        case 'base-gco':
+            from mealpy.system_based import GCO
+            model_object = GCO.BaseGCO(**solver_options)
+
+        case 'orig-wca':
+            from mealpy.system_based import WCA
+            model_object = WCA.OriginalWCA(**solver_options)
+
+        case 'orig-aeo':
+            from mealpy.system_based import AEO
+            model_object = AEO.OriginalAEO(**solver_options)
+
+        case 'enha-aeo':
+            from mealpy.system_based import AEO
+            model_object = AEO.EnhancedAEO(**solver_options)
+
+        case 'modi-aeo':
+            from mealpy.system_based import AEO
+            model_object = AEO.ModifiedAEO(**solver_options)
+
+        case 'impr-aeo':
+            from mealpy.system_based import AEO
+            model_object = AEO.ImprovedAEO(**solver_options)
+
+        case 'augm-aeo':
+            from mealpy.system_based import AEO
+            model_object = AEO.AugmentedAEO(**solver_options)
+
+        # Math-Inspired Heuristic Optimization Algorithms
+
+        case 'orig-hc':
+            from mealpy.math_based import HC
+            model_object = HC.OriginalHC(**solver_options)
+
+        case 'swarm-hc':
+            from mealpy.math_based import HC
+            model_object = HC.SwarmHC(**solver_options)
+
+        case 'orig-cem':
+            from mealpy.math_based import CEM
+            model_object = CEM.OriginalCEM(**solver_options)
+
+        case 'orig-sca':
+            from mealpy.math_based import SCA
+            model_object = SCA.OriginalSCA(**solver_options)
+
+        case 'base-sca':
+            from mealpy.math_based import SCA
+            model_object = SCA.BaseSCA(**solver_options)
+
+        case 'orig-beesa':
+            from mealpy.math_based import AOA
+            model_object = AOA.OriginalAOA(**solver_options)
+
+        case 'orig-cgo':
+            from mealpy.math_based import CGO
+            model_object = CGO.OriginalCGO(**solver_options)
+
+        case 'orig-gbo':
+            from mealpy.math_based import GBO
+            model_object = GBO.OriginalGBO(**solver_options)
+
+        case 'orig-info':
+            from mealpy.math_based import INFO
+            model_object = INFO.OriginalINFO(**solver_options)
+
+        case 'orig-pss':
+            from mealpy.math_based import PSS
+            model_object = PSS.OriginalPSS(**solver_options)
+
+        case 'orig-run':
+            from mealpy.math_based import RUN
+            model_object = RUN.OriginalRUN(**solver_options)
+
+        case 'orig-circle-sa':
+            from mealpy.math_based import CircleSA
+            model_object = CircleSA.OriginalCircleSA(**solver_options)
+
+        case 'ql-sca':
+            from mealpy.math_based import SCA
+            model_object = SCA.QleSCA(**solver_options)
+
+        case 'orig-shio':
+            from mealpy.math_based import SHIO
+            model_object = SHIO.OriginalSHIO(**solver_options)
+
+        # Music-Inspired Heuristic Optimization Algorithms
+
+        case 'orig-hs':
+            from mealpy.music_based import HS
+            model_object = HS.OriginalHS(**solver_options)
+
+        case 'base-hs':
+            from mealpy.music_based import HS
+            model_object = HS.BaseHS(**solver_options)
+
+    return model_object
```

### Comparing `feloopy-0.2.4/feloopy/generators/model_generator.py` & `feloopy-0.2.5/feloopy/generators/model_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,91 @@
-def generate_model(features):
-
-    match features['interface_name']:
-
-        case 'pulp':
-
-            from .model import pulp_model_generator
-            model_object = pulp_model_generator.generate_model(features)
-
-        case 'pyomo':
-
-            from .model import pyomo_model_generator
-            model_object = pyomo_model_generator.generate_model(features)
-
-        case 'ortools':
-
-            from .model import ortools_model_generator
-            model_object = ortools_model_generator.generate_model(features)
-
-        case 'ortools_cp':
-
-            from .model import ortools_cp_model_generator
-            model_object = ortools_cp_model_generator.generate_model(features)
-
-        case 'gekko':
-
-            from .model import gekko_model_generator
-            model_object = gekko_model_generator.generate_model(features)
-
-        case 'picos':
-
-            from .model import picos_model_generator
-            model_object = picos_model_generator.generate_model(features)
-
-        case 'cvxpy':
-
-            from .model import cvxpy_model_generator
-            model_object = cvxpy_model_generator.generate_model(features)
-
-        case 'cylp':
-
-            from .model import cylp_model_generator
-            model_object = cylp_model_generator.generate_model(features)
-
-        case 'pymprog':
-
-            from .model import pymprog_model_generator
-            model_object = pymprog_model_generator.generate_model(features)
-
-        case 'cplex':
-
-            from .model import cplex_model_generator
-            model_object = cplex_model_generator.generate_model(features)
-
-        case 'cplex_cp':
-
-            from .model import cplex_cp_model_generator
-            model_object = cplex_cp_model_generator.generate_model(features)
-
-        case 'gurobi':
-
-            from .model import gurobi_model_generator
-            model_object = gurobi_model_generator.generate_model(features)
-
-        case 'xpress':
-
-            from .model import xpress_model_generator
-            model_object = xpress_model_generator.generate_model(features)
-
-        case 'mip':
-
-            from .model import mip_model_generator
-            model_object = mip_model_generator.generate_model(features)
-
-        case 'linopy':
-
-            from .model import linopy_model_generator
-            model_object = linopy_model_generator.generate_model(features)
-    
-    return model_object
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+
+def generate_model(features):
+
+    match features['interface_name']:
+
+        case 'pulp':
+
+            from .model import pulp_model_generator
+            model_object = pulp_model_generator.generate_model(features)
+
+        case 'pyomo':
+
+            from .model import pyomo_model_generator
+            model_object = pyomo_model_generator.generate_model(features)
+
+        case 'ortools':
+
+            from .model import ortools_model_generator
+            model_object = ortools_model_generator.generate_model(features)
+
+        case 'ortools_cp':
+
+            from .model import ortools_cp_model_generator
+            model_object = ortools_cp_model_generator.generate_model(features)
+
+        case 'gekko':
+
+            from .model import gekko_model_generator
+            model_object = gekko_model_generator.generate_model(features)
+
+        case 'picos':
+
+            from .model import picos_model_generator
+            model_object = picos_model_generator.generate_model(features)
+
+        case 'cvxpy':
+
+            from .model import cvxpy_model_generator
+            model_object = cvxpy_model_generator.generate_model(features)
+
+        case 'cylp':
+
+            from .model import cylp_model_generator
+            model_object = cylp_model_generator.generate_model(features)
+
+        case 'pymprog':
+
+            from .model import pymprog_model_generator
+            model_object = pymprog_model_generator.generate_model(features)
+
+        case 'cplex':
+
+            from .model import cplex_model_generator
+            model_object = cplex_model_generator.generate_model(features)
+
+        case 'cplex_cp':
+
+            from .model import cplex_cp_model_generator
+            model_object = cplex_cp_model_generator.generate_model(features)
+
+        case 'gurobi':
+
+            from .model import gurobi_model_generator
+            model_object = gurobi_model_generator.generate_model(features)
+
+        case 'xpress':
+
+            from .model import xpress_model_generator
+            model_object = xpress_model_generator.generate_model(features)
+
+        case 'mip':
+
+            from .model import mip_model_generator
+            model_object = mip_model_generator.generate_model(features)
+
+        case 'linopy':
+
+            from .model import linopy_model_generator
+            model_object = linopy_model_generator.generate_model(features)
+
+    return model_object
```

### Comparing `feloopy-0.2.4/feloopy/generators/solution/cplex_cp_solution_generator.py` & `feloopy-0.2.5/feloopy/generators/solution/linopy_solution_generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,65 @@
-import cplex
-from docplex.mp.model import Model as CPLEXMODEL
-import docplex as cplex_interface
-import timeit
-from docplex.util.environment import get_environment
-env = get_environment()
-
-from docplex.cp.config import context
-
-cplex_solver_selector = {'cplex': 'cplex'}
-
-def generate_solution(features):
-
-    model_object = features['model_object_before_solve']
-    model_objectives = features['objectives']
-    model_constraints = features['constraints']
-    directions = features['directions']
-    constraint_labels= features['constraint_labels']
-    debug = features['debug_mode']
-    time_limit = features['time_limit']
-    absolute_gap = features['absolute_gap']
-    relative_gap = features['relative_gap']
-    thread_count = features['thread_count']
-    solver_name = features['solver_name']
-    objective_id = features['objective_being_optimized']
-    log = features['log']
-    save = features['save_solver_log']
-    save_model = features['write_model_file']
-    email = features['email_address']
-    max_iterations= features['max_iterations']
-    solver_options= features['solver_options']
-
-    if solver_name==None:
-        solver_name='cplex'
-    
-    if log:
-        context.solver.trace_cpo = True
-        context.solver.trace_log = True
-        context.params.LogPeriod = 5000
-
-    else:
-        context.solver.trace_cpo = False
-        context.solver.trace_log = False
-        context.params.LogPeriod = 1
-
-    if solver_name not in cplex_solver_selector.keys():
-        raise RuntimeError("Using solver '%s' is not supported by 'cplex'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
-    match debug:
-
-        case False:
-
-            if len(directions)!=0:
-
-                match directions[objective_id]:
-
-                    case 'min': 
-                        model_object.minimize(model_objectives[objective_id])
-
-                    case 'max': 
-                        model_object.maximize(model_objectives[objective_id])
-
-            for constraint in model_constraints:
-                model_object.add_constraint(constraint)
-
-            time_solve_begin = timeit.default_timer()
-            result = model_object.solve(TimeLimit=time_limit)
-            time_solve_end = timeit.default_timer()
-            generated_solution = [result, [time_solve_begin, time_solve_end]]
-
-    return generated_solution
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+from linopy import Model as LINOPYMODEL
+import timeit
+
+linopy_solver_selector = {'cbc': 'cbc',
+                          'glpk': 'glpk',
+                          'highs': 'highs',
+                          'gurobi': 'gurobi',
+                          'xpress': 'xpress',
+                          'cplex': 'cplex'}
+
+
+def generate_solution(features):
+
+    model_object = features['model_object_before_solve']
+    model_objectives = features['objectives']
+    model_constraints = features['constraints']
+    directions = features['directions']
+    constraint_labels = features['constraint_labels']
+    debug = features['debug_mode']
+    time_limit = features['time_limit']
+    absolute_gap = features['absolute_gap']
+    relative_gap = features['relative_gap']
+    thread_count = features['thread_count']
+    solver_name = features['solver_name']
+    objective_id = features['objective_being_optimized']
+    log = features['log']
+    save = features['save_solver_log']
+    save_model = features['write_model_file']
+    email = features['email_address']
+    max_iterations = features['max_iterations']
+    solver_options = features['solver_options']
+
+    if solver_name not in linopy_solver_selector.keys():
+        raise RuntimeError(
+            "Using solver '%s' is not supported by 'linopy'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
+
+    match debug:
+
+        case False:
+
+            match directions[objective_id]:
+                case "min":
+                    model_object.add_objective(model_objectives[objective_id])
+                case "max":
+                    model_object.add_objective(-model_objectives[objective_id])
+
+            for constraint in model_constraints:
+                model_object.add_constraints(constraint)
+
+            time_solve_begin = timeit.default_timer()
+            result = model_object.solve(solver_name=solver_name)
+            time_solve_end = timeit.default_timer()
+            generated_solution = [result, [time_solve_begin, time_solve_end]]
+
+    return generated_solution
```

### Comparing `feloopy-0.2.4/feloopy/generators/solution/ortools_cp_solution_generator.py` & `feloopy-0.2.5/feloopy/generators/solution/ortools_cp_solution_generator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,88 @@
-from ortools.sat.python import cp_model
-import timeit 
-
-ortools_solver_selector = {
-    'clp': 'CLP_LINEAR_PROGRAMMING',
-    'cbc': 'CBC_MIXED_INTEGER_PROGRAMMING',
-    'scip': 'SCIP_MIXED_INTEGER_PROGRAMMING',
-    'glop': 'GLOP_LINEAR_PROGRAMMING',
-    'bop': 'BOP_INTEGER_PROGRAMMING',
-    'sat': 'SAT_INTEGER_PROGRAMMING',
-    'gurobi_': 'GUROBI_LINEAR_PROGRAMMING',
-    'gurobi': 'GUROBI_MIXED_INTEGER_PROGRAMMING',
-    'cplex_': 'CPLEX_LINEAR_PROGRAMMING',
-    'cplex': 'CPLEX_MIXED_INTEGER_PROGRAMMING',
-    'xpress_': 'XPRESS_LINEAR_PROGRAMMING',
-    'xpress': 'XPRESS_MIXED_INTEGER_PROGRAMMING',
-    'glpk_': 'GLPK_LINEAR_PROGRAMMING',
-    'glpk': 'GLPK_MIXED_INTEGER_PROGRAMMING'
-}
-
-def generate_solution(features):
-
-    model_object = features['model_object_before_solve']
-    model_objectives = features['objectives']
-    model_constraints = features['constraints']
-    directions = features['directions']
-    constraint_labels= features['constraint_labels']
-    debug = features['debug_mode']
-    time_limit = features['time_limit']
-    absolute_gap = features['absolute_gap']
-    relative_gap = features['relative_gap']
-    thread_count = features['thread_count']
-    solver_name = features['solver_name']
-    objective_id = features['objective_being_optimized']
-    log = features['log']
-    save = features['save_solver_log']
-    save_model = features['write_model_file']
-    email = features['email_address']
-    max_iterations= features['max_iterations']
-    solver_options= features['solver_options']
-
-    match debug:
-
-        case False:
-
-            if len(directions)!=0:
-
-                match directions[objective_id]:
-
-                    case "min":
-                        model_object.Minimize(model_objectives[objective_id])
-
-                    case "max":
-                        model_object.Maximize(model_objectives[objective_id])
-
-            for constraint in model_constraints:
-                model_object.Add(constraint)
-
-            solver = cp_model.CpSolver()
-
-            if time_limit != None:
-                solver.parameters.max_time_in_seconds = time_limit
-
-            time_solve_begin = timeit.default_timer()
-            result = solver.Solve(model_object)
-            time_solve_end = timeit.default_timer()
-            generated_solution = [[result,solver], [time_solve_begin, time_solve_end]]
-
-
-            if log:
-
-                    print('\nStatistics')
-                    print(f'  conflicts      : {solver.NumConflicts()}')
-                    print(f'  branches       : {solver.NumBranches()}')
-                    print(f'  wall time      : {solver.WallTime()} s')
-
-                    
-    return generated_solution
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+from ortools.sat.python import cp_model
+import timeit
+
+ortools_solver_selector = {
+    'clp': 'CLP_LINEAR_PROGRAMMING',
+    'cbc': 'CBC_MIXED_INTEGER_PROGRAMMING',
+    'scip': 'SCIP_MIXED_INTEGER_PROGRAMMING',
+    'glop': 'GLOP_LINEAR_PROGRAMMING',
+    'bop': 'BOP_INTEGER_PROGRAMMING',
+    'sat': 'SAT_INTEGER_PROGRAMMING',
+    'gurobi_': 'GUROBI_LINEAR_PROGRAMMING',
+    'gurobi': 'GUROBI_MIXED_INTEGER_PROGRAMMING',
+    'cplex_': 'CPLEX_LINEAR_PROGRAMMING',
+    'cplex': 'CPLEX_MIXED_INTEGER_PROGRAMMING',
+    'xpress_': 'XPRESS_LINEAR_PROGRAMMING',
+    'xpress': 'XPRESS_MIXED_INTEGER_PROGRAMMING',
+    'glpk_': 'GLPK_LINEAR_PROGRAMMING',
+    'glpk': 'GLPK_MIXED_INTEGER_PROGRAMMING'
+}
+
+
+def generate_solution(features):
+
+    model_object = features['model_object_before_solve']
+    model_objectives = features['objectives']
+    model_constraints = features['constraints']
+    directions = features['directions']
+    constraint_labels = features['constraint_labels']
+    debug = features['debug_mode']
+    time_limit = features['time_limit']
+    absolute_gap = features['absolute_gap']
+    relative_gap = features['relative_gap']
+    thread_count = features['thread_count']
+    solver_name = features['solver_name']
+    objective_id = features['objective_being_optimized']
+    log = features['log']
+    save = features['save_solver_log']
+    save_model = features['write_model_file']
+    email = features['email_address']
+    max_iterations = features['max_iterations']
+    solver_options = features['solver_options']
+
+    match debug:
+
+        case False:
+
+            if len(directions) != 0:
+
+                match directions[objective_id]:
+
+                    case "min":
+                        model_object.Minimize(model_objectives[objective_id])
+
+                    case "max":
+                        model_object.Maximize(model_objectives[objective_id])
+
+            for constraint in model_constraints:
+                model_object.Add(constraint)
+
+            solver = cp_model.CpSolver()
+
+            if time_limit != None:
+                solver.parameters.max_time_in_seconds = time_limit
+
+            time_solve_begin = timeit.default_timer()
+            result = solver.Solve(model_object)
+            time_solve_end = timeit.default_timer()
+            generated_solution = [[result, solver],
+                                  [time_solve_begin, time_solve_end]]
+
+            if log:
+
+                print('\nStatistics')
+                print(f'  conflicts      : {solver.NumConflicts()}')
+                print(f'  branches       : {solver.NumBranches()}')
+                print(f'  wall time      : {solver.WallTime()} s')
+
+    return generated_solution
```

### Comparing `feloopy-0.2.4/feloopy/generators/solution/ortools_solution_generator.py` & `feloopy-0.2.5/feloopy/generators/solution/xpress_solution_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,64 @@
-from ortools.linear_solver import pywraplp as ortools_interface
-import timeit 
-
-ortools_solver_selector = {
-    'clp': 'CLP_LINEAR_PROGRAMMING',
-    'cbc': 'CBC_MIXED_INTEGER_PROGRAMMING',
-    'scip': 'SCIP_MIXED_INTEGER_PROGRAMMING',
-    'glop': 'GLOP_LINEAR_PROGRAMMING',
-    'bop': 'BOP_INTEGER_PROGRAMMING',
-    'sat': 'SAT_INTEGER_PROGRAMMING',
-    'gurobi_': 'GUROBI_LINEAR_PROGRAMMING',
-    'gurobi': 'GUROBI_MIXED_INTEGER_PROGRAMMING',
-    'cplex_': 'CPLEX_LINEAR_PROGRAMMING',
-    'cplex': 'CPLEX_MIXED_INTEGER_PROGRAMMING',
-    'xpress_': 'XPRESS_LINEAR_PROGRAMMING',
-    'xpress': 'XPRESS_MIXED_INTEGER_PROGRAMMING',
-    'glpk_': 'GLPK_LINEAR_PROGRAMMING',
-    'glpk': 'GLPK_MIXED_INTEGER_PROGRAMMING'
-}
-
-def generate_solution(features):
-
-    model_object = features['model_object_before_solve']
-    model_objectives = features['objectives']
-    model_constraints = features['constraints']
-    directions = features['directions']
-    constraint_labels= features['constraint_labels']
-    debug = features['debug_mode']
-    time_limit = features['time_limit']
-    absolute_gap = features['absolute_gap']
-    relative_gap = features['relative_gap']
-    thread_count = features['thread_count']
-    solver_name = features['solver_name']
-    objective_id = features['objective_being_optimized']
-    log = features['log']
-    save = features['save_solver_log']
-    save_model = features['write_model_file']
-    email = features['email_address']
-    max_iterations= features['max_iterations']
-    solver_options= features['solver_options']
-    
-    if solver_name not in ortools_solver_selector.keys():
-        raise RuntimeError("Using solver '%s' is not supported by 'ortools'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
-    
-    match debug:
-
-        case False:
-
-            match directions[objective_id]:
-
-                case "min":
-                    model_object.Minimize(model_objectives[objective_id])
-
-                case "max":
-                    model_object.Maximize(model_objectives[objective_id])
-
-            for constraint in model_constraints:
-                model_object.Add(constraint)
-
-            model_object.CreateSolver(ortools_solver_selector[solver_name])
-            solverParams = ortools_interface.MPSolverParameters()
-
-            if time_limit != None:
-                model_object.set_time_limit(time_limit)
-
-            if thread_count != None:
-                model_object.SetNumThreads(thread_count)
-
-            if relative_gap !=None:
-                solverParams.SetDoubleParam(solverParams.RELATIVE_MIP_GAP, relative_gap)
-
-            if absolute_gap != None:
-                "None"
-                
-            if log:
-
-                "None"
-
-            time_solve_begin = timeit.default_timer()
-            result = model_object.Solve()
-            time_solve_end = timeit.default_timer()
-            generated_solution = [result, [time_solve_begin, time_solve_end]]
-    
-    return generated_solution
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+import xpress as xpress_interface
+import timeit
+
+xpress_solver_selector = {'xpress': 'xpress'}
+
+
+def generate_solution(features):
+
+    model_object = features['model_object_before_solve']
+    model_objectives = features['objectives']
+    model_constraints = features['constraints']
+    directions = features['directions']
+    constraint_labels = features['constraint_labels']
+    debug = features['debug_mode']
+    time_limit = features['time_limit']
+    absolute_gap = features['absolute_gap']
+    relative_gap = features['relative_gap']
+    thread_count = features['thread_count']
+    solver_name = features['solver_name']
+    objective_id = features['objective_being_optimized']
+    log = features['log']
+    save = features['save_solver_log']
+    save_model = features['write_model_file']
+    email = features['email_address']
+    max_iterations = features['max_iterations']
+    solver_options = features['solver_options']
+
+    if solver_name not in xpress_solver_selector.keys():
+        raise RuntimeError(
+            "Using solver '%s' is not supported by 'xpress'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
+
+    match debug:
+
+        case False:
+
+            for constraint in model_constraints:
+                model_object.addConstraint(constraint)
+
+            match directions[objective_id]:
+
+                case "min":
+                    model_object.setObjective(
+                        model_objectives[objective_id], sense=xpress_interface.minimize)
+
+                case "max":
+                    model_object.setObjective(
+                        model_objectives[objective_id], sense=xpress_interface.maximize)
+
+            time_solve_begin = timeit.default_timer()
+            result = model_object.solve()
+            time_solve_end = timeit.default_timer()
+            generated_solution = [result, [time_solve_begin, time_solve_end]]
+
+    return generated_solution
```

### Comparing `feloopy-0.2.4/feloopy/generators/solution/pymprog_solution_generator.py` & `feloopy-0.2.5/feloopy/generators/solution/cylp_solution_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,64 @@
-import pymprog as pymprog_interface
-import timeit
-
-pymprog_solver_selector = {'glpk': 'glpk'}
-
-def generate_solution(features):
-
-    model_object = features['model_object_before_solve']
-    model_objectives = features['objectives']
-    model_constraints = features['constraints']
-    directions = features['directions']
-    constraint_labels= features['constraint_labels']
-    debug = features['debug_mode']
-    time_limit = features['time_limit']
-    absolute_gap = features['absolute_gap']
-    relative_gap = features['relative_gap']
-    thread_count = features['thread_count']
-    solver_name = features['solver_name']
-    objective_id = features['objective_being_optimized']
-    log = features['log']
-    save = features['save_solver_log']
-    save_model = features['write_model_file']
-    email = features['email_address']
-    max_iterations= features['max_iterations']
-    solver_options= features['solver_options']
-
-    if log:
-
-        ""
-    
-    else:
-
-        msg_lev=pymprog_interface.glpk.GLP_MSG_OFF
-
-    if time_limit!=None:
-        tmlim = time_limit
-    
-    if solver_name not in pymprog_solver_selector.keys():
-        raise RuntimeError("Using solver '%s' is not supported by 'pymprog'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
-
-    match debug:
-
-        case False:
-
-            match directions[objective_id]:
-
-                case "min":
-                    pymprog_interface.minimize(model_objectives[objective_id], 'objective')
-                case "max":
-                    pymprog_interface.maximize(model_objectives[objective_id], 'objective')
-
-            for constraint in model_constraints:
-                constraint
-            time_solve_begin = timeit.default_timer()
-            result = pymprog_interface.solve(msg_lev=msg_lev, tmlim= tmlim)
-            time_solve_end = timeit.default_timer()
-            generated_solution = result, [time_solve_begin, time_solve_end]
-    
-    return generated_solution
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+import cylp as cylp_interface
+from cylp.cy import CyClpSimplex
+import timeit
+
+cylp_solver_selector = {'cbc': 'cbc'}
+
+
+def generate_solution(features):
+
+    model_object = features['model_object_before_solve']
+    model_objectives = features['objectives']
+    model_constraints = features['constraints']
+    directions = features['directions']
+    constraint_labels = features['constraint_labels']
+    debug = features['debug_mode']
+    time_limit = features['time_limit']
+    absolute_gap = features['absolute_gap']
+    relative_gap = features['relative_gap']
+    thread_count = features['thread_count']
+    solver_name = features['solver_name']
+    objective_id = features['objective_being_optimized']
+    log = features['log']
+    save = features['save_solver_log']
+    save_model = features['write_model_file']
+    email = features['email_address']
+    max_iterations = features['max_iterations']
+    solver_options = features['solver_options']
+
+    if solver_name not in cylp_solver_selector.keys():
+        raise RuntimeError(
+            "Using solver '%s' is not supported by 'cylp'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
+
+    match debug:
+
+        case False:
+
+            match directions[objective_id]:
+                case 'min':
+                    model_object.objective = 1*(model_objectives[objective_id])
+                case 'max':
+                    model_object.objective = -1 * \
+                        (model_objectives[objective_id])
+
+            for constraint in model_constraints:
+                model_object += constraint
+
+            cbcModel = cylp_interface.cy.CyClpSimplex(
+                model_object).getCbcModel()
+            time_solve_begin = timeit.default_timer()
+            result = cbcModel.solve()
+            time_solve_end = timeit.default_timer()
+            generated_solution = [result, [time_solve_begin, time_solve_end]]
+
+    return generated_solution
```

### Comparing `feloopy-0.2.4/feloopy/generators/variable/gekko_variable_generator.py` & `feloopy-0.2.5/feloopy/generators/variable/cplex_cp_variable_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,122 @@
-import itertools as it
-
-sets = it.product
-
-def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
-
-    match variable_type:
-
-        case 'pvar':
-
-            '''
-
-            Positive Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                GeneratedVariable =  model_object.Var(lb=variable_bound[0], ub=variable_bound[1], integer=False)
-            else:
-                if len(variable_dim) == 1:
-                    GeneratedVariable =  {key:  model_object.Var(lb=variable_bound[0], ub=variable_bound[1], integer=False) for key in variable_dim[0]}
-                else:
-                    GeneratedVariable =  {key: model_object.Var(lb=variable_bound[0], ub=variable_bound[1], integer=False) for key in sets(*variable_dim)}
-                    
-        case 'bvar':
-
-            '''
-
-            Binary Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                GeneratedVariable =  model_object.Var(lb=variable_bound[0], ub=variable_bound[1], integer=True)
-            else:
-                if len(variable_dim) == 1:
-                    GeneratedVariable =  {key:  model_object.Var(lb=0, ub=1, integer=True) for key in variable_dim[0]}
-                else:
-                    GeneratedVariable =  {key: model_object.Var(lb=0, ub=1, integer=True) for key in sets(*variable_dim)}
-
-        case 'ivar':
-
-            '''
-
-            Integer Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                GeneratedVariable =  model_object.Var(lb=variable_bound[0], ub=variable_bound[1], integer=True)
-            else:
-                if len(variable_dim) == 1:
-                    GeneratedVariable =  {key:  model_object.Var(lb=variable_bound[0], ub=variable_bound[1], integer=True) for key in variable_dim[0]}
-                else:
-                    GeneratedVariable =  {key: model_object.Var(lb=variable_bound[0], ub=variable_bound[1], integer=True) for key in sets(*variable_dim)}
-
-                            
-        case 'fvar':
-
-            '''
-
-            Free Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                GeneratedVariable =  model_object.Var()
-            else:
-                if len(variable_dim) == 1:
-                    GeneratedVariable =  {key:  model_object.Var() for key in variable_dim[0]}
-                else:
-                    GeneratedVariable =  {key: model_object.Var() for key in sets(*variable_dim)}
-
-
-    return GeneratedVariable
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+import itertools as it
+
+sets = it.product
+
+
+def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
+
+    match variable_type:
+
+        case 'pvar':
+
+            '''
+
+            Positive Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = model_object.continuous_var(
+                    min=variable_bound[0], max=variable_bound[1])
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: model_object.continuous_var(
+                        min=variable_bound[0], max=variable_bound[1]) for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {key: model_object.continuous_var(
+                        min=variable_bound[0], max=variable_bound[1]) for key in sets(*variable_dim)}
+
+        case 'bvar':
+
+            '''
+
+            Binary Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = model_object.binary_var()
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {
+                        key: model_object.binary_var() for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {
+                        key: model_object.binary_var() for key in sets(*variable_dim)}
+
+        case 'ivar':
+
+            '''
+
+            Integer Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = model_object.integer_var(
+                    min=variable_bound[0], max=variable_bound[1])
+
+            else:
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: model_object.integer_var(
+                        min=variable_bound[0], max=variable_bound[1]) for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {key: model_object.integer_var(
+                        min=variable_bound[0], max=variable_bound[1]) for key in sets(*variable_dim)}
+
+        case 'fvar':
+
+            '''
+
+            Free Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = model_object.continuous_var(
+                    min=variable_bound[0], max=variable_bound[1])
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: model_object.continuous_var(
+                        min=variable_bound[0], max=variable_bound[1]) for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {key: model_object.continuous_var(
+                        min=variable_bound[0], max=variable_bound[1]) for key in sets(*variable_dim)}
+
+    return GeneratedVariable
```

### Comparing `feloopy-0.2.4/feloopy/generators/variable/gurobi_variable_generator.py` & `feloopy-0.2.5/feloopy/generators/variable/gurobi_variable_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,190 +1,240 @@
-import gurobipy as gurobi_interface
-import itertools as it
-
-sets = it.product
-
-POSITIVE = gurobi_interface.GRB.CONTINUOUS
-INTEGER = gurobi_interface.GRB.INTEGER
-BINARY = gurobi_interface.GRB.BINARY
-FREE = gurobi_interface.GRB.CONTINUOUS
-INFINITY = gurobi_interface.GRB.INFINITY
-
-def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
-
-    if variable_bound[0] == None: variable_bound[0] = -INFINITY
-    
-    if variable_bound[1] == None: variable_bound[1] = +INFINITY
-
-    match variable_type:
-
-        case 'pvar':
-
-            '''
-
-            Positive Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                
-                generated_variable = model_object.addVar(vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-            else:
-                
-                if len(variable_dim) == 1:
-                
-                    generated_variable = {key: model_object.addVar(vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    generated_variable = {key: model_object.addVar(vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
-
-        case 'bvar':
-
-            '''
-
-            Binary Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                
-                generated_variable = model_object.addVar(vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-            else:
-                
-                if len(variable_dim) == 1:
-                
-                    generated_variable = {key: model_object.addVar(vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    generated_variable = {key: model_object.addVar(vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
-
-       
-        case 'ivar':
-
-            '''
-
-            Integer Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                
-                generated_variable = model_object.addVar(vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-            else:
-                
-                if len(variable_dim) == 1:
-                
-                    generated_variable = {key: model_object.addVar(vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    generated_variable = {key: model_object.addVar(vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
-
-        case 'fvar':
-
-            '''
-
-            Free Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                
-                generated_variable = model_object.addVar(vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-            else:
-                
-                if len(variable_dim) == 1:
-                
-                    generated_variable = {key: model_object.addVar(vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    generated_variable = {key: model_object.addVar(vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
-
-
-        case 'ptvar':
-
-            '''
-
-            Positive Tensor Variable Generator
-
-            '''
-
-            if variable_dim == 0:
-                
-                generated_variable = model_object.addVar(vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-            else:
-                
-                if len(variable_dim) == 1:
-
-                    generated_variable = model_object.addMVar((len(variable_dim[0])),vtype=POSITIVE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-                elif len(variable_dim) == 2:
-
-                    generated_variable = model_object.addMVar((len(variable_dim[0]),len(variable_dim[1])),vtype=POSITIVE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-                else:
-                    
-                    generated_variable = model_object.addMVar(tuple([len(key) for key in variable_dim]),vtype=POSITIVE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-        case 'ftvar':
-
-            '''
-
-            Free Tensor Variable Generator
-
-            '''
-
-            if variable_dim == 0: generated_variable = model_object.addVar(vtype=FREE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-            else:
-                
-                if len(variable_dim) == 1: generated_variable = model_object.addMVar((len(variable_dim[0])),vtype=FREE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-                elif len(variable_dim) == 2: generated_variable = model_object.addMVar((len(variable_dim[0]),len(variable_dim[1])),vtype=FREE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-                else: generated_variable = model_object.addMVar(tuple([len(key) for key in variable_dim]),vtype=FREE,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-
-        case 'btvar':
-
-            '''
-
-            Binary Tensor Variable Generator
-
-
-            '''
-
-            if variable_dim == 0: generated_variable = model_object.addVar(vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-            else:
-
-                if len(variable_dim) == 1: generated_variable = model_object.addMVar((len(variable_dim[0])),vtype=BINARY,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-                elif len(variable_dim) == 2: generated_variable = model_object.addMVar((len(variable_dim[0]),len(variable_dim[1])),vtype=BINARY,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-                else: generated_variable = model_object.addMVar(tuple([len(key) for key in variable_dim]),vtype=BINARY,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-        case 'itvar':
-
-            '''
-
-            Integer Tensor Variable Generator
-
-            '''
-
-            if variable_dim == 0: generated_variable = model_object.addVar(vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-
-            else:
-                
-                if len(variable_dim) == 1: generated_variable = model_object.addMVar((len(variable_dim[0])),vtype=INTEGER,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-                elif len(variable_dim) == 2: generated_variable = model_object.addMVar((len(variable_dim[0]),len(variable_dim[1])),vtype=INTEGER,lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
-                else: generated_variable = model_object.addMVar(tuple([len(key) for key in variable_dim]),vtype=INTEGER,lb=variable_bound[0], ub=variable_bound[1],name=variable_name)
-
-    return generated_variable
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+import gurobipy as gurobi_interface
+import itertools as it
+
+sets = it.product
+
+POSITIVE = gurobi_interface.GRB.CONTINUOUS
+INTEGER = gurobi_interface.GRB.INTEGER
+BINARY = gurobi_interface.GRB.BINARY
+FREE = gurobi_interface.GRB.CONTINUOUS
+INFINITY = gurobi_interface.GRB.INFINITY
+
+
+def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
+
+    if variable_bound[0] == None:
+        variable_bound[0] = -INFINITY
+
+    if variable_bound[1] == None:
+        variable_bound[1] = +INFINITY
+
+    match variable_type:
+
+        case 'pvar':
+
+            '''
+
+            Positive Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                generated_variable = model_object.addVar(
+                    vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    generated_variable = {key: model_object.addVar(
+                        vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    generated_variable = {key: model_object.addVar(
+                        vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+
+        case 'bvar':
+
+            '''
+
+            Binary Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                generated_variable = model_object.addVar(
+                    vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    generated_variable = {key: model_object.addVar(
+                        vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    generated_variable = {key: model_object.addVar(
+                        vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+
+        case 'ivar':
+
+            '''
+
+            Integer Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                generated_variable = model_object.addVar(
+                    vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    generated_variable = {key: model_object.addVar(
+                        vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    generated_variable = {key: model_object.addVar(
+                        vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+
+        case 'fvar':
+
+            '''
+
+            Free Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                generated_variable = model_object.addVar(
+                    vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    generated_variable = {key: model_object.addVar(
+                        vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    generated_variable = {key: model_object.addVar(
+                        vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+
+        case 'ptvar':
+
+            '''
+
+            Positive Tensor Variable Generator
+
+            '''
+
+            if variable_dim == 0:
+
+                generated_variable = model_object.addVar(
+                    vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    generated_variable = model_object.addMVar(
+                        (len(variable_dim[0])), vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+                elif len(variable_dim) == 2:
+
+                    generated_variable = model_object.addMVar((len(variable_dim[0]), len(
+                        variable_dim[1])), vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+                else:
+
+                    generated_variable = model_object.addMVar(tuple(
+                        [len(key) for key in variable_dim]), vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+        case 'ftvar':
+
+            '''
+
+            Free Tensor Variable Generator
+
+            '''
+
+            if variable_dim == 0:
+                generated_variable = model_object.addVar(
+                    vtype=FREE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+            else:
+
+                if len(variable_dim) == 1:
+                    generated_variable = model_object.addMVar(
+                        (len(variable_dim[0])), vtype=FREE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+                elif len(variable_dim) == 2:
+                    generated_variable = model_object.addMVar((len(variable_dim[0]), len(
+                        variable_dim[1])), vtype=FREE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+                else:
+                    generated_variable = model_object.addMVar(tuple(
+                        [len(key) for key in variable_dim]), vtype=FREE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+        case 'btvar':
+
+            '''
+
+            Binary Tensor Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+                generated_variable = model_object.addVar(
+                    vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+            else:
+
+                if len(variable_dim) == 1:
+                    generated_variable = model_object.addMVar(
+                        (len(variable_dim[0])), vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+                elif len(variable_dim) == 2:
+                    generated_variable = model_object.addMVar((len(variable_dim[0]), len(
+                        variable_dim[1])), vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+                else:
+                    generated_variable = model_object.addMVar(tuple(
+                        [len(key) for key in variable_dim]), vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+        case 'itvar':
+
+            '''
+
+            Integer Tensor Variable Generator
+
+            '''
+
+            if variable_dim == 0:
+                generated_variable = model_object.addVar(
+                    vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+            else:
+
+                if len(variable_dim) == 1:
+                    generated_variable = model_object.addMVar(
+                        (len(variable_dim[0])), vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+                elif len(variable_dim) == 2:
+                    generated_variable = model_object.addMVar((len(variable_dim[0]), len(
+                        variable_dim[1])), vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+                else:
+                    generated_variable = model_object.addMVar(tuple(
+                        [len(key) for key in variable_dim]), vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+    return generated_variable
```

### Comparing `feloopy-0.2.4/feloopy/generators/variable/linopy_variable_generator.py` & `feloopy-0.2.5/feloopy/generators/variable/gekko_variable_generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,99 @@
-import itertools as it
-import pandas as pd
-
-sets = it.product
-
-def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
-
-    match variable_type:
-
-        case 'pvar':
-
-            '''
-
-            Positive Variable Generator
-
-
-            '''
-            if variable_dim == 0:
-                GeneratedVariable =  model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], name=variable_name)
-            else:
-                GeneratedVariable =  model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name)
-      
-        case 'bvar':
-
-            '''
-
-            Binary Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                GeneratedVariable =  model_object.add_variables(name=variable_name, binary=True)
-            else:
-                GeneratedVariable =  model_object.add_variables(coords=pd.Index(variable_dim), name=variable_name,  binary=True)
-
-                    
-                    
-        case 'ivar':
-
-            '''
-
-            Integer Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                GeneratedVariable =  model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], name=variable_name, binary=True)
-            else:
-                GeneratedVariable =  model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name,  integer=True)
-
-                            
-        case 'fvar':
-
-            '''
-
-            Free Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                GeneratedVariable =  model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], name=variable_name)
-            else:
-                GeneratedVariable =  model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name)
-
-    
-    return  GeneratedVariable
-    
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+import itertools as it
+
+sets = it.product
+
+
+def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
+
+    match variable_type:
+
+        case 'pvar':
+
+            '''
+
+            Positive Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+                GeneratedVariable = model_object.Var(
+                    lb=variable_bound[0], ub=variable_bound[1], integer=False)
+            else:
+                if len(variable_dim) == 1:
+                    GeneratedVariable = {key:  model_object.Var(
+                        lb=variable_bound[0], ub=variable_bound[1], integer=False) for key in variable_dim[0]}
+                else:
+                    GeneratedVariable = {key: model_object.Var(
+                        lb=variable_bound[0], ub=variable_bound[1], integer=False) for key in sets(*variable_dim)}
+
+        case 'bvar':
+
+            '''
+
+            Binary Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+                GeneratedVariable = model_object.Var(
+                    lb=variable_bound[0], ub=variable_bound[1], integer=True)
+            else:
+                if len(variable_dim) == 1:
+                    GeneratedVariable = {key:  model_object.Var(
+                        lb=0, ub=1, integer=True) for key in variable_dim[0]}
+                else:
+                    GeneratedVariable = {key: model_object.Var(
+                        lb=0, ub=1, integer=True) for key in sets(*variable_dim)}
+
+        case 'ivar':
+
+            '''
+
+            Integer Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+                GeneratedVariable = model_object.Var(
+                    lb=variable_bound[0], ub=variable_bound[1], integer=True)
+            else:
+                if len(variable_dim) == 1:
+                    GeneratedVariable = {key:  model_object.Var(
+                        lb=variable_bound[0], ub=variable_bound[1], integer=True) for key in variable_dim[0]}
+                else:
+                    GeneratedVariable = {key: model_object.Var(
+                        lb=variable_bound[0], ub=variable_bound[1], integer=True) for key in sets(*variable_dim)}
+
+        case 'fvar':
+
+            '''
+
+            Free Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+                GeneratedVariable = model_object.Var()
+            else:
+                if len(variable_dim) == 1:
+                    GeneratedVariable = {key:  model_object.Var()
+                                         for key in variable_dim[0]}
+                else:
+                    GeneratedVariable = {key: model_object.Var()
+                                         for key in sets(*variable_dim)}
+
+    return GeneratedVariable
```

### Comparing `feloopy-0.2.4/feloopy/generators/variable/ortools_cp_variable_generator.py` & `feloopy-0.2.5/feloopy/generators/variable/cplex_variable_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,124 +1,122 @@
-import itertools as it
-
-sets = it.product
-
-def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
-
-    match variable_type:
-
-        case 'pvar':
-
-            '''
-
-            Positive Variable Generator
-
-
-            '''
-
-            if variable_bound[0] == 0:
-
-                variable_bound[0] = 0
-
-            if variable_dim == 0:
-                
-                GeneratedVariable =  model_object.NewNumVar(variable_bound[0], variable_bound[1], variable_name)
-            
-            else:
-                
-                if len(variable_dim) == 1:
-                    
-                    GeneratedVariable =  {key: model_object.NewNumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    GeneratedVariable =  {key: model_object.NewNumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
-
-
-                    
-        case 'bvar':
-
-            '''
-
-            Binary Variable Generator
-
-
-            '''
-
-            if variable_bound[0] == 0:
-
-                variable_bound[0] = 0
-            
-            
-            if variable_bound[1] == 1:
-
-                variable_bound[1] = 1
-
-            if variable_dim == 0:
-                
-                GeneratedVariable =  model_object.NewIntVar(variable_bound[0], variable_bound[1], variable_name)
-            
-            else:
-                
-                if len(variable_dim) == 1:
-                    
-                    GeneratedVariable =  {key: model_object.NewIntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    GeneratedVariable =  {key: model_object.NewIntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
-
-                  
-                    
-        case 'ivar':
-
-            '''
-
-            Integer Variable Generator
-
-
-            '''
-
-            if variable_bound[0] == 0:
-
-                variable_bound[0] = 0
-
-            if variable_dim == 0:
-
-                GeneratedVariable = model_object.NewIntVar(variable_bound[0], variable_bound[1], variable_name)
-
-            else:
-                
-                if len(variable_dim) == 1:
-                    
-                    GeneratedVariable = {key: model_object.NewIntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    GeneratedVariable = {key: model_object.NewIntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
-
-
-
-        case 'fvar':
-
-            '''
-
-            Free Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                
-                GeneratedVariable = model_object.NewNumVar(variable_bound[0], variable_bound[1], variable_name)
-            
-            else:
-                
-                if len(variable_dim) == 1:
-                    
-                    GeneratedVariable = {key: model_object.NewNumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    GeneratedVariable = {key: model_object.NewNumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
-    
-    return GeneratedVariable
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+import cplex
+import itertools as it
+
+sets = it.product
+
+
+def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
+
+    match variable_type:
+
+        case 'pvar':
+
+            '''
+
+            Positive Variable Generator
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = model_object.continuous_var(
+                    lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: model_object.continuous_var(
+                        lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {key: model_object.continuous_var(
+                        lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+
+        case 'bvar':
+
+            ''', 
+
+            Binary Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = model_object.binary_var(name=variable_name)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: model_object.binary_var(
+                        name=f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {key: model_object.binary_var(
+                        name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+
+        case 'ivar':
+
+            '''
+
+            Integer Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = model_object.integer_var(
+                    lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+            else:
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: model_object.integer_var(
+                        lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {key: model_object.integer_var(
+                        lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+
+        case 'fvar':
+
+            '''
+
+            Free Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = model_object.continuous_var(
+                    lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: model_object.continuous_var(
+                        lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {key: model_object.continuous_var(
+                        lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+
+    return GeneratedVariable
```

### Comparing `feloopy-0.2.4/feloopy/generators/variable/ortools_variable_generator.py` & `feloopy-0.2.5/feloopy/generators/variable/xpress_variable_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,129 +1,159 @@
-import itertools as it
-
-sets = it.product
-
-
-def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
-
-    if variable_bound[0] == None: variable_bound[0] = -model_object.infinity()
-    
-    if variable_bound[1] == None: variable_bound[1] = model_object.infinity()
-
-    match variable_type:
-
-        case 'pvar':
-
-            '''
-
-            Positive Variable Generator
-
-
-            '''
-
-            
-            if variable_dim == 0:
-                
-                GeneratedVariable =  model_object.NumVar(variable_bound[0], variable_bound[1], variable_name)
-            
-            else:
-                
-                if len(variable_dim) == 1:
-                    
-                    GeneratedVariable =  {key: model_object.NumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    GeneratedVariable =  {key: model_object.NumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
-
-
-                    
-        case 'bvar':
-
-            '''
-
-            Binary Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                
-                GeneratedVariable =  model_object.IntVar(variable_bound[0], variable_bound[1], variable_name)
-            
-            else:
-                
-                if len(variable_dim) == 1:
-                    
-                    GeneratedVariable =  {key: model_object.IntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    GeneratedVariable =  {key: model_object.IntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
-
-                  
-                    
-        case 'ivar':
-
-            '''
-
-            Integer Variable Generator
-
-
-            '''
-
-            if variable_bound[0] == 0:
-
-                variable_bound[0] = 0
-
-            if variable_bound[1] == None:
-
-                variable_bound[1] = model_object.infinity()
-
-            if variable_dim == 0:
-
-                GeneratedVariable = model_object.IntVar(variable_bound[0], variable_bound[1], variable_name)
-
-            else:
-                
-                if len(variable_dim) == 1:
-                    
-                    GeneratedVariable = {key: model_object.IntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    GeneratedVariable = {key: model_object.IntVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
-
-
-
-        case 'fvar':
-
-            '''
-
-            Free Variable Generator
-
-
-            '''
-
-            if variable_bound[0] == None:
-                
-                variable_bound[0] = -model_object.infinity()
-            
-            if variable_bound[1] == None:
-                
-                variable_bound[1] = model_object.infinity()
-
-            if variable_dim == 0:
-                
-                GeneratedVariable = model_object.NumVar(variable_bound[0], variable_bound[1], variable_name)
-            
-            else:
-                
-                if len(variable_dim) == 1:
-                    
-                    GeneratedVariable = {key: model_object.NumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
-                
-                else:
-                    
-                    GeneratedVariable = {key: model_object.NumVar(variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
-    
-    return GeneratedVariable
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+import xpress as xpress_interface
+import itertools as it
+
+sets = it.product
+
+VariableGenerator = xpress_interface.var
+
+INFINITY = xpress_interface.infinity
+BINARY = xpress_interface.binary
+INTEGER = xpress_interface.integer
+
+
+def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
+
+    if variable_bound[0] == None:
+        variable_bound[0] = -INFINITY
+
+    if variable_bound[1] == None:
+        variable_bound[1] = +INFINITY
+
+    match variable_type:
+
+        case 'pvar':
+
+            '''
+
+            Positive Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = VariableGenerator(
+                    lb=variable_bound[0], ub=variable_bound[1])
+
+                model_object.addVariable(GeneratedVariable)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = [VariableGenerator(
+                        lb=variable_bound[0], ub=variable_bound[1]) for key in variable_dim[0]]
+
+                    model_object.addVariable(GeneratedVariable)
+
+                else:
+
+                    GeneratedVariable = {key: VariableGenerator(
+                        name=f"{variable_name}{key}", lb=variable_bound[0], ub=variable_bound[1]) for key in sets(*variable_dim)}
+
+                    model_object.addVariable(GeneratedVariable)
+
+        case 'bvar':
+
+            '''
+
+            Binary Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = VariableGenerator(vartype=BINARY)
+
+                model_object.addVariable(GeneratedVariable)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = [VariableGenerator(
+                        vartype=BINARY) for key in variable_dim[0]]
+
+                    model_object.addVariable(GeneratedVariable)
+
+                else:
+
+                    GeneratedVariable = {key: VariableGenerator(
+                        name=f"{variable_name}{key}", lb=variable_bound[0], ub=variable_bound[1], vartype=BINARY) for key in sets(*variable_dim)}
+
+                    model_object.addVariable(GeneratedVariable)
+
+        case 'ivar':
+
+            '''
+
+            Integer Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = VariableGenerator(vartype=INTEGER)
+
+                model_object.addVariable(GeneratedVariable)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: VariableGenerator(
+                        vartype=INTEGER) for key in variable_dim[0]}
+
+                    model_object.addVariable(GeneratedVariable)
+
+                else:
+
+                    GeneratedVariable = {key: VariableGenerator(
+                        name=f"{variable_name}{key}", lb=variable_bound[0], ub=variable_bound[1], vartype=INTEGER) for key in sets(*variable_dim)}
+
+                    model_object.addVariable(GeneratedVariable)
+
+        case 'fvar':
+
+            '''
+
+            Free Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+
+                GeneratedVariable = VariableGenerator(
+                    lb=variable_bound[0], ub=variable_bound[1])
+
+                model_object.addVariable(GeneratedVariable)
+
+            else:
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = [VariableGenerator(
+                        lb=variable_bound[0], ub=variable_bound[1]) for key in variable_dim[0]]
+
+                    model_object.addVariable(GeneratedVariable)
+
+                else:
+
+                    GeneratedVariable = {key: VariableGenerator(
+                        name=f"{variable_name}{key}", lb=variable_bound[0], ub=variable_bound[1]) for key in sets(*variable_dim)}
+
+                    model_object.addVariable(GeneratedVariable)
+
+    return GeneratedVariable
```

### Comparing `feloopy-0.2.4/feloopy/generators/variable/picos_variable_generator.py` & `feloopy-0.2.5/feloopy/generators/variable/linopy_variable_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,84 @@
-import itertools as it
-import picos as picos_interface
-
-
-sets = it.product
-
-BINARY = picos_interface.BinaryVariable
-POSITIVE = picos_interface.RealVariable
-INTEGER = picos_interface.IntegerVariable
-FREE = picos_interface.RealVariable
-
-def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
-
-    match variable_type:
-
-        case 'pvar':
-
-            '''
-
-            Positive Variable Generator
-
-
-            '''
-
-            if variable_dim == 0:
-                GeneratedVariable =  POSITIVE(variable_name, lower=variable_bound[0], upper=variable_bound[1])
-            else:
-                if len(variable_dim) == 1:
-                    GeneratedVariable =  {key: POSITIVE(variable_name, lower=variable_bound[0], upper=variable_bound[1]) for key in variable_dim[0]}
-                else:
-                    GeneratedVariable =  {key: POSITIVE(variable_name, lower=variable_bound[0], upper=variable_bound[1]) for key in it.product(*variable_dim)}
-                            
-        case 'bvar':
-
-            '''
-
-            Binary Variable Generator
-
-
-            '''
-            if variable_dim == 0:
-                GeneratedVariable =  BINARY(variable_name)
-            else:
-                if len(variable_dim) == 1:
-                    GeneratedVariable =  {key: BINARY(variable_name) for key in variable_dim[0]}
-                else:
-                    GeneratedVariable =  {key: BINARY(variable_name) for key in it.product(*variable_dim)}
-
-        case 'ivar':
-
-            '''
-
-            Integer Variable Generator
-
-
-            '''
-            if variable_dim == 0:
-                GeneratedVariable =  INTEGER(variable_name, lower=variable_bound[0], upper=variable_bound[1])
-            else:
-                if len(variable_dim) == 1:
-                    GeneratedVariable =  {key: INTEGER(variable_name, lower=variable_bound[0], upper=variable_bound[1]) for key in variable_dim[0]}
-                else:
-                    GeneratedVariable =  {key: INTEGER(variable_name, lower=variable_bound[0], upper=variable_bound[1]) for key in it.product(*variable_dim)}
-                            
-        case 'fvar':
-
-            '''
-
-            Free Variable Generator
-
-
-            '''
-            if variable_dim == 0:
-                GeneratedVariable = FREE(variable_name, lower=variable_bound[0], upper=variable_bound[1])
-            else:
-                if len(variable_dim) == 1:
-                    GeneratedVariable =  {key: FREE(variable_name, lower=variable_bound[0], upper=variable_bound[1]) for key in variable_dim[0]}
-                else:
-                    GeneratedVariable =  {key: FREE(variable_name, lower=variable_bound[0], upper=variable_bound[1]) for key in it.product(*variable_dim)}
-
-    return  GeneratedVariable
-
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+import itertools as it
+import pandas as pd
+
+sets = it.product
+
+
+def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
+
+    match variable_type:
+
+        case 'pvar':
+
+            '''
+
+            Positive Variable Generator
+
+
+            '''
+            if variable_dim == 0:
+                GeneratedVariable = model_object.add_variables(
+                    lower=variable_bound[0], upper=variable_bound[1], name=variable_name)
+            else:
+                GeneratedVariable = model_object.add_variables(
+                    lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name)
+
+        case 'bvar':
+
+            '''
+
+            Binary Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+                GeneratedVariable = model_object.add_variables(
+                    name=variable_name, binary=True)
+            else:
+                GeneratedVariable = model_object.add_variables(
+                    coords=pd.Index(variable_dim), name=variable_name,  binary=True)
+
+        case 'ivar':
+
+            '''
+
+            Integer Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+                GeneratedVariable = model_object.add_variables(
+                    lower=variable_bound[0], upper=variable_bound[1], name=variable_name, binary=True)
+            else:
+                GeneratedVariable = model_object.add_variables(
+                    lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name,  integer=True)
+
+        case 'fvar':
+
+            '''
+
+            Free Variable Generator
+
+
+            '''
+
+            if variable_dim == 0:
+                GeneratedVariable = model_object.add_variables(
+                    lower=variable_bound[0], upper=variable_bound[1], name=variable_name)
+            else:
+                GeneratedVariable = model_object.add_variables(
+                    lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name)
+
+    return GeneratedVariable
```

### Comparing `feloopy-0.2.4/feloopy/generators/variable_generator.py` & `feloopy-0.2.5/feloopy/generators/variable_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,95 @@
-def generate_variable(interface_name, model_object, variable_type, variable_name, variable_bound, variable_dim):
-
-    inputs = {'model_object': model_object, 
-              'variable_type': variable_type, 
-              'variable_name': variable_name, 
-              'variable_bound': variable_bound, 
-              'variable_dim': variable_dim }
-
-    match interface_name:
-
-        case 'pulp':
-
-            from .variable import pulp_variable_generator
-            return pulp_variable_generator.generate_variable(**inputs)
-
-        case 'pyomo':
-
-            from .variable import pyomo_variable_generator
-            return pyomo_variable_generator.generate_variable(**inputs)
-
-        case 'ortools':
-
-            from .variable import ortools_variable_generator
-            return ortools_variable_generator.generate_variable(**inputs)
-
-        case 'ortools_cp':
-
-            from .variable import ortools_cp_variable_generator
-            return ortools_cp_variable_generator.generate_variable(**inputs)
-
-        case 'gekko':
-
-            from .variable import gekko_variable_generator
-            return gekko_variable_generator.generate_variable(**inputs)
-
-        case 'picos':
-
-            from .variable import picos_variable_generator
-            return picos_variable_generator.generate_variable(**inputs)
-
-        case 'cvxpy':
-
-            from .variable import cvxpy_variable_generator
-            return cvxpy_variable_generator.generate_variable(**inputs)
-
-        case 'cylp':
-
-            from .variable import cylp_variable_generator
-            return cylp_variable_generator.generate_variable(**inputs)
-
-        case 'pymprog':
-
-            from .variable import pymprog_variable_generator
-            return pymprog_variable_generator.generate_variable(**inputs)
-
-        case 'cplex':
-
-            from .variable import cplex_variable_generator
-            return cplex_variable_generator.generate_variable(**inputs)
-
-        case 'cplex_cp':
-
-            from .variable import cplex_cp_variable_generator
-            return cplex_cp_variable_generator.generate_variable(**inputs)
-
-        case 'gurobi':
-
-            from .variable import gurobi_variable_generator
-            return gurobi_variable_generator.generate_variable(**inputs)
-
-        case 'xpress':
-
-            from .variable import xpress_variable_generator
-            return xpress_variable_generator.generate_variable(**inputs)
-
-        case 'mip':
-
-            from .variable import mip_variable_generator
-            return mip_variable_generator.generate_variable(**inputs)
-
-        case 'linopy':
-
-            from .variable import linopy_variable_generator
-            return linopy_variable_generator.generate_variable(**inputs)
+'''
+ # @ Author: Keivan Tafakkori
+ # @ Created: 2023-05-11
+ # @ Modified: 2023-05-12
+ # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
+ # @ Github: https://github.com/ktafakkori
+ # @ Website: https://ktafakkori.github.io/
+ # @ Copyright: 2023. MIT License. All Rights Reserved.
+ '''
+
+
+def generate_variable(interface_name, model_object, variable_type, variable_name, variable_bound, variable_dim):
+
+    inputs = {'model_object': model_object,
+              'variable_type': variable_type,
+              'variable_name': variable_name,
+              'variable_bound': variable_bound,
+              'variable_dim': variable_dim}
+
+    match interface_name:
+
+        case 'pulp':
+
+            from .variable import pulp_variable_generator
+            return pulp_variable_generator.generate_variable(**inputs)
+
+        case 'pyomo':
+
+            from .variable import pyomo_variable_generator
+            return pyomo_variable_generator.generate_variable(**inputs)
+
+        case 'ortools':
+
+            from .variable import ortools_variable_generator
+            return ortools_variable_generator.generate_variable(**inputs)
+
+        case 'ortools_cp':
+
+            from .variable import ortools_cp_variable_generator
+            return ortools_cp_variable_generator.generate_variable(**inputs)
+
+        case 'gekko':
+
+            from .variable import gekko_variable_generator
+            return gekko_variable_generator.generate_variable(**inputs)
+
+        case 'picos':
+
+            from .variable import picos_variable_generator
+            return picos_variable_generator.generate_variable(**inputs)
+
+        case 'cvxpy':
+
+            from .variable import cvxpy_variable_generator
+            return cvxpy_variable_generator.generate_variable(**inputs)
+
+        case 'cylp':
+
+            from .variable import cylp_variable_generator
+            return cylp_variable_generator.generate_variable(**inputs)
+
+        case 'pymprog':
+
+            from .variable import pymprog_variable_generator
+            return pymprog_variable_generator.generate_variable(**inputs)
+
+        case 'cplex':
+
+            from .variable import cplex_variable_generator
+            return cplex_variable_generator.generate_variable(**inputs)
+
+        case 'cplex_cp':
+
+            from .variable import cplex_cp_variable_generator
+            return cplex_cp_variable_generator.generate_variable(**inputs)
+
+        case 'gurobi':
+
+            from .variable import gurobi_variable_generator
+            return gurobi_variable_generator.generate_variable(**inputs)
+
+        case 'xpress':
+
+            from .variable import xpress_variable_generator
+            return xpress_variable_generator.generate_variable(**inputs)
+
+        case 'mip':
+
+            from .variable import mip_variable_generator
+            return mip_variable_generator.generate_variable(**inputs)
+
+        case 'linopy':
+
+            from .variable import linopy_variable_generator
+            return linopy_variable_generator.generate_variable(**inputs)
```

