# Comparing `tmp/econpizza-0.5.5.tar.gz` & `tmp/econpizza-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econpizza-0.5.5.tar", last modified: Fri May  5 14:43:28 2023, max compression
+gzip compressed data, was "econpizza-0.5.6.tar", last modified: Sat May 27 12:37:03 2023, max compression
```

## Comparing `econpizza-0.5.5.tar` & `econpizza-0.5.6.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.226970 econpizza-0.5.5/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.063634 econpizza-0.5.5/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.076968 econpizza-0.5.5/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1527 2023-04-15 12:29:25.000000 econpizza-0.5.5/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.5.5/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.5.5/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.5.5/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3829 2023-05-05 14:43:28.226970 econpizza-0.5.5/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3351 2023-05-05 14:03:24.000000 econpizza-0.5.5/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.096968 econpizza-0.5.5/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.5.5/docs/Makefile
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.066968 econpizza-0.5.5/docs/_static/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.096968 econpizza-0.5.5/docs/_static/css/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.5.5/docs/_static/css/custom.css
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1551 2023-05-02 19:15:35.000000 econpizza-0.5.5/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.5.5/docs/content.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.103635 econpizza-0.5.5/docs/guide/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1507 2023-04-22 17:10:18.000000 econpizza-0.5.5/docs/guide/installation.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.5.5/docs/guide/method.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2384 2023-04-22 17:32:46.000000 econpizza-0.5.5/docs/guide/solution.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2117 2023-03-30 06:41:47.000000 econpizza-0.5.5/docs/guide/steady_state.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    14328 2023-05-02 15:47:57.000000 econpizza-0.5.5/docs/guide/the_yaml.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2362 2023-05-02 19:11:53.000000 econpizza-0.5.5/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.5.5/docs/lin_and_nlin.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.5.5/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.5.5/docs/p_and_n.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.5.5/docs/requirements.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.176969 econpizza-0.5.5/docs/tutorial/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.5.5/docs/tutorial/boehl_hommes.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389792 2023-03-23 23:03:36.000000 econpizza-0.5.5/docs/tutorial/hank1.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.5.5/docs/tutorial/hank2.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.5.5/docs/tutorial/quickstart.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.5.5/docs/tutorial/rank.ipynb
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.206970 econpizza-0.5.5/econpizza/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3547 2023-03-28 11:53:45.000000 econpizza-0.5.5/econpizza/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-05-05 14:43:17.000000 econpizza-0.5.5/econpizza/__version__.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.213636 econpizza-0.5.5/econpizza/examples/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.5.5/econpizza/examples/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.5.5/econpizza/examples/bh.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7079 2023-03-25 09:51:02.000000 econpizza-0.5.5/econpizza/examples/dsge.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.5.5/econpizza/examples/ghls.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.5.5/econpizza/examples/hank2.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.5.5/econpizza/examples/hank2_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.5.5/econpizza/examples/hank2_no_capital.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-03-25 22:20:39.000000 econpizza-0.5.5/econpizza/examples/hank_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3716 2023-03-24 20:09:04.000000 econpizza-0.5.5/econpizza/examples/hank_labor.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.5.5/econpizza/examples/hank_labor_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6137 2023-03-24 20:09:14.000000 econpizza-0.5.5/econpizza/examples/hank_with_comments.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.5.5/econpizza/examples/nk.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.5.5/econpizza/examples/tank.yml
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.216970 econpizza-0.5.5/econpizza/parser/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12023 2023-03-31 05:55:10.000000 econpizza-0.5.5/econpizza/parser/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.5.5/econpizza/parser/build_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-04-21 09:07:56.000000 econpizza-0.5.5/econpizza/parser/checks.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.5.5/econpizza/parser/het_agent_base_funcs.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-03-30 18:29:58.000000 econpizza-0.5.5/econpizza/parser/write_dynamic_functions.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.220303 econpizza-0.5.5/econpizza/solvers/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.5.5/econpizza/solvers/shooting.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.5.5/econpizza/solvers/solve_linear.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.5.5/econpizza/solvers/solve_linear_state_space.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6106 2023-05-05 14:02:18.000000 econpizza-0.5.5/econpizza/solvers/stacking.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8549 2023-05-05 11:51:37.000000 econpizza-0.5.5/econpizza/solvers/steady_state.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.220303 econpizza-0.5.5/econpizza/testing/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.223636 econpizza-0.5.5/econpizza/testing/cache/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.5.5/econpizza/testing/cache/bh.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7064 2023-03-14 23:54:36.000000 econpizza-0.5.5/econpizza/testing/cache/hank_labor.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2984 2023-03-14 23:55:47.000000 econpizza-0.5.5/econpizza/testing/cache/hank_solid.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:35:27.000000 econpizza-0.5.5/econpizza/testing/test_nb_hank1.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:44:49.000000 econpizza-0.5.5/econpizza/testing/test_nb_hank2.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.5.5/econpizza/testing/test_nb_quickstart.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.5.5/econpizza/testing/test_nb_rank.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.5.5/econpizza/testing/test_nb_under_the_hood.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1877 2023-03-18 09:26:41.000000 econpizza-0.5.5/econpizza/testing/test_rest.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.5.5/econpizza/tools.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.226970 econpizza-0.5.5/econpizza/utilities/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.5.5/econpizza/utilities/dists.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-04-27 11:18:13.000000 econpizza-0.5.5/econpizza/utilities/grids.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4769 2023-05-04 15:35:28.000000 econpizza-0.5.5/econpizza/utilities/interp.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-30 22:34:43.000000 econpizza-0.5.5/econpizza/utilities/jacobian.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6363 2023-05-05 14:02:55.000000 econpizza-0.5.5/econpizza/utilities/newton.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.206970 econpizza-0.5.5/econpizza.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3829 2023-05-05 14:43:27.000000 econpizza-0.5.5/econpizza.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-05-05 14:43:27.000000 econpizza-0.5.5/econpizza.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-05-05 14:43:27.000000 econpizza-0.5.5/econpizza.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       77 2023-05-05 14:43:27.000000 econpizza-0.5.5/econpizza.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-05-05 14:43:27.000000 econpizza-0.5.5/econpizza.egg-info/top_level.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      113 2023-04-15 12:24:38.000000 econpizza-0.5.5/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-05-05 14:43:28.226970 econpizza-0.5.5/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1330 2023-04-15 12:24:22.000000 econpizza-0.5.5/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.744156 econpizza-0.5.6/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.744156 econpizza-0.5.6/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1527 2023-04-15 12:29:25.000000 econpizza-0.5.6/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.5.6/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.5.6/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.5.6/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3887 2023-05-27 12:37:03.754157 econpizza-0.5.6/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3409 2023-05-27 12:18:41.000000 econpizza-0.5.6/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.747490 econpizza-0.5.6/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.5.6/docs/Makefile
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.744156 econpizza-0.5.6/docs/_static/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.747490 econpizza-0.5.6/docs/_static/css/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.5.6/docs/_static/css/custom.css
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1551 2023-05-02 19:15:35.000000 econpizza-0.5.6/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.5.6/docs/content.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.747490 econpizza-0.5.6/docs/guide/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1759 2023-05-10 07:25:07.000000 econpizza-0.5.6/docs/guide/installation.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.5.6/docs/guide/method.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2606 2023-05-07 18:36:01.000000 econpizza-0.5.6/docs/guide/solution.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2161 2023-05-07 18:29:06.000000 econpizza-0.5.6/docs/guide/steady_state.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    14328 2023-05-02 15:47:57.000000 econpizza-0.5.6/docs/guide/the_yaml.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2420 2023-05-27 12:18:06.000000 econpizza-0.5.6/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.5.6/docs/lin_and_nlin.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.5.6/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.5.6/docs/p_and_n.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.5.6/docs/requirements.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.747490 econpizza-0.5.6/docs/tutorial/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.5.6/docs/tutorial/boehl_hommes.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389792 2023-03-23 23:03:36.000000 econpizza-0.5.6/docs/tutorial/hank1.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.5.6/docs/tutorial/hank2.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.5.6/docs/tutorial/quickstart.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.5.6/docs/tutorial/rank.ipynb
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.750823 econpizza-0.5.6/econpizza/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3547 2023-03-28 11:53:45.000000 econpizza-0.5.6/econpizza/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-05-27 12:36:57.000000 econpizza-0.5.6/econpizza/__version__.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.750823 econpizza-0.5.6/econpizza/examples/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.5.6/econpizza/examples/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.5.6/econpizza/examples/bh.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7086 2023-05-27 12:24:35.000000 econpizza-0.5.6/econpizza/examples/dsge.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.5.6/econpizza/examples/ghls.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.5.6/econpizza/examples/hank2.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.5.6/econpizza/examples/hank2_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.5.6/econpizza/examples/hank2_no_capital.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-05-13 03:15:20.000000 econpizza-0.5.6/econpizza/examples/hank_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3716 2023-03-24 20:09:04.000000 econpizza-0.5.6/econpizza/examples/hank_labor.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.5.6/econpizza/examples/hank_labor_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6137 2023-03-24 20:09:14.000000 econpizza-0.5.6/econpizza/examples/hank_with_comments.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.5.6/econpizza/examples/nk.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.5.6/econpizza/examples/tank.yml
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/econpizza/parser/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12187 2023-05-13 03:38:34.000000 econpizza-0.5.6/econpizza/parser/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.5.6/econpizza/parser/build_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-04-21 09:07:56.000000 econpizza-0.5.6/econpizza/parser/checks.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.5.6/econpizza/parser/het_agent_base_funcs.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4337 2023-05-12 08:16:06.000000 econpizza-0.5.6/econpizza/parser/write_dynamic_functions.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/econpizza/solvers/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.5.6/econpizza/solvers/shooting.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.5.6/econpizza/solvers/solve_linear.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.5.6/econpizza/solvers/solve_linear_state_space.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6278 2023-05-16 14:17:55.000000 econpizza-0.5.6/econpizza/solvers/stacking.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8561 2023-05-05 14:50:38.000000 econpizza-0.5.6/econpizza/solvers/steady_state.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/econpizza/testing/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/econpizza/testing/cache/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.5.6/econpizza/testing/cache/bh.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7064 2023-03-14 23:54:36.000000 econpizza-0.5.6/econpizza/testing/cache/hank_labor.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2984 2023-03-14 23:55:47.000000 econpizza-0.5.6/econpizza/testing/cache/hank_solid.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:35:27.000000 econpizza-0.5.6/econpizza/testing/test_nb_hank1.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:44:49.000000 econpizza-0.5.6/econpizza/testing/test_nb_hank2.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.5.6/econpizza/testing/test_nb_quickstart.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.5.6/econpizza/testing/test_nb_rank.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.5.6/econpizza/testing/test_nb_under_the_hood.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1883 2023-05-10 08:08:46.000000 econpizza-0.5.6/econpizza/testing/test_rest.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.5.6/econpizza/tools.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.754157 econpizza-0.5.6/econpizza/utilities/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.5.6/econpizza/utilities/dists.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-04-27 11:18:13.000000 econpizza-0.5.6/econpizza/utilities/grids.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4769 2023-05-04 15:35:28.000000 econpizza-0.5.6/econpizza/utilities/interp.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-30 22:34:43.000000 econpizza-0.5.6/econpizza/utilities/jacobian.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6395 2023-05-09 11:21:21.000000 econpizza-0.5.6/econpizza/utilities/newton.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-27 12:37:03.750823 econpizza-0.5.6/econpizza.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3887 2023-05-27 12:37:03.000000 econpizza-0.5.6/econpizza.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-05-27 12:37:03.000000 econpizza-0.5.6/econpizza.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-05-27 12:37:03.000000 econpizza-0.5.6/econpizza.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       77 2023-05-27 12:37:03.000000 econpizza-0.5.6/econpizza.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-05-27 12:37:03.000000 econpizza-0.5.6/econpizza.egg-info/top_level.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      147 2023-05-10 08:01:31.000000 econpizza-0.5.6/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-05-27 12:37:03.754157 econpizza-0.5.6/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1330 2023-04-15 12:24:22.000000 econpizza-0.5.6/setup.py
```

### Comparing `econpizza-0.5.5/.github/workflows/continuous-integration.yml` & `econpizza-0.5.6/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/.readthedocs.yaml` & `econpizza-0.5.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/LICENSE` & `econpizza-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/PKG-INFO` & `econpizza-0.5.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.5.5
+Version: 0.5.6
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
     :target: https://github.com/gboehl/econpizza/actions
 .. image:: https://readthedocs.org/projects/econpizza/badge/?version=latest
     :target: http://econpizza.readthedocs.io/en/latest/?badge=latest
 .. image:: https://badge.fury.io/py/econpizza.svg
     :target: https://badge.fury.io/py/econpizza
 
 **Econpizza** is a framework to solve and simulate *fully nonlinear* perfect foresight models, with or without heterogeneous agents.
-The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
+The package implements the solution method proposed in `HANK on Speed: Robust Nonlinear Solutions using Automatic Differentiation <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
 It allows to specify and solve nonlinear macroeconomic models quickly in a simple, high-level fashion.
 Generic and robust routines for steady state search are provided.
 
 The package can solve nonlinear models with heterogeneous agents, such as HANK models with one or two assets and portfolio choice. Steady state and nonlinear impulse responses (including, e.g., the ELB) can typically be found within a few seconds.
 The method extends the `Sequence-Space Jacobian <https://github.com/shade-econ/sequence-jacobian>`_ method (`Auclert et al., 2022, ECMA <https://doi.org/10.3982/ECTA17434>`_) to fully nonlinear heterogeneous agent models models by iteratively using `Jacobian-vector producs <https://jax.readthedocs.io/en/latest/notebooks/autodiff_cookbook.html#how-it-s-made-two-foundational-autodiff-functions>`_ to approximate the solution to the linear system of equations associated with each Newton iteration. This not only allows to study the dynamics of aggregate variables, but also the complete nonlinear transition dynamics of the cross-sectional distribution of assets and disaggregated objects.
 
 To solve models with representative agents a shooting methods similar to Laffargue (1990), Boucekkine (1995) and Juillard (1996) is implemented. It is faster and more reliable than the extended path method in dynare due to the use of automatic differentiation for the efficient jacobian decompositions during each Newton-step. Nonlinear perfect-foresight transition dynamics can - even for large-scale nonlinear models with several occassionally binding constraints - be computed in less than a second.
@@ -50,12 +50,12 @@
  * `Quickstart tutorial <https://econpizza.readthedocs.io/en/stable/tutorial/quickstart.html>`_
 
 Citation
 --------
 .. code-block:: bibtex
 
     @article{boehl2023goodpizza,
-        title       = {Robust Nonlinear Transition Dynamics in HANK},
+        title       = {HANK on Speed: Robust Nonlinear Solutions using Automatic Differentiation},
         author      = {Boehl, Gregor},
         journal     = {Available at SSRN 4433585},
         year        = {2023}
     }
```

### Comparing `econpizza-0.5.5/README.rst` & `econpizza-0.5.6/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     :target: https://github.com/gboehl/econpizza/actions
 .. image:: https://readthedocs.org/projects/econpizza/badge/?version=latest
     :target: http://econpizza.readthedocs.io/en/latest/?badge=latest
 .. image:: https://badge.fury.io/py/econpizza.svg
     :target: https://badge.fury.io/py/econpizza
 
 **Econpizza** is a framework to solve and simulate *fully nonlinear* perfect foresight models, with or without heterogeneous agents.
-The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
+The package implements the solution method proposed in `HANK on Speed: Robust Nonlinear Solutions using Automatic Differentiation <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
 It allows to specify and solve nonlinear macroeconomic models quickly in a simple, high-level fashion.
 Generic and robust routines for steady state search are provided.
 
 The package can solve nonlinear models with heterogeneous agents, such as HANK models with one or two assets and portfolio choice. Steady state and nonlinear impulse responses (including, e.g., the ELB) can typically be found within a few seconds.
 The method extends the `Sequence-Space Jacobian <https://github.com/shade-econ/sequence-jacobian>`_ method (`Auclert et al., 2022, ECMA <https://doi.org/10.3982/ECTA17434>`_) to fully nonlinear heterogeneous agent models models by iteratively using `Jacobian-vector producs <https://jax.readthedocs.io/en/latest/notebooks/autodiff_cookbook.html#how-it-s-made-two-foundational-autodiff-functions>`_ to approximate the solution to the linear system of equations associated with each Newton iteration. This not only allows to study the dynamics of aggregate variables, but also the complete nonlinear transition dynamics of the cross-sectional distribution of assets and disaggregated objects.
 
 To solve models with representative agents a shooting methods similar to Laffargue (1990), Boucekkine (1995) and Juillard (1996) is implemented. It is faster and more reliable than the extended path method in dynare due to the use of automatic differentiation for the efficient jacobian decompositions during each Newton-step. Nonlinear perfect-foresight transition dynamics can - even for large-scale nonlinear models with several occassionally binding constraints - be computed in less than a second.
@@ -35,12 +35,12 @@
  * `Quickstart tutorial <https://econpizza.readthedocs.io/en/stable/tutorial/quickstart.html>`_
 
 Citation
 --------
 .. code-block:: bibtex
 
     @article{boehl2023goodpizza,
-        title       = {Robust Nonlinear Transition Dynamics in HANK},
+        title       = {HANK on Speed: Robust Nonlinear Solutions using Automatic Differentiation},
         author      = {Boehl, Gregor},
         journal     = {Available at SSRN 4433585},
         year        = {2023}
     }
```

### Comparing `econpizza-0.5.5/docs/Makefile` & `econpizza-0.5.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/docs/conf.py` & `econpizza-0.5.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/docs/guide/installation.rst` & `econpizza-0.5.6/docs/guide/installation.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 Installation
 ============
 
+The package is under active development. Stable releases can be installed from the official Python repositories, which are updated frequently. The `changelog and release history <https://github.com/gboehl/econpizza/releases>`_ can be found on GitHub.
+
 On Linux & MacOS
 ----------------
 
 Installing the `repository version <https://pypi.org/project/econpizza/>`_ from PyPi is as simple as typing
 
 .. code-block:: bash
```

### Comparing `econpizza-0.5.5/docs/guide/method.ipynb` & `econpizza-0.5.6/docs/guide/method.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/docs/guide/solution.rst` & `econpizza-0.5.6/docs/guide/solution.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 The main functionality of nonlinear simulations is provided by the function :meth:`econpizza.PizzaModel.find_path`
 The main arguments are either ``shock`` or ``init_state``, which allows to specify an economic shock as a tuple of the shock name (as specified in ``shocks`` in the YAML) and the size of the shock, or a vector of initial states, respectively.
 The function :meth:`econpizza.PizzaModel.get_distributions` allows to retrieve the full nonlinear sequence of the distribution.
 
 .. note::
 
-   All numerical methods are subject to numerical errors. To reduce these, you can decrease the numerical tolerance ``tol``. However, this should not be below the tolerance level for the steady state search, or below machine precision.
+   All numerical methods are subject to numerical errors. To reduce these, you can decrease the numerical tolerance ``tol``. However, this should not be below the tolerance level used for the steady state search.
 
 .. hint::
 
-   As stated in the paper, a sufficient condition for convergence of the solution routine is that the generalized eigenvalues of the sequence space Jacobian and its steady-state pendant are all positive (which is prohibitory expensive to check). If the method does not converge, the ``use_solid_solver=True`` flag can be used to check if the model solves when using a conventional Newton method with the true Jacobian.
+   A sufficient condition for convergence of the solution routine is that the `generalized eigenvalues <https://en.wikipedia.org/wiki/Eigendecomposition_of_a_matrix#Generalized_eigenvalue_problem>`_ of the sequence space Jacobian and its steady-state pendant are all positive. [#f1]_ If the procedure does not converge, the ``use_solid_solver=True`` flag can be used to check if the model solves when using a conventional Newton method with the true Jacobian (this may take quite a while).
 
 .. autofunction:: econpizza.PizzaModel.find_path
 
 If the model has heterogeneous agents, the routine will automatically compute the steady state sequence space Jacobian. This can be skipped using the ``skip_jacobian`` flag.
 
 Any additional argument will be passed on to the specific Newton method. For models with heterogeneous agents this is :meth:`econpizza.utilities.newton.newton_for_jvp`:
 
@@ -26,7 +26,11 @@
 .. autofunction:: econpizza.utilities.newton.newton_for_banded_jac
 
 If ``use_solid_solver`` is set to `True`, the Newton method `newton_jax_jit <https://grgrjax.readthedocs.io/en/latest/#grgrjax.newton_jax_jit>`_ from the `grgrjax <https://grgrjax.readthedocs.io>`_ package is used.
 
 The function :meth:`econpizza.PizzaModel.get_distributions` allows to retrieve the sequence of distributions and decision variables. To that end it requires the shocks and initial distribution together with the trajectory of aggregated variables as input.
 
 .. autofunction:: econpizza.PizzaModel.get_distributions
+
+.. rubric:: Footnotes
+
+.. [#f1] Unfortunately, this is prohibitory expensive to check as it would require to calculate the full sequence space Jacobian and its eigenvalues.
```

### Comparing `econpizza-0.5.5/docs/guide/steady_state.rst` & `econpizza-0.5.6/docs/guide/steady_state.rst`

 * *Files 21% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 
 Upon failure, the function tries to be as informative as possible. If the search is not successful, a possible path to find the error is to set the function's keyword argument ``raise_errors`` to ``False``. The function then raises a warning instead of failing with an exception, and returns a dictionary containing the results from the root finding routine, such as, e.g. the last Jacobian matrix.
 
 .. note::
 
    A classic complaint is "**The Jacobian contains NaNs**". This is usually due to numerical errors somewhere along the way. While the package tries to provide more information about where the error occurred, a good idea is to follow JAX's hints on `how to debug NaNs <https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#debugging-nans>`_.
 
-.. hint::
+.. tip::
 
-   A common gotcha for heterogeneous agent models is that the distribution contains negative values. The routine will be informative about that. This is usually due to too much interpolation outside the grid and can often be fixed by using a grid with larger maximum values.
-
-.. hint::
-
-   The steady state procedure is based on the pseudoinverse of the Jacobian (see the original paper). If the procedure fails, it will tell you the rank of the Jacobian and the number of degrees of freedom. More degrees of freedom than the Jacobian rank normally implies that you should fix more steady state values and vice versa.
-
-.. hint::
-
-   If the desired precision is not reached, the error message will tell you in which equation the maximum error did arise. You can use the ``equations`` key to get the list of equations (as strings), e.g. ``print(model['equations'][17])`` to get the equation with index 17.
+   * A common gotcha for heterogeneous agent models is that the distribution contains negative values. The routine will be informative about that. This is usually due to rather excessive interpolation outside the grid and can often be fixed by using a grid with larger minimum/maximum values.
+   * The steady state procedure is based on the `pseudoinverse <https://en.wikipedia.org/wiki/Moore%E2%80%93Penrose_inverse>`_ of the Jacobian. If the procedure fails, it will try to tell you the rank of the Jacobian and the number of degrees of freedom. More degrees of freedom than the Jacobian rank normally implies that you should fix more steady state values and vice versa.
+   * If the desired precision is not reached, the error message will tell you in which equation the maximum error did arise. You can use the ``equations`` key to get the list of equations (as strings), e.g. ``print(model['equations'][17])`` to get the equation with index 17.
 
 .. autofunction:: econpizza.PizzaModel.solve_stst
```

### Comparing `econpizza-0.5.5/docs/guide/the_yaml.rst` & `econpizza-0.5.6/docs/guide/the_yaml.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/docs/index.rst` & `econpizza-0.5.6/docs/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     It is synced with the online package documentation that is hosted at `Read the Docs <https://econpizza.readthedocs.io>`_.
 
 
 Overview: **Econpizza**
 -----------------------
 
 **Econpizza** is a framework to solve and simulate *fully nonlinear* perfect foresight models, with or without heterogeneous agents.
-The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
+The package implements the solution method proposed in `HANK on Speed: Robust Nonlinear Solutions using Automatic Differentiation <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
 It allows to specify and solve nonlinear macroeconomic models quickly in a simple, high-level fashion.
 
 The package builds heavily on `automatic differentiation <https://en.wikipedia.org/wiki/Automatic_differentiation>`_ via `JAX <https://jax.readthedocs.io/en/latest/notebooks/quickstart.html>`_.
 A central philosophy is to consequently separate the low-level routines for *model solution* (which is what happens under the hood) from
 *model specification* (via a ``yaml`` file) and *model analysis* (what the user does with the model).
 
 The package can solve nonlinear models with heterogeneous households or firms with one or two assets and portfolio choice. Steady state and nonlinear impulse responses (including, e.g., the ZLB) can typically be found within a few seconds.
@@ -23,12 +23,12 @@
 -----------
 
 Please cite with
 
 .. code-block:: bibtex
 
     @article{boehl2023goodpizza,
-        title       = {Robust Nonlinear Transition Dynamics in HANK},
+        title       = {HANK on Speed: Robust Nonlinear Solutions using Automatic Differentiation},
         author      = {Boehl, Gregor},
         journal     = {Available at SSRN 4433585},
         year        = {2023}
     }
```

### Comparing `econpizza-0.5.5/docs/lin_and_nlin.png` & `econpizza-0.5.6/docs/lin_and_nlin.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/docs/make.bat` & `econpizza-0.5.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/docs/p_and_n.png` & `econpizza-0.5.6/docs/p_and_n.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/docs/tutorial/boehl_hommes.rst` & `econpizza-0.5.6/docs/tutorial/boehl_hommes.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/docs/tutorial/hank1.ipynb` & `econpizza-0.5.6/docs/tutorial/hank1.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/docs/tutorial/hank2.ipynb` & `econpizza-0.5.6/docs/tutorial/hank2.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/docs/tutorial/quickstart.ipynb` & `econpizza-0.5.6/docs/tutorial/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/docs/tutorial/rank.ipynb` & `econpizza-0.5.6/docs/tutorial/rank.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/__init__.py` & `econpizza-0.5.6/econpizza/__init__.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/examples/bh.yml` & `econpizza-0.5.6/econpizza/examples/bh.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/examples/dsge.yml` & `econpizza-0.5.6/econpizza/examples/dsge.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # The model is a marriage of "A Baseline DSGE Model" (Fernández-Villaverde and Rubio-Ramírez, manuscript) and "The Empirical Implications of the Interest-Rate Lower Bound" (Gust et al., 2012 FED DP)
 # Author: Gregor Boehl [mail@gregorboehl.com]
 ---
 
 name: 'nk_capital'
 description: 'A medium scale NK model with capital, capital adjustement costs, capital utilization costs, and habits'
 variables: [ y, c, pi, R, Rn, Rk, beta, w, q, mc, k, i, n, z, eps_i, eps_u, lamda, g, b, qb, t, ds, bprof, dd, MPK, cap_util, cap_util_costs, y_prod, pitilde, piwntilde, piwn, price_markup, wage_markup, Rstar, wn, div ]
-parameters: [ theta, kappa, delta, alpha, h, psi_i, psi_p, psi_w, phi_pi, phi_y, rho, sigma_l, chi, psi_u, omega_p, omega_w, theta_w, iota_w, elb, rho_beta, rho_z, rho_g, rho_p, rho_w, rho_i, rho_r ]
+parameters: [ theta, kappa, delta, alpha, h, psi_i, psi_p, psi_w, phi_pi, phi_y, rho, sigma_l, chi, psi_u, omega_p, omega_w, theta_w, iota_w, elb, rho_beta, rho_z, rho_g, rho_p, rho_w, rho_i, rho_r, rho_u ]
 shocks: [ e_beta, e_z, e_g, e_p, e_w, e_i, e_r, e_u ]
 
 equations:
     ## households block
     ~ lamda = 1/(c - h*cLag) - h*beta/(cPrime - h*c) # stochastic discount factor
     ~ lamda = beta*eps_u*lamdaPrime*R/piPrime # Euler equation
     ~ piwn = wn/wnLag*pi # wage inflation
```

### Comparing `econpizza-0.5.5/econpizza/examples/ghls.yml` & `econpizza-0.5.6/econpizza/examples/ghls.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/examples/hank2.yml` & `econpizza-0.5.6/econpizza/examples/hank2.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/examples/hank2_functions.py` & `econpizza-0.5.6/econpizza/examples/hank2_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/examples/hank2_no_capital.yml` & `econpizza-0.5.6/econpizza/examples/hank2_no_capital.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/examples/hank_functions.py` & `econpizza-0.5.6/econpizza/examples/hank_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/examples/hank_labor.yml` & `econpizza-0.5.6/econpizza/examples/hank_labor.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/examples/hank_labor_functions.py` & `econpizza-0.5.6/econpizza/examples/hank_labor_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/examples/hank_with_comments.yml` & `econpizza-0.5.6/econpizza/examples/hank_with_comments.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/examples/nk.yml` & `econpizza-0.5.6/econpizza/examples/nk.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/examples/tank.yml` & `econpizza-0.5.6/econpizza/examples/tank.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/parser/__init__.py` & `econpizza-0.5.6/econpizza/parser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,23 +83,24 @@
     """Evaluate a dictionary of strings into a given context
     """
 
     if vdict is None:
         return None
     else:
         vdict = vdict.copy()
+    context = context.copy()
 
     for v in vdict:
         if isinstance(vdict[v], str):
             context[v] = eval(vdict[v], context)
             vdict[v] = eval(v, context)
         else:
             context[v] = vdict[v]
 
-    return vdict
+    return vdict, context
 
 
 def _parse_external_functions_file(model):
     """Parse the functions file.
     """
     try:
         # prepare path
@@ -229,22 +230,22 @@
     # remove old values from model context
     [context.pop(key) for key in par_names if key in context]
     [context.pop(key) for key in evars if key in context]
 
     # collect fixed values and ensure ordering and lenght is fine
     fixed_values = _define_subdict_if_absent(
         model["steady_state"], "fixed_values")
-    fixed_values_evaluated = _eval_strs(fixed_values, context=context)
+    fixed_values_evaluated, context = _eval_strs(fixed_values, context=context)
     fixed_values_names = tuple(
         sorted([k for k in fixed_values_evaluated if k in par_names or k in evars]))
     fixed_evaluated = {
         k: fixed_values_evaluated[k] for k in fixed_values_names}
 
     # collect initial guesses
-    init_guesses = _eval_strs(model["steady_state"].get(
+    init_guesses, context = _eval_strs(model["steady_state"].get(
         "init_guesses"), context=context)
     init_vals = _compile_init_values(
         evars, par_names, init_guesses, fixed_evaluated)
 
     # get the initial decision functions
     if model.get('distributions'):
         dist_names = list(model['distributions'].keys())
@@ -313,15 +314,17 @@
     # make it a model
     model = PizzaModel(model)
     # initialize objects
     model['context'] = _initialize_context()
     model['cache'] = _initialize_cache()
     _load_external_functions_file(model, model['context'])
 
-    # compile definitions
+    # compile globals & definitions
+    _ = _define_subdict_if_absent(model, "globals")
+    model['context'].update(model['globals'])
     defs = model.get("definitions")
     defs = '' if defs is None else defs
     defs = '\n'.join(defs) if isinstance(defs, list) else defs
     exec(defs, model['context'])
     # get aggregate equations
     eqns = model["equations"].copy()
```

### Comparing `econpizza-0.5.5/econpizza/parser/build_functions.py` & `econpizza-0.5.6/econpizza/parser/build_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/parser/checks.py` & `econpizza-0.5.6/econpizza/parser/checks.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/parser/het_agent_base_funcs.py` & `econpizza-0.5.6/econpizza/parser/het_agent_base_funcs.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/parser/write_dynamic_functions.py` & `econpizza-0.5.6/econpizza/parser/write_dynamic_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Functions that write other functions.
 """
+import re
 import jax
 from .build_functions import func_forw_generic, func_forw_stst_generic
 
 
 def compile_func_basics_str(evars, par, shocks):
 
     func_str = f"""
@@ -80,19 +81,21 @@
 
 def compile_eqn_func_str(evars, eqns, par, eqns_aux, shocks, distributions, decisions_outputs):
     """Compile all information from 'equations' section' to a string that defines the function.
     """
 
     # start compiling root_container
     for i, eqn in enumerate(eqns):
-        if "=" in eqn:
-            lhs, rhs = eqn.split("=")
-            eqns[i] = f"root_container{i} = {lhs} - ({rhs})"
-        else:
+        eqsplit = re.split("(?<!=)=(?!=)", eqn)
+        if len(eqsplit) == 1:
             eqns[i] = f"root_container{i} = {eqn}"
+        elif len(eqsplit) == 2:
+            eqns[i] = f"root_container{i} = {eqsplit[0]} - ({eqsplit[1]})"
+        else:
+            raise SyntaxError(f'More than one " = " in equation {i}: "{eqn}"')
 
     if isinstance(eqns_aux, str):
         eqns_aux = eqns_aux.splitlines()
 
     eqns_aux_stack = "\n ".join(eqns_aux) if eqns_aux else ""
     eqns_stack = "\n ".join(eqns)
```

### Comparing `econpizza-0.5.5/econpizza/solvers/shooting.py` & `econpizza-0.5.6/econpizza/solvers/shooting.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/solvers/solve_linear.py` & `econpizza-0.5.6/econpizza/solvers/solve_linear.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/solvers/solve_linear_state_space.py` & `econpizza-0.5.6/econpizza/solvers/solve_linear_state_space.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/solvers/stacking.py` & `econpizza-0.5.6/econpizza/solvers/stacking.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,38 +37,38 @@
     Parameters
     ----------
     model : PizzaModel
         PizzaModel instance
     shock : tuple, optional
         shock in period 0 as in `(shock_name_as_str, shock_size)`
     init_state : array, optional
-        tial state
+        initial state, defaults to the steady state values
     init_dist : array, optional
-        tial distribution
+        initial distribution, defaults to the steady state distribution
     pars : dict, optional
         alternative parameters. Warning: do only change those parameters that are invariant to the steady state.
     horizon : int, optional
-        number of periods until the system is assumed to be back in the steady state. Defaults to 200
+        number of periods until the system is assumed to be back in the steady state. Defaults to ``200``
     use_solid_solver : bool, optional
-        calculate the full jacobian and use a standard Newton method. Defaults to False
+        calculate the full jacobian and use a standard Newton method. Defaults to ``False``
     skip_jacobian : bool, optional
-        whether to skip the calculation of the steady state sequence space Jacobian. If True, the last cached Jacobian will be used. Defaults to False
+        whether to skip the calculation of the steady state sequence space Jacobian. If True, the last cached Jacobian will be used. Defaults to ``False``
     verbose : bool, optional
-        degree of verbosity. 0/`False` is silent
+        degree of verbosity. ``0``/``False`` is silent. Defaults to ``False``
     raise_errors : bool, optional
-        whether to raise errors as exceptions, or just inform about them. Defaults to `True`
+        whether to raise errors as exceptions, or just inform about them. Defaults to ``True``
     newton_args : optional
         any additional arguments to be passed on to the Newton solver (see the documentations of the solvers)
 
     Returns
     -------
     x : array
         array of the trajectory
     flag : bool
-        returns False if the solver was successful, else True
+        Error flag. Returns `False` if the solver was successful, otherwise returns `True`
     """
 
     st = time.time()
     # only skip jacobian calculation if it exists
     skip_jacobian = skip_jacobian if model['cache'].get(
         'jac_factorized') else False
 
@@ -104,15 +104,15 @@
                 jav_func_eqns, XSS=stst, pars=pars, distributions=[], decisions_outputs=[])
             model['context']['jav_func'] = jav_func_eqns_partial
             # mark as compiled
             write_cache(model, horizon, pars, stst)
 
         # actual newton iterations
         jav_func_eqns_partial = model['context']['jav_func']
-        x_out, flag, mess = newton_for_banded_jac(
+        x_out, f, flag, mess = newton_for_banded_jac(
             jav_func_eqns_partial, nvars, horizon, x_init, shock_series, verbose, **newton_args)
 
     else:
         if not check_if_compiled(model, horizon, pars, stst) or not model['context'].get('jvp_func'):
             # get derivatives via AD and compile functions
             zero_shocks = jnp.zeros_like(shock_series).T
             build_aggr_het_agent_funcs(model, jnp.zeros_like(
@@ -129,27 +129,27 @@
 
         # get jvp function and steady state jacobian
         jvp_partial = jax.tree_util.Partial(
             model['context']['jvp_func'], x0=x0, dist0=dist0, shocks=shock_series.T, pars=pars)
         if not use_solid_solver:
             jacobian = model['cache']['jac_factorized']
             # actual newton iterations
-            x, flag, mess = newton_for_jvp(
+            x, f, flag, mess = newton_for_jvp(
                 jvp_partial, jacobian, x_init, verbose, **newton_args)
         else:
             # define function returning value and jacobian calculated in slices
             value_and_jac_func = get_jac_and_value_sliced(
                 (horizon-1)*nvars, jvp_partial, newton_args)
-            x, flag, mess = newton_jax_jit_wrapper(
+            x, f, flag, mess = newton_jax_jit_wrapper(
                 value_and_jac_func, x_init[1:-1].flatten(), **newton_args)
         x_out = x_init.at[1:-1].set(x.reshape((horizon - 1, nvars)))
 
     # some informative print messages
     duration = time.time() - st
     result = 'done' if not flag else 'FAILED'
     mess = f"(find_path:) Stacking {result} ({duration:1.3f}s). " + mess
     if flag and raise_errors:
         raise Exception(mess)
     elif verbose:
         print(mess)
 
-    return x_out, flag
+    return x_out, (flag, f)
```

### Comparing `econpizza-0.5.5/econpizza/solvers/steady_state.py` & `econpizza-0.5.6/econpizza/solvers/steady_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,23 +52,23 @@
     Parameters
     ----------
     model : PizzaModel
         PizzaModel instance
     tol : float, optional
         tolerance of the Newton method, defaults to ``1e-8``
     maxit : int, optional
-        maximum of iterations for the Newton method, defaults to 15
+        maximum of iterations for the Newton method, defaults to ``15``
     tol_backwards : float, optional
         tolerance required for backward iteration. Defaults to ``tol``
     maxit_backwards : int, optional
-        maximum of iterations for the backward iteration. Defaults to 2000
+        maximum of iterations for the backward iteration. Defaults to ``2000``
     tol_forwards : float, optional
         tolerance required for forward iteration. Defaults to ``tol*1e-2``
     maxit_forwards : int, optional
-        maximum of iterations for the forward iteration. Defaults to 5000
+        maximum of iterations for the forward iteration. Defaults to ``5000``
     force : bool, optional
         force recalculation of steady state, even if it is already evaluated. Defaults to ``False``
     raise_errors : bool, optional
         raise an error if Newton method does not converge. Useful for debuggin models. Defaults to ``True``
     check_rank : bool, optional
         force checking the rank of the Jacobian, even if the Newton method was successful. Defualts to ``False``
     verbose : bool, optional
```

### Comparing `econpizza-0.5.5/econpizza/testing/cache/bh.npy` & `econpizza-0.5.6/econpizza/testing/cache/bh.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/testing/cache/hank_labor.npy` & `econpizza-0.5.6/econpizza/testing/cache/hank_labor.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/testing/cache/hank_solid.npy` & `econpizza-0.5.6/econpizza/testing/cache/hank_solid.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/testing/test_rest.py` & `econpizza-0.5.6/econpizza/testing/test_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     shocks = ('e_beta', .005)
 
     x, flag = mod.find_path(shocks, horizon=50)
 
     path = os.path.join(filepath, "cache", "hank_labor.npy")
 
-    assert flag == 0
+    assert flag[0] == 0
     if create:
         jnp.save(path, x)
         print(f'Test file updated at {path}')
     else:
         test_x = jnp.load(path)
         assert jnp.allclose(x, test_x)
 
@@ -63,15 +63,15 @@
     shocks = ('e_beta', .005)
 
     x, flag = mod.find_path(shocks, use_solid_solver=True,
                             horizon=20, chunk_size=90)
 
     path = os.path.join(filepath, "cache", "hank_solid.npy")
 
-    assert flag == 0
+    assert flag[0] == 0
     if create:
         jnp.save(path, x)
         print(f'Test file updated at {path}')
     else:
         test_x = jnp.load(path)
         assert jnp.allclose(x, test_x)
```

### Comparing `econpizza-0.5.5/econpizza/tools.py` & `econpizza-0.5.6/econpizza/tools.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/utilities/dists.py` & `econpizza-0.5.6/econpizza/utilities/dists.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/utilities/grids.py` & `econpizza-0.5.6/econpizza/utilities/grids.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/utilities/interp.py` & `econpizza-0.5.6/econpizza/utilities/interp.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/utilities/jacobian.py` & `econpizza-0.5.6/econpizza/utilities/jacobian.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/econpizza/utilities/newton.py` & `econpizza-0.5.6/econpizza/utilities/newton.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,20 +40,21 @@
     f = lu_solve(*jacobian[0], f, 0)[jacobian[1]]
     # other iterations
     iteration_tol = jnp.minimum(1e-5, 1e-1*amax(f))
     init = ((f, 1., 0), (x, f, jvp_func, jacobian, factor),
             (1e8, iteration_tol, nsteps))
     (y, dampening, fev_inner), _, (err_inner, _, _) = jax.lax.while_loop(
         iteration_cond, iteration_step, init)
-    return (x-y, amax(f), dampening, cnt+1, fev+fev_inner, err_inner), (jvp_func, jacobian, maxit, nsteps, tol, factor, verbose)
+    return (x-y, f, dampening, cnt+1, fev+fev_inner, err_inner), (jvp_func, jacobian, maxit, nsteps, tol, factor, verbose)
 
 
 def jvp_while_cond(carry):
-    (_, err, dampening, cnt, fev, err_inner), (_,
-                                               _, maxit, nsteps, tol, _, verbose) = carry
+    (_, f, dampening, cnt, fev, err_inner), (_,
+                                             _, maxit, nsteps, tol, _, verbose) = carry
+    err = amax(f)
     cond = jnp.logical_and(err > tol, cnt < maxit)
     verbose = jnp.logical_and(cond, verbose)
     verbose = jnp.logical_and(fev, verbose)
     jax.debug.callback(callback_with_damp, cnt, err, fev=fev,
                        err_inner=err_inner, dampening=dampening, ltime=None, verbose=verbose)
     return cond
 
@@ -103,25 +104,26 @@
     factor : float, optional
         dampening factor (gamma in the paper), Defaults to 1.5
     """
 
     start_time = time.time()
     x = x_init[1:-1].flatten()
 
-    (x, err, dampening, cnt, fev, err_inner), _ = jax.lax.while_loop(jvp_while_cond, jvp_while_body,
-                                                                     ((x, 1., 0., 0, 0, 0), (jvp_func, jacobian, maxit, nsteps, tol, factor, verbose)))
+    (x, f, dampening, cnt, fev, err_inner), _ = jax.lax.while_loop(jvp_while_cond, jvp_while_body,
+                                                                   ((x, x, 0., 0, 0, 0), (jvp_func, jacobian, maxit, nsteps, tol, factor, verbose)))
+    err = amax(f)
     ltime = time.time() - start_time
     callback_with_damp(cnt, err, fev=fev, err_inner=err_inner,
                        dampening=dampening, ltime=ltime, verbose=verbose)
     _, (success, mess) = check_status(err, cnt, maxit, tol)
     # compile error/report message
     if not success and not jnp.isnan(err):
         mess += f" Max. error is {err:1.2e}."
 
-    return x, not success, mess
+    return x, f, not success, mess
 
 
 def newton_for_banded_jac(jav_func, nvars, horizon, X, shocks, verbose, maxit=30, tol=1e-8):
     """Newton solver for representative agents models.
 
     Parameters
     ----------
@@ -154,15 +156,15 @@
         do_break, (success, mess) = check_status(err, cnt, maxit, tol)
         if do_break:
             break
 
     if not success:
         mess += f" Max. error is {err:1.2e}."
 
-    return X, not success, mess
+    return X, out, not success, mess
 
 
 def newton_jax_jit_wrapper(func, init, **args):
     """Wrapper around grgrjax.newton.newton_jax_jit. Returns correct flags and messages.
     """
 
     if 'tol' not in args:
@@ -174,8 +176,8 @@
     err = amax(f)
     _, (success, mess) = check_status(err, cnt, args['maxit'], args['tol'])
     flag |= not success
 
     # compile error/report message
     if not success and not jnp.isnan(err):
         mess += f" Max. error is {err:1.2e}."
-    return x, flag, mess
+    return x, f, flag, mess
```

### Comparing `econpizza-0.5.5/econpizza.egg-info/PKG-INFO` & `econpizza-0.5.6/econpizza.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.5.5
+Version: 0.5.6
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
     :target: https://github.com/gboehl/econpizza/actions
 .. image:: https://readthedocs.org/projects/econpizza/badge/?version=latest
     :target: http://econpizza.readthedocs.io/en/latest/?badge=latest
 .. image:: https://badge.fury.io/py/econpizza.svg
     :target: https://badge.fury.io/py/econpizza
 
 **Econpizza** is a framework to solve and simulate *fully nonlinear* perfect foresight models, with or without heterogeneous agents.
-The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
+The package implements the solution method proposed in `HANK on Speed: Robust Nonlinear Solutions using Automatic Differentiation <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
 It allows to specify and solve nonlinear macroeconomic models quickly in a simple, high-level fashion.
 Generic and robust routines for steady state search are provided.
 
 The package can solve nonlinear models with heterogeneous agents, such as HANK models with one or two assets and portfolio choice. Steady state and nonlinear impulse responses (including, e.g., the ELB) can typically be found within a few seconds.
 The method extends the `Sequence-Space Jacobian <https://github.com/shade-econ/sequence-jacobian>`_ method (`Auclert et al., 2022, ECMA <https://doi.org/10.3982/ECTA17434>`_) to fully nonlinear heterogeneous agent models models by iteratively using `Jacobian-vector producs <https://jax.readthedocs.io/en/latest/notebooks/autodiff_cookbook.html#how-it-s-made-two-foundational-autodiff-functions>`_ to approximate the solution to the linear system of equations associated with each Newton iteration. This not only allows to study the dynamics of aggregate variables, but also the complete nonlinear transition dynamics of the cross-sectional distribution of assets and disaggregated objects.
 
 To solve models with representative agents a shooting methods similar to Laffargue (1990), Boucekkine (1995) and Juillard (1996) is implemented. It is faster and more reliable than the extended path method in dynare due to the use of automatic differentiation for the efficient jacobian decompositions during each Newton-step. Nonlinear perfect-foresight transition dynamics can - even for large-scale nonlinear models with several occassionally binding constraints - be computed in less than a second.
@@ -50,12 +50,12 @@
  * `Quickstart tutorial <https://econpizza.readthedocs.io/en/stable/tutorial/quickstart.html>`_
 
 Citation
 --------
 .. code-block:: bibtex
 
     @article{boehl2023goodpizza,
-        title       = {Robust Nonlinear Transition Dynamics in HANK},
+        title       = {HANK on Speed: Robust Nonlinear Solutions using Automatic Differentiation},
         author      = {Boehl, Gregor},
         journal     = {Available at SSRN 4433585},
         year        = {2023}
     }
```

### Comparing `econpizza-0.5.5/econpizza.egg-info/SOURCES.txt` & `econpizza-0.5.6/econpizza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.5/setup.py` & `econpizza-0.5.6/setup.py`

 * *Files identical despite different names*

