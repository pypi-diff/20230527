# Comparing `tmp/jaxopt-0.6.tar.gz` & `tmp/jaxopt-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxopt-0.6.tar", last modified: Thu Feb  9 15:55:00 2023, max compression
+gzip compressed data, was "jaxopt-0.7.tar", last modified: Fri May 26 21:59:11 2023, max compression
```

## Comparing `jaxopt-0.6.tar` & `jaxopt-0.7.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:55:00.685740 jaxopt-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-02-09 15:54:49.000000 jaxopt-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-02-09 15:55:00.681740 jaxopt-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-02-09 15:54:49.000000 jaxopt-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:55:00.681740 jaxopt-0.6/jaxopt/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:55:00.681740 jaxopt-0.6/jaxopt/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/anderson.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/anderson_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/armijo_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/backtracking_linesearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/bfgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/bisection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/block_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/cd_qp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/cvxpy_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/eq_qp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/fixed_point_iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/gauss_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/gradient_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/hager_zhang_linesearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/implicit_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/isotonic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/iterative_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/lbfgs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19174 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/levenberg_marquardt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/linear_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/mirror_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/nonlinear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/optax_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    42799 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/osqp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/polyak_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/projected_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    28465 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/prox.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/proximal_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    27813 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/scipy_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/tree_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/_src/zoom_linesearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/implicit_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/isotonic.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/linear_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/prox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/tree_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-09 15:54:49.000000 jaxopt-0.6/jaxopt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:55:00.681740 jaxopt-0.6/jaxopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-02-09 15:55:00.000000 jaxopt-0.6/jaxopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-02-09 15:55:00.000000 jaxopt-0.6/jaxopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 15:55:00.000000 jaxopt-0.6/jaxopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-09 15:55:00.000000 jaxopt-0.6/jaxopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-09 15:55:00.000000 jaxopt-0.6/jaxopt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 15:55:00.685740 jaxopt-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-02-09 15:54:49.000000 jaxopt-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:59:11.237593 jaxopt-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-26 21:58:59.000000 jaxopt-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-26 21:59:11.237593 jaxopt-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-26 21:58:59.000000 jaxopt-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:59:11.233593 jaxopt-0.7/jaxopt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:59:11.237593 jaxopt-0.7/jaxopt/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/anderson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/anderson_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/armijo_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/backtracking_linesearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/bfgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/bisection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/block_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/cd_qp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/cvxpy_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/eq_qp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/fixed_point_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/gauss_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/gradient_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17578 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/hager_zhang_linesearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/implicit_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/isotonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/iterative_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/lbfgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23341 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/lbfgsb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19174 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/levenberg_marquardt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/linear_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/mirror_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/nonlinear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/optax_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42799 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/osqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/polyak_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/projected_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28465 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/prox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/proximal_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29672 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/scipy_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/_src/zoom_linesearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/implicit_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/isotonic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/linear_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/prox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-26 21:58:59.000000 jaxopt-0.7/jaxopt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:59:11.233593 jaxopt-0.7/jaxopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-26 21:59:11.000000 jaxopt-0.7/jaxopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-26 21:59:11.000000 jaxopt-0.7/jaxopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:59:11.000000 jaxopt-0.7/jaxopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 21:59:11.000000 jaxopt-0.7/jaxopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 21:59:11.000000 jaxopt-0.7/jaxopt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:59:11.237593 jaxopt-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-26 21:58:59.000000 jaxopt-0.7/setup.py
```

### Comparing `jaxopt-0.6/LICENSE` & `jaxopt-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/PKG-INFO` & `jaxopt-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxopt
-Version: 0.6
+Version: 0.7
 Summary: Hardware accelerated, batchable and differentiable optimizers in JAX.
 Home-page: https://github.com/google/jaxopt
 Author: Google LLC
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: optimization,root finding,implicit differentiation,jax
 Classifier: Intended Audience :: Science/Research
```

### Comparing `jaxopt-0.6/README.md` & `jaxopt-0.7/README.md`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/__init__.py` & `jaxopt-0.7/jaxopt/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from jaxopt import implicit_diff
+from jaxopt import isotonic
 from jaxopt import loss
 from jaxopt import objective
 from jaxopt import projection
 from jaxopt import prox
 
 from jaxopt._src.anderson import AndersonAcceleration
 from jaxopt._src.anderson_wrapper import AndersonWrapper
@@ -31,14 +32,15 @@
 from jaxopt._src.eq_qp import EqualityConstrainedQP
 from jaxopt._src.fixed_point_iteration import FixedPointIteration
 from jaxopt._src.gauss_newton import GaussNewton
 from jaxopt._src.gradient_descent import GradientDescent
 from jaxopt._src.hager_zhang_linesearch import HagerZhangLineSearch
 from jaxopt._src.iterative_refinement import IterativeRefinement
 from jaxopt._src.lbfgs import LBFGS
+from jaxopt._src.lbfgsb import LBFGSB
 from jaxopt._src.levenberg_marquardt import LevenbergMarquardt
 from jaxopt._src.mirror_descent import MirrorDescent
 from jaxopt._src.nonlinear_cg import NonlinearCG
 from jaxopt._src.optax_wrapper import OptaxSolver
 from jaxopt._src.osqp import BoxOSQP
 from jaxopt._src.osqp import OSQP
 from jaxopt._src.polyak_sgd import PolyakSGD
```

### Comparing `jaxopt-0.6/jaxopt/_src/__init__.py` & `jaxopt-0.7/jaxopt/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/anderson.py` & `jaxopt-0.7/jaxopt/_src/anderson.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/anderson_wrapper.py` & `jaxopt-0.7/jaxopt/_src/anderson_wrapper.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/armijo_sgd.py` & `jaxopt-0.7/jaxopt/_src/armijo_sgd.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/backtracking_linesearch.py` & `jaxopt-0.7/jaxopt/_src/backtracking_linesearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
   value: float
   error: float
   done: bool
   params: Any
   grad: Any
   num_fun_eval: int
   num_grad_eval: int
+  failed: bool
   aux: Optional[Any] = None
 
 
 @dataclass(eq=False)
 class BacktrackingLineSearch(base.IterativeLineSearch):
   """Backtracking line search.
 
@@ -129,15 +130,16 @@
                                        aux=None,  # we do not need to have aux in the
                                        # initial state
                                        error=jnp.asarray(jnp.inf),
                                        params=params,
                                        num_fun_eval=num_fun_eval,
                                        num_grad_eval=num_grad_eval,
                                        done=jnp.asarray(False),
-                                       grad=grad)
+                                       grad=grad,
+                                       failed=jnp.asarray(False))
 
   def update(self,
              stepsize: float,
              state: NamedTuple,
              params: Any,
              value: Optional[float] = None,
              grad: Optional[Any] = None,
@@ -229,24 +231,26 @@
       raise ValueError("condition should be one of "
                        "'armijo', 'goldstein', 'strong-wolfe' or 'wolfe'.")
 
     new_stepsize = jnp.where(error <= self.tol,
                              stepsize,
                              stepsize * self.decrease_factor)
     done = state.done | (error <= self.tol)
+    failed = state.failed | ((state.iter_num + 1 == self.maxiter) & ~done)
 
     new_state = BacktrackingLineSearchState(iter_num=state.iter_num + 1,
                                             value=new_value,
                                             aux=new_aux,
                                             grad=new_grad,
                                             params=new_params,
                                             num_fun_eval=num_fun_eval,
                                             num_grad_eval=num_grad_eval,
                                             done=done,
-                                            error=error)
+                                            error=error,
+                                            failed=failed)
 
     return base.LineSearchStep(stepsize=new_stepsize, state=new_state)
 
   def __post_init__(self):
     if self.value_and_grad:
       self._value_and_grad_fun = self.fun
     else:
```

### Comparing `jaxopt-0.6/jaxopt/_src/base.py` & `jaxopt-0.7/jaxopt/_src/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -52,49 +52,148 @@
 
 class KKTSolution(NamedTuple):
   primal: Any
   dual_eq: Optional[Any] = None
   dual_ineq: Optional[Any] = None
 
 
-def _make_funs_with_aux(fun: Callable,
-                        value_and_grad: bool,
-                        has_aux: bool):
-  """
-  This utility creates fun, grad_fun and value_and_grad_fun functions
-  with aux output. If `has_aux` is False, then a None aux is returned.
-  If `value_and_grad` is True, `fun` is assumed to return both a value and a
-  gradient.
-  """
-  if value_and_grad:
+# pylint: disable=g-bare-generic
+def _add_aux_to_value_and_grad(value_and_grad: Callable) -> Callable:
+  def value_and_grad_with_aux(*a, **kw):
+    v, g = value_and_grad(*a, **kw)
+    return (v, None), g
+
+  return value_and_grad_with_aux
+
+
+def _add_aux_to_fun(fun: Callable) -> Callable:
+  def fun_with_aux(*a, **kw):
+    return fun(*a, **kw), None
+
+  return fun_with_aux
+
+
+def _split_value_and_grad_with_aux(
+    value_and_grad_with_aux: Callable,
+) -> Callable:
+  def fun_with_aux(*a, **kw):
+    (v, aux), _ = value_and_grad_with_aux(*a, **kw)
+    return (v, aux)
+
+  def grad_with_aux(*a, **kw):
+    (_, aux), g = value_and_grad_with_aux(*a, **kw)
+    return (g, aux)
+
+  return fun_with_aux, grad_with_aux
+
+
+def _remove_aux_from_value_and_grad(
+    value_and_grad_with_aux: Callable,
+) -> Tuple[Callable, Callable, Callable]:
+  def grad_without_aux(*a, **kw):
+    (_, aux), g = value_and_grad_with_aux(*a, **kw)
+    return g
+
+  def fun_without_aux(*a, **kw):
+    (v, aux), g = value_and_grad_with_aux(*a, **kw)
+    return v
+
+  def value_and_grad_without_aux(*a, **kw):
+    (v, aux), g = value_and_grad_with_aux(*a, **kw)
+    return (v, g)
+
+  return fun_without_aux, grad_without_aux, value_and_grad_without_aux
+
+
+def _make_funs_without_aux(
+    fun: Callable,
+    value_and_grad: Union[bool, Callable],
+    has_aux: bool,
+) -> Tuple[Callable, Callable, Callable]:
+  """Creates fun, grad_fun and value_and_grad_fun functions without aux."""
+  if isinstance(value_and_grad, bool) and value_and_grad:
     # Case when `fun` is a user-provided `value_and_grad`.
+    if has_aux:
+      return _remove_aux_from_value_and_grad(fun)
+    else:
+      return _remove_aux_from_value_and_grad(_add_aux_to_value_and_grad(fun))
+  if isinstance(value_and_grad, bool) and not value_and_grad:
+    # Case when `fun` is just a scalar-valued function.
+    if has_aux:
+      return _remove_aux_from_value_and_grad(
+          jax.value_and_grad(fun, has_aux=True)
+      )
+    else:
+      value_and_grad_ = jax.value_and_grad(fun)
+      grad = lambda *a, **ka: value_and_grad_(*a, **ka)[1]
+      return fun, grad, value_and_grad_
+  else:
+    # Case when `fun` is the value function, and `value_and_grad` returns
+    # both value and grad.
+    if has_aux:
+      fun_ = lambda *a, **ka: fun(*a, **ka)[0]
+      _, grad_, value_and_grad_ = _remove_aux_from_value_and_grad(
+          value_and_grad
+      )
+      return fun_, grad_, value_and_grad_
+    else:
+      grad_ = lambda *a, **ka: value_and_grad(*a, **ka)[1]
+      return fun, grad_, value_and_grad
 
+
+def _make_funs_with_aux(
+    fun: Callable,
+    value_and_grad: Union[bool, Callable],
+    has_aux: bool,
+):
+  """Creates fun, grad_fun and value_and_grad_fun functions with aux output.
+
+  Args:
+    fun:
+    value_and_grad: If `value_and_grad` is True, `fun` should return both value
+      and gradient. If `value_and_grad` is a Callable, `fun` should return value
+      only, and `value_and_grad` returns value and gradient.
+    has_aux: If `has_aux` is True, then any Callable arguments should return
+      `(value, aux)` tuple in place of just `value`.
+
+  Returns:
+    Three callables, fun, grad, and value_and_grad.
+    `fun` returns (value, aux) tuple.
+    `grad` returns (grad, aux) tuple.
+    `value_and_grad` returns ((value, aux), grad) nested tuple.
+    If has_aux is False, then all three returned functions return aux=None.
+  """
+  if isinstance(value_and_grad, bool) and value_and_grad:
+    # Case when `fun` is a user-provided `value_and_grad`.
     if has_aux:
-      fun_ = lambda *a, **kw: fun(*a, **kw)[0]
-      value_and_grad_fun = fun
+      value_and_grad_ = fun
     else:
-      fun_ = lambda *a, **kw: (fun(*a, **kw)[0], None)
-      def value_and_grad_fun(*a, **kw):
-        v, g = fun(*a, **kw)
-        return (v, None), g
+      value_and_grad_ = _add_aux_to_value_and_grad(fun)
+    fun_, grad_ = _split_value_and_grad_with_aux(value_and_grad_)
+    return fun_, grad_, value_and_grad_
 
-  else:
+  if isinstance(value_and_grad, bool) and not value_and_grad:
     # Case when `fun` is just a scalar-valued function.
     if has_aux:
       fun_ = fun
     else:
-      fun_ = lambda p, *a, **kw: (fun(p, *a, **kw), None)
-
-    value_and_grad_fun = jax.value_and_grad(fun_, has_aux=True)
-
-  def grad_fun(*a, **kw):
-    (v, a), g = value_and_grad_fun(*a, **kw)
-    return g, a
+      fun_ = _add_aux_to_fun(fun)
+    value_and_grad_ = jax.value_and_grad(fun_, has_aux=True)
+  else:
+    # Case when `fun` is the value function, and `value_and_grad` returns
+    # both value and grad.
+    if has_aux:
+      fun_ = fun
+      value_and_grad_ = value_and_grad
+    else:
+      fun_ = _add_aux_to_fun(fun)
+      value_and_grad_ = _add_aux_to_value_and_grad(value_and_grad)
 
-  return fun_, grad_fun, value_and_grad_fun
+  _, grad_ = _split_value_and_grad_with_aux(value_and_grad_)
+  return fun_, grad_, value_and_grad_
 
 
 class Solver(abc.ABC):
   """Base class for solvers.
 
   A solver should implement a `run` method:
 
@@ -377,8 +476,7 @@
           grad: Optional[Any] = None,
           descent_direction: Optional[Any] = None,
           *args,
           **kwargs) -> LineSearchStep:
 
     return super()._run(init_stepsize, params, value, grad, descent_direction,
                         *args, **kwargs)
-
```

### Comparing `jaxopt-0.6/jaxopt/_src/bfgs.py` & `jaxopt-0.7/jaxopt/_src/bfgs.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/bisection.py` & `jaxopt-0.7/jaxopt/_src/bisection.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/block_cd.py` & `jaxopt-0.7/jaxopt/_src/block_cd.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/cd_qp.py` & `jaxopt-0.7/jaxopt/_src/cd_qp.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/cvxpy_wrapper.py` & `jaxopt-0.7/jaxopt/_src/cvxpy_wrapper.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/eq_qp.py` & `jaxopt-0.7/jaxopt/_src/eq_qp.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/fixed_point_iteration.py` & `jaxopt-0.7/jaxopt/_src/fixed_point_iteration.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/gauss_newton.py` & `jaxopt-0.7/jaxopt/_src/gauss_newton.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/gradient_descent.py` & `jaxopt-0.7/jaxopt/_src/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/hager_zhang_linesearch.py` & `jaxopt-0.7/jaxopt/_src/hager_zhang_linesearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
   done: bool
   low: float
   high: float
   value: float
   error: float
   params: Any
   grad: Any
+  failed: bool
   aux: Optional[Any] = None
 
 
 @dataclass(eq=False)
 class HagerZhangLineSearch(base.IterativeLineSearch):
   """Hager-Zhang line search.
 
@@ -235,24 +236,25 @@
 
   def _bracket(
       self, x, c, approx_wolfe_threshold_value,
       descent_direction, *args, **kwargs):
     # Initial interval that satisfies the opposite slope condition.
 
     def cond_fn(state):
-      return jnp.any(~state[0])
+      return jnp.any(~state[0]) | jnp.any(state[-1])
 
     def body_fn(state):
       (done,
        low,
        middle,
        high,
        value_middle,
        grad_middle,
-       best_middle) = state
+       best_middle,
+       failed) = state
       # Correspond to B1 in the paper.
       update_right_endpoint = grad_middle >= 0.
       new_high = jnp.where(~done & update_right_endpoint, middle, high)
       new_low = jnp.where(~done & update_right_endpoint, best_middle, low)
       done = done | update_right_endpoint
 
       # Correspond to B2 in the paper.
@@ -281,36 +283,42 @@
 
       # Corresponds to B3 in the paper. Increase the point and recompute.
       new_middle = jnp.where(~done, self.expansion_factor * middle, middle)
 
       new_value_middle, new_grad_middle = self._value_and_grad_on_line(
           x, new_middle, descent_direction, *args, **kwargs)
 
+      # Terminate on encountering NaNs to avoid an infinite loop.
+      failed = (failed |
+                jnp.any(jnp.isnan(new_value_middle)) |
+                jnp.any(jnp.isnan(new_grad_middle)))
       return (done,
               new_low,
               new_middle,
               new_high,
               new_value_middle,
               new_grad_middle,
-              best_middle)
+              best_middle,
+              failed)
 
     value_c, grad_c = self._value_and_grad_on_line(
         x, c, descent_direction, *args, **kwargs)
 
-    _, final_low, _, final_high, _, _, _ = jax.lax.while_loop(
+    _, final_low, _, final_high, _, _, _, failed = jax.lax.while_loop(
         cond_fn,
         body_fn,
         (jnp.array(False),
          jnp.array(0.),
          c,
          c,
          value_c,
          grad_c,
-         jnp.array(0.)))
-    return final_low, final_high
+         jnp.array(0.),
+         jnp.array(False)))
+    return final_low, final_high, failed
 
   def init_state(self,  # pylint:disable=keyword-arg-before-vararg
                  init_stepsize: float,
                  params: Any,
                  value: Optional[float] = None,
                  grad: Optional[Any] = None,
                  descent_direction: Optional[Any] = None,
@@ -341,15 +349,15 @@
     if descent_direction is None:
       descent_direction = tree_scalar_mul(-1, grad)
 
     approx_wolfe_threshold_value = (
         value + self.approximate_wolfe_threshold * jnp.abs(value))
 
     # Create initial interval.
-    low, high = self._bracket(
+    low, high, failed = self._bracket(
         params, jnp.ones_like(value),
         approx_wolfe_threshold_value, descent_direction, *args, **kwargs)
 
     value_low, grad_low = self._value_and_grad_on_line(
         params, low, descent_direction, *args, **kwargs)
 
     value_high, grad_high = self._value_and_grad_on_line(
@@ -374,15 +382,16 @@
         low=low,
         high=high,
         error=error,
         done=done,
         value=value,
         aux=None,  # we do not need to have aux in the initial state
         params=params,
-        grad=grad)
+        grad=grad,
+        failed=failed)
 
   def update(self,  # pylint:disable=keyword-arg-before-vararg
              stepsize: float,
              state: NamedTuple,
              params: Any,
              value: Optional[float] = None,
              grad: Optional[Any] = None,
@@ -406,15 +415,14 @@
 
     if value is None or grad is None:
       if self.has_aux:
         (value, _), grad = self._value_and_grad_fun(params, *args, **kwargs)
       else:
         value, grad = self._value_and_grad_fun(params, *args, **kwargs)
 
-
     if descent_direction is None:
       descent_direction = tree_scalar_mul(-1, grad)
 
     approx_wolfe_threshold_value = (
         value + self.approximate_wolfe_threshold * jnp.abs(value))
 
     new_low, new_high = self._secant2(
@@ -467,25 +475,27 @@
                           value_best_point,
                           gd_vdot_best_point,
                           value,
                           grad,
                           approx_wolfe_threshold_value,
                           descent_direction))
     done = state.done | (error <= self.tol)
+    failed = state.failed | ((state.iter_num + 1 == self.maxiter) & ~done)
 
     new_state = HagerZhangLineSearchState(
         iter_num=state.iter_num + 1,
         value=new_value,
         grad=new_grad,
         aux=new_aux,
         params=new_params,
         low=new_low,
         high=new_high,
         error=error,
-        done=done)
+        done=done,
+        failed=failed)
 
     return base.LineSearchStep(stepsize=new_stepsize, state=new_state)
 
   def __post_init__(self):
     if self.value_and_grad:
       self._value_and_grad_fun = self.fun
     else:
```

### Comparing `jaxopt-0.6/jaxopt/_src/implicit_diff.py` & `jaxopt-0.7/jaxopt/_src/implicit_diff.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/isotonic.py` & `jaxopt-0.7/jaxopt/_src/isotonic.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/iterative_refinement.py` & `jaxopt-0.7/jaxopt/_src/iterative_refinement.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/lbfgs.py` & `jaxopt-0.7/jaxopt/_src/lbfgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,24 +387,26 @@
                                         *args, **kwargs)
         new_params = ls_state.params
         new_value = ls_state.value
         new_grad = ls_state.grad
         new_aux = ls_state.aux
       else:
         raise ValueError("Invalid name in 'linesearch' option.")
+      failed_linesearch = ls_state.failed
 
     else:
       # without line search
       if isinstance(self.stepsize, Callable):
         new_stepsize = self.stepsize(state.iter_num)
       else:
         new_stepsize = self.stepsize
 
       new_params = tree_add_scalar_mul(params, new_stepsize, descent_direction)
       (new_value, new_aux), new_grad = self._value_and_grad_with_aux(new_params, *args, **kwargs)
+      failed_linesearch = jnp.asarray(False)
     s = tree_sub(new_params, params)
     y = tree_sub(new_grad, grad)
     vdot_sy = tree_vdot(s, y)
     rho = jnp.where(vdot_sy == 0, 0, 1. / vdot_sy)
 
     last = (start + self.history_size) % self.history_size
     s_history = update_history(state.s_history, s, last)
@@ -412,19 +414,14 @@
     rho_history = update_history(state.rho_history, rho, last)
 
     if self.use_gamma:
       gamma = compute_gamma(s_history, y_history, last)
     else:
       gamma = jnp.array(1.0)
 
-    if use_linesearch and self.linesearch == "zoom":
-      failed_linesearch = ls_state.failed
-    else:  # backtracking linesearch doesn't support failed state yet
-      failed_linesearch = jnp.asarray(False)
-
     new_state = LbfgsState(iter_num=state.iter_num + 1,
                            value=new_value,
                            grad=new_grad,
                            stepsize=jnp.asarray(new_stepsize),
                            error=tree_l2_norm(new_grad),
                            s_history=s_history,
                            y_history=y_history,
```

### Comparing `jaxopt-0.6/jaxopt/_src/levenberg_marquardt.py` & `jaxopt-0.7/jaxopt/_src/levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/linear_operator.py` & `jaxopt-0.7/jaxopt/_src/linear_operator.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/linear_solve.py` & `jaxopt-0.7/jaxopt/_src/linear_solve.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/loop.py` & `jaxopt-0.7/jaxopt/_src/loop.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/loss.py` & `jaxopt-0.7/jaxopt/_src/loss.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/mirror_descent.py` & `jaxopt-0.7/jaxopt/_src/mirror_descent.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/nonlinear_cg.py` & `jaxopt-0.7/jaxopt/_src/nonlinear_cg.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/objective.py` & `jaxopt-0.7/jaxopt/_src/objective.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/optax_wrapper.py` & `jaxopt-0.7/jaxopt/_src/optax_wrapper.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/osqp.py` & `jaxopt-0.7/jaxopt/_src/osqp.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/perturbations.py` & `jaxopt-0.7/jaxopt/_src/perturbations.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,26 +41,29 @@
   def log_prob(self, inputs: jax.Array) -> jax.Array:
     return -inputs - jnp.exp(-inputs)
 
 
 def make_perturbed_argmax(argmax_fun: Callable[[jax.Array], jax.Array],
                           num_samples: int = 1000,
                           sigma: float = 0.1,
-                          noise=Gumbel()):
+                          noise=Gumbel(),
+                          control_variate: bool = False):
   """Transforms a function into a differentiable version with perturbations.
 
   Args:
     argmax_fun: the argmax function to transform into a differentiable version.
-      The signature for argmax_fn currently supported for custom jvp and jit is:
+      Signature for argmax_fun currently supported for custom jvp and jit is:
       + input [D1, ..., Dk], output [D1, ..., Dk], k >= 1
     num_samples: an int, the number of perturbed outputs to average over.
     sigma: a float, the scale of the random perturbation.
     noise: a distribution object that must implement a sample function and a
       log-pdf of the desired distribution, similar to the examples above.
       Default is Gumbel distribution.
+    control_variate : Boolean indicating whether a control variate is used in
+      the Monte-Carlo estimate of the Jacobian.
 
   Returns:
     A function with the same signature (and an rng) that can be differentiated.
 
   Example:
     Given an argmax function such as::
 
@@ -77,15 +80,15 @@
       pert_argmax = pert_argmax_fun(x, rng)
 
     When handling a batched input, vmap can be applied to this function, with
     some care in splitting the rng key::
 
       batch_size = x_batch.shape[0]
       rngs_batch = jax.random.split(rng, batch_size)
-      pert_argmax = jax.vmap(pert_argmax_fun)(x_batch, rngs_batch)
+      pert_argmax_batch = jax.vmap(pert_argmax_fun)(x_batch, rngs_batch)
 
     Further, if the argmax_fun is jittable, then so is pert_argmax_fun.
   """
 
   @jax.custom_jvp
   def forward_pert(inputs, rng):
     samples = noise.sample(seed=rng,
@@ -102,28 +105,45 @@
     tangent_flat = 1.0 / (num_samples * sigma) * jnp.einsum(
         'nd,ne,e->d',
         jnp.reshape(output_pert, (num_samples, -1)),
         jnp.reshape(nabla_z_flat, (num_samples, -1)),
         jnp.reshape(tangent, (-1,)))
     return jnp.reshape(tangent_flat, inputs.shape)
 
-  forward_pert.defjvps(pert_jvp, None)
+  def pert_jvp_control_variate(tangent, _, inputs, rng):
+    samples = noise.sample(seed=rng,
+                           sample_shape=(num_samples,) + inputs.shape)
+    output_pert = jax.vmap(argmax_fun)(inputs + sigma * samples)
+    output = argmax_fun(inputs)
+    # noise.log_prob corresponds to -nu in the paper.
+    nabla_z_flat = -jax.vmap(jax.grad(noise.log_prob))(samples.reshape([-1]))
+    tangent_flat = 1.0 / (num_samples * sigma) * jnp.einsum(
+        'nd,ne,e->d',
+        jnp.reshape(output_pert - output, (num_samples, -1)),
+        jnp.reshape(nabla_z_flat, (num_samples, -1)),
+        jnp.reshape(tangent, (-1,)))
+    return jnp.reshape(tangent_flat, inputs.shape)
+
+  if control_variate:
+      forward_pert.defjvps(pert_jvp_control_variate, None)
+  else:
+      forward_pert.defjvps(pert_jvp, None)
 
   return forward_pert
 
 
 def make_perturbed_max(argmax_fun: Callable[[jax.Array], jax.Array],
                        num_samples: int = 1000,
                        sigma: float = 0.1,
                        noise=Gumbel()):
   """Turns an argmax in a differentiable version of the max with perturbations.
 
   Args:
     argmax_fun: the argmax function to transform into a differentiable version.
-      The signature for argmax_fn currently supported for custom jvp and jit is:
+      Signature for argmax_fun currently supported for custom jvp and jit is:
       + input [D1, ..., Dk], output [D1, ..., Dk], k >= 1
     num_samples: an int, the number of perturbed outputs to average over.
     sigma: a float, the scale of the random perturbation.
     noise: a distribution object that must implement a sample function and a
       log-pdf of the desired distribution, similar to the examples above.
       Default is Gumbel distribution.
 
@@ -146,15 +166,15 @@
       pert_max = pert_max_fun(x, rng)
 
     When handling a batched input, vmap can be applied to this function, with
     some care in splitting the rng key::
 
       batch_size = x_batch.shape[0]
       rngs_batch = jax.random.split(rng, batch_size)
-      pert_max = jax.vmap(pert_max_fun)(x_batch, rngs_batch)
+      pert_max_batch = jax.vmap(pert_max_fun)(x_batch, rngs_batch)
 
     Furthermore, if the argmax_fun is jittable, then so is pert_max_fun.
   """
 
   @jax.custom_jvp
   def forward_pert(inputs, rng):
     samples = noise.sample(seed=rng,
@@ -173,7 +193,77 @@
                                             noise)
     pert_argmax = pert_argmax_fun(inputs, rng)
     return jnp.sum(pert_argmax * tangent)
 
   forward_pert.defjvps(pert_jvp, None)
 
   return forward_pert
+
+
+def make_perturbed_fun(fun: Callable[[jax.Array], float],
+                       num_samples: int = 1000,
+                       sigma: float = 0.1,
+                       noise=Gumbel()):
+  """Transforms a function into a differentiable version with perturbations.
+
+  Args:
+    fun: the function to transform into a differentiable version.
+      Signature for fun currently supported for custom jvp and jit is:
+      + input [D1, ..., Dk], output [R_1, ..., R_r]
+    num_samples: an int, the number of perturbed outputs to average over.
+    sigma: a float, the scale of the random perturbation.
+    noise: a distribution object that must implement a sample function and a
+      log-pdf of the desired distribution, similar to the examples above.
+      Default is Gumbel distribution.
+
+  Returns:
+    A function with the same signature (and an rng) that can be differentiated.
+
+  Example:
+    Given an argmax function such as::
+
+      def fun(x):
+        return jax.nn.relu(x)
+
+      pert_fun = make_perturbed_fun(fun,
+                                    num_samples=200,
+                                    sigma=0.01)
+
+    Then pert_fun is differentiable, a perturbed version of fun.
+    Since it relies on randomness, it requires an rng key::
+
+      pert_output = pert_fun(x, rng)
+
+    When handling a batched input, vmap can be applied to this function, with
+    some care in splitting the rng key::
+
+      batch_size = x_batch.shape[0]
+      rngs_batch = jax.random.split(rng, batch_size)
+      pert_batch = jax.vmap(pert_fun)(x_batch, rngs_batch)
+
+    Further, if fun is jittable, then so is pert_fun.
+  """
+
+  @jax.custom_jvp
+  def forward_pert(inputs, rng):
+    samples = noise.sample(seed=rng,
+                           sample_shape=(num_samples,) + inputs.shape)
+    output_pert = jax.vmap(fun)(inputs + sigma * samples)
+    return jnp.mean(output_pert, axis=0)
+
+  def pert_jvp(tangent, _, inputs, rng):
+    samples = noise.sample(seed=rng,
+                           sample_shape=(num_samples,) + inputs.shape)
+    output_pert = jax.vmap(fun)(inputs + sigma * samples)[..., jnp.newaxis]
+    # noise.log_prob corresponds to -nu in the paper.
+    nabla_z_flat = -jax.vmap(jax.grad(noise.log_prob))(samples.reshape([-1]))
+    tangent_flat = 1.0 / (num_samples * sigma) * jnp.einsum(
+        'nd,ne,e->d',
+        jnp.reshape(output_pert, (num_samples, -1)),
+        jnp.reshape(nabla_z_flat, (num_samples, -1)),
+        jnp.reshape(tangent, (-1,)))
+    tangent_out = jnp.squeeze(jnp.reshape(tangent_flat, output_pert.shape[1:]))
+    return tangent_out
+
+  forward_pert.defjvps(pert_jvp, None)
+
+  return forward_pert
```

### Comparing `jaxopt-0.6/jaxopt/_src/polyak_sgd.py` & `jaxopt-0.7/jaxopt/_src/polyak_sgd.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/projected_gradient.py` & `jaxopt-0.7/jaxopt/_src/projected_gradient.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/projection.py` & `jaxopt-0.7/jaxopt/_src/projection.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/prox.py` & `jaxopt-0.7/jaxopt/_src/prox.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,17 +66,19 @@
 
   Returns:
     output pytree, with same structure as ``x``.
   """
   if l1reg is None:
     l1reg = 1.0
 
-  fun = lambda u, v: jnp.sign(u) * jax.nn.relu(jnp.abs(u) - v * scaling)
-  return tree_util.tree_map(fun, x, l1reg)
+  if type(l1reg) == float:
+    l1reg = tree_util.tree_map(lambda y: l1reg*jnp.ones_like(y), x)
 
+  def fun(u, v): return jnp.sign(u) * jax.nn.relu(jnp.abs(u) - v * scaling)
+  return tree_util.tree_map(fun, x, l1reg)
 
 def prox_non_negative_lasso(x: Any,
                             l1reg: Optional[float] = None,
                             scaling: float = 1.0) -> Any:
   r"""Proximal operator for the l1 norm on the non-negative orthant.
 
   .. math::
@@ -91,15 +93,15 @@
 
   Returns:
     output pytree, with the same structure as ``x``.
   """
   if l1reg is None:
     l1reg = 1.0
 
-  pytree = tree_util.tree_add(x, -l1reg * scaling)
+  pytree = tree_util.tree_map(lambda y: y - l1reg*scaling, x)
   return tree_util.tree_map(jax.nn.relu, pytree)
 
 
 def prox_elastic_net(x: Any,
                      hyperparams: Optional[Tuple[Any, Any]] = None,
                      scaling: float = 1.0) -> Any:
   r"""Proximal operator for the elastic net.
@@ -119,18 +121,24 @@
 
   Returns:
     output pytree, with the same structure as ``x``.
   """
   if hyperparams is None:
     hyperparams = (1.0, 1.0)
 
-  prox_l1 = lambda u, lam: jnp.sign(u) * jax.nn.relu(jnp.abs(u) - lam)
-  fun = lambda u, lam, gamma: (prox_l1(u, scaling * lam) /
-                               (1.0 + scaling * lam * gamma))
-  return tree_util.tree_map(fun, x, hyperparams[0], hyperparams[1])
+  lam = tree_util.tree_map(lambda y: hyperparams[0]*jnp.ones_like(
+      y), x) if type(hyperparams[0]) == float else hyperparams[0]
+  gam = tree_util.tree_map(lambda y: hyperparams[1]*jnp.ones_like(
+      y), x) if type(hyperparams[1]) == float else hyperparams[1]
+
+  def prox_l1(u, lambd): return jnp.sign(u) * jax.nn.relu(jnp.abs(u) - lambd)
+
+  def fun(u, lambd, gamma): return (prox_l1(u, scaling * lambd) /
+                                    (1.0 + scaling * lambd * gamma))
+  return tree_util.tree_map(fun, x, lam, gam)
 
 
 def prox_group_lasso(x: Any,
                      l2reg: Optional[float] = 1.0,
                      scaling=1.0) -> Any:
   r"""Proximal operator for the l2 norm, i.e., block soft-thresholding operator.
```

### Comparing `jaxopt-0.6/jaxopt/_src/proximal_gradient.py` & `jaxopt-0.7/jaxopt/_src/proximal_gradient.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/scipy_wrappers.py` & `jaxopt-0.7/jaxopt/_src/scipy_wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,44 +18,85 @@
 # TODO(fllinares): add support for methods requiring Hessian / Hessian prods.
 # TODO(fllinares): possibly hardcode `dtype` attribute, as likely useless.
 # TODO(pedregosa): add a 'maxiter' and 'callback' keyword option for all wrappers,
 #   currently only ScipyMinimize exposes this option.
 """
 
 import abc
+import dataclasses
 from dataclasses import dataclass
-
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import NamedTuple
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
 import jax
+from jax.config import config
 import jax.numpy as jnp
 import jax.tree_util as tree_util
-
+from jax.tree_util import register_pytree_node_class
 from jaxopt._src import base
 from jaxopt._src import implicit_diff as idf
 from jaxopt._src import projection
 from jaxopt._src.tree_util import tree_sub
-
 import numpy as onp
 import scipy as osp
+from scipy.optimize import LbfgsInvHessProduct
+
+
+@register_pytree_node_class
+class LbfgsInvHessProductPyTree(LbfgsInvHessProduct):
+  """
+  Registers the LbfgsInvHessProduct object as a PyTree.
+  This object is typically returned by the L-BFSG-B optimizer to efficiently 
+  store the inverse of the Hessian matrix evaluated at the best-fit parameters. 
+  """
+
+  def __init__(self, sk, yk):
+    """
+    Construct the operator.
+    This is the same constructor as the original LbfgsInvHessProduct class,
+    except that numpy has been replaced by jax.numpy and no call to the 
+    numpy.ndarray constuctor is performed.
+    """
+    if sk.shape != yk.shape or sk.ndim != 2:
+      raise ValueError('sk and yk must have matching shape, (n_corrs, n)')
+    n_corrs, n = sk.shape
+    self.dtype = jnp.float64 if config.jax_enable_x64 is True else jnp.float32
+    self.shape = (n, n)
+    self.sk = sk
+    self.yk = yk
+    self.n_corrs = n_corrs
+    self.rho = 1 / jnp.einsum('ij,ij->i', sk, yk)
+
+
+  def __repr__(self):
+      return "LbfgsInvHessProduct(sk={}, yk={})".format(self.sk, self.yk)
+
+  def tree_flatten(self):
+      children = (self.sk, self.yk)
+      aux_data = None
+      return (children, aux_data)
+
+  @classmethod
+  def tree_unflatten(cls, aux_data, children):
+      return cls(*children)
 
 
 class ScipyMinimizeInfo(NamedTuple):
   """Named tuple with results for `scipy.optimize.minimize` wrappers."""
   fun_val: jnp.ndarray
   success: bool
   status: int
   iter_num: int
+  hess_inv: Optional[Union[jnp.ndarray, LbfgsInvHessProductPyTree]]
 
 
 class ScipyRootInfo(NamedTuple):
   """Named tuple with results for `scipy.optimize.root` wrappers."""
   fun_val: float
   success: bool
   status: int
@@ -237,48 +278,38 @@
   """`scipy.optimize.minimize` wrapper
 
   This wrapper is for unconstrained minimization only.
   It supports pytrees and implicit diff.
 
   Attributes:
     fun: a smooth function of the form `fun(x, *args, **kwargs)`.
-    method: the `method` argument for `scipy.optimize.minimize`.
-      Should be one of
-        * 'Nelder-Mead'
-        * 'Powell'
-        * 'CG'
-        * 'BFGS'
-        * 'Newton-CG'
-        * 'L-BFGS-B'
-        * 'TNC'
-        * 'COBYLA'
-        * 'SLSQP'
-        * 'trust-constr'
-        * 'dogleg'
-        * 'trust-ncg'
-        * 'trust-exact'
-        * 'trust-krylov'
+    method: the `method` argument for `scipy.optimize.minimize`. Should be one
+      of * 'Nelder-Mead' * 'Powell' * 'CG' * 'BFGS' * 'Newton-CG' * 'L-BFGS-B' *
+      'TNC' * 'COBYLA' * 'SLSQP' * 'trust-constr' * 'dogleg' * 'trust-ncg' *
+      'trust-exact' * 'trust-krylov'
     tol: the `tol` argument for `scipy.optimize.minimize`.
     options: the `options` argument for `scipy.optimize.minimize`.
     callback: called after each iteration, as callback(xk), where xk is the
       current parameter vector.
     dtype: if not None, cast all NumPy arrays to this dtype. Note that some
       methods relying on FORTRAN code, such as the `L-BFGS-B` solver for
       `scipy.optimize.minimize`, require casting to float64.
     jit: whether to JIT-compile JAX-based values and grad evals.
     implicit_diff_solve: the linear system solver to use.
     has_aux: whether function `fun` outputs one (False) or more values (True).
       When True it will be assumed by default that `fun(...)[0]` is the
       objective.
+    value_and_grad: See base.make_funs_with_aux for more detail.
   """
   fun: Callable = None
   callback: Callable = None
   tol: Optional[float] = None
   options: Optional[Dict[str, Any]] = None
   maxiter: int = 500
+  value_and_grad: Union[bool, Callable] = False
 
   def optimality_fun(self, sol, *args, **kwargs):
     """Optimality function mapping compatible with `@custom_root`."""
     return self._grad_fun(sol, *args, **kwargs)
 
   def _run(self, init_params, bounds, *args, **kwargs):
     """Wraps `scipy.optimize.minimize`."""
@@ -308,18 +339,29 @@
                                 tol=self.tol,
                                 bounds=bounds,
                                 method=self.method,
                                 callback=scipy_callback,
                                 options=self.options)
 
     params = tree_util.tree_map(jnp.asarray, onp_to_jnp(res.x))
+
+    if hasattr(res, 'hess_inv'):
+      if isinstance(res.hess_inv, osp.optimize.LbfgsInvHessProduct):
+        hess_inv = LbfgsInvHessProductPyTree(res.hess_inv.sk,
+                                             res.hess_inv.yk)
+      elif isinstance(res.hess_inv, onp.ndarray):
+        hess_inv = jnp.asarray(res.hess_inv)
+    else:
+      hess_inv = None
+
     info = ScipyMinimizeInfo(fun_val=jnp.asarray(res.fun),
                              success=res.success,
                              status=res.status,
-                             iter_num=res.nit)
+                             iter_num=res.nit,
+                             hess_inv=hess_inv)
     return base.OptStep(params, info)
 
   def run(self,
           init_params: Any,
           *args,
           **kwargs) -> base.OptStep:
     """Runs the solver.
@@ -331,22 +373,21 @@
     Returns:
       (params, info).
     """
     return self._run(init_params, None, *args, **kwargs)
 
   def __post_init__(self):
     super().__post_init__()
-
-    if self.has_aux:
-      self.fun = lambda x, *args, **kwargs: self.fun(x, *args, **kwargs)[0]
+    self.fun, self._grad_fun, self._value_and_grad_fun = (
+        base._make_funs_without_aux(self.fun, self.value_and_grad, self.has_aux)
+    )
 
     # Pre-compile useful functions.
-    self._grad_fun = jax.grad(self.fun)
-    self._value_and_grad_fun = jax.value_and_grad(self.fun)
     if self.jit:
+      self.fun = jax.jit(self.fun)
       self._grad_fun = jax.jit(self._grad_fun)
       self._value_and_grad_fun = jax.jit(self._value_and_grad_fun)
 
     if self.options is None:
       self.options = {}
     if 'maxiter' in self.options:
       raise ValueError("Cannot pass maxiter through options dictionary, use maxiter keyword argument instead.")
```

### Comparing `jaxopt-0.6/jaxopt/_src/test_util.py` & `jaxopt-0.7/jaxopt/_src/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,29 +319,34 @@
     else:
       self.assertEqual(_dtype(x), _dtype(y))
 
   def assertAllClose(self, x, y, *, check_dtypes=True, atol=None, rtol=None,
                      canonicalize_dtypes=True, err_msg=''):
     """Assert that x and y, either arrays or nested tuples/lists, are close."""
     if isinstance(x, dict):
-      self.assertIsInstance(y, dict)
-      self.assertEqual(set(x.keys()), set(y.keys()))
+      self.assertIsInstance(y, dict, msg=err_msg)
+      self.assertEqual(set(x.keys()), set(y.keys()), msg=err_msg)
       for k in x.keys():
         self.assertAllClose(x[k], y[k], check_dtypes=check_dtypes, atol=atol,
                             rtol=rtol, canonicalize_dtypes=canonicalize_dtypes,
                             err_msg=err_msg)
     elif is_sequence(x) and not hasattr(x, '__array__'):
-      self.assertTrue(is_sequence(y) and not hasattr(y, '__array__'))
-      self.assertEqual(len(x), len(y))
+      self.assertTrue(
+          is_sequence(y) and not hasattr(y, '__array__'), msg=err_msg
+      )
+      self.assertEqual(len(x), len(y), msg=err_msg)
       for x_elt, y_elt in zip(x, y):
         self.assertAllClose(x_elt, y_elt, check_dtypes=check_dtypes, atol=atol,
                             rtol=rtol, canonicalize_dtypes=canonicalize_dtypes,
                             err_msg=err_msg)
     elif hasattr(x, '__array__') or onp.isscalar(x):
-      self.assertTrue(hasattr(y, '__array__') or onp.isscalar(y))
+      self.assertTrue(
+          hasattr(y, '__array__') or onp.isscalar(y),
+          msg=f'{err_msg}: {x} is an array but {y} is not.',
+      )
       if check_dtypes:
         self.assertDtypesMatch(x, y, canonicalize_dtypes=canonicalize_dtypes)
       x = onp.asarray(x)
       y = onp.asarray(y)
       self.assertArraysAllClose(x, y, check_dtypes=False, atol=atol, rtol=rtol,
                                 err_msg=err_msg)
     elif x == y:
```

### Comparing `jaxopt-0.6/jaxopt/_src/tree_util.py` & `jaxopt-0.7/jaxopt/_src/tree_util.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/_src/zoom_linesearch.py` & `jaxopt-0.7/jaxopt/_src/zoom_linesearch.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/base.py` & `jaxopt-0.7/jaxopt/base.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/implicit_diff.py` & `jaxopt-0.7/jaxopt/implicit_diff.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/isotonic.py` & `jaxopt-0.7/jaxopt/isotonic.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/linear_solve.py` & `jaxopt-0.7/jaxopt/linear_solve.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/loop.py` & `jaxopt-0.7/jaxopt/loop.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/loss.py` & `jaxopt-0.7/jaxopt/loss.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/objective.py` & `jaxopt-0.7/jaxopt/objective.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/perturbations.py` & `jaxopt-0.7/jaxopt/perturbations.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,7 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from jaxopt._src.perturbations import Gumbel
 from jaxopt._src.perturbations import Normal
 from jaxopt._src.perturbations import make_perturbed_argmax
 from jaxopt._src.perturbations import make_perturbed_max
+from jaxopt._src.perturbations import make_perturbed_fun
```

### Comparing `jaxopt-0.6/jaxopt/projection.py` & `jaxopt-0.7/jaxopt/projection.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/prox.py` & `jaxopt-0.7/jaxopt/prox.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/tree_util.py` & `jaxopt-0.7/jaxopt/tree_util.py`

 * *Files identical despite different names*

### Comparing `jaxopt-0.6/jaxopt/version.py` & `jaxopt-0.7/jaxopt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """JAXopt version."""
 
-__version__ = "0.6"
+__version__ = "0.7"
```

### Comparing `jaxopt-0.6/jaxopt.egg-info/PKG-INFO` & `jaxopt-0.7/jaxopt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxopt
-Version: 0.6
+Version: 0.7
 Summary: Hardware accelerated, batchable and differentiable optimizers in JAX.
 Home-page: https://github.com/google/jaxopt
 Author: Google LLC
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: optimization,root finding,implicit differentiation,jax
 Classifier: Intended Audience :: Science/Research
```

### Comparing `jaxopt-0.6/jaxopt.egg-info/SOURCES.txt` & `jaxopt-0.7/jaxopt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 jaxopt/_src/gauss_newton.py
 jaxopt/_src/gradient_descent.py
 jaxopt/_src/hager_zhang_linesearch.py
 jaxopt/_src/implicit_diff.py
 jaxopt/_src/isotonic.py
 jaxopt/_src/iterative_refinement.py
 jaxopt/_src/lbfgs.py
+jaxopt/_src/lbfgsb.py
 jaxopt/_src/levenberg_marquardt.py
 jaxopt/_src/linear_operator.py
 jaxopt/_src/linear_solve.py
 jaxopt/_src/loop.py
 jaxopt/_src/loss.py
 jaxopt/_src/mirror_descent.py
 jaxopt/_src/nonlinear_cg.py
```

### Comparing `jaxopt-0.6/setup.py` & `jaxopt-0.7/setup.py`

 * *Files identical despite different names*

