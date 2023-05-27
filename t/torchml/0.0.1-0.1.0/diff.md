# Comparing `tmp/torchml-0.0.1.tar.gz` & `tmp/torchml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchml-0.0.1.tar", last modified: Sat Apr 16 03:40:15 2022, max compression
+gzip compressed data, was "torchml-0.1.0.tar", last modified: Sat May 27 09:21:08 2023, max compression
```

## Comparing `torchml-0.0.1.tar` & `torchml-0.1.0.tar`

### file list

```diff
@@ -1,44 +1,111 @@
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.647128 torchml-0.0.1/
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.642500 torchml-0.0.1/.github/
--rw-r--r--   0 seba-1511   (501) staff       (20)      626 2022-04-16 03:36:38.000000 torchml-0.0.1/.github/pull_request_template.md
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.642702 torchml-0.0.1/.github/workflows/
--rw-r--r--   0 seba-1511   (501) staff       (20)      911 2022-04-16 03:36:38.000000 torchml-0.0.1/.github/workflows/python_unittest.yaml
--rw-r--r--   0 seba-1511   (501) staff       (20)     1825 2022-04-16 03:36:38.000000 torchml-0.0.1/.gitignore
--rw-r--r--   0 seba-1511   (501) staff       (20)      307 2022-04-16 03:36:38.000000 torchml-0.0.1/CHANGELOG.md
--rw-r--r--   0 seba-1511   (501) staff       (20)     1068 2022-04-16 03:36:38.000000 torchml-0.0.1/LICENSE
--rw-r--r--   0 seba-1511   (501) staff       (20)       84 2022-04-16 03:36:38.000000 torchml-0.0.1/MANIFEST.in
--rw-r--r--   0 seba-1511   (501) staff       (20)     1392 2022-04-16 03:36:38.000000 torchml-0.0.1/Makefile
--rw-r--r--   0 seba-1511   (501) staff       (20)      759 2022-04-16 03:40:15.647286 torchml-0.0.1/PKG-INFO
--rw-r--r--   0 seba-1511   (501) staff       (20)      291 2022-04-16 03:36:38.000000 torchml-0.0.1/README.md
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.643382 torchml-0.0.1/docs/
--rw-r--r--   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:36:38.000000 torchml-0.0.1/docs/CNAME
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.643811 torchml-0.0.1/docs/api/
--rw-r--r--   0 seba-1511   (501) staff       (20)       13 2022-04-16 03:36:38.000000 torchml-0.0.1/docs/api/index.md
--rw-r--r--   0 seba-1511   (501) staff       (20)      253 2022-04-16 03:36:38.000000 torchml-0.0.1/docs/api/utils.md
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.639504 torchml-0.0.1/docs/assets/
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.644015 torchml-0.0.1/docs/assets/css/
--rw-r--r--   0 seba-1511   (501) staff       (20)     1476 2022-04-16 03:36:38.000000 torchml-0.0.1/docs/assets/css/custom.css
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.644420 torchml-0.0.1/docs/assets/images/
--rw-r--r--   0 seba-1511   (501) staff       (20)     1150 2022-04-16 03:36:38.000000 torchml-0.0.1/docs/assets/images/favicon.ico
--rw-r--r--   0 seba-1511   (501) staff       (20)   276362 2022-04-16 03:36:38.000000 torchml-0.0.1/docs/assets/images/mypackage.png
--rw-r--r--   0 seba-1511   (501) staff       (20)      307 2022-04-16 03:36:38.000000 torchml-0.0.1/docs/changelog.md
--rw-r--r--   0 seba-1511   (501) staff       (20)      291 2022-04-16 03:36:38.000000 torchml-0.0.1/docs/index.md
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.645304 torchml-0.0.1/examples/
--rw-r--r--   0 seba-1511   (501) staff       (20)       12 2022-04-16 03:36:38.000000 torchml-0.0.1/examples/README.md
--rw-r--r--   0 seba-1511   (501) staff       (20)     2232 2022-04-16 03:36:38.000000 torchml-0.0.1/mkdocs.yml
--rw-r--r--   0 seba-1511   (501) staff       (20)      245 2022-04-16 03:36:38.000000 torchml-0.0.1/requirements-dev.txt
--rw-r--r--   0 seba-1511   (501) staff       (20)        2 2022-04-16 03:36:38.000000 torchml-0.0.1/requirements.txt
--rw-r--r--   0 seba-1511   (501) staff       (20)       38 2022-04-16 03:40:15.647654 torchml-0.0.1/setup.cfg
--rw-r--r--   0 seba-1511   (501) staff       (20)     1074 2022-04-16 03:39:18.000000 torchml-0.0.1/setup.py
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.645690 torchml-0.0.1/tests/
--rw-r--r--   0 seba-1511   (501) staff       (20)       23 2022-04-16 03:36:38.000000 torchml-0.0.1/tests/__init__.py
--rw-r--r--   0 seba-1511   (501) staff       (20)      250 2022-04-16 03:36:38.000000 torchml-0.0.1/tests/mypackage_test.py
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.646249 torchml-0.0.1/torchml/
--rw-r--r--   0 seba-1511   (501) staff       (20)       78 2022-04-16 03:36:38.000000 torchml-0.0.1/torchml/__init__.py
--rw-r--r--   0 seba-1511   (501) staff       (20)       22 2022-04-16 03:36:38.000000 torchml-0.0.1/torchml/_version.py
--rw-r--r--   0 seba-1511   (501) staff       (20)     3092 2022-04-16 03:36:38.000000 torchml-0.0.1/torchml/utils.py
-drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2022-04-16 03:40:15.646970 torchml-0.0.1/torchml.egg-info/
--rw-r--r--   0 seba-1511   (501) staff       (20)      759 2022-04-16 03:40:15.000000 torchml-0.0.1/torchml.egg-info/PKG-INFO
--rw-r--r--   0 seba-1511   (501) staff       (20)      614 2022-04-16 03:40:15.000000 torchml-0.0.1/torchml.egg-info/SOURCES.txt
--rw-r--r--   0 seba-1511   (501) staff       (20)        1 2022-04-16 03:40:15.000000 torchml-0.0.1/torchml.egg-info/dependency_links.txt
--rw-r--r--   0 seba-1511   (501) staff       (20)       14 2022-04-16 03:40:15.000000 torchml-0.0.1/torchml.egg-info/top_level.txt
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.365820 torchml-0.1.0/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.347323 torchml-0.1.0/.github/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      626 2022-09-19 06:11:14.000000 torchml-0.1.0/.github/pull_request_template.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.347616 torchml-0.1.0/.github/workflows/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      922 2022-09-19 06:11:14.000000 torchml-0.1.0/.github/workflows/python_unittest.yaml
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1906 2023-05-27 03:09:03.000000 torchml-0.1.0/.gitignore
+-rw-r--r--   0 seba-1511   (501) staff       (20)      795 2023-05-27 09:18:28.000000 torchml-0.1.0/CHANGELOG.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1068 2022-09-19 06:11:14.000000 torchml-0.1.0/LICENSE
+-rw-r--r--   0 seba-1511   (501) staff       (20)       84 2022-09-19 06:11:14.000000 torchml-0.1.0/MANIFEST.in
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1535 2023-05-27 09:05:46.000000 torchml-0.1.0/Makefile
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2228 2023-05-27 09:21:08.365931 torchml-0.1.0/PKG-INFO
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1821 2023-05-27 09:16:12.000000 torchml-0.1.0/README.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.348650 torchml-0.1.0/docs/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2022-09-19 06:11:14.000000 torchml-0.1.0/docs/CNAME
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.350581 torchml-0.1.0/docs/api/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      168 2023-05-27 08:58:04.000000 torchml-0.1.0/docs/api/decomposition.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      404 2023-05-27 06:30:46.000000 torchml-0.1.0/docs/api/discriminant_analysis.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)       11 2022-09-19 06:11:14.000000 torchml-0.1.0/docs/api/index.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      181 2023-05-27 05:50:05.000000 torchml-0.1.0/docs/api/kernel_approximations.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      341 2022-11-04 22:00:53.000000 torchml-0.1.0/docs/api/linear_model.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      137 2022-11-04 22:00:53.000000 torchml-0.1.0/docs/api/naive_bayes.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      402 2022-11-04 22:00:53.000000 torchml-0.1.0/docs/api/neighbors.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.343005 torchml-0.1.0/docs/assets/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.351206 torchml-0.1.0/docs/assets/css/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1476 2022-09-19 06:11:14.000000 torchml-0.1.0/docs/assets/css/custom.css
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.353526 torchml-0.1.0/docs/assets/images/
+-rw-rw-r--   0 seba-1511   (501) staff       (20)     9908 2023-05-27 10:21:24.000000 torchml-0.1.0/docs/assets/images/android-chrome-192x192.png
+-rw-rw-r--   0 seba-1511   (501) staff       (20)    34692 2023-05-27 10:21:24.000000 torchml-0.1.0/docs/assets/images/android-chrome-512x512.png
+-rw-rw-r--   0 seba-1511   (501) staff       (20)     9100 2023-05-27 10:21:24.000000 torchml-0.1.0/docs/assets/images/apple-touch-icon.png
+-rw-rw-r--   0 seba-1511   (501) staff       (20)      508 2023-05-27 10:21:24.000000 torchml-0.1.0/docs/assets/images/favicon-16x16.png
+-rw-rw-r--   0 seba-1511   (501) staff       (20)     1077 2023-05-27 10:21:24.000000 torchml-0.1.0/docs/assets/images/favicon-32x32.png
+-rw-rw-r--   0 seba-1511   (501) staff       (20)    15406 2023-05-27 10:21:24.000000 torchml-0.1.0/docs/assets/images/favicon.ico
+-rw-r--r--   0 seba-1511   (501) staff       (20)    39012 2023-05-27 03:20:01.000000 torchml-0.1.0/docs/assets/images/torchml-icon.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)    44200 2023-05-27 03:13:04.000000 torchml-0.1.0/docs/assets/images/torchml-logo.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)      742 2023-05-27 09:16:52.000000 torchml-0.1.0/docs/changelog.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1128 2022-11-04 22:00:53.000000 torchml-0.1.0/docs/getting_start.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1821 2023-05-27 09:16:52.000000 torchml-0.1.0/docs/index.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.355530 torchml-0.1.0/docs/tutorials/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2766 2022-11-04 22:25:47.000000 torchml-0.1.0/docs/tutorials/gaussian_nb.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4508 2023-05-27 03:09:03.000000 torchml-0.1.0/docs/tutorials/linear_model.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3751 2023-05-27 07:37:11.000000 torchml-0.1.0/docs/tutorials/nearest_centroid.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5664 2023-05-27 07:35:26.000000 torchml-0.1.0/docs/tutorials/neighbors.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.355834 torchml-0.1.0/examples/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       12 2022-09-19 06:11:14.000000 torchml-0.1.0/examples/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2614 2023-05-27 06:35:07.000000 torchml-0.1.0/mkdocs.yml
+-rw-r--r--   0 seba-1511   (501) staff       (20)      321 2023-05-27 05:50:05.000000 torchml-0.1.0/requirements-dev.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)        1 2022-09-19 06:11:14.000000 torchml-0.1.0/requirements.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)       38 2023-05-27 09:21:08.366231 torchml-0.1.0/setup.cfg
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1086 2022-11-04 22:00:53.000000 torchml-0.1.0/setup.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.356122 torchml-0.1.0/tests/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       23 2022-09-19 06:11:14.000000 torchml-0.1.0/tests/__init__.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.356398 torchml-0.1.0/tests/unit/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:09:03.000000 torchml-0.1.0/tests/unit/__init__.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.356613 torchml-0.1.0/tests/unit/discriminant_analysis/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2023-05-27 06:30:46.000000 torchml-0.1.0/tests/unit/discriminant_analysis/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2527 2023-05-27 08:58:04.000000 torchml-0.1.0/tests/unit/discriminant_analysis/linear_discriminant_analysis_test.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.357030 torchml-0.1.0/tests/unit/gaussian_naive_bayes/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2022-11-04 22:00:53.000000 torchml-0.1.0/tests/unit/gaussian_naive_bayes/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1040 2023-05-27 08:58:04.000000 torchml-0.1.0/tests/unit/gaussian_naive_bayes/gaussian_nb_test.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.357468 torchml-0.1.0/tests/unit/kernel_approximations/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2023-05-27 05:50:05.000000 torchml-0.1.0/tests/unit/kernel_approximations/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2899 2023-05-27 05:50:05.000000 torchml-0.1.0/tests/unit/kernel_approximations/rbfsampler_test.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.358377 torchml-0.1.0/tests/unit/linear_model/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2022-09-19 06:11:14.000000 torchml-0.1.0/tests/unit/linear_model/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4275 2023-05-27 08:58:04.000000 torchml-0.1.0/tests/unit/linear_model/lasso_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1335 2023-05-27 08:58:04.000000 torchml-0.1.0/tests/unit/linear_model/linear_regression_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2356 2023-05-27 08:58:04.000000 torchml-0.1.0/tests/unit/linear_model/ridge_test.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.359126 torchml-0.1.0/tests/unit/neighbors/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2022-09-19 06:11:14.000000 torchml-0.1.0/tests/unit/neighbors/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1949 2023-05-27 08:58:04.000000 torchml-0.1.0/tests/unit/neighbors/k_neighbors_classifier_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1328 2023-05-27 08:58:04.000000 torchml-0.1.0/tests/unit/neighbors/nearest_centroids_test.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1911 2023-05-27 08:58:04.000000 torchml-0.1.0/tests/unit/neighbors/nearest_neighbors_test.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.359451 torchml-0.1.0/tests/unit/pca/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2023-05-27 08:58:04.000000 torchml-0.1.0/tests/unit/pca/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      660 2023-05-27 08:58:04.000000 torchml-0.1.0/tests/unit/pca/pca_test.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.359747 torchml-0.1.0/tests/unit/quadratic_discriminant_analysis/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2023-05-27 06:30:46.000000 torchml-0.1.0/tests/unit/quadratic_discriminant_analysis/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2366 2023-05-27 08:58:04.000000 torchml-0.1.0/tests/unit/quadratic_discriminant_analysis/quadratic_discriminant_analysis_test.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.360300 torchml-0.1.0/torchml/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      235 2023-05-27 08:58:04.000000 torchml-0.1.0/torchml/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)       22 2023-05-27 08:45:12.000000 torchml-0.1.0/torchml/_version.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      431 2022-11-04 22:00:53.000000 torchml-0.1.0/torchml/base.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.361606 torchml-0.1.0/torchml/decomposition/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       21 2023-05-27 08:58:04.000000 torchml-0.1.0/torchml/decomposition/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3826 2023-05-27 08:58:04.000000 torchml-0.1.0/torchml/decomposition/pca.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.362294 torchml-0.1.0/torchml/discriminant_analysis/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      144 2023-05-27 06:30:46.000000 torchml-0.1.0/torchml/discriminant_analysis/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9416 2023-05-27 08:58:04.000000 torchml-0.1.0/torchml/discriminant_analysis/linear_discriminant_analysis.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7715 2023-05-27 08:58:04.000000 torchml-0.1.0/torchml/discriminant_analysis/quadratic_discriminant_analysis.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.362757 torchml-0.1.0/torchml/kernel_approximations/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       35 2023-05-27 05:50:05.000000 torchml-0.1.0/torchml/kernel_approximations/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3764 2023-05-27 05:50:05.000000 torchml-0.1.0/torchml/kernel_approximations/rbfsampler.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.363741 torchml-0.1.0/torchml/linear_model/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       98 2022-11-04 22:00:53.000000 torchml-0.1.0/torchml/linear_model/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4607 2023-05-27 08:58:04.000000 torchml-0.1.0/torchml/linear_model/lasso.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2227 2023-05-27 08:14:46.000000 torchml-0.1.0/torchml/linear_model/linear_regression.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3639 2023-05-27 08:58:04.000000 torchml-0.1.0/torchml/linear_model/ridge.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.364189 torchml-0.1.0/torchml/naive_bayes/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       45 2022-11-04 22:00:53.000000 torchml-0.1.0/torchml/naive_bayes/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4986 2022-11-04 22:00:53.000000 torchml-0.1.0/torchml/naive_bayes/gaussian_naive_bayes.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.365618 torchml-0.1.0/torchml/neighbors/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      153 2022-11-04 22:00:53.000000 torchml-0.1.0/torchml/neighbors/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9936 2023-05-27 08:58:04.000000 torchml-0.1.0/torchml/neighbors/k_neighbors_classifier.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4011 2023-05-27 08:58:04.000000 torchml-0.1.0/torchml/neighbors/nearest_centroid.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5173 2022-11-04 22:00:53.000000 torchml-0.1.0/torchml/neighbors/nearest_neighbors.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-05-27 09:21:08.361225 torchml-0.1.0/torchml.egg-info/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2228 2023-05-27 09:21:08.000000 torchml-0.1.0/torchml.egg-info/PKG-INFO
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2701 2023-05-27 09:21:08.000000 torchml-0.1.0/torchml.egg-info/SOURCES.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)        1 2023-05-27 09:21:08.000000 torchml-0.1.0/torchml.egg-info/dependency_links.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)       30 2023-05-27 09:21:08.000000 torchml-0.1.0/torchml.egg-info/requires.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)       14 2023-05-27 09:21:08.000000 torchml-0.1.0/torchml.egg-info/top_level.txt
```

### Comparing `torchml-0.0.1/.github/pull_request_template.md` & `torchml-0.1.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `torchml-0.0.1/.github/workflows/python_unittest.yaml` & `torchml-0.1.0/.github/workflows/python_unittest.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -21,13 +21,13 @@
               with:
                 python-version: ${{ matrix.python }}
                 architecture: x64
             - name: Install Dependencies
               run: |
                   python3 --version
                   python3 -m pip install -U pip
-                  pip3 install requests
-                  make dev
+                  pip3 install requests pycodestyle
+                  make ci
             - name: Lint Code
               run: make lint
             - name: Run Tests
               run: make tests
```

### Comparing `torchml-0.0.1/.gitignore` & `torchml-0.1.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -126,7 +126,13 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # Custom
 docs/mkdocs.yml
+log_install.txt
+.vscode/
+.idea/
+.all_objects.cache.DS_Store
+.DS_Store
+data/MNIST
```

### Comparing `torchml-0.0.1/LICENSE` & `torchml-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchml-0.0.1/Makefile` & `torchml-0.1.0/Makefile`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 
 .PHONY: *
 
 # Admin
 dev:
-	pip install --progress-bar off -r requirements.txt >> log_install.txt
+	pip install -e .
+	pip install -r requirements-dev.txt
+
+ci:
+	pip install --progress-bar off -r requirements-dev.txt >> log_install.txt
 	python setup.py develop
 
 lint:
-	pycodestyle mypackage/ --max-line-length=160
+	pycodestyle torchml/ --max-line-length=160 --ignore=E501
 
 lint-examples:
 	pycodestyle examples/ --max-line-length=80
 
 lint-tests:
 	pycodestyle tests/ --max-line-length=180
 
@@ -26,25 +30,31 @@
 	MKL_NUM_THREADS=1 \
 	python -W ignore -m unittest discover -s 'tests' -p '*_test_notravis.py' -v
 
 alltests: 
 	rm -f alltests.txt
 	make tests >>alltests.txt 2>&1
 	make notravis-tests >>alltests.txt 2>&1
-
+	
 predocs:
 	cp ./README.md docs/index.md
 	cp ./CHANGELOG.md docs/changelog.md
 
 docs: predocs
 	mkdocs serve
 
 docs-deploy: predocs
 	mkdocs gh-deploy
 
+format:
+	black .
+	make lint
+	make lint-examples
+	make lint-tests
+
 # https://dev.to/neshaz/a-tutorial-for-tagging-releases-in-git-147e
 release:
 	echo 'Do not forget to bump the CHANGELOG.md'
 	echo 'Tagging v'$(shell python -c 'print(open("mypackage/_version.py").read()[15:-2])')
 	sleep 3
 	git tag -a v$(shell python -c 'print(open("mypackage/_version.py").read()[15:-2])')
 	git push origin --tags
```

### Comparing `torchml-0.0.1/docs/assets/css/custom.css` & `torchml-0.1.0/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `torchml-0.0.1/mkdocs.yml` & `torchml-0.1.0/mkdocs.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 
 nav:
   - Home: index.md
   - Documentation:
-    - mypackage: api/index.md
-    - mypackage.utils: api/utils.md
+    - torchml.linear_model: api/linear_model.md
+    - torchml.naive_bayes: api/naive_bayes.md
+    - torchml.neighbors: api/neighbors.md
+    - torchml.discriminant_analysis: api/discriminant_analysis.md
+    - torchml.kernel_approximations: api/kernel_approximations.md
+  - Tutorials:
+    - Linear Models: tutorials/linear_model.md
+    - Naive Bayes: tutorials/gaussian_nb.md
+    - Nearest Neighbors: tutorials/neighbors.md
+    - Nearest Centroid: tutorials/nearest_centroid.md
   - Changelog: changelog.md
-  - GitHub: https://github.com/seba-1511/mypackage/
+  - Getting Started: getting_started.md
+  - GitHub: https://github.com/learnables/torchml/
 
 docs_dir: ./docs
-site_name: mypackage
-site_url: http://mypackage.net
+site_name: torchml
+site_url: http://torchml.net
 site_author: 'Séb Arnold'
-google_analytics: ['UA-68693545-3', 'seba-1511.github.com']
-repo_name: 'seba-1511/mypackage'
-repo_url: 'https://github.com/seba-1511/mypackage'
+google_analytics: ['UA-68693545-3', 'learnables.github.com']
+repo_name: 'learnables/torchml'
+repo_url: 'https://github.com/learnables/torchml'
 edit_uri: ''
 theme:
   name: 'material'
-  logo: 'assets/images/mypackage.png'
+  logo: 'assets/images/torchml-icon.png'
   favicon: 'assets/images/favicon.ico'
   palette:
     primary: 'white'
     accent: 'orange'
   font:
       text: 'Source Sans Pro'
       code: 'Ubuntu Mono'
@@ -35,19 +44,17 @@
 extra_css:
     - https://cdn.jsdelivr.net/npm/katex/dist/katex.min.css
     - 'assets/css/custom.css'
 
 extra:
   social:
     - type: 'github'
-      link: 'https://github.com/seba-1511'
-    - type: 'twitter'
-      link: 'https://twitter.com/seba1511'
+      link: 'https://github.com/learnables'
     - type: 'bug'
-      link: 'https://github.com/seba-1511/mypackage/issues/new'
+      link: 'https://github.com/learnables/torchml/issues/new'
 
 plugins:
   - search
   - autorefs
   - mkdocstrings:
       default_handler: python
       handlers:
```

### Comparing `torchml-0.0.1/setup.py` & `torchml-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 #!/usr/bin/env python3
 
 import re
 from setuptools import (
-        setup,
-        find_packages,
-        )
+    setup,
+    find_packages,
+)
 
 # Parses version number: https://stackoverflow.com/a/7071358
-VERSIONFILE = 'torchml/_version.py'
+VERSIONFILE = "torchml/_version.py"
 verstrline = open(VERSIONFILE, "rt").read()
 VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
 mo = re.search(VSRE, verstrline, re.M)
 if mo:
     VERSION = mo.group(1)
 else:
-    raise RuntimeError('Unable to find version string in %s.' % (VERSIONFILE,))
+    raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Installs the package
 setup(
-    name='torchml',
+    name="torchml",
     packages=find_packages(),
     version=VERSION,
-    description='Classical ML on top of PyTorch',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    author='Seb Arnold',
-    author_email='smr.arnold@gmail.com',
-    url='https://learnables.github.com/torchml',
-    download_url='https://github.com/learnables/torchml/archive/' + str(VERSION) + '.zip',
-    license='License :: OSI Approved :: Apache Software License',
+    description="Classical ML on top of PyTorch",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    author="Seb Arnold",
+    author_email="smr.arnold@gmail.com",
+    url="https://learnables.github.com/torchml",
+    download_url="https://github.com/learnables/torchml/archive/"
+    + str(VERSION)
+    + ".zip",
+    license="License :: OSI Approved :: Apache Software License",
     classifiers=[],
     scripts=[],
     install_requires=[
-        # Add requirements here
+        "torch>=1.4",
+        "cvxpylayers>=0.1.5",
     ],
 )
```

