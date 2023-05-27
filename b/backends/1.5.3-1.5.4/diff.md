# Comparing `tmp/backends-1.5.3.tar.gz` & `tmp/backends-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backends-1.5.3.tar", last modified: Tue Mar  7 07:10:36 2023, max compression
+gzip compressed data, was "backends-1.5.4.tar", last modified: Sat May 27 10:26:07 2023, max compression
```

## Comparing `backends-1.5.3.tar` & `backends-1.5.4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.458555 backends-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-07 07:10:18.000000 backends-1.5.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.434555 backends-1.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.438555 backends-1.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-07 07:10:18.000000 backends-1.5.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-07 07:10:18.000000 backends-1.5.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-07 07:10:18.000000 backends-1.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-07 07:10:18.000000 backends-1.5.3/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-07 07:10:18.000000 backends-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-07 07:10:18.000000 backends-1.5.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-03-07 07:10:36.458555 backends-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-03-07 07:10:18.000000 backends-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.442555 backends-1.5.3/backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-03-07 07:10:36.000000 backends-1.5.3/backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-07 07:10:36.000000 backends-1.5.3/backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 07:10:36.000000 backends-1.5.3/backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-07 07:10:36.000000 backends-1.5.3/backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-07 07:10:36.000000 backends-1.5.3/backends.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-07 07:10:18.000000 backends-1.5.3/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.442555 backends-1.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-07 07:10:18.000000 backends-1.5.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-07 07:10:18.000000 backends-1.5.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-03-07 07:10:18.000000 backends-1.5.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-07 07:10:18.000000 backends-1.5.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.446555 backends-1.5.3/lab/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-07 07:10:18.000000 backends-1.5.3/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-07 07:10:36.000000 backends-1.5.3/lab/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.446555 backends-1.5.3/lab/autograd/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-07 07:10:18.000000 backends-1.5.3/lab/autograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-07 07:10:18.000000 backends-1.5.3/lab/autograd/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-03-07 07:10:18.000000 backends-1.5.3/lab/autograd/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-03-07 07:10:18.000000 backends-1.5.3/lab/autograd/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-07 07:10:18.000000 backends-1.5.3/lab/autograd/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-07 07:10:18.000000 backends-1.5.3/lab/autograd/shaping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.446555 backends-1.5.3/lab/bvn_cdf/
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-03-07 07:10:18.000000 backends-1.5.3/lab/bvn_cdf/bvn_cdf.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    25945 2023-03-07 07:10:18.000000 backends-1.5.3/lab/bvn_cdf/tvpack.f
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-07 07:10:18.000000 backends-1.5.3/lab/bvn_cdf/tvpack.h
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-07 07:10:18.000000 backends-1.5.3/lab/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-03-07 07:10:18.000000 backends-1.5.3/lab/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-03-07 07:10:18.000000 backends-1.5.3/lab/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.450555 backends-1.5.3/lab/jax/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-07 07:10:18.000000 backends-1.5.3/lab/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-03-07 07:10:18.000000 backends-1.5.3/lab/jax/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-03-07 07:10:18.000000 backends-1.5.3/lab/jax/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-03-07 07:10:18.000000 backends-1.5.3/lab/jax/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-07 07:10:18.000000 backends-1.5.3/lab/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-07 07:10:18.000000 backends-1.5.3/lab/jax/shaping.py
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-03-07 07:10:18.000000 backends-1.5.3/lab/linear_algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.450555 backends-1.5.3/lab/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-07 07:10:18.000000 backends-1.5.3/lab/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-03-07 07:10:18.000000 backends-1.5.3/lab/numpy/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-07 07:10:18.000000 backends-1.5.3/lab/numpy/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-07 07:10:18.000000 backends-1.5.3/lab/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-07 07:10:18.000000 backends-1.5.3/lab/numpy/shaping.py
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-03-07 07:10:18.000000 backends-1.5.3/lab/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-03-07 07:10:18.000000 backends-1.5.3/lab/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-03-07 07:10:18.000000 backends-1.5.3/lab/shaping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.450555 backends-1.5.3/lab/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-07 07:10:18.000000 backends-1.5.3/lab/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-07 07:10:18.000000 backends-1.5.3/lab/tensorflow/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-03-07 07:10:18.000000 backends-1.5.3/lab/tensorflow/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-07 07:10:18.000000 backends-1.5.3/lab/tensorflow/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-03-07 07:10:18.000000 backends-1.5.3/lab/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-07 07:10:18.000000 backends-1.5.3/lab/tensorflow/shaping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.454555 backends-1.5.3/lab/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-07 07:10:18.000000 backends-1.5.3/lab/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-07 07:10:18.000000 backends-1.5.3/lab/torch/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-03-07 07:10:18.000000 backends-1.5.3/lab/torch/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-07 07:10:18.000000 backends-1.5.3/lab/torch/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-03-07 07:10:18.000000 backends-1.5.3/lab/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-03-07 07:10:18.000000 backends-1.5.3/lab/torch/shaping.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-03-07 07:10:18.000000 backends-1.5.3/lab/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-03-07 07:10:18.000000 backends-1.5.3/lab/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-07 07:10:18.000000 backends-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-07 07:10:18.000000 backends-1.5.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-07 07:10:18.000000 backends-1.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-07 07:10:36.458555 backends-1.5.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4224 2023-03-07 07:10:18.000000 backends-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 07:10:36.458555 backends-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-07 07:10:18.000000 backends-1.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-07 07:10:18.000000 backends-1.5.3/tests/test_control_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-03-07 07:10:18.000000 backends-1.5.3/tests/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-03-07 07:10:18.000000 backends-1.5.3/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14489 2023-03-07 07:10:18.000000 backends-1.5.3/tests/test_linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-03-07 07:10:18.000000 backends-1.5.3/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-07 07:10:18.000000 backends-1.5.3/tests/test_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-03-07 07:10:18.000000 backends-1.5.3/tests/test_shaping.py
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-03-07 07:10:18.000000 backends-1.5.3/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-03-07 07:10:18.000000 backends-1.5.3/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-03-07 07:10:18.000000 backends-1.5.3/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-07 07:10:18.000000 backends-1.5.3/todo.tasks
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.234579 backends-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-27 10:25:47.000000 backends-1.5.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.226579 backends-1.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.230579 backends-1.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-27 10:25:47.000000 backends-1.5.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-27 10:25:47.000000 backends-1.5.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-27 10:25:47.000000 backends-1.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-27 10:25:47.000000 backends-1.5.4/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-27 10:25:47.000000 backends-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-27 10:25:47.000000 backends-1.5.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-05-27 10:26:07.234579 backends-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-05-27 10:25:47.000000 backends-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.230579 backends-1.5.4/backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-05-27 10:26:07.000000 backends-1.5.4/backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-27 10:26:07.000000 backends-1.5.4/backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:26:07.000000 backends-1.5.4/backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-27 10:26:07.000000 backends-1.5.4/backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 10:26:07.000000 backends-1.5.4/backends.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-27 10:25:47.000000 backends-1.5.4/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.230579 backends-1.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-27 10:25:47.000000 backends-1.5.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-27 10:25:47.000000 backends-1.5.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-05-27 10:25:47.000000 backends-1.5.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-27 10:25:47.000000 backends-1.5.4/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.230579 backends-1.5.4/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-27 10:25:47.000000 backends-1.5.4/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-27 10:26:07.000000 backends-1.5.4/lab/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.230579 backends-1.5.4/lab/autograd/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-27 10:25:47.000000 backends-1.5.4/lab/autograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-27 10:25:47.000000 backends-1.5.4/lab/autograd/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-27 10:25:47.000000 backends-1.5.4/lab/autograd/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-27 10:25:47.000000 backends-1.5.4/lab/autograd/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-27 10:25:47.000000 backends-1.5.4/lab/autograd/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-27 10:25:47.000000 backends-1.5.4/lab/autograd/shaping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.230579 backends-1.5.4/lab/bvn_cdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-27 10:25:47.000000 backends-1.5.4/lab/bvn_cdf/bvn_cdf.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    25945 2023-05-27 10:25:47.000000 backends-1.5.4/lab/bvn_cdf/tvpack.f
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-27 10:25:47.000000 backends-1.5.4/lab/bvn_cdf/tvpack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-27 10:25:47.000000 backends-1.5.4/lab/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-27 10:25:47.000000 backends-1.5.4/lab/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-05-27 10:25:47.000000 backends-1.5.4/lab/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.234579 backends-1.5.4/lab/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-27 10:25:47.000000 backends-1.5.4/lab/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-27 10:25:47.000000 backends-1.5.4/lab/jax/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-27 10:25:47.000000 backends-1.5.4/lab/jax/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-27 10:25:47.000000 backends-1.5.4/lab/jax/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-27 10:25:47.000000 backends-1.5.4/lab/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-27 10:25:47.000000 backends-1.5.4/lab/jax/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-05-27 10:25:47.000000 backends-1.5.4/lab/linear_algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.234579 backends-1.5.4/lab/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-27 10:25:47.000000 backends-1.5.4/lab/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-27 10:25:47.000000 backends-1.5.4/lab/numpy/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-27 10:25:47.000000 backends-1.5.4/lab/numpy/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-27 10:25:47.000000 backends-1.5.4/lab/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-27 10:25:47.000000 backends-1.5.4/lab/numpy/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-05-27 10:25:47.000000 backends-1.5.4/lab/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-27 10:25:47.000000 backends-1.5.4/lab/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-05-27 10:25:47.000000 backends-1.5.4/lab/shaping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.234579 backends-1.5.4/lab/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-27 10:25:47.000000 backends-1.5.4/lab/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-27 10:25:47.000000 backends-1.5.4/lab/tensorflow/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-27 10:25:47.000000 backends-1.5.4/lab/tensorflow/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-27 10:25:47.000000 backends-1.5.4/lab/tensorflow/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-27 10:25:47.000000 backends-1.5.4/lab/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-27 10:25:47.000000 backends-1.5.4/lab/tensorflow/shaping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.234579 backends-1.5.4/lab/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-27 10:25:47.000000 backends-1.5.4/lab/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-27 10:25:47.000000 backends-1.5.4/lab/torch/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-27 10:25:47.000000 backends-1.5.4/lab/torch/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-27 10:25:47.000000 backends-1.5.4/lab/torch/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-27 10:25:47.000000 backends-1.5.4/lab/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-27 10:25:47.000000 backends-1.5.4/lab/torch/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-27 10:25:47.000000 backends-1.5.4/lab/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-05-27 10:25:47.000000 backends-1.5.4/lab/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-27 10:25:47.000000 backends-1.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 10:25:47.000000 backends-1.5.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-27 10:25:47.000000 backends-1.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-27 10:26:07.238579 backends-1.5.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4224 2023-05-27 10:25:47.000000 backends-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:26:07.234579 backends-1.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-27 10:25:47.000000 backends-1.5.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-27 10:25:47.000000 backends-1.5.4/tests/test_control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-05-27 10:25:47.000000 backends-1.5.4/tests/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-05-27 10:25:47.000000 backends-1.5.4/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14489 2023-05-27 10:25:47.000000 backends-1.5.4/tests/test_linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-27 10:25:47.000000 backends-1.5.4/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-27 10:25:47.000000 backends-1.5.4/tests/test_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-05-27 10:25:47.000000 backends-1.5.4/tests/test_shaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-05-27 10:25:47.000000 backends-1.5.4/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-27 10:25:47.000000 backends-1.5.4/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-27 10:25:47.000000 backends-1.5.4/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-27 10:25:47.000000 backends-1.5.4/todo.tasks
```

### Comparing `backends-1.5.3/.github/workflows/ci.yml` & `backends-1.5.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/.github/workflows/publish.yml` & `backends-1.5.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/LICENCE.txt` & `backends-1.5.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/Makefile` & `backends-1.5.4/Makefile`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/PKG-INFO` & `backends-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backends
-Version: 1.5.3
+Version: 1.5.4
 Summary: A generic interface for linear algebra backends
 Home-page: https://github.com/wesselb/lab
 Author: Wessel Bruinsma
 Author-email: wessel.p.bruinsma@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `backends-1.5.3/README.md` & `backends-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/backends.egg-info/PKG-INFO` & `backends-1.5.4/backends.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backends
-Version: 1.5.3
+Version: 1.5.4
 Summary: A generic interface for linear algebra backends
 Home-page: https://github.com/wesselb/lab
 Author: Wessel Bruinsma
 Author-email: wessel.p.bruinsma@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `backends-1.5.3/backends.egg-info/SOURCES.txt` & `backends-1.5.4/backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/benchmark.py` & `backends-1.5.4/benchmark.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/docs/Makefile` & `backends-1.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/docs/conf.py` & `backends-1.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/autograd/__init__.py` & `backends-1.5.4/lab/autograd/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/autograd/custom.py` & `backends-1.5.4/lab/autograd/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/autograd/generic.py` & `backends-1.5.4/lab/autograd/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/autograd/linear_algebra.py` & `backends-1.5.4/lab/autograd/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/autograd/random.py` & `backends-1.5.4/lab/autograd/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/autograd/shaping.py` & `backends-1.5.4/lab/autograd/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/bvn_cdf/bvn_cdf.pyx` & `backends-1.5.4/lab/bvn_cdf/bvn_cdf.pyx`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/bvn_cdf/tvpack.f` & `backends-1.5.4/lab/bvn_cdf/tvpack.f`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/control_flow.py` & `backends-1.5.4/lab/control_flow.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/custom.py` & `backends-1.5.4/lab/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/generic.py` & `backends-1.5.4/lab/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/jax/__init__.py` & `backends-1.5.4/lab/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/jax/custom.py` & `backends-1.5.4/lab/jax/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/jax/generic.py` & `backends-1.5.4/lab/jax/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/jax/linear_algebra.py` & `backends-1.5.4/lab/jax/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/jax/random.py` & `backends-1.5.4/lab/jax/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/jax/shaping.py` & `backends-1.5.4/lab/jax/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/linear_algebra.py` & `backends-1.5.4/lab/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/numpy/__init__.py` & `backends-1.5.4/lab/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/numpy/generic.py` & `backends-1.5.4/lab/numpy/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/numpy/linear_algebra.py` & `backends-1.5.4/lab/numpy/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/numpy/random.py` & `backends-1.5.4/lab/numpy/random.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import warnings
 from typing import Union
 
 import numpy as np
 
-from . import dispatch, B, Numeric
-from ..types import NPDType, NPRandomState, Int
+from ..types import Int, NPDType, NPRandomState
 from ..util import broadcast_shapes
+from . import B, Numeric, dispatch
 
 __all__ = []
 
 
 @dispatch
 def create_random_state(_: NPDType, seed: Int = 0):
     return np.random.RandomState(seed=seed)
@@ -55,15 +55,15 @@
 @dispatch
 def randcat(state: NPRandomState, p: Numeric, n: Int):
     # Probabilities must sum to one.
     p = p / np.sum(p, axis=-1, keepdims=True)
     # Perform sampling routine.
     cdf = np.cumsum(p, axis=-1)
     u = state.rand(n, *p.shape[:-1])
-    inds = np.sum(u[..., None] < cdf[None], axis=-1) - 1
+    inds = np.sum(u[..., None] >= cdf[None], axis=-1)
     # Be sure to return the right data type.
     return state, B.cast(B.dtype_int(p), inds)
 
 
 @dispatch
 def randcat(p: Numeric, *shape: Int):
     return randcat(global_random_state(p), p, *shape)[1]
```

### Comparing `backends-1.5.3/lab/numpy/shaping.py` & `backends-1.5.4/lab/numpy/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/random.py` & `backends-1.5.4/lab/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/shape.py` & `backends-1.5.4/lab/shape.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/shaping.py` & `backends-1.5.4/lab/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/tensorflow/__init__.py` & `backends-1.5.4/lab/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/tensorflow/custom.py` & `backends-1.5.4/lab/tensorflow/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/tensorflow/generic.py` & `backends-1.5.4/lab/tensorflow/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/tensorflow/linear_algebra.py` & `backends-1.5.4/lab/tensorflow/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/tensorflow/random.py` & `backends-1.5.4/lab/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/tensorflow/shaping.py` & `backends-1.5.4/lab/tensorflow/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/torch/__init__.py` & `backends-1.5.4/lab/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/torch/custom.py` & `backends-1.5.4/lab/torch/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/torch/generic.py` & `backends-1.5.4/lab/torch/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/torch/linear_algebra.py` & `backends-1.5.4/lab/torch/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/torch/random.py` & `backends-1.5.4/lab/torch/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/torch/shaping.py` & `backends-1.5.4/lab/torch/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/types.py` & `backends-1.5.4/lab/types.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/lab/util.py` & `backends-1.5.4/lab/util.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/setup.py` & `backends-1.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/tests/test_control_flow.py` & `backends-1.5.4/tests/test_control_flow.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/tests/test_custom.py` & `backends-1.5.4/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/tests/test_generic.py` & `backends-1.5.4/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/tests/test_linear_algebra.py` & `backends-1.5.4/tests/test_linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/tests/test_random.py` & `backends-1.5.4/tests/test_random.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import warnings
 
-import lab.torch
-import lab.tensorflow
-import lab.jax
-import lab.autograd
-
 import jax.numpy as jnp
 import lab as B
+import lab.autograd
+import lab.jax
+import lab.tensorflow
+import lab.torch
 import numpy as np
 import pytest
 import tensorflow as tf
 import torch
 from plum import isinstance
 
 # noinspection PyUnresolvedReferences
-from .util import Tensor, PositiveTensor, approx, to_np, check_lazy_shapes
+from .util import PositiveTensor, Tensor, approx, check_lazy_shapes, to_np
 
 
 @pytest.mark.parametrize(
     "dtype, f_plain",
     [
         (np.float32, np.random.randn),
         (tf.float32, lambda: tf.random.normal(())),
@@ -136,14 +135,21 @@
         assert B.shape(f(state, f(t, 2))[1]) == (2,)
         assert isinstance(f(state, f(t, 2, 3))[0], B.RandomState)
         assert B.dtype(f(state, f(t, 2, 3))[1]) is dtype_transform(t)
         assert B.shape(f(state, f(t, 2, 3))[1]) == (2, 3)
 
 
 @pytest.mark.parametrize("t", [np.float32, tf.float32, torch.float32, jnp.float32])
+def test_randcat_correctness(t, check_lazy_shapes):
+    assert int(B.randcat(B.cast(t, np.array([1.0, 0.0, 0.0])))) == 0
+    assert int(B.randcat(B.cast(t, np.array([0.0, 1.0, 0.0])))) == 1
+    assert int(B.randcat(B.cast(t, np.array([0.0, 0.0, 1.0])))) == 2
+
+
+@pytest.mark.parametrize("t", [np.float32, tf.float32, torch.float32, jnp.float32])
 def test_randint_bounds(t, check_lazy_shapes):
     assert B.randint(t, lower=10, upper=11) == 10
 
 
 @pytest.mark.parametrize("t", [np.float32, tf.float32, torch.float32, jnp.float32])
 def test_randgamma_parameters(t, check_lazy_shapes):
     approx(B.randgamma(t, alpha=1, scale=0), 0, atol=1e-6)
```

### Comparing `backends-1.5.3/tests/test_shape.py` & `backends-1.5.4/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/tests/test_shaping.py` & `backends-1.5.4/tests/test_shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/tests/test_types.py` & `backends-1.5.4/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/tests/test_util.py` & `backends-1.5.4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/tests/util.py` & `backends-1.5.4/tests/util.py`

 * *Files identical despite different names*

### Comparing `backends-1.5.3/todo.tasks` & `backends-1.5.4/todo.tasks`

 * *Files identical despite different names*

