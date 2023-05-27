# Comparing `tmp/jsmetrics-0.1.1b0.tar.gz` & `tmp/jsmetrics-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsmetrics-0.1.1b0.tar", last modified: Tue Apr 11 16:09:24 2023, max compression
+gzip compressed data, was "jsmetrics-0.1.2a0.tar", last modified: Sat May 27 11:23:57 2023, max compression
```

## Comparing `jsmetrics-0.1.1b0.tar` & `jsmetrics-0.1.2a0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.548435 jsmetrics-0.1.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-04-11 16:09:24.548435 jsmetrics-0.1.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.540434 jsmetrics-0.1.1b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.536434 jsmetrics-0.1.1b0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.540434 jsmetrics-0.1.1b0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)  1519071 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
--rw-r--r--   0 runner    (1001) docker     (123)   788211 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/_static/images/jet_shift_violin.png
--rw-r--r--   0 runner    (1001) docker     (123)    87261 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/_static/images/kuang_jet_centers.png
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/statement.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.540434 jsmetrics-0.1.1b0/jsmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.544435 jsmetrics-0.1.1b0/jsmetrics/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/core/check_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/details_for_all_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.544435 jsmetrics-0.1.1b0/jsmetrics/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/jet_core_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/jet_core_algorithms_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    22290 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/jet_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/jet_statistics_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/waviness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/metrics/waviness_metrics_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.544435 jsmetrics-0.1.1b0/jsmetrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/utils/spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/jsmetrics/utils/windspeed_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.544435 jsmetrics-0.1.1b0/jsmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 16:09:24.000000 jsmetrics-0.1.1b0/jsmetrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-11 16:09:24.552435 jsmetrics-0.1.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.544435 jsmetrics-0.1.1b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.548435 jsmetrics-0.1.1b0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1262096 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1260860 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1104721 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.548435 jsmetrics-0.1.1b0/tests/metric_verification/
--rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/metric_verification/metric_verification.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:09:24.548435 jsmetrics-0.1.1b0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_jet_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_jet_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_waviness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-11 16:09:21.000000 jsmetrics-0.1.1b0/tests/unit/test_windspeed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12787 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.116666 jsmetrics-0.1.2a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.112666 jsmetrics-0.1.2a0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.116666 jsmetrics-0.1.2a0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  1083764 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png
+-rw-r--r--   0 runner    (1001) docker     (123)   279496 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1519071 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
+-rw-r--r--   0 runner    (1001) docker     (123)   788211 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/jet_shift_violin.png
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/statement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.116666 jsmetrics-0.1.2a0/jsmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/core/check_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/details_for_all_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22302 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42201 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/spatial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/windspeed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1262096 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1260860 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1104721 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/tests/metric_verification/
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/metric_verification/metric_verification.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_jet_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_jet_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_spatial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_waviness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_windspeed_utils.py
```

### Comparing `jsmetrics-0.1.1b0/CONTRIBUTING.rst` & `jsmetrics-0.1.2a0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/HISTORY.rst` & `jsmetrics-0.1.2a0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 =======
 History
 =======
 
+
+0.1.2-alpha (2023-05-27)
+-------------------------
+* Add check for NoLeapDatetime
+
+
+0.1.1 (2023-05-26)
+-------------------------
+* Fix Woollings et al. 2010 and filter windows to use day timeunits for window to stop it removing too much data.
+* Add data util function to add number of days to 360Day Datetime type
+
 0.1.1-beta (2023-04-07)
 -------------------------
 * add parameter for Kerr et al. 2020
 * Add Ceppi et al jet speed adaptation from Screen et al. 2022
 * Add fix for sort_xarray_data_coords so it works when only one coord value in coordinate (i.e. so each metric can work when only one longitude)
 * Supress warning for quadratic func
```

### Comparing `jsmetrics-0.1.1b0/LICENSE` & `jsmetrics-0.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/PKG-INFO` & `jsmetrics-0.1.2a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsmetrics
-Version: 0.1.1b0
+Version: 0.1.2a0
 Summary: Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray.
 Home-page: https://github.com/Thomasjkeel/jsmetrics
 Author: Thomas Keel
 Author-email: thomas.keel.18@ucl.ac.uk
 License: MIT License
 Keywords: jet-stream climate metrics algorithms xarray
 Platform: UNKNOWN
@@ -30,68 +30,95 @@
 ============================================
 
 |pypi| |pre-commit| |codefactor| |coveralls| |docs| |license| |black| |zenodo|  
 ------------------------------------------------------------------------------
 
 This is jsmetrics, a package containing implementations of various metrics and algorithms for identifying or characterising jet-streams
 written in Python and built from xarray.
-*WORK IN PROGRESS*
 
 .. WRITE WHY JET-STREAM (maybe in blog, maybe in readme) -> heatwaves, beast from the east, climate proxy (put it all down)
 .. At the foundation of studies that look at jet-streams is the metric used to describe or characterise it.
 
 .. WRITE CURRENT PROGRESS WITH MODULDE in highlighted section near the top of this readme 
 
 The philosophy of this package was to keep the methodology of each metric as close as possible to the given research paper's description of it (if not exact),
 *but* to not limit the method to a given:
-- time period,  
-- time unit (i.e. day, month, DJF),  
-- latitude/longitude resolution,  
-- latitude/longitude region (where possible),  
-- pressure level height.  
 
-All of these can be handled user-side.
+        * time period,  
+        * time unit (i.e. day, month, DJF),  
+        * latitude/longitude resolution,  
+        * region (where possible),  
+        * pressure level height.  
+
+All can be handled user-side.
 
 .. 
         ALSO all algorithms have been broken down into various components and these components are not coupled to a given methodology.
         As such each can be used seperately and this allows users to rebuilt aspects of a methodology (e.g. to replace a filtering method)
 
 
 Installation 
 -------------
 .. code-block:: bash
     
     pip install jsmetrics
+
+Let me know if you have any problems installing this package, as I have not extensively tested for Mac-OS and Windows versions. 
     
 Documentation
 -------------
 The official documentation is at https://jsmetrics.readthedocs.io/en/latest/  
 
 My email is: thomas.keel.18@ucl.ac.uk
 
 Usage
 -------------
 .. code-block:: python
 
-    import xarray as xr
-    import jsmetrics
+ import xarray as xr
+ import jsmetrics
+
+ # load windspeed data with u- and v- component wind.
+ uv_data = xr.open_dataset(filename)
+
+ # run Woollings et al. 2010 metric
+ w10 = jsmetrics.jet_statistics.woollings_et_al_2010(uv_data)
+
+ print(w10['jet_lat'])
+ print(w10['jet_speed'])
+
+ # run Kuang et al. 2014 metric. NOTE: may take a long time after you have more than 50 time steps.
+ k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
+ print(k14['jet_center'].sel(time=0))
 
-    # load windspeed data with u- and v- component wind.
-    uv_data = xr.open_dataset(filename)
+Gallery
+-------------
+.. image:: docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
+  :width: 560
+  :align: center
+  :alt: Jet latitude circbars with errorbars
+
+*Estimation of North Pacific mean jet latitude by month with 1-stdev errorbars. Data is monthly ERA5 700-850 hPa u-wind between 1980-2020.*
 
-   # run Woollings et al. 2010 metric 
-    w10 = jsmetrics.jet_metrics.woolling_et_al_2010(uv_data)
+.. image:: docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
+  :width: 560
+  :align: center
+  :alt: Comparison of jet core algorithms during Feb 2021 Texas Cold Wave
+
+*Comparison of jet core algorithms estimation of the 6-hourly jet position. Data is 6-hourly ERA5 100-500 hPa u-v-wind.*
 
-    # run Kuang et al. 2014 metric 
-    k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
 
-.. image:: docs/_static/images/kuang_jet_centers.png
-  :width: 360
+.. image:: docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png
+  :width: 560
   :align: center
-  :alt: Kuang et al. 2014 Jet-core algorithm
+  :alt: STJ and PFJ by metric and longitude
+
+*By latitude estimation of the jet latitude of the subtropical and polar jet stream. Data is monthly ERA5 differenced-250 hPa (orange) and 700-850 hPa (blue) u-wind between 1980-2020.*
+
+
 
 DISCLAIMER
 -------------
 We have tried to replicate the various metrics based on the equations and details in the methodology as accurately as possible.
 However, in some cases, we have chosen to exclude or alter parts of the methodology which reduce the resolution of the output (i.e. grouping into season or region) with the hope to preserve the parts of the method that specifically isolate a characteristics of the jet-stream at any inputted scale.
 Again, any further subsetting is passed onto the user.
 *If data input is at a daily resolution, part of the output should also be daily resolution.*  
@@ -145,26 +172,24 @@
 
 .. 
         _also mention related references (i.e. Manney et al. )
         also Local Wave Activity (maybe martineu?)
         Gallego
 
 
-.. Contributing
-.. ------------
-.. jsmetrics is in active development.
-
-.. * If you're interested in participating in the development of jsmetrics by suggesting new features, new metrics or algorithms or report bugs, please leave us a message on the `issue tracker`_. There is also a chat room on gitter (|gitter|).
+Contributing
+------------
+jsmetrics is in active development. 
 
-.. * If you would like to contribute code or documentation (which is greatly appreciated!), check out the `Contributing Guidelines`_ before you begin!
-
-.. .. _issue tracker: https://github.com/Thomasjkeel/jsmetrics/issues
-.. .. _Contributing Guidelines: https://github.com/Thomasjkeel/jsmetrics/blob/master/.github/CONTRIBUTING.rst
+* If you're interested in participating in the development of jsmetrics by suggesting new features, new metrics or algorithms or report bugs, please leave us a message on the `issue tracker`_
 
+* If you would like to contribute code or documentation (which is greatly appreciated!), check out the `Contributing Guidelines`_ before you begin!
 
+.. _issue tracker: https://github.com/Thomasjkeel/jsmetrics/issues
+.. _Contributing Guidelines: https://jsmetrics.readthedocs.io/en/latest/contributing.html
 .. How to cite this package
 .. ------------------------
 .. If you wish to cite `jsmetrics` in a research publication, we kindly ask that you use the bibliographical reference information available through `Zenodo`
 
 
 Project To-Do's
 ---------------
@@ -202,35 +227,44 @@
 .. |codefactor| image:: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics/badge
    :target: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics
    :alt: CodeFactor
    
 .. |coveralls| image:: https://coveralls.io/repos/github/Thomasjkeel/jsmetrics/badge.svg?branch=main
    :target: https://coveralls.io/github/Thomasjkeel/jsmetrics?branch=main
 
-.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7081634.svg
-        :target: https://doi.org/10.5281/zenodo.7081634
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7974550.svg
+        :target:  https://doi.org/10.5281/zenodo.7974550
         :alt: DOI
-
 .. |docs| image:: https://readthedocs.org/projects/jsmetrics/badge/?version=latest
-    :target: https://jsmetrics.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-
+       :target: https://jsmetrics.readthedocs.io/en/latest/?badge=latest
+       :alt: Documentation Status
 .. |pypi| image:: https://img.shields.io/pypi/v/jsmetrics.svg
         :target: https://pypi.org/project/jsmetrics/
         :alt: Python Package Index Build
 
 .. .. |conda| image:: https://img.shields.io/conda/vn/conda-forge/jsmetrics.svg
 ..         :target: https://anaconda.org/conda-forge/jsmetrics
 ..         :alt: Conda-forge Build Version
 
 
 =======
 History
 =======
 
+
+0.1.2-alpha (2023-05-27)
+-------------------------
+* Add check for NoLeapDatetime
+
+
+0.1.1 (2023-05-26)
+-------------------------
+* Fix Woollings et al. 2010 and filter windows to use day timeunits for window to stop it removing too much data.
+* Add data util function to add number of days to 360Day Datetime type
+
 0.1.1-beta (2023-04-07)
 -------------------------
 * add parameter for Kerr et al. 2020
 * Add Ceppi et al jet speed adaptation from Screen et al. 2022
 * Add fix for sort_xarray_data_coords so it works when only one coord value in coordinate (i.e. so each metric can work when only one longitude)
 * Supress warning for quadratic func
```

### Comparing `jsmetrics-0.1.1b0/README.rst` & `jsmetrics-0.1.2a0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,68 +3,95 @@
 ============================================
 
 |pypi| |pre-commit| |codefactor| |coveralls| |docs| |license| |black| |zenodo|  
 ------------------------------------------------------------------------------
 
 This is jsmetrics, a package containing implementations of various metrics and algorithms for identifying or characterising jet-streams
 written in Python and built from xarray.
-*WORK IN PROGRESS*
 
 .. WRITE WHY JET-STREAM (maybe in blog, maybe in readme) -> heatwaves, beast from the east, climate proxy (put it all down)
 .. At the foundation of studies that look at jet-streams is the metric used to describe or characterise it.
 
 .. WRITE CURRENT PROGRESS WITH MODULDE in highlighted section near the top of this readme 
 
 The philosophy of this package was to keep the methodology of each metric as close as possible to the given research paper's description of it (if not exact),
 *but* to not limit the method to a given:
-- time period,  
-- time unit (i.e. day, month, DJF),  
-- latitude/longitude resolution,  
-- latitude/longitude region (where possible),  
-- pressure level height.  
 
-All of these can be handled user-side.
+        * time period,  
+        * time unit (i.e. day, month, DJF),  
+        * latitude/longitude resolution,  
+        * region (where possible),  
+        * pressure level height.  
+
+All can be handled user-side.
 
 .. 
         ALSO all algorithms have been broken down into various components and these components are not coupled to a given methodology.
         As such each can be used seperately and this allows users to rebuilt aspects of a methodology (e.g. to replace a filtering method)
 
 
 Installation 
 -------------
 .. code-block:: bash
     
     pip install jsmetrics
+
+Let me know if you have any problems installing this package, as I have not extensively tested for Mac-OS and Windows versions. 
     
 Documentation
 -------------
 The official documentation is at https://jsmetrics.readthedocs.io/en/latest/  
 
 My email is: thomas.keel.18@ucl.ac.uk
 
 Usage
 -------------
 .. code-block:: python
 
-    import xarray as xr
-    import jsmetrics
+ import xarray as xr
+ import jsmetrics
+
+ # load windspeed data with u- and v- component wind.
+ uv_data = xr.open_dataset(filename)
+
+ # run Woollings et al. 2010 metric
+ w10 = jsmetrics.jet_statistics.woollings_et_al_2010(uv_data)
+
+ print(w10['jet_lat'])
+ print(w10['jet_speed'])
+
+ # run Kuang et al. 2014 metric. NOTE: may take a long time after you have more than 50 time steps.
+ k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
+ print(k14['jet_center'].sel(time=0))
+
+Gallery
+-------------
+.. image:: docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
+  :width: 560
+  :align: center
+  :alt: Jet latitude circbars with errorbars
+
+*Estimation of North Pacific mean jet latitude by month with 1-stdev errorbars. Data is monthly ERA5 700-850 hPa u-wind between 1980-2020.*
 
-    # load windspeed data with u- and v- component wind.
-    uv_data = xr.open_dataset(filename)
+.. image:: docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
+  :width: 560
+  :align: center
+  :alt: Comparison of jet core algorithms during Feb 2021 Texas Cold Wave
 
-   # run Woollings et al. 2010 metric 
-    w10 = jsmetrics.jet_metrics.woolling_et_al_2010(uv_data)
+*Comparison of jet core algorithms estimation of the 6-hourly jet position. Data is 6-hourly ERA5 100-500 hPa u-v-wind.*
 
-    # run Kuang et al. 2014 metric 
-    k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
 
-.. image:: docs/_static/images/kuang_jet_centers.png
-  :width: 360
+.. image:: docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png
+  :width: 560
   :align: center
-  :alt: Kuang et al. 2014 Jet-core algorithm
+  :alt: STJ and PFJ by metric and longitude
+
+*By latitude estimation of the jet latitude of the subtropical and polar jet stream. Data is monthly ERA5 differenced-250 hPa (orange) and 700-850 hPa (blue) u-wind between 1980-2020.*
+
+
 
 DISCLAIMER
 -------------
 We have tried to replicate the various metrics based on the equations and details in the methodology as accurately as possible.
 However, in some cases, we have chosen to exclude or alter parts of the methodology which reduce the resolution of the output (i.e. grouping into season or region) with the hope to preserve the parts of the method that specifically isolate a characteristics of the jet-stream at any inputted scale.
 Again, any further subsetting is passed onto the user.
 *If data input is at a daily resolution, part of the output should also be daily resolution.*  
@@ -118,26 +145,24 @@
 
 .. 
         _also mention related references (i.e. Manney et al. )
         also Local Wave Activity (maybe martineu?)
         Gallego
 
 
-.. Contributing
-.. ------------
-.. jsmetrics is in active development.
+Contributing
+------------
+jsmetrics is in active development. 
 
-.. * If you're interested in participating in the development of jsmetrics by suggesting new features, new metrics or algorithms or report bugs, please leave us a message on the `issue tracker`_. There is also a chat room on gitter (|gitter|).
-
-.. * If you would like to contribute code or documentation (which is greatly appreciated!), check out the `Contributing Guidelines`_ before you begin!
-
-.. .. _issue tracker: https://github.com/Thomasjkeel/jsmetrics/issues
-.. .. _Contributing Guidelines: https://github.com/Thomasjkeel/jsmetrics/blob/master/.github/CONTRIBUTING.rst
+* If you're interested in participating in the development of jsmetrics by suggesting new features, new metrics or algorithms or report bugs, please leave us a message on the `issue tracker`_
 
+* If you would like to contribute code or documentation (which is greatly appreciated!), check out the `Contributing Guidelines`_ before you begin!
 
+.. _issue tracker: https://github.com/Thomasjkeel/jsmetrics/issues
+.. _Contributing Guidelines: https://jsmetrics.readthedocs.io/en/latest/contributing.html
 .. How to cite this package
 .. ------------------------
 .. If you wish to cite `jsmetrics` in a research publication, we kindly ask that you use the bibliographical reference information available through `Zenodo`
 
 
 Project To-Do's
 ---------------
@@ -175,22 +200,20 @@
 .. |codefactor| image:: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics/badge
    :target: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics
    :alt: CodeFactor
    
 .. |coveralls| image:: https://coveralls.io/repos/github/Thomasjkeel/jsmetrics/badge.svg?branch=main
    :target: https://coveralls.io/github/Thomasjkeel/jsmetrics?branch=main
 
-.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7081634.svg
-        :target: https://doi.org/10.5281/zenodo.7081634
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7974550.svg
+        :target:  https://doi.org/10.5281/zenodo.7974550
         :alt: DOI
-
 .. |docs| image:: https://readthedocs.org/projects/jsmetrics/badge/?version=latest
-    :target: https://jsmetrics.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-
+       :target: https://jsmetrics.readthedocs.io/en/latest/?badge=latest
+       :alt: Documentation Status
 .. |pypi| image:: https://img.shields.io/pypi/v/jsmetrics.svg
         :target: https://pypi.org/project/jsmetrics/
         :alt: Python Package Index Build
 
 .. .. |conda| image:: https://img.shields.io/conda/vn/conda-forge/jsmetrics.svg
 ..         :target: https://anaconda.org/conda-forge/jsmetrics
 ..         :alt: Conda-forge Build Version
```

### Comparing `jsmetrics-0.1.1b0/docs/Makefile` & `jsmetrics-0.1.2a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png` & `jsmetrics-0.1.2a0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/docs/_static/images/jet_shift_violin.png` & `jsmetrics-0.1.2a0/docs/_static/images/jet_shift_violin.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/docs/conf.py` & `jsmetrics-0.1.2a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/docs/index.rst` & `jsmetrics-0.1.2a0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/docs/installation.rst` & `jsmetrics-0.1.2a0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/docs/make.bat` & `jsmetrics-0.1.2a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/docs/metrics.rst` & `jsmetrics-0.1.2a0/docs/metrics.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/jsmetrics/core/check_data.py` & `jsmetrics-0.1.2a0/jsmetrics/core/check_data.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/jsmetrics/details_for_all_metrics.py` & `jsmetrics-0.1.2a0/jsmetrics/details_for_all_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/jsmetrics/metrics/jet_core_algorithms.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/jsmetrics/metrics/jet_core_algorithms_components.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms_components.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/jsmetrics/metrics/jet_statistics.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,17 +96,17 @@
     Method from Woollings et al (2010) http://dx.doi.org/10.1002/qj.625
 
     Parameters
     ----------
     data : xarray.Dataset
         Data containing u- component wind
     filter_freq : int
-        number of days in filter (default=10 timeunits)
+        number of days in filter (default=10 days)
     window_size : int
-        number of days in window for Lancoz filter (default=61 timeunits)
+        number of days in window for Lancoz filter (default=61 days)
 
     Returns
     ----------
     fourier_filtered_data : xarray.Dataset
         Data containing maximum latitudes and maximum windspeed at those lats and fourier-filtered versions of those two variables
     """
     if isinstance(data, xarray.DataArray):
@@ -299,16 +299,16 @@
             print(
                 "this metric was meant to only work on one plev, please subset plev to one value. For now taking the mean..."
             )
             data = data.mean("plev")
     data = data.mean("lon")
     if data["time"].size == 1 and "time" not in data.dims:
         data = data.expand_dims("time")
-    if not data.indexes["time"].is_monotonic:
-        raise IndexError("Data needs to have a montonic index")
+    if not data.indexes["time"].is_monotonic_increasing:
+        raise IndexError("Data needs to have a montonic increasing index")
     # Check that data can be resampled into 10 days
     if not data["time"].size == 1:
         time_step_in_data = int((data["time"][1] - data["time"][0]).dt.days)
         if time_step_in_data <= 10:
             data = data.resample(time="10D").mean()
             time_step_in_data = 10
         else:
```

### Comparing `jsmetrics-0.1.1b0/jsmetrics/metrics/jet_statistics_components.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,30 +334,72 @@
         number of days in window for Lancoz filter
 
     Returns
     ----------
     window_cons : xarray.DataArray
         Filtered zonal mean data
     """
-    if (
-        dataarray["time"].count() <= filter_freq
-        or dataarray["time"].count() <= window_size
-        or window_size <= filter_freq
-    ):
+    if window_size <= filter_freq or filter_freq <= 0 or window_size <= 0:
         raise ValueError(
-            "Time series is too short to apply %s window for Lanczos filter"
-            % (window_size)
+            "Lanczos filter frequency cannot be larger than window size and both need to be more than 0"
+        )
+
+    if not xr.infer_freq(dataarray["time"]) == "D":
+        print(
+            f"Warning: The 'apply_lanczos_filter' function was built to work on a datetime index of freq 'D'. Frequency in data is '{xr.infer_freq(dataarray['time'])}'"
         )
 
-    assert (
-        filter_freq >= 0 and window_size >= 0
-    ), "both filter_freq and window need to be more than 0"
     assert isinstance(dataarray, xr.DataArray), "Input data needs to be a data array"
 
-    lanczos_weights = calc_low_pass_weights(window_size, 1 / filter_freq)
+    try:
+        start_date = dataarray["time"].astype(np.datetime64)[0]
+        filter_end_date = start_date + np.timedelta64(
+            filter_freq, "D"
+        )  # add filter end date for check if data is outside the filter size
+        window_end_date = start_date + np.timedelta64(
+            window_size, "D"
+        )  # add window end date for check if data is outside the filter size
+        end_date = dataarray["time"].astype(np.datetime64)[-1]
+    except (ValueError, TypeError):
+        # makes assumption that if times not coerced into numpy datetime then is 360
+        start_date = dataarray["time"].values[0]
+        end_date = dataarray["time"].values[-1]
+        if not hasattr(start_date, "calendar"):
+            raise ValueError(
+                f"Error: datetime type inputted ({start_date}) cannot be coerced into numpy.datetime64 and is not in cftime format."
+            )
+        if start_date.calendar == "360_day":
+            datetime_added_func_to_use = data_utils.add_num_of_days_to_360Datetime
+        elif start_date.calendar == "noleap":
+            datetime_added_func_to_use = data_utils.add_num_of_days_to_NoLeapDatetime
+        else:
+            raise ValueError(
+                f"Error: datetime type inputted ({start_date}) cannot be coerced into numpy.datetime64 and is not in cftime format."
+            )
+        filter_end_date = datetime_added_func_to_use(
+            start_date, num_of_days_to_add=filter_freq
+        )
+        window_end_date = datetime_added_func_to_use(
+            start_date, num_of_days_to_add=window_size
+        )
+
+    # add filter day for check if data is outside the filter size
+    if window_end_date > end_date or filter_end_date > end_date:
+        raise ValueError(
+            f"Time series is too short to apply {window_size} day window for Lanczos filter frequency of {filter_freq} days"
+        )
+
+    #  As the data may not actually be in day format, it will return the number of values within window in data i.e. if in monthly format but filter window is 60, then actual filter size will be 2
+    actual_filter_freq = dataarray.sel(
+        time=slice(start_date, filter_end_date)
+    ).time.size
+    actual_window_size = dataarray.sel(
+        time=slice(start_date, window_end_date)
+    ).time.size
+    lanczos_weights = calc_low_pass_weights(actual_window_size, 1 / actual_filter_freq)
     lanczos_weights_arr = xr.DataArray(lanczos_weights, dims=["window"])
     window_cons = (
         dataarray.rolling(time=len(lanczos_weights_arr), center=True)
         .construct("window")
         .dot(lanczos_weights_arr)
     )
     return window_cons
@@ -394,15 +436,15 @@
     if not data_row.isnull().all():
         data_row = data_row.fillna(0.0)
         max_ws = data_row.where(
             np.abs(data_row) == np.abs(data_row).max(), drop=True
         ).squeeze()
         if max_ws.size > 1:
             print(
-                "'get_latitude_and_speed_where_max_ws method': Warning: more than one max value found, picking the max!"
+                "'get_latitude_and_speed_where_max_ws method': Warning: more than one max value found, picking the first occurence!"
             )
             max_ws = max_ws[0].max()
         lat_at_max = float(max_ws["lat"])
         speed_at_max = float(max_ws.data)
         return lat_at_max, speed_at_max
     else:
         return np.nan, np.nan
```

### Comparing `jsmetrics-0.1.1b0/jsmetrics/metrics/waviness_metrics.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/jsmetrics/metrics/waviness_metrics_components.py` & `jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics_components.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/jsmetrics/utils/spatial_utils.py` & `jsmetrics-0.1.2a0/jsmetrics/utils/spatial_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/jsmetrics/utils/windspeed_utils.py` & `jsmetrics-0.1.2a0/jsmetrics/utils/windspeed_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/jsmetrics.egg-info/PKG-INFO` & `jsmetrics-0.1.2a0/jsmetrics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsmetrics
-Version: 0.1.1b0
+Version: 0.1.2a0
 Summary: Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray.
 Home-page: https://github.com/Thomasjkeel/jsmetrics
 Author: Thomas Keel
 Author-email: thomas.keel.18@ucl.ac.uk
 License: MIT License
 Keywords: jet-stream climate metrics algorithms xarray
 Platform: UNKNOWN
@@ -30,68 +30,95 @@
 ============================================
 
 |pypi| |pre-commit| |codefactor| |coveralls| |docs| |license| |black| |zenodo|  
 ------------------------------------------------------------------------------
 
 This is jsmetrics, a package containing implementations of various metrics and algorithms for identifying or characterising jet-streams
 written in Python and built from xarray.
-*WORK IN PROGRESS*
 
 .. WRITE WHY JET-STREAM (maybe in blog, maybe in readme) -> heatwaves, beast from the east, climate proxy (put it all down)
 .. At the foundation of studies that look at jet-streams is the metric used to describe or characterise it.
 
 .. WRITE CURRENT PROGRESS WITH MODULDE in highlighted section near the top of this readme 
 
 The philosophy of this package was to keep the methodology of each metric as close as possible to the given research paper's description of it (if not exact),
 *but* to not limit the method to a given:
-- time period,  
-- time unit (i.e. day, month, DJF),  
-- latitude/longitude resolution,  
-- latitude/longitude region (where possible),  
-- pressure level height.  
 
-All of these can be handled user-side.
+        * time period,  
+        * time unit (i.e. day, month, DJF),  
+        * latitude/longitude resolution,  
+        * region (where possible),  
+        * pressure level height.  
+
+All can be handled user-side.
 
 .. 
         ALSO all algorithms have been broken down into various components and these components are not coupled to a given methodology.
         As such each can be used seperately and this allows users to rebuilt aspects of a methodology (e.g. to replace a filtering method)
 
 
 Installation 
 -------------
 .. code-block:: bash
     
     pip install jsmetrics
+
+Let me know if you have any problems installing this package, as I have not extensively tested for Mac-OS and Windows versions. 
     
 Documentation
 -------------
 The official documentation is at https://jsmetrics.readthedocs.io/en/latest/  
 
 My email is: thomas.keel.18@ucl.ac.uk
 
 Usage
 -------------
 .. code-block:: python
 
-    import xarray as xr
-    import jsmetrics
+ import xarray as xr
+ import jsmetrics
+
+ # load windspeed data with u- and v- component wind.
+ uv_data = xr.open_dataset(filename)
+
+ # run Woollings et al. 2010 metric
+ w10 = jsmetrics.jet_statistics.woollings_et_al_2010(uv_data)
+
+ print(w10['jet_lat'])
+ print(w10['jet_speed'])
+
+ # run Kuang et al. 2014 metric. NOTE: may take a long time after you have more than 50 time steps.
+ k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
+ print(k14['jet_center'].sel(time=0))
 
-    # load windspeed data with u- and v- component wind.
-    uv_data = xr.open_dataset(filename)
+Gallery
+-------------
+.. image:: docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
+  :width: 560
+  :align: center
+  :alt: Jet latitude circbars with errorbars
+
+*Estimation of North Pacific mean jet latitude by month with 1-stdev errorbars. Data is monthly ERA5 700-850 hPa u-wind between 1980-2020.*
 
-   # run Woollings et al. 2010 metric 
-    w10 = jsmetrics.jet_metrics.woolling_et_al_2010(uv_data)
+.. image:: docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
+  :width: 560
+  :align: center
+  :alt: Comparison of jet core algorithms during Feb 2021 Texas Cold Wave
+
+*Comparison of jet core algorithms estimation of the 6-hourly jet position. Data is 6-hourly ERA5 100-500 hPa u-v-wind.*
 
-    # run Kuang et al. 2014 metric 
-    k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
 
-.. image:: docs/_static/images/kuang_jet_centers.png
-  :width: 360
+.. image:: docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png
+  :width: 560
   :align: center
-  :alt: Kuang et al. 2014 Jet-core algorithm
+  :alt: STJ and PFJ by metric and longitude
+
+*By latitude estimation of the jet latitude of the subtropical and polar jet stream. Data is monthly ERA5 differenced-250 hPa (orange) and 700-850 hPa (blue) u-wind between 1980-2020.*
+
+
 
 DISCLAIMER
 -------------
 We have tried to replicate the various metrics based on the equations and details in the methodology as accurately as possible.
 However, in some cases, we have chosen to exclude or alter parts of the methodology which reduce the resolution of the output (i.e. grouping into season or region) with the hope to preserve the parts of the method that specifically isolate a characteristics of the jet-stream at any inputted scale.
 Again, any further subsetting is passed onto the user.
 *If data input is at a daily resolution, part of the output should also be daily resolution.*  
@@ -145,26 +172,24 @@
 
 .. 
         _also mention related references (i.e. Manney et al. )
         also Local Wave Activity (maybe martineu?)
         Gallego
 
 
-.. Contributing
-.. ------------
-.. jsmetrics is in active development.
-
-.. * If you're interested in participating in the development of jsmetrics by suggesting new features, new metrics or algorithms or report bugs, please leave us a message on the `issue tracker`_. There is also a chat room on gitter (|gitter|).
+Contributing
+------------
+jsmetrics is in active development. 
 
-.. * If you would like to contribute code or documentation (which is greatly appreciated!), check out the `Contributing Guidelines`_ before you begin!
-
-.. .. _issue tracker: https://github.com/Thomasjkeel/jsmetrics/issues
-.. .. _Contributing Guidelines: https://github.com/Thomasjkeel/jsmetrics/blob/master/.github/CONTRIBUTING.rst
+* If you're interested in participating in the development of jsmetrics by suggesting new features, new metrics or algorithms or report bugs, please leave us a message on the `issue tracker`_
 
+* If you would like to contribute code or documentation (which is greatly appreciated!), check out the `Contributing Guidelines`_ before you begin!
 
+.. _issue tracker: https://github.com/Thomasjkeel/jsmetrics/issues
+.. _Contributing Guidelines: https://jsmetrics.readthedocs.io/en/latest/contributing.html
 .. How to cite this package
 .. ------------------------
 .. If you wish to cite `jsmetrics` in a research publication, we kindly ask that you use the bibliographical reference information available through `Zenodo`
 
 
 Project To-Do's
 ---------------
@@ -202,35 +227,44 @@
 .. |codefactor| image:: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics/badge
    :target: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics
    :alt: CodeFactor
    
 .. |coveralls| image:: https://coveralls.io/repos/github/Thomasjkeel/jsmetrics/badge.svg?branch=main
    :target: https://coveralls.io/github/Thomasjkeel/jsmetrics?branch=main
 
-.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7081634.svg
-        :target: https://doi.org/10.5281/zenodo.7081634
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7974550.svg
+        :target:  https://doi.org/10.5281/zenodo.7974550
         :alt: DOI
-
 .. |docs| image:: https://readthedocs.org/projects/jsmetrics/badge/?version=latest
-    :target: https://jsmetrics.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-
+       :target: https://jsmetrics.readthedocs.io/en/latest/?badge=latest
+       :alt: Documentation Status
 .. |pypi| image:: https://img.shields.io/pypi/v/jsmetrics.svg
         :target: https://pypi.org/project/jsmetrics/
         :alt: Python Package Index Build
 
 .. .. |conda| image:: https://img.shields.io/conda/vn/conda-forge/jsmetrics.svg
 ..         :target: https://anaconda.org/conda-forge/jsmetrics
 ..         :alt: Conda-forge Build Version
 
 
 =======
 History
 =======
 
+
+0.1.2-alpha (2023-05-27)
+-------------------------
+* Add check for NoLeapDatetime
+
+
+0.1.1 (2023-05-26)
+-------------------------
+* Fix Woollings et al. 2010 and filter windows to use day timeunits for window to stop it removing too much data.
+* Add data util function to add number of days to 360Day Datetime type
+
 0.1.1-beta (2023-04-07)
 -------------------------
 * add parameter for Kerr et al. 2020
 * Add Ceppi et al jet speed adaptation from Screen et al. 2022
 * Add fix for sort_xarray_data_coords so it works when only one coord value in coordinate (i.e. so each metric can work when only one longitude)
 * Supress warning for quadratic func
```

### Comparing `jsmetrics-0.1.1b0/jsmetrics.egg-info/SOURCES.txt` & `jsmetrics-0.1.2a0/jsmetrics.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/metrics.rst
 docs/statement.rst
 docs/usage.rst
+docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png
+docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
 docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
 docs/_static/images/jet_shift_violin.png
-docs/_static/images/kuang_jet_centers.png
 jsmetrics/__init__.py
 jsmetrics/details_for_all_metrics.py
 jsmetrics.egg-info/PKG-INFO
 jsmetrics.egg-info/SOURCES.txt
 jsmetrics.egg-info/dependency_links.txt
 jsmetrics.egg-info/not-zip-safe
 jsmetrics.egg-info/requires.txt
```

### Comparing `jsmetrics-0.1.1b0/setup.cfg` & `jsmetrics-0.1.2a0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1-beta
+current_version = 0.1.2-alpha
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+).(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
```

### Comparing `jsmetrics-0.1.1b0/setup.py` & `jsmetrics-0.1.2a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = "jsmetrics"
 DESCRIPTION = "Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray."
 URL = "https://github.com/Thomasjkeel/jsmetrics"
 AUTHOR = "Thomas Keel"
 AUTHOR_EMAIL = "thomas.keel.18@ucl.ac.uk"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.1.1-beta"
+VERSION = "0.1.2-alpha"
 LICENSE = "MIT License"
 
 KEYWORDS = "jet-stream climate metrics algorithms xarray"
 
 with open("README.rst") as file:
     readme = file.read()
```

### Comparing `jsmetrics-0.1.1b0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.2a0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.2a0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.2a0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/tests/metric_verification/metric_verification.ipynb` & `jsmetrics-0.1.2a0/tests/metric_verification/metric_verification.ipynb`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/tests/unit/__init__.py` & `jsmetrics-0.1.2a0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/tests/unit/test_jet_algorithms.py` & `jsmetrics-0.1.2a0/tests/unit/test_jet_algorithms.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/tests/unit/test_jet_statistics.py` & `jsmetrics-0.1.2a0/tests/unit/test_jet_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,34 +163,34 @@
         )
         return test_sig
 
     def test_metric(self):
         tested_func = jet_statistics.woollings_et_al_2010
         result = tested_func(self.data, filter_freq=1, window_size=2)
         self.assertIsInstance(result, xr.Dataset)
-        self.assertEqual(result["ff_jet_lat"][0], 36.25)
-        self.assertEqual(result["ff_jet_speed"][0], 43.365413665771484)
+        self.assertEqual(round(float(result["ff_jet_lat"][0]), 2), 36.25)
+        self.assertEqual(round(float(result["ff_jet_speed"][0]), 2), 22.01)
         tested_func(self.data["ua"], filter_freq=1, window_size=2)
 
-    def test_apply_lancoz_filter(self):
+    def test_apply_lanczos_filter(self):
         tested_func = jet_statistics_components.apply_lanczos_filter
         test_ua = self.data["ua"]
         self.assertRaises(AssertionError, lambda: tested_func(self.data, 2, 4))
-        self.assertRaises(AssertionError, lambda: tested_func(test_ua, -2, 1))
+        self.assertRaises(ValueError, lambda: tested_func(test_ua, -2, 1))
         self.assertRaises(ValueError, lambda: tested_func(test_ua, 2, -1))
         self.assertRaises(ValueError, lambda: tested_func(test_ua, 2, 1))
         self.assertRaises(
             ValueError,
             lambda: tested_func(test_ua, test_ua["time"].count() + 2, 1),
         )
         self.assertRaises(
             ValueError,
             lambda: tested_func(test_ua, 2, test_ua["time"].count() + 1),
         )
-        self.assertEqual(float(tested_func(test_ua, 2, 4).max()), 99.514892578125)
+        self.assertEqual(round(float(tested_func(test_ua, 2, 4).max()), 2), 99.18)
 
     def test_get_latitude_and_speed_where_max_ws(self):
         tested_func = jet_statistics_components.get_latitude_and_speed_where_max_ws
         self.assertRaises(AttributeError, lambda: tested_func(["lol"]))
         tested_data = self.data["ua"].isel(plev=0, lon=0, time=0)
         self.assertEqual(tested_func(tested_data)[0], 81.25)
         self.assertEqual(tested_func(tested_data)[1], -9.87109375)
@@ -211,16 +211,16 @@
         self.data = set_up_test_u_data()
 
     def test_metric(self):
         result = jet_statistics.barnes_polvani_2013(
             self.data, filter_freq=1, window_size=2
         )
         self.assertIsInstance(result, xr.Dataset)
-        self.assertEqual(result["jet_lat"][1], 35.85)
-        self.assertEqual(round(float(result["jet_speed"][2]), 5), 33.1134)
+        self.assertEqual(round(float(result["jet_lat"][1]), 2), 35.97)
+        self.assertEqual(round(float(result["jet_speed"][2]), 2), 16.82)
         self.assertEqual(float(result["jet_width"][1]), 17.5)
 
     def test_calc_jet_width_for_one_day(self):
         test_func = jet_statistics_components.calc_jet_width_for_one_day
         self.assertTrue(
             np.isnan(test_func(self.data["ua"].isel(time=0, plev=0), 25, None))
         )
```

### Comparing `jsmetrics-0.1.1b0/tests/unit/test_spatial_utils.py` & `jsmetrics-0.1.2a0/tests/unit/test_spatial_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/tests/unit/test_waviness_metrics.py` & `jsmetrics-0.1.2a0/tests/unit/test_waviness_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.1b0/tests/unit/test_windspeed_utils.py` & `jsmetrics-0.1.2a0/tests/unit/test_windspeed_utils.py`

 * *Files identical despite different names*

