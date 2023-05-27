# Comparing `tmp/CUQIpy-0.3.0.post0.dev7.tar.gz` & `tmp/CUQIpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUQIpy-0.3.0.post0.dev7.tar", last modified: Sun Apr 23 09:57:21 2023, max compression
+gzip compressed data, was "CUQIpy-0.4.0.tar", last modified: Sat May 27 08:12:48 2023, max compression
```

## Comparing `CUQIpy-0.3.0.post0.dev7.tar` & `CUQIpy-0.4.0.tar`

### file list

```diff
@@ -1,112 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.362814 CUQIpy-0.3.0.post0.dev7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.350814 CUQIpy-0.3.0.post0.dev7/CUQIpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-04-23 09:57:21.000000 CUQIpy-0.3.0.post0.dev7/CUQIpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-23 09:57:21.000000 CUQIpy-0.3.0.post0.dev7/CUQIpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 09:57:21.000000 CUQIpy-0.3.0.post0.dev7/CUQIpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 09:57:21.000000 CUQIpy-0.3.0.post0.dev7/CUQIpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 09:57:21.000000 CUQIpy-0.3.0.post0.dev7/CUQIpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-04-23 09:57:21.362814 CUQIpy-0.3.0.post0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.362814 CUQIpy-0.3.0.post0.dev7/cuqi/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-23 09:57:21.362814 CUQIpy-0.3.0.post0.dev7/cuqi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.350814 CUQIpy-0.3.0.post0.dev7/cuqi/array/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/array/_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.354814 CUQIpy-0.3.0.post0.dev7/cuqi/data/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/data/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)   786696 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/data/astronaut.npz
--rw-r--r--   0 runner    (1001) docker     (123)   262408 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/data/camera.npz
--rw-r--r--   0 runner    (1001) docker     (123)   406164 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/data/cat.npz
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/data/satellite.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.354814 CUQIpy-0.3.0.post0.dev7/cuqi/density/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/density/_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.354814 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_cauchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_cauchy_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    15873 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_gmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_inverse_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_laplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_laplace_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_lmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_lognormal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.354814 CUQIpy-0.3.0.post0.dev7/cuqi/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39613 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/geometry/_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.354814 CUQIpy-0.3.0.post0.dev7/cuqi/likelihood/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/likelihood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/likelihood/_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.354814 CUQIpy-0.3.0.post0.dev7/cuqi/model/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21525 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/model/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.354814 CUQIpy-0.3.0.post0.dev7/cuqi/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/operator/_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.358814 CUQIpy-0.3.0.post0.dev7/cuqi/pde/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/pde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/pde/_pde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.358814 CUQIpy-0.3.0.post0.dev7/cuqi/problem/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29508 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/problem/_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.358814 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_conjugate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_conjugate_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_cwmh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_langevin_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_laplace_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_mh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_pcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_rto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.358814 CUQIpy-0.3.0.post0.dev7/cuqi/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/samples/_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.358814 CUQIpy-0.3.0.post0.dev7/cuqi/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19377 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/solver/_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.358814 CUQIpy-0.3.0.post0.dev7/cuqi/testproblem/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/testproblem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52310 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/testproblem/_testproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.358814 CUQIpy-0.3.0.post0.dev7/cuqi/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/utilities/_get_python_variable_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/cuqi/utilities/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 09:57:21.362814 CUQIpy-0.3.0.post0.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 09:57:21.362814 CUQIpy-0.3.0.post0.dev7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_abstract_distribution_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_bayesian_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    28779 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_pde.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_testproblem.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-23 09:57:12.000000 CUQIpy-0.3.0.post0.dev7/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.543003 CUQIpy-0.4.0/CUQIpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-05-27 08:12:48.000000 CUQIpy-0.4.0/CUQIpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-27 08:12:48.000000 CUQIpy-0.4.0/CUQIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:12:48.000000 CUQIpy-0.4.0/CUQIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-27 08:12:48.000000 CUQIpy-0.4.0/CUQIpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-27 08:12:48.000000 CUQIpy-0.4.0/CUQIpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/cuqi/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/cuqi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.547003 CUQIpy-0.4.0/cuqi/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/array/_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.547003 CUQIpy-0.4.0/cuqi/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   786696 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/astronaut.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   262408 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/camera.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   406164 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/cat.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/satellite.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.547003 CUQIpy-0.4.0/cuqi/density/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/density/_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_cauchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_cmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15873 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_gmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_inverse_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_lmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39613 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/geometry/_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/likelihood/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/likelihood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/likelihood/_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24201 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/operator/_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/pde/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/pde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/pde/_pde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28944 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/problem/_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.555003 CUQIpy-0.4.0/cuqi/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_conjugate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_conjugate_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_cwmh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_langevin_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_laplace_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_mh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_pcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_rto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.555003 CUQIpy-0.4.0/cuqi/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/samples/_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.555003 CUQIpy-0.4.0/cuqi/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19377 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.555003 CUQIpy-0.4.0/cuqi/testproblem/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/testproblem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52242 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/testproblem/_testproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.555003 CUQIpy-0.4.0/cuqi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/utilities/_get_python_variable_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/utilities/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_abstract_distribution_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_bayesian_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29794 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_pde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_testproblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_utilities.py
```

### Comparing `CUQIpy-0.3.0.post0.dev7/CUQIpy.egg-info/PKG-INFO` & `CUQIpy-0.4.0/CUQIpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 0.3.0.post0.dev7
+Version: 0.4.0
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -227,22 +227,22 @@
 Image deconvolution with uncertainty quantification
 ```python
 # Imports
 import numpy as np
 import matplotlib.pyplot as plt
 from cuqi.testproblem import Deconvolution2D
 from cuqi.data import grains
-from cuqi.distribution import Laplace_diff, Gaussian
+from cuqi.distribution import LMRF, Gaussian
 from cuqi.problem import BayesianProblem
 
 # Step 1: Model and data, y = Ax
 A, y_data, info = Deconvolution2D.get_components(dim=128, phantom=grains())
 
-# Step 2: Prior, x ~ Laplace_diff(0, 0.01)
-x = Laplace_diff(location=np.zeros(A.domain_dim),
+# Step 2: Prior, x ~ LMRF(0, 0.01)
+x = LMRF(location=np.zeros(A.domain_dim),
                  scale=0.01,
                  bc_type='neumann',
                  physical_dim=2)
 
 # Step 3: Likelihood, y ~ N(Ax, 0.0036^2)
 y = Gaussian(mean=A@x, cov=0.0036**2)
```

### Comparing `CUQIpy-0.3.0.post0.dev7/CUQIpy.egg-info/SOURCES.txt` & `CUQIpy-0.4.0/CUQIpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,23 @@
 cuqi/data/cat.npz
 cuqi/data/satellite.mat
 cuqi/density/__init__.py
 cuqi/density/_density.py
 cuqi/distribution/__init__.py
 cuqi/distribution/_beta.py
 cuqi/distribution/_cauchy.py
-cuqi/distribution/_cauchy_diff.py
+cuqi/distribution/_cmrf.py
 cuqi/distribution/_custom.py
 cuqi/distribution/_distribution.py
 cuqi/distribution/_gamma.py
 cuqi/distribution/_gaussian.py
 cuqi/distribution/_gmrf.py
 cuqi/distribution/_inverse_gamma.py
 cuqi/distribution/_joint_distribution.py
 cuqi/distribution/_laplace.py
-cuqi/distribution/_laplace_diff.py
 cuqi/distribution/_lmrf.py
 cuqi/distribution/_lognormal.py
 cuqi/distribution/_normal.py
 cuqi/distribution/_posterior.py
 cuqi/distribution/_uniform.py
 cuqi/geometry/__init__.py
 cuqi/geometry/_geometry.py
```

### Comparing `CUQIpy-0.3.0.post0.dev7/LICENSE` & `CUQIpy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/PKG-INFO` & `CUQIpy-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 0.3.0.post0.dev7
+Version: 0.4.0
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -227,22 +227,22 @@
 Image deconvolution with uncertainty quantification
 ```python
 # Imports
 import numpy as np
 import matplotlib.pyplot as plt
 from cuqi.testproblem import Deconvolution2D
 from cuqi.data import grains
-from cuqi.distribution import Laplace_diff, Gaussian
+from cuqi.distribution import LMRF, Gaussian
 from cuqi.problem import BayesianProblem
 
 # Step 1: Model and data, y = Ax
 A, y_data, info = Deconvolution2D.get_components(dim=128, phantom=grains())
 
-# Step 2: Prior, x ~ Laplace_diff(0, 0.01)
-x = Laplace_diff(location=np.zeros(A.domain_dim),
+# Step 2: Prior, x ~ LMRF(0, 0.01)
+x = LMRF(location=np.zeros(A.domain_dim),
                  scale=0.01,
                  bc_type='neumann',
                  physical_dim=2)
 
 # Step 3: Likelihood, y ~ N(Ax, 0.0036^2)
 y = Gaussian(mean=A@x, cov=0.0036**2)
```

### Comparing `CUQIpy-0.3.0.post0.dev7/README.md` & `CUQIpy-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 Image deconvolution with uncertainty quantification
 ```python
 # Imports
 import numpy as np
 import matplotlib.pyplot as plt
 from cuqi.testproblem import Deconvolution2D
 from cuqi.data import grains
-from cuqi.distribution import Laplace_diff, Gaussian
+from cuqi.distribution import LMRF, Gaussian
 from cuqi.problem import BayesianProblem
 
 # Step 1: Model and data, y = Ax
 A, y_data, info = Deconvolution2D.get_components(dim=128, phantom=grains())
 
-# Step 2: Prior, x ~ Laplace_diff(0, 0.01)
-x = Laplace_diff(location=np.zeros(A.domain_dim),
+# Step 2: Prior, x ~ LMRF(0, 0.01)
+x = LMRF(location=np.zeros(A.domain_dim),
                  scale=0.01,
                  bc_type='neumann',
                  physical_dim=2)
 
 # Step 3: Likelihood, y ~ N(Ax, 0.0036^2)
 y = Gaussian(mean=A@x, cov=0.0036**2)
```

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/array/_array.py` & `CUQIpy-0.4.0/cuqi/array/_array.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/config.py` & `CUQIpy-0.4.0/cuqi/config.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/data/_data.py` & `CUQIpy-0.4.0/cuqi/data/_data.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/data/astronaut.npz` & `CUQIpy-0.4.0/cuqi/data/astronaut.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/data/camera.npz` & `CUQIpy-0.4.0/cuqi/data/camera.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/data/cat.npz` & `CUQIpy-0.4.0/cuqi/data/cat.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/data/satellite.mat` & `CUQIpy-0.4.0/cuqi/data/satellite.mat`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/density/_density.py` & `CUQIpy-0.4.0/cuqi/density/_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/diagnostics.py` & `CUQIpy-0.4.0/cuqi/diagnostics.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_beta.py` & `CUQIpy-0.4.0/cuqi/distribution/_beta.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_cauchy.py` & `CUQIpy-0.4.0/cuqi/distribution/_cauchy.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_cauchy_diff.py` & `CUQIpy-0.4.0/cuqi/distribution/_cmrf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import warnings
 from cuqi.geometry import _DefaultGeometry, Image2D, _get_identity_geometries
 from cuqi.distribution import Distribution
 from cuqi.operator import FirstOrderFiniteDifference
 from cuqi.geometry import _DefaultGeometry, Image2D, _get_identity_geometries
 
-class Cauchy_diff(Distribution):
+class CMRF(Distribution):
     """Cauchy distribution on the difference between neighboring nodes.
 
     For 1D `(physical_dim=1)`, the Cauchy difference distribution assumes that
 
     .. math::
 
         x_i-x_{i-1} \sim \mathrm{Cauchy}(0, \gamma),
@@ -38,15 +38,15 @@
 
     Example
     -------
     .. code-block:: python
 
         import cuqi
         import numpy as np
-        prior = cuqi.distribution.Cauchy_diff(location=np.zeros(128), scale=0.1)
+        prior = cuqi.distribution.CMRF(location=np.zeros(128), scale=0.1)
  
     """
    
     def __init__(self, location, scale, bc_type="zero", physical_dim=1, **kwargs):
         # Init from abstract distribution class
         super().__init__(**kwargs) 
         
@@ -56,15 +56,15 @@
         self._physical_dim = physical_dim
 
         if physical_dim == 2:
             N = int(np.sqrt(self.dim))
             num_nodes = (N, N)
             if isinstance(self.geometry, _DefaultGeometry):
                 self.geometry = Image2D(num_nodes)
-            print("Warning: 2D Cauchy_diff is still experimental. Use at own risk.")
+            print("Warning: 2D CMRF is still experimental. Use at own risk.")
         elif physical_dim == 1:
             num_nodes = self.dim
         else:
             raise ValueError("Only physical dimension 1 or 2 supported.")
 
         self._diff_op = FirstOrderFiniteDifference(num_nodes=num_nodes, bc_type=bc_type)
 
@@ -85,14 +85,14 @@
         if not callable(self.location): # for prior
             diff = self._diff_op._matrix @ val
             return (-2*diff/(diff**2+self.scale**2)) @ self._diff_op._matrix
         else:
             warnings.warn('Gradient not implemented for {}'.format(type(self.location)))
 
     def _sample(self,N=1,rng=None):
-        raise NotImplementedError("'Cauchy_diff.sample' is not implemented. Sampling can be performed with the 'sampler' module.")
+        raise NotImplementedError("'CMRF.sample' is not implemented. Sampling can be performed with the 'sampler' module.")
 
     # def cdf(self, x):   # TODO
     #     return 1/np.pi * np.atan((x-self.loc)/self.scale)
 
     # def sample(self):   # TODO
     #     return self.loc + self.scale*np.tan(np.pi*(np.random.rand(self.dim)-1/2))
```

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_custom.py` & `CUQIpy-0.4.0/cuqi/distribution/_custom.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_distribution.py` & `CUQIpy-0.4.0/cuqi/distribution/_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_gamma.py` & `CUQIpy-0.4.0/cuqi/distribution/_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_gaussian.py` & `CUQIpy-0.4.0/cuqi/distribution/_gaussian.py`

 * *Files 0% similar despite different names*

```diff
@@ -650,14 +650,23 @@
         logdet = np.sum(-np.log(sqrtprec**2))
         rank = dim
         if sparse_flag:
             sqrtprec = spa.diags(sqrtprec)
         else:
             sqrtprec = np.diag(sqrtprec)
 
+    # check if sqrtprec matrix is square
+    elif sqrtprec.ndim == 2 and sqrtprec.shape[0] != sqrtprec.shape[1]:
+        raise ValueError("sqrtprec must be square")     
+
+    # sqrtprec is sparse diagonal
+    elif spa.isspmatrix_dia(sqrtprec):
+        logdet = np.sum(-np.log(sqrtprec.data**2))
+        rank = dim
+
     # sqrtprec diagonal
     elif np.count_nonzero(sqrtprec-np.diag(sqrtprec.diagonal())) == 0:
         stdinv = sqrtprec.diagonal()
         precision = stdinv**2
         logdet = np.sum(-np.log(precision))
         rank = dim
```

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_gmrf.py` & `CUQIpy-0.4.0/cuqi/distribution/_gmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_inverse_gamma.py` & `CUQIpy-0.4.0/cuqi/distribution/_inverse_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_joint_distribution.py` & `CUQIpy-0.4.0/cuqi/distribution/_joint_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_laplace.py` & `CUQIpy-0.4.0/cuqi/distribution/_laplace.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_laplace_diff.py` & `CUQIpy-0.4.0/cuqi/distribution/_lmrf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from cuqi.geometry import _DefaultGeometry, Image2D
 from cuqi.operator import FirstOrderFiniteDifference
 from cuqi.distribution import Distribution
 
-class Laplace_diff(Distribution):
+class LMRF(Distribution):
     """Laplace distribution on the difference between neighboring nodes.
 
     For 1D `(physical_dim=1)`, the Laplace difference distribution assumes that
 
     .. math::
 
         x_i-x_{i-1} \sim \mathrm{Laplace}(0, b),
@@ -36,15 +36,15 @@
 
     Example
     -------
     .. code-block:: python
 
         import cuqi
         import numpy as np
-        prior = cuqi.distribution.Laplace_diff(location=np.zeros(128), scale=0.1)
+        prior = cuqi.distribution.LMRF(location=np.zeros(128), scale=0.1)
  
     """
     def __init__(self, location, scale, bc_type="zero", physical_dim=1, **kwargs):
         # Init from abstract distribution class
         super().__init__(**kwargs) 
 
         self.location = location
@@ -74,15 +74,15 @@
         return (1/(2*self.scale))**(len(Dx)) * np.exp(-np.linalg.norm(Dx, ord=1, axis=0)/self.scale)
 
     def logpdf(self, x):
         Dx = self._diff_op @ (x-self.location)
         return len(Dx)*(-(np.log(2)+np.log(self.scale))) - np.linalg.norm(Dx, ord=1, axis=0)/self.scale
 
     def _sample(self,N=1,rng=None):
-        raise NotImplementedError("'Laplace_diff.sample' is not implemented. Sampling can be performed with the 'sampler' module.")
+        raise NotImplementedError("'LMRF.sample' is not implemented. Sampling can be performed with the 'sampler' module.")
 
     # def cdf(self, x):   # TODO
     #     return 1/2 + 1/2*np.sign(x-self.loc)*(1-np.exp(-np.linalg.norm(x, ord=1, axis=0)/self.scale))
 
     # def sample(self):   # TODO
     #     p = np.random.rand(self.dim)
     #     return self.loc - self.scale*np.sign(p-1/2)*np.log(1-2*abs(p-1/2))
```

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_lognormal.py` & `CUQIpy-0.4.0/cuqi/distribution/_lognormal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_normal.py` & `CUQIpy-0.4.0/cuqi/distribution/_normal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_posterior.py` & `CUQIpy-0.4.0/cuqi/distribution/_posterior.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/distribution/_uniform.py` & `CUQIpy-0.4.0/cuqi/distribution/_uniform.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/geometry/__init__.py` & `CUQIpy-0.4.0/cuqi/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/geometry/_geometry.py` & `CUQIpy-0.4.0/cuqi/geometry/_geometry.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/likelihood/__init__.py` & `CUQIpy-0.4.0/cuqi/likelihood/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/likelihood/_likelihood.py` & `CUQIpy-0.4.0/cuqi/likelihood/_likelihood.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/model/_model.py` & `CUQIpy-0.4.0/cuqi/model/_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import numpy as np
 from scipy.sparse import csc_matrix
 from scipy.sparse import hstack
 from scipy.linalg import solve
 from cuqi.samples import Samples
 from cuqi.array import CUQIarray
 from cuqi.geometry import Geometry, _DefaultGeometry, _get_identity_geometries
@@ -19,44 +20,98 @@
 
     range_geometry : integer or cuqi.geometry.Geometry
         If integer is given a _DefaultGeometry is created with dimension of the integer.
 
     domain_geometry : integer or cuqi.geometry.Geometry
         If integer is given a _DefaultGeometry is created with dimension of the integer.
 
-    gradient : callable function
+    gradient : callable function, optional
         The direction-Jacobian product of the forward operator Jacobian with 
         respect to the forward operator input, evaluated at a point (`wrt`).
         The signature of the gradient function should be (`direction`, `wrt`),
         where `direction` is the direction by which the Jacobian matrix is
         multiplied and `wrt` is the point at which the Jacobian is computed.
 
-    Attributes
-    -----------
-    range_geometry : cuqi.geometry.Geometry
-        The geometry representing the range.
+    jacobian : callable function, optional
+        The Jacobian of the forward operator with respect to the forward operator input,
+        evaluated at a point (`wrt`). The signature of the Jacobian function should be (`wrt`).
+        The Jacobian function should return a 2D ndarray of shape (range_dim, domain_dim).
+        The Jacobian function is used to specify the gradient function (vector-Jacobian product)
+        automatically and thus the gradient function should not be specified when the Jacobian
+        function is specified.
 
-    domain_geometry : cuqi.geometry.Geometry
-        The geometry representing the domain.
+    Example
+    -------
+
+    Consider a forward model :math:`F: \mathbb{R}^2 \rightarrow \mathbb{R}` defined by the following forward operator:
+
+    .. math::
+
+        F(x) = 10x_2 - 10x_1^3 + 5x_1^2 + 6x_1
+
+    The jacobian matrix of the forward operator is given by:
+
+    .. math::
+
+        J_F(x) = \\begin{bmatrix} -30x_1^2 + 10x_1 + 6 & 10 \\end{bmatrix}
+
+    The forward model can be defined as follows:
+
+    .. code-block:: python
+
+        import numpy as np
+        from cuqi.model import Model
+
+        def forward(x):
+            return 10*x[1] - 10*x[0]**3 + 5*x[0]**2 + 6*x[0]
+
+        def jacobian(x): # Can use "x" or "wrt" as the input argument name
+            return np.array([[-30*x[0]**2 + 10*x[0] + 6, 10]])
+
+        model = Model(forward, range_geometry=1, domain_geometry=2, jacobian=jacobian)
+
+    Alternatively, the gradient information in the forward model can be defined by direction-Jacobian product using the gradient keyword argument.
+
+    This may be more efficient if forming the Jacobian matrix is expensive.
+
+    .. code-block:: python
+
+        import numpy as np
+        from cuqi.model import Model
+
+        def forward(x):
+            return 10*x[1] - 10*x[0]**3 + 5*x[0]**2 + 6*x[0]
+
+        def gradient(direction, wrt):
+            # Direction-Jacobian product direction@jacobian(wrt)
+            return direction@np.array([[-30*wrt[0]**2 + 10*wrt[0] + 6, 10]])
+
+        model = Model(forward, range_geometry=1, domain_geometry=2, gradient=gradient)
 
-    Methods
-    -----------
-    :meth:`forward` the forward operator.
-    :meth:`range_dim` the dimension of the range.
-    :meth:`domain_dim` the dimension of the domain.
     """
-    def __init__(self, forward, range_geometry, domain_geometry, gradient=None):
+    def __init__(self, forward, range_geometry, domain_geometry, gradient=None, jacobian=None):
 
         #Check if input is callable
         if callable(forward) is not True:
-            raise TypeError("Forward needs to be callable function of some kind")
+            raise TypeError("Forward needs to be callable function.")
+        
+        # Check if only one of gradient and jacobian is given
+        if (gradient is not None) and (jacobian is not None):
+            raise TypeError("Only one of gradient and jacobian should be specified")
         
         #Check if input is callable
         if (gradient is not None) and (callable(gradient) is not True):
-            raise TypeError("Gradient needs to be callable function of some kind")
+            raise TypeError("Gradient needs to be callable function.")
+        
+        if (jacobian is not None) and (callable(jacobian) is not True):
+            raise TypeError("Jacobian needs to be callable function.")
+        
+        # Use jacobian function to specify gradient function (vector-Jacobian product)
+        if jacobian is not None:
+            gradient = lambda direction, wrt: direction@jacobian(wrt)
  
         #Store forward func
         self._forward_func = forward
         self._gradient_func = gradient
          
         #Store range_geometry
         if isinstance(range_geometry, int):
@@ -255,15 +310,15 @@
                                 self.domain_geometry,
                                 x, is_par)
 
     def __call__(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
 
     def gradient(self, direction, wrt, is_direction_par=True, is_wrt_par=True):
-        """ Gradient of the forward operator.
+        """ Gradient of the forward operator (Direction-Jacobian product)
 
         For non-linear models the gradient is computed using the
         forward operator and the Jacobian of the forward operator.
 
         Parameters
         ----------
         direction : ndarray
@@ -342,15 +397,15 @@
 
         return grad
     
     def __len__(self):
         return self.range_dim
 
     def __repr__(self) -> str:
-        return "CUQI {}: {} -> {}. Forward parameters: {}".format(self.__class__.__name__,self.domain_geometry,self.range_geometry,cuqi.utilities.get_non_default_args(self))
+        return "CUQI {}: {} -> {}.\n    Forward parameters: {}.".format(self.__class__.__name__,self.domain_geometry,self.range_geometry,cuqi.utilities.get_non_default_args(self))
     
 class LinearModel(Model):
     """Model based on a Linear forward operator.
 
     Parameters
     -----------
     forward : 2D ndarray or callable function.
@@ -499,32 +554,39 @@
 
     Methods
     -----------
     :meth:`forward` the forward operator.
     :meth:`range_dim` the dimension of the range.
     :meth:`domain_dim` the dimension of the domain.
     """
-    def __init__(self, PDE, range_geometry, domain_geometry):
-        #....
-        if not isinstance(PDE,cuqi.pde.PDE):
+    def __init__(self, PDE: cuqi.pde.PDE, range_geometry, domain_geometry):
+
+        if not isinstance(PDE, cuqi.pde.PDE):
             raise ValueError("PDE needs to be a cuqi PDE.")
 
-        super().__init__(self._forward_func, range_geometry, domain_geometry)
+        super().__init__(self._forward_func, range_geometry, domain_geometry, gradient=self._gradient_func)
 
         self.pde = PDE
-        if hasattr(self.pde, "gradient_wrt_parameter"):
-            self._gradient_func = self.pde.gradient_wrt_parameter
 
-    def _forward_func(self,x):
+    def _forward_func(self, x):
         
         self.pde.assemble(parameter=x)
 
         sol, info = self.pde.solve()
 
         obs = self.pde.observe(sol)
 
         return obs
+    
+    def _gradient_func(self, direction, wrt):
+        """ Compute direction-Jacobian product (gradient) of the model. """
+        if hasattr(self.pde, "gradient_wrt_parameter"):
+            return self.pde.gradient_wrt_parameter(direction, wrt)
+        elif hasattr(self.pde, "jacobian_wrt_parameter"):
+            return direction@self.pde.jacobian_wrt_parameter(wrt)
+        else:
+            raise NotImplementedError("Gradient is not implemented for this model.")
 
     # Add the underlying PDE class name to the repr.
     def __repr__(self) -> str:
-        return super().__repr__()+". PDE: {}".format(self.pde.__class__.__name__)
+        return super().__repr__()+"\n    PDE: {}.".format(self.pde.__class__.__name__)
```

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/operator/_operator.py` & `CUQIpy-0.4.0/cuqi/operator/_operator.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/pde/_pde.py` & `CUQIpy-0.4.0/cuqi/pde/_pde.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/problem/_problem.py` & `CUQIpy-0.4.0/cuqi/problem/_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 import numpy as np
 import time
 from typing import Tuple
 
 import cuqi
 from cuqi import config
-from cuqi.distribution import Distribution, Gaussian, InverseGamma, Laplace_diff, GMRF, Lognormal, Posterior, LMRF, Beta, JointDistribution, Gamma, Cauchy_diff
+from cuqi.distribution import Distribution, Gaussian, InverseGamma, LMRF, GMRF, Lognormal, Posterior, Beta, JointDistribution, Gamma, CMRF
 from cuqi.density import Density
 from cuqi.model import LinearModel, Model
 from cuqi.likelihood import Likelihood
 from cuqi.geometry import _DefaultGeometry
 from cuqi.utilities import ProblemInfo
 from cuqi.array import CUQIarray
 
@@ -326,31 +326,27 @@
         if self._check_posterior(self, Gaussian, Gaussian, LinearModel, config.MAX_DIM_INV) and not self._check_posterior(self, GMRF):
             return self._sampleMapCholesky(Ns, callback)
 
         # For larger-scale Gaussian we use Linear RTO. TODO: Improve checking once we have a common Gaussian class.
         elif hasattr(self.prior,"sqrtprecTimesMean") and hasattr(self.likelihood.distribution,"sqrtprec") and isinstance(self.model,LinearModel):
             return self._sampleLinearRTO(Ns, callback)
 
-        # For Laplace_diff we use our awesome unadjusted Laplace approximation!
-        elif self._check_posterior(self, Laplace_diff, Gaussian):
-            return self._sampleUnadjustedLaplaceApproximation(Ns, callback)
+        # For LMRF we use our awesome unadjusted Laplace approximation!
+        elif self._check_posterior(self, LMRF, Gaussian):
+            return self._sampleUGLA(Ns, callback)
 
         # If we have gradients, use NUTS!
         # TODO: Fix cases where we have gradients but NUTS fails (see checks)
         elif self._check_posterior(self, must_have_gradient=True) and not self._check_posterior(self, (Beta, InverseGamma, Lognormal)):
             return self._sampleNUTS(Ns, callback)
 
         # For Gaussians with non-linear model we use pCN
         elif self._check_posterior(self, (Gaussian, GMRF), Gaussian):
             return self._samplepCN(Ns, callback)
 
-        # For the remainder of valid cases we use CWMH
-        elif self._check_posterior(self, LMRF):
-            return self._sampleCWMH(Ns, callback)
-
         else:
             raise NotImplementedError(f"Automatic sampler choice is not implemented for model: {type(self.model)}, likelihood: {type(self.likelihood.distribution)} and prior: {type(self.prior)} and dim {self.prior.dim}. Manual sampler choice can be done via the 'sampler' module. Posterior distribution can be extracted via '.posterior' of any testproblem (BayesianProblem).")
 
     def sample_prior(self, Ns, callback=None) -> cuqi.samples.Samples:
         """ Sample the prior distribution. Sampler choice and tuning is handled automatically. """
 
         # Try sampling prior directly
@@ -413,19 +409,15 @@
         """ Do a fitting UQ plot for a single variable given by samples. """
         # Potentially extract exact solution
         if exact is None and hasattr(self, 'exactSolution'):
             exact = self.exactSolution
 
         # Plot traces for single parameters
         if samples.shape[0] == 1:
-            if exact is not None:
-                par_name = samples.geometry.variables[0]
-                samples.plot_trace(lines=((par_name, {}, exact),))
-            else:
-                samples.plot_trace()
+            samples.plot_trace(exact=exact)
         else: # Else plot credible intervals
             samples.plot_ci(exact=exact)
 
     def _sampleLinearRTO(self,Ns, callback=None):
         print("Using Linear_RTO sampler.")
         print("burn-in: 20%")
 
@@ -535,24 +527,24 @@
         Nb = int(0.2*Ns)   # burn-in
         ti = time.time()
         x_s = MCMC.sample_adapt(Ns,Nb)
         print('Elapsed time:', time.time() - ti)
         
         return x_s
 
-    def _sampleUnadjustedLaplaceApproximation(self, Ns, callback=None):
-        print("Using Unadjusted Laplace Approximation sampler")
+    def _sampleUGLA(self, Ns, callback=None):
+        print("Using UGLA sampler")
         print("burn-in: 20%")
 
         # Start timing
         ti = time.time()
 
         # Sample
         Nb = int(0.2*Ns)
-        sampler = cuqi.sampler.UnadjustedLaplaceApproximation(self.posterior, callback=callback)
+        sampler = cuqi.sampler.UGLA(self.posterior, callback=callback)
         samples = sampler.sample(Ns, Nb)
 
         # Print timing
         print('Elapsed time:', time.time() - ti)
 
         return samples
 
@@ -581,15 +573,15 @@
             def gradfunc(x): return -density.gradient(x)
             if disp: print("Optimizing with exact gradients")
         except (NotImplementedError, AttributeError):
             gradfunc = None
             if disp: print("Optimizing with approximate gradients.") 
 
         # Compute point estimate
-        if self._check_posterior(self, Cauchy_diff, must_have_gradient=True): # Use L-BFGS-B for Cauchy_diff prior as it has better performance for this multi-modal posterior
+        if self._check_posterior(self, CMRF, must_have_gradient=True): # Use L-BFGS-B for CMRF prior as it has better performance for this multi-modal posterior
             if disp: print(f"Using scipy.optimize.L_BFGS_B on negative log of {density.__class__.__name__}")
             if disp: print("x0: ones vector")
             solver = cuqi.solver.L_BFGS_B(func, x0, gradfunc=gradfunc)
         else:
             if disp: print(f"Using scipy.optimize.minimize on negative log of {density.__class__.__name__}")
             if disp: print("x0: ones vector")
             solver = cuqi.solver.minimize(func, x0, gradfunc=gradfunc)
@@ -717,25 +709,25 @@
             if not isinstance(cond_target, Posterior):
                 raise NotImplementedError(f"Unable to determine sampling strategy for {par_name} with target {cond_target}")
 
             # Gamma prior, Gaussian likelihood -> Conjugate
             if self._check_posterior(cond_target, Gamma, (Gaussian, GMRF)): 
                 sampling_strategy[par_name] = cuqi.sampler.Conjugate
 
-            # Gamma prior, Laplace_diff likelihood -> ConjugateApprox
-            elif self._check_posterior(cond_target, Gamma, Laplace_diff):
+            # Gamma prior, LMRF likelihood -> ConjugateApprox
+            elif self._check_posterior(cond_target, Gamma, LMRF):
                 sampling_strategy[par_name] = cuqi.sampler.ConjugateApprox
 
             # Gaussian prior, Gaussian likelihood, Linear model -> Linear_RTO
             elif self._check_posterior(cond_target, (Gaussian, GMRF), Gaussian, LinearModel):
                 sampling_strategy[par_name] = cuqi.sampler.Linear_RTO
 
-            # Laplace_diff prior, Gaussian likelihood, Linear model -> UnadjustedLaplaceApproximation
-            elif self._check_posterior(cond_target, Laplace_diff, Gaussian, LinearModel):
-                sampling_strategy[par_name] = cuqi.sampler.UnadjustedLaplaceApproximation
+            # LMRF prior, Gaussian likelihood, Linear model -> UGLA
+            elif self._check_posterior(cond_target, LMRF, Gaussian, LinearModel):
+                sampling_strategy[par_name] = cuqi.sampler.UGLA
 
             else:
                 raise NotImplementedError(f"Unable to determine sampling strategy for {par_name} with target {cond_target}")
 
         print("Automatically determined sampling strategy:")
         for dist_name, strategy in sampling_strategy.items():
             print(f"\t{dist_name}: {strategy.__name__}")
```

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_conjugate.py` & `CUQIpy-0.4.0/cuqi/sampler/_conjugate.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_conjugate_approx.py` & `CUQIpy-0.4.0/cuqi/sampler/_conjugate_approx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from cuqi.distribution import Posterior, Laplace_diff, Gamma
+from cuqi.distribution import Posterior, LMRF, Gamma
 import numpy as np
 import scipy as sp
 
 class ConjugateApprox: # TODO: Subclass from Sampler once updated
     """ Approximate Conjugate sampler
 
     Sampler for sampling a posterior distribution where the likelihood and prior can be approximated
     by a conjugate pair.
 
     Currently supported pairs are:
-    - (Laplace_diff, Gamma): Approximated by (Gaussian, Gamma)
+    - (LMRF, Gamma): Approximated by (Gaussian, Gamma)
 
     For more information on conjugate pairs, see https://en.wikipedia.org/wiki/Conjugate_prior.
 
     """
 
     
     def __init__(self, target: Posterior):
-        if not isinstance(target.likelihood.distribution, Laplace_diff):
+        if not isinstance(target.likelihood.distribution, LMRF):
             raise ValueError("Conjugate sampler only works with Laplace diff likelihood function")
         if not isinstance(target.prior, Gamma):
             raise ValueError("Conjugate sampler only works with Gamma prior")
         self.target = target
 
     def step(self, x=None):
         # Extract variables
         # Here we approximate the Laplace diff with a Gaussian
 
         # Extract diff_op from target likelihood
         D = self.target.likelihood.distribution._diff_op
         n = D.shape[0]
 
-        # Gaussian approximation of Laplace_diff prior as function of x_k
+        # Gaussian approximation of LMRF prior as function of x_k
         # See Uribe et al. (2022) for details
         # Current has a zero mean assumption on likelihood! TODO
         beta=1e-5
         def Lk_fun(x_k):
             dd =  1/np.sqrt((D @ x_k)**2 + beta*np.ones(n))
             W = sp.sparse.diags(dd)
             return W.sqrt() @ D
```

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_cwmh.py` & `CUQIpy-0.4.0/cuqi/sampler/_cwmh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_gibbs.py` & `CUQIpy-0.4.0/cuqi/sampler/_gibbs.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_hmc.py` & `CUQIpy-0.4.0/cuqi/sampler/_hmc.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_langevin_algorithm.py` & `CUQIpy-0.4.0/cuqi/sampler/_langevin_algorithm.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_laplace_approximation.py` & `CUQIpy-0.4.0/cuqi/sampler/_laplace_approximation.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import numpy as np
 import cuqi
 from cuqi.distribution import Normal
 from cuqi.solver import CGLS
 from cuqi.sampler import Sampler
 
 
-class UnadjustedLaplaceApproximation(Sampler):
-    """ Unadjusted Laplace approximation sampler
+class UGLA(Sampler):
+    """ Unadjusted (Gaussian) Laplace Approximation sampler
     
     Samples an approximate posterior where the prior is approximated
     by a Gaussian distribution. The likelihood must be Gaussian.
 
-    Currently only works for Laplace_diff priors.
+    Currently only works for LMRF priors.
 
     The inner solver is Conjugate Gradient Least Squares (CGLS) solver.
 
     For more details see: Uribe, Felipe, et al. "A hybrid Gibbs sampler for edge-preserving 
     tomographic reconstruction with uncertain view angles." arXiv preprint arXiv:2104.06919 (2021).
 
     Parameters
@@ -64,17 +64,17 @@
         if not isinstance(self.target.likelihood.model, cuqi.model.LinearModel):
             raise TypeError("Model needs to be linear")
 
         # Check Gaussian likelihood
         if not hasattr(self.target.likelihood.distribution, "sqrtprec"):
             raise TypeError("Distribution in Likelihood must contain a sqrtprec attribute")
 
-        # Check that prior is Laplace_diff
-        if not isinstance(self.target.prior, cuqi.distribution.Laplace_diff):
-            raise ValueError('Unadjusted Laplace approximation requires Laplace_diff prior')
+        # Check that prior is LMRF
+        if not isinstance(self.target.prior, cuqi.distribution.LMRF):
+            raise ValueError('Unadjusted Gaussian Laplace approximation (UGLA) requires LMRF prior')
 
         # Modify initial guess since Sampler sets it to ones.       
         if x0 is not None:
             self.x0 = x0
         else:
             self.x0 = np.zeros(self.target.prior.dim)
         
@@ -111,15 +111,15 @@
 
         """
 
         # Extract diff_op from target prior
         D = self.target.prior._diff_op
         n = D.shape[0]
 
-        # Gaussian approximation of Laplace_diff prior as function of x_k
+        # Gaussian approximation of LMRF prior as function of x_k
         def Lk_fun(x_k):
             dd =  1/np.sqrt((D @ x_k)**2 + self.beta*np.ones(n))
             W = sp.sparse.diags(dd)
             return W.sqrt() @ D
 
         # Now prepare "Linear_RTO" type sampler. TODO: Use Linear_RTO for this instead
         self._shift = 0
```

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_mh.py` & `CUQIpy-0.4.0/cuqi/sampler/_mh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import cuqi
 from cuqi.sampler import ProposalBasedSampler
 
 
-class MetropolisHastings(ProposalBasedSampler):
+class MH(ProposalBasedSampler):
     """Metropolis Hastings sampler.
 
     Allows sampling of a target distribution by random-walk sampling of a proposal distribution along with an accept/reject step.
 
     Parameters
     ----------
 
@@ -44,15 +44,15 @@
         # Logpdf function
         logpdf_func = lambda x: -1/(std**2)*np.sum((x-mu)**2)
 
         # Define distribution from logpdf as UserDefinedDistribution (sample and gradients also supported)
         target = cuqi.distribution.UserDefinedDistribution(dim=dim, logpdf_func=logpdf_func)
 
         # Set up sampler
-        sampler = cuqi.sampler.MetropolisHastings(target, scale=1)
+        sampler = cuqi.sampler.MH(target, scale=1)
 
         # Sample
         samples = sampler.sample(2000)
 
     """
     #target,  proposal=None, scale=1, x0=None, dim=None
     #    super().__init__(target, proposal=proposal, scale=scale,  x0=x0, dim=dim)
```

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_pcn.py` & `CUQIpy-0.4.0/cuqi/sampler/_pcn.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_rto.py` & `CUQIpy-0.4.0/cuqi/sampler/_rto.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/sampler/_sampler.py` & `CUQIpy-0.4.0/cuqi/sampler/_sampler.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/samples/_samples.py` & `CUQIpy-0.4.0/cuqi/samples/_samples.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from cuqi.diagnostics import Geweke
 from cuqi.geometry import _DefaultGeometry, Continuous2D, Image2D
 from cuqi.array import CUQIarray
+from cuqi.utilities import force_ndarray
 from copy import copy
 import arviz # Plotting tool
 
 
 class Samples(object):
     """
     An object used to store samples from distributions. 
@@ -428,22 +429,25 @@
         datadict = self.to_arviz_inferencedata(variable_indices)
         
         # Plot autocorrelation using arviz
         axis = arviz.plot_autocorr(datadict, max_lag=max_lag, combined=combined, **kwargs)
 
         return axis
 
-    def plot_trace(self, variable_indices=None, combined=True, tight_layout=True, **kwargs):
+    def plot_trace(self, variable_indices=None, exact=None, combined=True, tight_layout=True, **kwargs):
         """Creates a traceplot of the samples consisting of 1) a histogram/density plot of the samples and 2) an MCMC chain plot.
         
         Parameters
         ----------
         variable_indices : list, optional
             List of variable indices to plot the autocorrelation for. If no input is given and less than 5 variables exist all are plotted and with more 5 are randomly chosen.
 
+        exact : array-like, optional
+            Exact solution to compare with the samples.
+
         combined : bool, default=True
             Flag for combining multiple chains into a single chain. If False, chains will be
             plotted separately. Note multiple chains are not fully supported yet.        
 
         tight_layout: bool, default=True
             Improves the layout of the traceplot for multiple variables by calling `plt.tight_layout()`.
             Set to False if this causes issues.
@@ -463,14 +467,37 @@
         if variable_indices is None:
             if Nv<dim: print("Selecting 5 randomly chosen variables")
             variable_indices = self._select_random_indices(Nv, dim)
 
         # Convert to arviz InferenceData object
         datadict = self.to_arviz_inferencedata(variable_indices)
 
+        # If exact solution is given, add it via lines argument to arviz using the variable names
+        if exact is not None:
+
+            # Convert exact to ndarray (in case single parameter etc.)
+            exact = force_ndarray(exact, flatten=True)
+
+            # Attempt to extract variables of the exact solution if given in full dimension
+            if len(exact) == dim:
+                exact = exact[variable_indices]
+
+            # If exact is given in reduced dimension, check that the number of variables match
+            if len(variable_indices) != len(exact):
+                raise ValueError(f"The shape of the exact argument {exact.shape} must match the number of variables to be plotted by variable indices {variable_indices.shape}.")
+            
+            # Extract variable names
+            par_names = [self.geometry.variables[i] for i in variable_indices]
+
+            # Arviz style adding lines to traceplot
+            if "lines" in kwargs:
+                raise ValueError("The lines argument is already defined in kwargs. Please remove it to use the exact keyword argument.")
+            
+            kwargs["lines"] = tuple([(par_names[i], {}, exact[i]) for i in range(len(par_names))])
+
         # Plot using arviz
         ax =  arviz.plot_trace(datadict, combined=combined, **kwargs)
 
         # Improves subplot spacing
         if tight_layout: plt.tight_layout() 
 
         return ax
```

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/solver/_solver.py` & `CUQIpy-0.4.0/cuqi/solver/_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/testproblem/_testproblem.py` & `CUQIpy-0.4.0/cuqi/testproblem/_testproblem.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,15 +571,15 @@
         return x
 
 
     else:
         raise NotImplementedError("This phantom is not implemented")
 
 
-class Poisson_1D(BayesianProblem):
+class Poisson1D(BayesianProblem):
     """
     1D Poisson test problem. Discretized 1D Poisson equation (steady-state linear PDE).
 
     Parameters
     ------------
     dim : int
         | size of the grid for the poisson problem
@@ -616,15 +616,15 @@
         | Function that takes the grid as input and returns a sub-grid of the nodes where observations are available, e.g. `observation_grid_map = lambda x: x[np.where(x>5.0)]`. 
 
     Attributes
     ----------
     data : ndarray
         Generated (noisy) data
 
-    model : cuqi.model.PDEModel_1D
+    model : cuqi.model.PDEModel
         Poisson 1D model
 
     prior : cuqi.distribution.Distribution
         Distribution of the prior
 
     likelihood : cuqi.likelihood.Likelihood
         Likelihood function
@@ -716,15 +716,15 @@
         # Initialize Deconvolution as BayesianProblem problem
         super().__init__(y, x, y=data)
 
         # Store exact values
         self.exactSolution = x_exact
         self.exactData = y_exact
 
-class Heat_1D(BayesianProblem):
+class Heat1D(BayesianProblem):
     """
     1D Heat test problem. Discretized Heat equation (time-dependent linear PDE).
 
     Parameters
     ------------
     dim : int
         | size of the grid for the heat problem
@@ -764,15 +764,15 @@
        | Function that takes the grid as input and returns a sub-grid of the nodes where observations are available, e.g. `observation_grid_map = lambda x: x[np.where(x>5.0)]`. 
  
     Attributes
     ----------
     data : ndarray
         Generated (noisy) data
 
-    model : cuqi.model.PDEModel_1D
+    model : cuqi.model.PDEModel
         Heat 1D model
 
     prior : cuqi.distribution.Distribution
         Distribution of the prior
 
     likelihood : cuqi.likelihood.Likelihood
         Likelihood function
@@ -869,15 +869,15 @@
 
         # Store exact values
         self.exactSolution = x_exact
         self.exactData = y_exact
         self.infoString = f"Noise type: Additive i.i.d. noise with mean zero and signal to noise ratio: {SNR}"
 
 
-class Abel_1D(BayesianProblem):
+class Abel1D(BayesianProblem):
     """
     1D Abel test problem. 1D model of rotationally symmetric computed tomography.
 
     Parameters
     ------------
     dim : int
         size of the grid for the problem
@@ -1421,18 +1421,17 @@
     https://dspace.mit.edu/bitstream/handle/1721.1/98815/921147308-MIT.pdf?sequence=1&isAllowed=y
 
     """
     def __init__(self, noise_std=1, prior=None, data=None):
         # forward model and gradient
         def forward(x):
             return 10*x[1] - 10*x[0]**3 + 5*x[0]**2 + 6*x[0]
-        def gradient(direction, x):
-            # Jacobian.T @ direction
-            return np.vstack([-30*x[0]**2 + 10*x[0] + 6, 10]) @ direction
-        model = cuqi.model.Model(forward, range_geometry=1, domain_geometry=2, gradient=gradient)
+        def jacobian(x):
+            return np.array([[-30*x[0]**2 + 10*x[0] + 6, 10]])
+        model = cuqi.model.Model(forward, range_geometry=1, domain_geometry=2, jacobian=jacobian)
 
         # define prior
         if prior is None:
             prior = cuqi.distribution.Gaussian(np.array([1, 0]), 1, name="x")
 
         # data
         if data is None:
```

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/utilities/_get_python_variable_name.py` & `CUQIpy-0.4.0/cuqi/utilities/_get_python_variable_name.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/cuqi/utilities/_utilities.py` & `CUQIpy-0.4.0/cuqi/utilities/_utilities.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/pyproject.toml` & `CUQIpy-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_abstract_distribution_density.py` & `CUQIpy-0.4.0/tests/test_abstract_distribution_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_bayesian_inversion.py` & `CUQIpy-0.4.0/tests/test_bayesian_inversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from typing import Dict
 
 import pytest
 import numpy as np
 import sys
 
 from cuqi.testproblem import Deconvolution1D
-from cuqi.distribution import Gaussian, GMRF, Cauchy_diff, Laplace_diff, LMRF, Gamma
+from cuqi.distribution import Gaussian, GMRF, CMRF, LMRF, Gamma
 from cuqi.problem import BayesianProblem
 from cuqi.density import Density
 
 #All Ns are reduced by a factor of 10 for speed. Best results are obtained by increasing Ns by at least 10 times.
 @pytest.mark.parametrize("TP_type, phantom, prior, Ns", 
                          [
                              (Deconvolution1D, "gauss", Gaussian(np.zeros(128), 0.071**2), 20),
                              (Deconvolution1D, "gauss", GMRF(np.zeros(128), 100, 1, "zero"), 20),
-                             (Deconvolution1D, "square", LMRF(np.zeros(128), 100, 128, 1, "zero"), 100),
-                             (Deconvolution1D, "square", Laplace_diff(np.zeros(128), 0.005), 100),
-                             (Deconvolution1D, "square", Cauchy_diff(np.zeros(128), 0.01), 50),
+                             (Deconvolution1D, "square", LMRF(np.zeros(128), 0.005), 100),
+                             (Deconvolution1D, "square", CMRF(np.zeros(128), 0.01), 50),
                          ])
 def test_TP_BayesianProblem_sample(copy_reference, TP_type, phantom, prior, Ns):
     # SKIP NUTS test if not windows (for now)
-    if isinstance(prior, Cauchy_diff) and not sys.platform.startswith('win'):
-        pytest.skip("NUTS(Cauchy_diff) regression test is not implemented for this platform")
+    if isinstance(prior, CMRF) and not sys.platform.startswith('win'):
+        pytest.skip("NUTS(CMRF) regression test is not implemented for this platform")
 
     np.random.seed(19937)
 
     # Generate TP using this seed (for data consistency)
     # Legacy convolution is used for consistency with the reference data.
     TP = TP_type(dim=prior.dim, phantom=phantom, use_legacy=True, noise_std=0.05) 
 
@@ -39,15 +38,15 @@
     res = samples.samples    
     med_xpos = np.median(res, axis=1)
     sigma_xpos = res.std(axis=1)
     lo95, up95 = np.percentile(res, [2.5, 97.5], axis=1)
 
     # Load reference file into temp folder and load
     ref_fname = f"{TP_type.__name__}_{phantom}_{prior.__class__.__name__}_{Ns}"
-    #if isinstance(prior, Laplace_diff): #Put the case you want to update for here.
+    #if isinstance(prior, LMRF): #Put the case you want to update for here.
     #    np.savez(ref_fname, median=med_xpos, sigma=sigma_xpos, lo95=lo95, up95=up95) #uncomment to update
     ref_file = copy_reference(f"data/{ref_fname}.npz")
     ref = np.load(ref_file)
 
     # Check results with reference data
     assert med_xpos == pytest.approx(ref["median"], rel=1e-3, abs=1e-6)
     assert sigma_xpos == pytest.approx(ref["sigma"], rel=1e-3, abs=1e-6)
@@ -82,20 +81,20 @@
             [
                 Gaussian(np.zeros(128), lambda d: 1/d, name="x"),
                 Gamma(1, 1e-4, name="l"),
                 Gamma(1, 1e-4, name="d")
             ],
             50
         ),
-        # Case 2: Laplace_diff with Gamma hyperpriors on both noise and prior precision
+        # Case 2: LMRF with Gamma hyperpriors on both noise and prior precision
         (
             Deconvolution1D,
             "square",
             [
-                Laplace_diff(np.zeros(128), lambda d: 1/d, name="x"),
+                LMRF(np.zeros(128), lambda d: 1/d, name="x"),
                 Gamma(1, 1e-4, name="l"),
                 Gamma(1, 1e-4, name="d")
             ],
             50,
         ),
     ]
 )
```

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_density.py` & `CUQIpy-0.4.0/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_distribution.py` & `CUQIpy-0.4.0/tests/test_distribution.py`

 * *Files 3% similar despite different names*

```diff
@@ -617,29 +617,29 @@
     g_FD = posterior.gradient(x_i)
 
     # Assert that the exact and FD gradient are close,
     # but not exactly equal (since we use a different method)
     assert np.allclose(g_exact, g_FD) and np.all(g_exact != g_FD)\
         or (np.all(np.isnan(g_exact)) and np.all(np.isnan(g_FD)))
 
-def test_Cauchy_diff_should_not_allow_non_zero_location():
-    """" Cauchy_diff should not allow non-zero location. """
+def test_CMRF_should_not_allow_non_zero_location():
+    """" CMRF should not allow non-zero location. """
     with pytest.raises(ValueError):
-        cuqi.distribution.Cauchy_diff(np.ones(5), 1)
+        cuqi.distribution.CMRF(np.ones(5), 1)
 
     with pytest.raises(ValueError):
-        cuqi.distribution.Cauchy_diff(lambda x: x, 1)
+        cuqi.distribution.CMRF(lambda x: x, 1)
 
-def test_Laplace_diff_should_not_allow_non_zero_location():
-    """" Laplace_diff should not allow non-zero location. """
+def test_LMRF_should_not_allow_non_zero_location():
+    """" LMRF should not allow non-zero location. """
     with pytest.raises(ValueError):
-        cuqi.distribution.Laplace_diff(np.ones(5), 1)
+        cuqi.distribution.LMRF(np.ones(5), 1)
 
     with pytest.raises(ValueError):
-        cuqi.distribution.Laplace_diff(lambda x: x, 1)
+        cuqi.distribution.LMRF(lambda x: x, 1)
 
 def test_Cauchy_against_scipy():
     """ Test Cauchy distribution logpdf, cdf, pdf, gradient """
 
     x = cuqi.distribution.Cauchy(np.random.randn(5), np.abs(np.random.rand(5)))
 
     val = np.random.randn(5)
@@ -663,7 +663,31 @@
 
     x.scale[0] = 0 # This is not a valid scale
 
     val = np.random.randn(5)
 
     # Test logpdf
     assert np.allclose(x.logpdf(val), -np.inf)
+
+def test_Gaussian_sqrtprec_must_be_square():
+    """ Test Gaussian distribution raises ValueError if sqrtprec (sparse and dense) is not square """
+    N = 10; M = 5
+
+    # Create non square sqrtprec as sparse (later converted to dense)
+    sqrtprec = sp.sparse.csr_matrix(np.random.randn(N, M))
+
+    with pytest.raises(ValueError, match="sqrtprec must be square"):
+        cuqi.distribution.Gaussian(mean = np.zeros(N), sqrtprec = sqrtprec)
+
+    with pytest.raises(ValueError, match="sqrtprec must be square"):
+        cuqi.distribution.Gaussian(mean = np.zeros(N), sqrtprec = sqrtprec.todense())
+
+def test_Gaussian_from_sparse_sqrtprec():
+    """ Test Gaussian distribution from sparse sqrtprec is equal to dense sqrtprec """
+    N = 10; M = 5
+
+    sqrtprec = sp.sparse.spdiags(np.random.randn(N), 0, N, N)
+
+    y_from_sparse = cuqi.distribution.Gaussian(mean = np.zeros(N), sqrtprec = sqrtprec)
+    y_from_dense = cuqi.distribution.Gaussian(mean = np.zeros(N), sqrtprec = sqrtprec.todense())
+
+    assert y_from_dense.logpdf(np.ones(N)) == y_from_sparse.logpdf(np.ones(N))
```

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_geometry.py` & `CUQIpy-0.4.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_joint_distribution.py` & `CUQIpy-0.4.0/tests/test_joint_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import cuqi
 import numpy as np
 import pytest
 
 def test_joint_dist_dim_geometry():
     """ Test the dimension and geometry properties of a joint distribution """
 
-    model, data, _ = cuqi.testproblem.Poisson_1D.get_components() # Model is m times n, m != n.
+    model, data, _ = cuqi.testproblem.Poisson1D.get_components() # Model is m times n, m != n.
 
     # Bayesian model
     d = cuqi.distribution.Gamma(1, 1e-4)
     x = cuqi.distribution.Gaussian(np.zeros(model.domain_dim), lambda d: d)
     y = cuqi.distribution.Gaussian(model, 1)
 
     # Joint distribution
```

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_likelihood.py` & `CUQIpy-0.4.0/tests/test_likelihood.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     likelihood = cuqi.distribution.Gaussian(model,1).to_likelihood(data)
 
     # Tests log and gradient calls do not cause errors
     likelihood.logd(probInfo.exactSolution)
     likelihood.gradient(probInfo.exactSolution)
 
 def test_likelihood_attributes():
-    model, data, _ = cuqi.testproblem.Poisson_1D.get_components(dim=128, field_type="Step")
+    model, data, _ = cuqi.testproblem.Poisson1D.get_components(dim=128, field_type="Step")
     likelihood = cuqi.distribution.Gaussian(model,1).to_likelihood(data)
 
     # dim of domain
     assert likelihood.dim == model.domain_dim
 
     # Geometry of domain
     assert likelihood.geometry == model.domain_geometry
```

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_model.py` & `CUQIpy-0.4.0/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,15 +366,15 @@
     assert cuqi.utilities.get_non_default_args(model_y) == ['y']
     assert cuqi.utilities.get_non_default_args(model_y2) == ['y']
     assert cuqi.utilities.get_non_default_args(model_y3) == ['y']
 
 def test_model_parameter_name_switch_errors():
     """ Check that an error is raised if dim does not match or if distribution has no name """
 
-    model = cuqi.testproblem.Poisson_1D().model # domain_dim != range_dim
+    model = cuqi.testproblem.Poisson1D().model # domain_dim != range_dim
 
     y = cuqi.distribution.Gaussian(np.zeros(model.domain_dim-1), 1)
 
     with pytest.raises(ValueError, match=r"dimension does not match"):
         model(y)    
 
 def test_model_allow_other_parameter_names():
@@ -440,7 +440,34 @@
     assert model_mat(np.ones(1)) == np.ones(1)
 
     # Check that matrix multiplication works
     assert model_x@1 == 1
     assert model_y@1 == 1
     assert model_z@1 == 1
     assert model_mat@np.ones(1) == np.ones(1)
+
+def test_model_allows_jacobian_or_gradient():
+    """ Test that either Jacobian or gradient (vector-jacobian product) can be specified and that it gives the same result. """
+    # This is the Wang Cubic test problem model
+    def forward(x):
+        return 10*x[1] - 10*x[0]**3 + 5*x[0]**2 + 6*x[0]
+    def jacobian(x):
+        return np.array([[-30*x[0]**2 + 10*x[0] + 6, 10]])
+    def gradient(dir, wrt):
+        return dir@jacobian(wrt)
+    
+    # Check not both can be specified
+    with pytest.raises(TypeError, match=r"Only one of gradient and jacobian"):
+        model = cuqi.model.Model(forward, range_geometry=1, domain_geometry=2, jacobian=jacobian, gradient=gradient)
+
+    # Check that we can specify jacobian
+    model_jac = cuqi.model.Model(forward, range_geometry=1, domain_geometry=2, jacobian=jacobian)
+
+    # Check that we can specify gradient
+    model_grad = cuqi.model.Model(forward, range_geometry=1, domain_geometry=2, gradient=gradient)
+
+    # Check that we can evaluate the model gradient and get the same result as the jacobian
+    wrt = np.random.randn(1)
+    dir = np.random.randn(1)
+
+    assert np.allclose(model_grad.gradient(dir, wrt), model_jac.gradient(dir, wrt))
+
```

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_pde.py` & `CUQIpy-0.4.0/tests/test_pde.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_problem.py` & `CUQIpy-0.4.0/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_sampler.py` & `CUQIpy-0.4.0/tests/test_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import cuqi
 import numpy as np
 
 import sys
 
-from cuqi.distribution import Gaussian, Cauchy_diff, Gaussian, Laplace_diff, GMRF, LMRF
+from cuqi.distribution import Gaussian, CMRF, Gaussian, LMRF, GMRF
 from cuqi.sampler import pCN
 
 import pytest
 
 
 def test_CWMH_modify_proposal():
     # Parameters
     n = 2
     scale = 0.05*np.ones(n)
     x0 = 0.5*np.ones(n)
 
     # Set up target
-    target_dist = cuqi.distribution.Cauchy_diff(np.zeros(n), 0.5, 'neumann')
+    target_dist = cuqi.distribution.CMRF(np.zeros(n), 0.5, 'neumann')
     def target(x): return target_dist.pdf(x)
 
     # Set up proposals
     #proposal1 = cuqi.distribution.Normal(np.zeros(n),1 )
     #proposal2 = cuqi.distribution.Normal(np.zeros(n),2 )
     #def proposal1(x, sigma): return np.random.normal(x, sigma)
     #def proposal2(x, sigma): return np.random.normal(x, 2*sigma)
@@ -81,15 +81,15 @@
     # target function to sample
     dist = cuqi.distribution.Gaussian(mu, sigma**2)
 
     ref = cuqi.distribution.Gaussian(mu, np.ones(d))   # standard Gaussian
 
     scale = 0.1
     x0 = 0.5*np.ones(d)
-    MCMC2 = cuqi.sampler.MetropolisHastings( dist,proposal = ref,scale =scale, x0=x0)
+    MCMC2 = cuqi.sampler.MH( dist,proposal = ref,scale =scale, x0=x0)
 
     # run sampler
     Ns = int(1e1)      # number of samples
     Nb = int(0.2*Ns)   # burn-in
 
     #
     x_s2 = MCMC2.sample_adapt(Ns, Nb)
@@ -136,15 +136,15 @@
 def test_sampler_geometry_assignment():
 
     n = 2
     scale = 0.05*np.ones(n)
     x0 = 0.5*np.ones(n)
 
     # Set up target
-    target = cuqi.distribution.Cauchy_diff(np.zeros(n), 0.5, 'neumann')
+    target = cuqi.distribution.CMRF(np.zeros(n), 0.5, 'neumann')
     target.geometry = cuqi.geometry.Continuous2D((1,2))
 
     # Set up proposals
     proposal =cuqi.distribution.Normal(mean = lambda location:location,std = lambda scale:scale )
 
     # Set up sampler
     MCMC_sampler = cuqi.sampler.CWMH(target, proposal, scale, x0)
@@ -162,15 +162,15 @@
     X = cuqi.distribution.Gaussian(np.array([2,3]),np.array([[2,0.1],[0.1,5]]))
     distX = cuqi.distribution.UserDefinedDistribution(X.dim, X.logpdf, X.gradient, X.sample)
 
     # Parameters
     Ns = 500   # number of samples
     Nb = 100   # burn-in
 
-    s_MH = cuqi.sampler.MetropolisHastings(distX).sample_adapt(Ns,Nb)
+    s_MH = cuqi.sampler.MH(distX).sample_adapt(Ns,Nb)
     s_CWMH = cuqi.sampler.CWMH(distX).sample_adapt(Ns,Nb)
     s_NUTS = cuqi.sampler.NUTS(distX).sample_adapt(Ns,Nb)
 
     assert np.allclose(s_MH.shape,(X.dim,Ns))
     assert np.allclose(s_CWMH.shape,(X.dim,Ns))
     assert np.allclose(s_NUTS.shape,(X.dim,Ns))
 
@@ -275,15 +275,15 @@
     # Extract Likelihood
     likelihood  = test.likelihood
     
     # Define Prior
     loc = np.zeros(n)
     delta = 1
     scale = delta*h
-    prior = cuqi.distribution.Cauchy_diff(loc, scale, 'neumann')
+    prior = cuqi.distribution.CMRF(loc, scale, 'neumann')
     
     # %% Create the posterior and the sampler
     posterior = cuqi.distribution.Posterior(likelihood, prior)
     MCMC = cuqi.sampler.ULA(posterior, scale=0.0001)
 
     # %% Sample
     samples  = MCMC.sample(5)
@@ -354,15 +354,15 @@
 
 @pytest.mark.parametrize("prior, sample_method, expected", [
     (Gaussian(np.zeros(128), 0.1), "_sampleMapCholesky", np.arange(10)), # Direct (no burn-in, no initial guess)
     (Gaussian(np.zeros(128), 0.1), "_sampleLinearRTO", np.arange(1,12)), # 20% burn-in + initial guess
     (Gaussian(np.zeros(128), 0.1), "_sampleNUTS", np.arange(1,12)),      # 20% burn-in + initial guess
     (Gaussian(np.zeros(128), 0.1), "_samplepCN", np.arange(1,12)),       # 20% burn-in + initial guess
     (Gaussian(np.zeros(128), 0.1), "_sampleCWMH", np.arange(1,12)),      # 20% burn-in + initial guess
-    (Laplace_diff(np.zeros(128), 0.1),"_sampleUnadjustedLaplaceApproximation", np.arange(1,12)), # 20% burn-in + initial guess
+    (LMRF(np.zeros(128), 0.1),"_sampleUGLA", np.arange(1,12)),   # 20% burn-in + initial guess
     ])
 def test_TP_callback(prior, sample_method, expected):
     """ Test that the callback function is called with the correct sample index by comparing to the expected output.
     
     This tests the pipeline from testproblem all the way to the sampler.
     """
```

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_samples.py` & `CUQIpy-0.4.0/tests/test_samples.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 @pytest.mark.parametrize("kwargs",[
                         ({}),
                         ({"max_lag":10,"textsize":25}),
                         ])
 def test_samples_plot_autocorrelation(kwargs):
     # Make basic distribution and sample
     dist = cuqi.distribution.DistributionGallery("CalSom91")
-    sampler = cuqi.sampler.MetropolisHastings(dist)
+    sampler = cuqi.sampler.MH(dist)
     samples = sampler.sample_adapt(1000)
 
     # Switch to discrete geometry (easiest for "variable" names)
     samples.geometry = cuqi.geometry.Discrete(["alpha","beta"])
 
     # Plot with defaults
     samples.plot_autocorrelation()
@@ -51,19 +51,20 @@
     # Plot for single parameter + arguments
     samples.plot_autocorrelation([0],**kwargs)
 
 
 @pytest.mark.parametrize("kwargs",[
                         ({}),
                         ({"combined":False,"tight_layout":False}),
+                        ({"exact":[1, 1]}) # Check exact can be compared with
                         ])
 def test_samples_plot_trace(kwargs):
     # Make basic distribution and sample
     dist = cuqi.distribution.DistributionGallery("CalSom91")
-    sampler = cuqi.sampler.MetropolisHastings(dist)
+    sampler = cuqi.sampler.MH(dist)
     samples = sampler.sample_adapt(1000)
 
     # Switch to discrete geometry (easiest for "variable" names)
     samples.geometry = cuqi.geometry.Discrete(["alpha","beta"])
 
     # Plot with defaults
     samples.plot_trace()
@@ -81,15 +82,15 @@
                         ({"kind":"kde","marginals":True}),
                         ({"kind":"hexbin","marginals":False}),
                         ({"kind":"hexbin","marginals":True}),
                         ])
 def test_samples_plot_pair(kwargs):
     # Make basic distribution and sample
     dist = cuqi.distribution.Gaussian(np.array([1,2,3,4]),1)
-    sampler = cuqi.sampler.MetropolisHastings(dist)
+    sampler = cuqi.sampler.MH(dist)
     samples = sampler.sample_adapt(1000)
     samples.geometry = cuqi.geometry.Discrete(["a","b","c","d"])
 
     # Plot with defaults
     samples.plot_pair()
 
     # Plot with defaults arguments
@@ -118,15 +119,15 @@
     samples1.geometry = cuqi.geometry.Discrete(["alpha","beta1"])
     samples2.geometry = cuqi.geometry.Discrete(["alpha","beta2"])
     with pytest.raises(TypeError): #Type error since geometry does not match.
         samples1.compute_rhat(samples2)
 
 def test_ess():
     dist = cuqi.distribution.DistributionGallery("CalSom91")
-    sampler = cuqi.sampler.MetropolisHastings(dist)
+    sampler = cuqi.sampler.MH(dist)
     samples = sampler.sample_adapt(500)
     assert samples.compute_ess().shape == samples.geometry.par_shape
 
 @pytest.mark.parametrize("geometry", [cuqi.geometry.Discrete(2),
                                       cuqi.geometry.MappedGeometry(
                                           cuqi.geometry.Continuous1D(2), map=lambda x: x**2),
                                       cuqi.geometry.KLExpansion(np.arange(0, 1, .1))])
@@ -146,15 +147,15 @@
 @pytest.mark.parametrize("percent", [10, 50, 90, 95, 99])
 @pytest.mark.parametrize("compute_on_par", [False, True])
 @pytest.mark.parametrize("geometry", [cuqi.geometry.Discrete(2),
                                       cuqi.geometry.MappedGeometry(
                                         cuqi.geometry.Continuous1D(2), map=lambda x: x**2)])
 def test_compute_ci(percent, compute_on_par, geometry):
     dist = cuqi.distribution.DistributionGallery("CalSom91")
-    sampler = cuqi.sampler.MetropolisHastings(dist)
+    sampler = cuqi.sampler.MH(dist)
     par_samples = sampler.sample_adapt(500)
     par_samples.geometry = geometry
     
     samples = par_samples if compute_on_par else par_samples.funvals
     ci = samples.compute_ci(percent)
 
     # manually compute ci
@@ -287,15 +288,15 @@
         X = cuqi.array.CUQIarray([1,2,3], is_par=False)
     assert "geometry cannot be none when initializing a CUQIarray as function values (with is_par False)." in str(e.value) # this message
     assert e.type == ValueError   
 
 def test_violin_plot():
     """ Test that the violin plot is generated correctly. """
     dist = cuqi.distribution.DistributionGallery("CalSom91")
-    sampler = cuqi.sampler.MetropolisHastings(dist)
+    sampler = cuqi.sampler.MH(dist)
     samples = sampler.sample_adapt(1000)
     samples.geometry = cuqi.geometry.Discrete(["alpha","beta"])
 
     ax = samples.plot_violin(shade=0.1)
 
     assert ax[0].get_title() == "alpha"
     assert ax[1].get_title() == "beta"
```

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_solver.py` & `CUQIpy-0.4.0/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_testproblem.py` & `CUQIpy-0.4.0/tests/test_testproblem.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         TP = cuqi.testproblem.Deconvolution1D(dim=128, phantom=np.ones((128, 128)))
 
     # Test raising of error if phantom is not same length as dim
     with pytest.raises(ValueError, match=r"phantom must be a 1D array of length dim"):
         TP = cuqi.testproblem.Deconvolution1D(dim=128, phantom=np.ones(125))
 
 
-@pytest.mark.parametrize("model_class", [cuqi.testproblem.Poisson_1D, cuqi.testproblem.Heat_1D])
+@pytest.mark.parametrize("model_class", [cuqi.testproblem.Poisson1D, cuqi.testproblem.Heat1D])
 @pytest.mark.parametrize("observation_map, expected_grid_equal",
                          [(None, True),
                           (lambda x: x[np.where(x > np.pi/2)], False)])
 def test_testproblem_pde_grid_obs(model_class, observation_map, expected_grid_equal):
     """ Test that the observation operator works on grids or not. """
     N = 128
     L = np.pi
@@ -113,49 +113,49 @@
     L = np.pi   # Length of domain
     amp_fact = 10
     f = lambda xs: 10*np.exp( -( (xs - 0.5)**2 ) / 0.02)
     map = lambda x: np.exp(amp_fact*x)
     dx = L/(N-1)
     x = np.linspace(dx/2,L-dx/2,N)
     true_kappa = np.exp( 5*x*np.exp(-2*x)*np.sin(L-x) )
-    model = cuqi.testproblem.Poisson_1D(dim=N, endpoint=L, source=f, field_type="KL", map=map).model
+    model = cuqi.testproblem.Poisson1D(dim=N, endpoint=L, source=f, field_type="KL", map=map).model
 
     assert np.linalg.norm(model.forward(true_kappa, is_par=False)) == approx(6.183419642601269)
     assert np.linalg.norm(model.forward(np.ones(model.domain_dim))) == approx(5.195849938761418)
 
 def test_Heat():
     # %% HEAT
     N = 128
     L = np.pi
     dx = L/(N+1)
     x = np.linspace(dx,L,N,endpoint=False)
     true_kappa = x*np.exp(-2*x)*np.sin(L-x)
-    model = cuqi.testproblem.Heat_1D(dim=N, endpoint=L, field_type="KL").model
+    model = cuqi.testproblem.Heat1D(dim=N, endpoint=L, field_type="KL").model
 
     assert np.linalg.norm(model.forward(true_kappa, is_par=False)) == approx(0.5476375563249378)
     assert np.linalg.norm(model.forward(np.ones(model.domain_dim))) == approx(0.548657107830281)
 
 def test_Abel():
     N = 128
     L = 1
     h = L/N
     tvec = np.linspace(h/2, L-h/2, N)
     true_image = np.sin(tvec*np.pi)*np.exp(-2*tvec)
     KL_map = lambda x: 10*x
-    model = cuqi.testproblem.Abel_1D(dim=N, endpoint=L, field_type="KL", KL_map=KL_map).model
+    model = cuqi.testproblem.Abel1D(dim=N, endpoint=L, field_type="KL", KL_map=KL_map).model
 
     assert np.linalg.norm(model.forward(true_image, is_par=False)) == approx(4.580752014966276)
     assert np.linalg.norm(model.forward(np.ones(model.domain_dim))) == approx(9.37456136258068)
 
 #Deconv 2D tests
 #TODO. Add tests for custom PSF
 @pytest.mark.parametrize("prior",[
     (cuqi.distribution.Gaussian(np.zeros(128**2), 1, name="x")),
-    #(cuqi.distribution.Laplace_diff(np.zeros(128**2), 1, "zeros")),
-    #(cuqi.distribution.Cauchy_diff(np.zeros(128**2), 1, "zeros")),
+    #(cuqi.distribution.LMRF(np.zeros(128**2), 1, "zeros")),
+    #(cuqi.distribution.CMRF(np.zeros(128**2), 1, "zeros")),
 ])
 def test_Deconvolution2D_Sampling_prior(prior): 
     tp = cuqi.testproblem.Deconvolution2D(prior=prior)
     tp.prior.geometry = tp.model.domain_geometry
     tp.sample_posterior(10) # Tests that sampling at least runs withour error.
     #TODO. Make into regression tests + other samplers. Move some tests to BayesianProblem
 
@@ -195,8 +195,14 @@
 
     # Compare forward
     assert np.allclose(forward(x), TP.model.forward(x).funvals)
     
     # Compare adjoint
     assert np.allclose(adjoint(y), TP.model.adjoint(y).funvals)
 
+def test_WangCubic():
+    """ Test the WangCubic testproblem with simple regression test"""
+    TP = cuqi.testproblem.WangCubic()
+    assert TP.posterior.logd([0.7, 1.3]) == approx(-119.4710156)
+    assert np.allclose(TP.posterior.gradient([0.7, 1.3]), np.array([[26.174, -153.5]]))
+
```

### Comparing `CUQIpy-0.3.0.post0.dev7/tests/test_utilities.py` & `CUQIpy-0.4.0/tests/test_utilities.py`

 * *Files identical despite different names*

