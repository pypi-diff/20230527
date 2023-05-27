# Comparing `tmp/omnixai-1.2.5.tar.gz` & `tmp/omnixai-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnixai-1.2.5.tar", last modified: Wed Feb  8 06:57:29 2023, max compression
+gzip compressed data, was "omnixai-1.3.0.tar", last modified: Sat May 27 06:16:07 2023, max compression
```

## Comparing `omnixai-1.2.5.tar` & `omnixai-1.3.0.tar`

### file list

```diff
@@ -1,429 +1,432 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.825364 omnixai-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (116)     1482 2023-02-08 06:57:12.000000 omnixai-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)    23994 2023-02-08 06:57:29.825364 omnixai-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    23502 2023-02-08 06:57:12.000000 omnixai-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.777362 omnixai-1.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     3403 2023-02-08 06:57:12.000000 omnixai-1.2.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.777362 omnixai-1.2.5/omnixai/
--rw-r--r--   0 runner    (1001) docker     (116)      453 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.777362 omnixai-1.2.5/omnixai/data/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      999 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/data/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     7594 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/data/image.py
--rw-r--r--   0 runner    (1001) docker     (116)     2447 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/data/multi_inputs.py
--rw-r--r--   0 runner    (1001) docker     (116)     9288 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/data/tabular.py
--rw-r--r--   0 runner    (1001) docker     (116)     3793 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/data/text.py
--rw-r--r--   0 runner    (1001) docker     (116)     7308 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/data/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.777362 omnixai-1.2.5/omnixai/deployment/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.777362 omnixai-1.2.5/omnixai/deployment/bentoml/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/deployment/bentoml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8423 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/deployment/bentoml/omnixai.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.777362 omnixai-1.2.5/omnixai/explainers/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15333 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.777362 omnixai-1.2.5/omnixai/explainers/data/
--rw-r--r--   0 runner    (1001) docker     (116)      542 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3030 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/data/auto.py
--rw-r--r--   0 runner    (1001) docker     (116)     2619 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/data/chi_square.py
--rw-r--r--   0 runner    (1001) docker     (116)     2384 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/data/correlation.py
--rw-r--r--   0 runner    (1001) docker     (116)     5470 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/data/imbalance.py
--rw-r--r--   0 runner    (1001) docker     (116)     2937 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/data/mutual_info.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.781362 omnixai-1.2.5/omnixai/explainers/nlp/
--rw-r--r--   0 runner    (1001) docker     (116)      581 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.781362 omnixai-1.2.5/omnixai/explainers/nlp/agnostic/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/nlp/agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13999 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/nlp/agnostic/l2x.py
--rw-r--r--   0 runner    (1001) docker     (116)     3624 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/nlp/agnostic/lime.py
--rw-r--r--   0 runner    (1001) docker     (116)     3713 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/nlp/agnostic/shap.py
--rw-r--r--   0 runner    (1001) docker     (116)     3171 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/nlp/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.781362 omnixai-1.2.5/omnixai/explainers/nlp/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/nlp/counterfactual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7776 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/nlp/counterfactual/polyjuice.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.781362 omnixai-1.2.5/omnixai/explainers/nlp/specific/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/nlp/specific/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12781 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/nlp/specific/ig.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.781362 omnixai-1.2.5/omnixai/explainers/prediction/
--rw-r--r--   0 runner    (1001) docker     (116)      297 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12257 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/prediction/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.781362 omnixai-1.2.5/omnixai/explainers/ranking/
--rw-r--r--   0 runner    (1001) docker     (116)      390 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/ranking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.781362 omnixai-1.2.5/omnixai/explainers/ranking/agnostic/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/ranking/agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6199 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/ranking/agnostic/permutation.py
--rw-r--r--   0 runner    (1001) docker     (116)     8572 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/ranking/agnostic/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.781362 omnixai-1.2.5/omnixai/explainers/ranking/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/ranking/counterfactual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13597 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/ranking/counterfactual/mace.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.781362 omnixai-1.2.5/omnixai/explainers/tabular/
--rw-r--r--   0 runner    (1001) docker     (116)     1605 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.785362 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.785362 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/L2X/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/L2X/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14425 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/L2X/l2x.py
--rw-r--r--   0 runner    (1001) docker     (116)     5936 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/L2X/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11890 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/ale.py
--rw-r--r--   0 runner    (1001) docker     (116)    15687 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/bias.py
--rw-r--r--   0 runner    (1001) docker     (116)     7493 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/lime.py
--rw-r--r--   0 runner    (1001) docker     (116)     6632 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/pdp.py
--rw-r--r--   0 runner    (1001) docker     (116)     4433 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/permutation.py
--rw-r--r--   0 runner    (1001) docker     (116)     3555 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (116)     7285 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/shap.py
--rw-r--r--   0 runner    (1001) docker     (116)     4935 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/agnostic/shap_global.py
--rw-r--r--   0 runner    (1001) docker     (116)     5322 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/auto.py
--rw-r--r--   0 runner    (1001) docker     (116)    10220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.785362 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18191 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/ce.py
--rw-r--r--   0 runner    (1001) docker     (116)     4685 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/knn.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.785362 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/
--rw-r--r--   0 runner    (1001) docker     (116)     6913 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/diversify.py
--rw-r--r--   0 runner    (1001) docker     (116)    10231 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/gld.py
--rw-r--r--   0 runner    (1001) docker     (116)     2720 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/greedy.py
--rw-r--r--   0 runner    (1001) docker     (116)     6616 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/mace.py
--rw-r--r--   0 runner    (1001) docker     (116)     3461 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/refine.py
--rw-r--r--   0 runner    (1001) docker     (116)    10768 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (116)    12648 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/rl.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.785362 omnixai-1.2.5/omnixai/explainers/tabular/specific/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/specific/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8023 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/specific/decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (116)    12323 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/specific/ig.py
--rw-r--r--   0 runner    (1001) docker     (116)     8461 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/specific/linear.py
--rw-r--r--   0 runner    (1001) docker     (116)     5309 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/tabular/specific/shap_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.785362 omnixai-1.2.5/omnixai/explainers/timeseries/
--rw-r--r--   0 runner    (1001) docker     (116)      517 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.789363 omnixai-1.2.5/omnixai/explainers/timeseries/agnostic/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/timeseries/agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5365 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/timeseries/agnostic/shap.py
--rw-r--r--   0 runner    (1001) docker     (116)     3133 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/timeseries/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.789363 omnixai-1.2.5/omnixai/explainers/timeseries/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/timeseries/counterfactual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11919 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/timeseries/counterfactual/ce.py
--rw-r--r--   0 runner    (1001) docker     (116)    14166 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/timeseries/counterfactual/mace.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.789363 omnixai-1.2.5/omnixai/explainers/vision/
--rw-r--r--   0 runner    (1001) docker     (116)     1210 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.789363 omnixai-1.2.5/omnixai/explainers/vision/agnostic/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12137 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/agnostic/l2x.py
--rw-r--r--   0 runner    (1001) docker     (116)     3328 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/agnostic/lime.py
--rw-r--r--   0 runner    (1001) docker     (116)     6200 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/agnostic/pdp.py
--rw-r--r--   0 runner    (1001) docker     (116)     6946 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/agnostic/shap.py
--rw-r--r--   0 runner    (1001) docker     (116)     4430 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.789363 omnixai-1.2.5/omnixai/explainers/vision/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/counterfactual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6078 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/counterfactual/ce.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.789363 omnixai-1.2.5/omnixai/explainers/vision/specific/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    20052 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/cem.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.789363 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.789363 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/pytorch/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1221 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/pytorch/feature_maps.py
--rw-r--r--   0 runner    (1001) docker     (116)     8979 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (116)     3820 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/pytorch/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/tf/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      568 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/tf/feature_maps.py
--rw-r--r--   0 runner    (1001) docker     (116)    10233 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/tf/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (116)     4710 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/tf/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (116)     3525 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    11892 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explainers/vision/specific/gradcam/
--rw-r--r--   0 runner    (1001) docker     (116)      322 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/gradcam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7815 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/gradcam/gradcam.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explainers/vision/specific/gradcam/pytorch/
--rw-r--r--   0 runner    (1001) docker     (116)     8344 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/gradcam/pytorch/gradcam.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explainers/vision/specific/gradcam/tf/
--rw-r--r--   0 runner    (1001) docker     (116)     7820 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/gradcam/tf/gradcam.py
--rw-r--r--   0 runner    (1001) docker     (116)     2655 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/guided_bp.py
--rw-r--r--   0 runner    (1001) docker     (116)     7351 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/ig.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/
--rw-r--r--   0 runner    (1001) docker     (116)      275 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/pytorch/
--rw-r--r--   0 runner    (1001) docker     (116)     4944 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/pytorch/scorecam.py
--rw-r--r--   0 runner    (1001) docker     (116)     3020 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/scorecam.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/tf/
--rw-r--r--   0 runner    (1001) docker     (116)     4111 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/tf/scorecam.py
--rw-r--r--   0 runner    (1001) docker     (116)     1339 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     3576 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/smoothgrad.py
--rw-r--r--   0 runner    (1001) docker     (116)    12357 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision/specific/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explainers/vision_language/
--rw-r--r--   0 runner    (1001) docker     (116)      357 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision_language/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explainers/vision_language/specific/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision_language/specific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explainers/vision_language/specific/gradcam/
--rw-r--r--   0 runner    (1001) docker     (116)      272 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision_language/specific/gradcam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3586 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision_language/specific/gradcam/gradcam.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explainers/vision_language/specific/gradcam/pytorch/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision_language/specific/gradcam/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7249 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision_language/specific/gradcam/pytorch/gradcam.py
--rw-r--r--   0 runner    (1001) docker     (116)     7890 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explainers/vision_language/specific/ig.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explanations/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9953 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.793363 omnixai-1.2.5/omnixai/explanations/image/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8304 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/image/contrast.py
--rw-r--r--   0 runner    (1001) docker     (116)     7679 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/image/counterfactual.py
--rw-r--r--   0 runner    (1001) docker     (116)     6849 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/image/mask.py
--rw-r--r--   0 runner    (1001) docker     (116)    16919 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/image/pixel_importance.py
--rw-r--r--   0 runner    (1001) docker     (116)     5431 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/image/plain.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.797363 omnixai-1.2.5/omnixai/explanations/prediction/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4120 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/prediction/confusion.py
--rw-r--r--   0 runner    (1001) docker     (116)     5909 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/prediction/cumulative.py
--rw-r--r--   0 runner    (1001) docker     (116)     4739 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/prediction/lift.py
--rw-r--r--   0 runner    (1001) docker     (116)     5036 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/prediction/metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     4454 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/prediction/pr.py
--rw-r--r--   0 runner    (1001) docker     (116)     4060 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/prediction/residual.py
--rw-r--r--   0 runner    (1001) docker     (116)     6236 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/prediction/roc.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.797363 omnixai-1.2.5/omnixai/explanations/tabular/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7331 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/ale.py
--rw-r--r--   0 runner    (1001) docker     (116)     4752 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/bias.py
--rw-r--r--   0 runner    (1001) docker     (116)     2904 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/correlation.py
--rw-r--r--   0 runner    (1001) docker     (116)    13514 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/counterfactual.py
--rw-r--r--   0 runner    (1001) docker     (116)    14586 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (116)     4198 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/imbalance.py
--rw-r--r--   0 runner    (1001) docker     (116)     9103 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/linear.py
--rw-r--r--   0 runner    (1001) docker     (116)     7804 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/pdp.py
--rw-r--r--   0 runner    (1001) docker     (116)     4161 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (116)     9267 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/tree.py
--rw-r--r--   0 runner    (1001) docker     (116)     7965 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/tabular/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.797363 omnixai-1.2.5/omnixai/explanations/text/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11622 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/text/word_importance.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.797363 omnixai-1.2.5/omnixai/explanations/timeseries/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7839 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/timeseries/counterfactual.py
--rw-r--r--   0 runner    (1001) docker     (116)    10436 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/timeseries/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/explanations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.801363 omnixai-1.2.5/omnixai/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1597 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/preprocessing/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     3628 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/preprocessing/encode.py
--rw-r--r--   0 runner    (1001) docker     (116)     4754 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/preprocessing/fill.py
--rw-r--r--   0 runner    (1001) docker     (116)     4044 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (116)     1614 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/preprocessing/normalize.py
--rw-r--r--   0 runner    (1001) docker     (116)     2345 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/preprocessing/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)     8156 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/preprocessing/tabular.py
--rw-r--r--   0 runner    (1001) docker     (116)     2880 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.801363 omnixai-1.2.5/omnixai/sampler/
--rw-r--r--   0 runner    (1001) docker     (116)     7285 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/sampler/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.773362 omnixai-1.2.5/omnixai/tests/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.801363 omnixai-1.2.5/omnixai/tests/data/
--rw-r--r--   0 runner    (1001) docker     (116)     1761 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/data/test_image.py
--rw-r--r--   0 runner    (1001) docker     (116)      976 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/data/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (116)     1371 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/data/test_tabular.py
--rw-r--r--   0 runner    (1001) docker     (116)      931 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/data/test_text.py
--rw-r--r--   0 runner    (1001) docker     (116)     1623 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/data/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.773362 omnixai-1.2.5/omnixai/tests/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.801363 omnixai-1.2.5/omnixai/tests/deployment/bentoml/
--rw-r--r--   0 runner    (1001) docker     (116)     1659 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/api_server.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.801363 omnixai-1.2.5/omnixai/tests/deployment/bentoml/nlp/
--rw-r--r--   0 runner    (1001) docker     (116)     1540 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/nlp/model.py
--rw-r--r--   0 runner    (1001) docker     (116)     1007 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/nlp/request.py
--rw-r--r--   0 runner    (1001) docker     (116)      428 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/nlp/service.py
--rw-r--r--   0 runner    (1001) docker     (116)     1058 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/nlp/test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2683 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/nlp/train.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.801363 omnixai-1.2.5/omnixai/tests/deployment/bentoml/tabular/
--rw-r--r--   0 runner    (1001) docker     (116)     2130 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/tabular/request.py
--rw-r--r--   0 runner    (1001) docker     (116)      445 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/tabular/service.py
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/tabular/test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2634 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/tabular/train.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.805363 omnixai-1.2.5/omnixai/tests/deployment/bentoml/vision/
--rw-r--r--   0 runner    (1001) docker     (116)     1599 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/vision/request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1666 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/vision/save.py
--rw-r--r--   0 runner    (1001) docker     (116)      440 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/vision/service.py
--rw-r--r--   0 runner    (1001) docker     (116)     1272 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/deployment/bentoml/vision/test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.805363 omnixai-1.2.5/omnixai/tests/explainers/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.805363 omnixai-1.2.5/omnixai/tests/explainers/L2X/
--rw-r--r--   0 runner    (1001) docker     (116)     4068 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/L2X/test_l2x.py
--rw-r--r--   0 runner    (1001) docker     (116)     6572 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/L2X/test_l2x_image_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     2766 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/L2X/test_l2x_tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1089 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/L2X/test_l2x_tabular_regression.py
--rw-r--r--   0 runner    (1001) docker     (116)     2384 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/L2X/test_l2x_text_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.805363 omnixai-1.2.5/omnixai/tests/explainers/ale/
--rw-r--r--   0 runner    (1001) docker     (116)     1925 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ale/test_ale_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1082 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ale/test_ale_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.805363 omnixai-1.2.5/omnixai/tests/explainers/bias/
--rw-r--r--   0 runner    (1001) docker     (116)     1342 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/bias/test_bias_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1194 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/bias/test_bias_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.805363 omnixai-1.2.5/omnixai/tests/explainers/ce/
--rw-r--r--   0 runner    (1001) docker     (116)     2331 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ce/test_ce_imagenet.py
--rw-r--r--   0 runner    (1001) docker     (116)     8048 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ce/test_ce_tabular.py
--rw-r--r--   0 runner    (1001) docker     (116)     3130 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ce/test_ce_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     2041 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ce/test_ce_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (116)     6241 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ce/test_ce_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.805363 omnixai-1.2.5/omnixai/tests/explainers/cem/
--rw-r--r--   0 runner    (1001) docker     (116)     3968 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/cem/cem_optimizer_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     5627 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/cem/cem_optimizer_torch.py
--rw-r--r--   0 runner    (1001) docker     (116)     3157 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/cem/test_cem_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     4905 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/cem/test_cem_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.805363 omnixai-1.2.5/omnixai/tests/explainers/data/
--rw-r--r--   0 runner    (1001) docker     (116)     2148 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/data/test_chi2.py
--rw-r--r--   0 runner    (1001) docker     (116)     1604 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/data/test_correlation.py
--rw-r--r--   0 runner    (1001) docker     (116)     1622 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/data/test_imbalance.py
--rw-r--r--   0 runner    (1001) docker     (116)     2003 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/data/test_mutual.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.809363 omnixai-1.2.5/omnixai/tests/explainers/decision_tree/
--rw-r--r--   0 runner    (1001) docker     (116)     4369 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/decision_tree/test_tree_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1282 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/decision_tree/test_tree_regression.py
--rw-r--r--   0 runner    (1001) docker     (116)     2766 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.809363 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/
--rw-r--r--   0 runner    (1001) docker     (116)     1157 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/explainer_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1425 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/explainer_torch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1354 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/feature_explainer.py
--rw-r--r--   0 runner    (1001) docker     (116)     1649 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/feature_map_explainer_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1547 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/feature_map_explainer_torch.py
--rw-r--r--   0 runner    (1001) docker     (116)     6033 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1703 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_torch.py
--rw-r--r--   0 runner    (1001) docker     (116)     2540 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_fft.py
--rw-r--r--   0 runner    (1001) docker     (116)     2566 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     2163 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_torch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1303 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_map_extractor_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1261 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_map_extractor_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.809363 omnixai-1.2.5/omnixai/tests/explainers/gradcam/
--rw-r--r--   0 runner    (1001) docker     (116)     2194 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/gradcam/test_gradcam_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     2293 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/gradcam/test_gradcam_torch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1918 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/gradcam/test_layercam_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1741 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/gradcam/test_layercam_torch.py
--rw-r--r--   0 runner    (1001) docker     (116)     2188 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/gradcam/vlm_gradcam_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.809363 omnixai-1.2.5/omnixai/tests/explainers/guided_bp/
--rw-r--r--   0 runner    (1001) docker     (116)     1842 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/guided_bp/test_guided_bp_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1699 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/guided_bp/test_guided_bp_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.809363 omnixai-1.2.5/omnixai/tests/explainers/ig/
--rw-r--r--   0 runner    (1001) docker     (116)     5783 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ig/nlp_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     6529 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ig/nlp_torch.py
--rw-r--r--   0 runner    (1001) docker     (116)     7498 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ig/test_compute_integrated_gradients.py
--rw-r--r--   0 runner    (1001) docker     (116)     1691 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ig/test_ig_image.py
--rw-r--r--   0 runner    (1001) docker     (116)     8873 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ig/test_ig_tabular.py
--rw-r--r--   0 runner    (1001) docker     (116)     1996 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ig/vlm_ig_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.809363 omnixai-1.2.5/omnixai/tests/explainers/knn/
--rw-r--r--   0 runner    (1001) docker     (116)     1447 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/knn/test_ce_knn.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.813363 omnixai-1.2.5/omnixai/tests/explainers/lime/
--rw-r--r--   0 runner    (1001) docker     (116)     2911 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/lime/test_lime_image_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     5527 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/lime/test_lime_tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1392 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/lime/test_lime_tabular_regression.py
--rw-r--r--   0 runner    (1001) docker     (116)     2526 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/lime/test_lime_text_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.813363 omnixai-1.2.5/omnixai/tests/explainers/linear/
--rw-r--r--   0 runner    (1001) docker     (116)     3763 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/linear/test_linear_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1272 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/linear/test_linear_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.813363 omnixai-1.2.5/omnixai/tests/explainers/mace/
--rw-r--r--   0 runner    (1001) docker     (116)     2057 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/mace/test_mace.py
--rw-r--r--   0 runner    (1001) docker     (116)     1577 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/mace/test_mace_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (116)     1374 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/mace/test_ranking.py
--rw-r--r--   0 runner    (1001) docker     (116)     1344 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/mace/test_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (116)     1750 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/mace/test_rl_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.813363 omnixai-1.2.5/omnixai/tests/explainers/pdp/
--rw-r--r--   0 runner    (1001) docker     (116)     2053 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/pdp/pdp_image.py
--rw-r--r--   0 runner    (1001) docker     (116)     2285 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/pdp/test_tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1097 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/pdp/test_tabular_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.813363 omnixai-1.2.5/omnixai/tests/explainers/permutation/
--rw-r--r--   0 runner    (1001) docker     (116)     1046 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/permutation/test_permutation_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)      942 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/permutation/test_permutation_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.813363 omnixai-1.2.5/omnixai/tests/explainers/polyjuice/
--rw-r--r--   0 runner    (1001) docker     (116)     1565 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/polyjuice/polyjuice_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1567 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/polyjuice/polyjuice_qa.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.813363 omnixai-1.2.5/omnixai/tests/explainers/prediction/
--rw-r--r--   0 runner    (1001) docker     (116)     1395 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/prediction/test_classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     1507 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/prediction/test_confusion.py
--rw-r--r--   0 runner    (1001) docker     (116)     1446 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/prediction/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (116)     1437 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/prediction/test_lift.py
--rw-r--r--   0 runner    (1001) docker     (116)     1509 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/prediction/test_pr.py
--rw-r--r--   0 runner    (1001) docker     (116)      970 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/prediction/test_regression_metric.py
--rw-r--r--   0 runner    (1001) docker     (116)      927 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/prediction/test_residual.py
--rw-r--r--   0 runner    (1001) docker     (116)     1423 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/prediction/test_roc.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.813363 omnixai-1.2.5/omnixai/tests/explainers/ranking/
--rw-r--r--   0 runner    (1001) docker     (116)     1711 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ranking/test_perm_ranking.py
--rw-r--r--   0 runner    (1001) docker     (116)     1657 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/ranking/test_validity_ranking.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.817364 omnixai-1.2.5/omnixai/tests/explainers/scorecam/
--rw-r--r--   0 runner    (1001) docker     (116)     1896 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/scorecam/scorecam_torch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1982 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/scorecam/test_scorecam_tf.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.817364 omnixai-1.2.5/omnixai/tests/explainers/sensitivity/
--rw-r--r--   0 runner    (1001) docker     (116)     1773 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/sensitivity/test_sa_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.817364 omnixai-1.2.5/omnixai/tests/explainers/shap/
--rw-r--r--   0 runner    (1001) docker     (116)     3085 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/shap/shap_image_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     6134 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/shap/shap_image_torch.py
--rw-r--r--   0 runner    (1001) docker     (116)     2376 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/shap/shap_merlion.py
--rw-r--r--   0 runner    (1001) docker     (116)     1083 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/shap/shap_text.py
--rw-r--r--   0 runner    (1001) docker     (116)     3940 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/shap/test_shap_tabular_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1131 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/shap/test_shap_tabular_global.py
--rw-r--r--   0 runner    (1001) docker     (116)     1357 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/shap/test_shap_tabular_regression.py
--rw-r--r--   0 runner    (1001) docker     (116)     2045 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/shap/test_shap_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.817364 omnixai-1.2.5/omnixai/tests/explainers/shap_tree/
--rw-r--r--   0 runner    (1001) docker     (116)     4693 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/shap_tree/shaptree_classification.py
--rw-r--r--   0 runner    (1001) docker     (116)     1228 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/shap_tree/shaptree_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.817364 omnixai-1.2.5/omnixai/tests/explainers/smoothgrad/
--rw-r--r--   0 runner    (1001) docker     (116)     1847 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/smoothgrad/test_smooth_grad_tf.py
--rw-r--r--   0 runner    (1001) docker     (116)     1704 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/smoothgrad/test_smooth_grad_torch.py
--rw-r--r--   0 runner    (1001) docker     (116)    10940 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/explainers/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.817364 omnixai-1.2.5/omnixai/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (116)     1357 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/preprocessing/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (116)     2895 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/preprocessing/test_fill.py
--rw-r--r--   0 runner    (1001) docker     (116)     2396 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/preprocessing/test_image_transform.py
--rw-r--r--   0 runner    (1001) docker     (116)      977 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/preprocessing/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (116)     1303 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/preprocessing/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)     2059 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/preprocessing/test_tabular_transform.py
--rw-r--r--   0 runner    (1001) docker     (116)     1200 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/preprocessing/test_text_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.817364 omnixai-1.2.5/omnixai/tests/sampler/
--rw-r--r--   0 runner    (1001) docker     (116)     2577 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/sampler/test_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.817364 omnixai-1.2.5/omnixai/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.817364 omnixai-1.2.5/omnixai/tests/utils/json/
--rw-r--r--   0 runner    (1001) docker     (116)      796 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/utils/json/test_counterfactual.py
--rw-r--r--   0 runner    (1001) docker     (116)     1560 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/utils/json/test_feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (116)     1264 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/utils/json/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (116)     1345 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/utils/test_explanation_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      881 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/utils/test_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.821364 omnixai-1.2.5/omnixai/tests/visualization/
--rw-r--r--   0 runner    (1001) docker     (116)     1991 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/visualization/dashboard_da.py
--rw-r--r--   0 runner    (1001) docker     (116)     3211 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/visualization/dashboard_image.py
--rw-r--r--   0 runner    (1001) docker     (116)     2685 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/visualization/dashboard_image_compare.py
--rw-r--r--   0 runner    (1001) docker     (116)     5016 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/visualization/dashboard_tabular.py
--rw-r--r--   0 runner    (1001) docker     (116)     3539 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/visualization/dashboard_tabular_regression.py
--rw-r--r--   0 runner    (1001) docker     (116)     1808 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/visualization/dashboard_text.py
--rw-r--r--   0 runner    (1001) docker     (116)     5571 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/visualization/dashboard_text_imdb.py
--rw-r--r--   0 runner    (1001) docker     (116)     1840 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/tests/visualization/dashboard_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.821364 omnixai-1.2.5/omnixai/utils/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6489 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (116)     2833 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/utils/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.821364 omnixai-1.2.5/omnixai/visualization/
--rw-r--r--   0 runner    (1001) docker     (116)      220 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.821364 omnixai-1.2.5/omnixai/visualization/assets/
--rwxr-xr-x   0 runner    (1001) docker     (116)    83784 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/assets/Acumin-BdPro.otf
--rw-r--r--   0 runner    (1001) docker     (116)    12235 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/assets/base.css
--rw-r--r--   0 runner    (1001) docker     (116)    28366 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/assets/logo_small.png
--rw-r--r--   0 runner    (1001) docker     (116)     6085 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/assets/modal.css
--rw-r--r--   0 runner    (1001) docker     (116)      292 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/assets/resizing.js
--rw-r--r--   0 runner    (1001) docker     (116)      981 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/assets/styles.css
--rw-r--r--   0 runner    (1001) docker     (116)     2684 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/assets/xai.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.825364 omnixai-1.2.5/omnixai/visualization/callbacks/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1396 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/callbacks/data_exp.py
--rw-r--r--   0 runner    (1001) docker     (116)     1416 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/callbacks/global_exp.py
--rw-r--r--   0 runner    (1001) docker     (116)     1569 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/callbacks/local_exp.py
--rw-r--r--   0 runner    (1001) docker     (116)     1456 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/callbacks/prediction_exp.py
--rw-r--r--   0 runner    (1001) docker     (116)     5041 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/callbacks/whatif_exp.py
--rw-r--r--   0 runner    (1001) docker     (116)     8589 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (116)     2709 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.825364 omnixai-1.2.5/omnixai/visualization/pages/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2088 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/pages/data_exp.py
--rw-r--r--   0 runner    (1001) docker     (116)     2110 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/pages/global_exp.py
--rw-r--r--   0 runner    (1001) docker     (116)     3180 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/pages/local_exp.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/pages/prediction_exp.py
--rw-r--r--   0 runner    (1001) docker     (116)     2565 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/pages/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     6981 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/pages/whatif_exp.py
--rw-r--r--   0 runner    (1001) docker     (116)     3251 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/plot.py
--rw-r--r--   0 runner    (1001) docker     (116)     7443 2023-02-08 06:57:12.000000 omnixai-1.2.5/omnixai/visualization/state.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-08 06:57:29.777362 omnixai-1.2.5/omnixai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    23994 2023-02-08 06:57:29.000000 omnixai-1.2.5/omnixai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    15745 2023-02-08 06:57:29.000000 omnixai-1.2.5/omnixai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-08 06:57:29.000000 omnixai-1.2.5/omnixai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-08 06:57:29.000000 omnixai-1.2.5/omnixai.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      595 2023-02-08 06:57:29.000000 omnixai-1.2.5/omnixai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       28 2023-02-08 06:57:29.000000 omnixai-1.2.5/omnixai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-08 06:57:29.825364 omnixai-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1782 2023-02-08 06:57:12.000000 omnixai-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.515314 omnixai-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-05-27 06:15:55.000000 omnixai-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    25485 2023-05-27 06:16:07.515314 omnixai-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24993 2023-05-27 06:15:55.000000 omnixai-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.443313 omnixai-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-05-27 06:15:55.000000 omnixai-1.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.443313 omnixai-1.3.0/omnixai/
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.447313 omnixai-1.3.0/omnixai/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7594 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/multi_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9288 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7308 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/data/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.447313 omnixai-1.3.0/omnixai/deployment/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.447313 omnixai-1.3.0/omnixai/deployment/bentoml/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/deployment/bentoml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8423 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/deployment/bentoml/omnixai.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.447313 omnixai-1.3.0/omnixai/explainers/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15333 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/auto.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/chi_square.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5470 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2937 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/data/mutual_info.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/nlp/
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/nlp/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13999 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/agnostic/l2x.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/agnostic/lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3713 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/agnostic/shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3171 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/nlp/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/counterfactual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7776 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/counterfactual/polyjuice.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/nlp/specific/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/specific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12781 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/nlp/specific/ig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/prediction/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12257 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/prediction/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/ranking/
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.451313 omnixai-1.3.0/omnixai/explainers/ranking/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6199 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/agnostic/permutation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8572 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/agnostic/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.455313 omnixai-1.3.0/omnixai/explainers/ranking/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/counterfactual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13597 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/ranking/counterfactual/mace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.455313 omnixai-1.3.0/omnixai/explainers/tabular/
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.455313 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.455313 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14425 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/l2x.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5936 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11890 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/ale.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15687 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/bias.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6964 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7493 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6632 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4433 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/permutation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7285 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/agnostic/shap_global.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/auto.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.459313 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18191 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/ce.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/knn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.459313 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/
+-rw-r--r--   0 runner    (1001) docker     (122)     6913 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/diversify.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10231 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/gld.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6616 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/mace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3461 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/refine.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10768 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12648 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/rl.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.459313 omnixai-1.3.0/omnixai/explainers/tabular/specific/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/specific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8023 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/specific/decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12323 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/specific/ig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8461 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/specific/linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5309 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/tabular/specific/shap_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.459313 omnixai-1.3.0/omnixai/explainers/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.459313 omnixai-1.3.0/omnixai/explainers/timeseries/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/agnostic/shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3133 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.463313 omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11919 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/ce.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14166 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/mace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.463313 omnixai-1.3.0/omnixai/explainers/vision/
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.463313 omnixai-1.3.0/omnixai/explainers/vision/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12137 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/agnostic/l2x.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/agnostic/lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6200 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/agnostic/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6946 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/agnostic/shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.463313 omnixai-1.3.0/omnixai/explainers/vision/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/counterfactual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6078 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/counterfactual/ce.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20052 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/cem.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/feature_maps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8979 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/feature_maps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10233 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3525 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11892 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7815 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/gradcam.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.467313 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (122)     8344 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/pytorch/gradcam.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/tf/
+-rw-r--r--   0 runner    (1001) docker     (122)     7820 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/tf/gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/guided_bp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7351 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/ig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (122)     4944 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/pytorch/scorecam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3020 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/scorecam.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/tf/
+-rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/tf/scorecam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/smoothgrad.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12357 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision/specific/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision_language/
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision_language/specific/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/gradcam.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7249 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/pytorch/gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7890 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explainers/vision_language/specific/ig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explanations/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12095 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.471313 omnixai-1.3.0/omnixai/explanations/image/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8304 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/contrast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7679 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/counterfactual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6849 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/mask.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16919 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/pixel_importance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5431 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/image/plain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.475314 omnixai-1.3.0/omnixai/explanations/prediction/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4120 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/confusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5909 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4739 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/lift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5036 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/pr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4060 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/residual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/prediction/roc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.475314 omnixai-1.3.0/omnixai/explanations/tabular/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7331 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/ale.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/bias.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13514 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/counterfactual.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14586 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9103 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7804 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4161 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9267 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7965 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/tabular/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.475314 omnixai-1.3.0/omnixai/explanations/text/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11622 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/text/word_importance.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.475314 omnixai-1.3.0/omnixai/explanations/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7839 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/timeseries/counterfactual.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10436 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/timeseries/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/explanations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.479313 omnixai-1.3.0/omnixai/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/encode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4754 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/fill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4044 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2880 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.479313 omnixai-1.3.0/omnixai/sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)     7285 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/sampler/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.443313 omnixai-1.3.0/omnixai/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.479313 omnixai-1.3.0/omnixai/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1761 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/data/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      976 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/data/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/data/test_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)      931 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/data/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/data/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.439313 omnixai-1.3.0/omnixai/tests/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.479313 omnixai-1.3.0/omnixai/tests/deployment/bentoml/
+-rw-r--r--   0 runner    (1001) docker     (122)     1879 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/api_server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.479313 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2683 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/
+-rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2634 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/explainers/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/explainers/L2X/
+-rw-r--r--   0 runner    (1001) docker     (122)     4068 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6572 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2766 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_tabular_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2384 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_text_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/explainers/ale/
+-rw-r--r--   0 runner    (1001) docker     (122)     1925 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ale/test_ale_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ale/test_ale_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.483313 omnixai-1.3.0/omnixai/tests/explainers/bias/
+-rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/bias/test_bias_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/bias/test_bias_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.487314 omnixai-1.3.0/omnixai/tests/explainers/ce/
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8048 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3130 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2261 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6241 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.487314 omnixai-1.3.0/omnixai/tests/explainers/cem/
+-rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/cem/cem_optimizer_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5627 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/cem/cem_optimizer_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/cem/test_cem_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/cem/test_cem_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.487314 omnixai-1.3.0/omnixai/tests/explainers/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/data/test_chi2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/data/test_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/data/test_imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/data/test_mutual.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.487314 omnixai-1.3.0/omnixai/tests/explainers/decision_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)     4369 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/decision_tree/test_tree_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/decision_tree/test_tree_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2766 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.491314 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/explainer_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/explainer_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_map_explainer_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1547 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_map_explainer_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6033 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2540 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fft.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_map_extractor_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_map_extractor_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.491314 omnixai-1.3.0/omnixai/tests/explainers/gpt/
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gpt/gpt_explainer_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.491314 omnixai-1.3.0/omnixai/tests/explainers/gradcam/
+-rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_gradcam_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_gradcam_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_layercam_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_layercam_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/gradcam/vlm_gradcam_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.491314 omnixai-1.3.0/omnixai/tests/explainers/guided_bp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/guided_bp/test_guided_bp_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/guided_bp/test_guided_bp_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.491314 omnixai-1.3.0/omnixai/tests/explainers/ig/
+-rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/nlp_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6529 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/nlp_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7498 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/test_compute_integrated_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/test_ig_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8873 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/test_ig_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ig/vlm_ig_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.495314 omnixai-1.3.0/omnixai/tests/explainers/knn/
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/knn/test_ce_knn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.495314 omnixai-1.3.0/omnixai/tests/explainers/lime/
+-rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5527 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1392 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_tabular_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_text_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.495314 omnixai-1.3.0/omnixai/tests/explainers/linear/
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/linear/test_linear_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/linear/test_linear_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.495314 omnixai-1.3.0/omnixai/tests/explainers/mace/
+-rw-r--r--   0 runner    (1001) docker     (122)     2057 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/mace/test_mace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/mace/test_mace_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/mace/test_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/mace/test_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1750 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/mace/test_rl_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/pdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/pdp/pdp_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/pdp/test_tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/pdp/test_tabular_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/permutation/
+-rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/permutation/test_permutation_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/permutation/test_permutation_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/polyjuice/
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/polyjuice/polyjuice_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/polyjuice/polyjuice_qa.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/prediction/
+-rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_confusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_lift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_pr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_regression_metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_residual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/prediction/test_roc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/ranking/
+-rw-r--r--   0 runner    (1001) docker     (122)     1711 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ranking/test_perm_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/ranking/test_validity_ranking.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/scorecam/
+-rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/scorecam/scorecam_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/scorecam/test_scorecam_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.499314 omnixai-1.3.0/omnixai/tests/explainers/sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/sensitivity/test_sa_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.503314 omnixai-1.3.0/omnixai/tests/explainers/shap/
+-rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/shap_image_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6134 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/shap_image_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/shap_merlion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/shap_text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3940 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_global.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.503314 omnixai-1.3.0/omnixai/tests/explainers/shap_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)     4693 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap_tree/shaptree_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/shap_tree/shaptree_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.503314 omnixai-1.3.0/omnixai/tests/explainers/smoothgrad/
+-rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/smoothgrad/test_smooth_grad_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/smoothgrad/test_smooth_grad_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10940 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/explainers/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.503314 omnixai-1.3.0/omnixai/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_fill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2059 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_tabular_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1200 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/preprocessing/test_text_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.507314 omnixai-1.3.0/omnixai/tests/sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/sampler/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.507314 omnixai-1.3.0/omnixai/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.507314 omnixai-1.3.0/omnixai/tests/utils/json/
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/utils/json/test_counterfactual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/utils/json/test_feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/utils/json/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/utils/test_explanation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/utils/test_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.507314 omnixai-1.3.0/omnixai/tests/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_da.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3211 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_image_compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5016 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_tabular_regression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_text_imdb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/tests/visualization/dashboard_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.507314 omnixai-1.3.0/omnixai/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/utils/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.511314 omnixai-1.3.0/omnixai/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.511314 omnixai-1.3.0/omnixai/visualization/assets/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    83784 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/Acumin-BdPro.otf
+-rw-r--r--   0 runner    (1001) docker     (122)    12235 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/base.css
+-rw-r--r--   0 runner    (1001) docker     (122)    28366 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6085 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/modal.css
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/resizing.js
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/styles.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2684 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/assets/xai.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.511314 omnixai-1.3.0/omnixai/visualization/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/data_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/global_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/local_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/prediction_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/callbacks/whatif_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8589 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2709 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.515314 omnixai-1.3.0/omnixai/visualization/pages/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/data_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/global_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/local_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/prediction_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6981 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/pages/whatif_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7663 2023-05-27 06:15:55.000000 omnixai-1.3.0/omnixai/visualization/state.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-27 06:16:07.447313 omnixai-1.3.0/omnixai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    25485 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    15849 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-27 06:16:07.000000 omnixai-1.3.0/omnixai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-27 06:16:07.515314 omnixai-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-05-27 06:15:55.000000 omnixai-1.3.0/setup.py
```

### Comparing `omnixai-1.2.5/LICENSE` & `omnixai-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omnixai-1.2.5/PKG-INFO` & `omnixai-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnixai
-Version: 1.2.5
+Version: 1.3.0
 Summary: OmniXAI: An Explainable AI Toolbox
 Home-page: https://github.com/salesforce/omnixai
 Author: Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi
 License: 3-Clause BSD
 Keywords: XAI Explainable AI Explanation
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
@@ -47,14 +47,20 @@
 4. [Documentation](https://opensource.salesforce.com/OmniXAI/latest/index.html)
 5. [Tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html)
 6. [Deployment](#deployment)
 7. [Dashboard Demo](https://sfr-omnixai-demo.herokuapp.com/)
 8. [How to Contribute](https://opensource.salesforce.com/OmniXAI/latest/omnixai.html#how-to-contribute)
 9. [Technical Report and Citing OmniXAI](#technical-report-and-citing-omnixai)
 
+## What's New
+
+The latest version includes an experimental GPT explainer. This explainer leverages the outcomes 
+produced by SHAP and MACE to formulate the input prompt for ChatGPT. Subsequently, ChatGPT 
+analyzes these results and generates the corresponding explanations that provide developers with 
+a clearer understanding of the rationale behind the model's predictions.
 
 ## Introduction
 
 OmniXAI (short for Omni eXplainable AI) is a Python machine-learning library for explainable AI (XAI), offering omni-way explainable AI and interpretable 
 machine learning capabilities to address many pain points in explaining decisions made by machine learning 
 models in practice. OmniXAI aims to be a one-stop comprehensive library that makes explainable AI easy for 
 data scientists, ML researchers and practitioners who need explanation for various types of data, models and 
@@ -80,17 +86,18 @@
 |       Bias metrics        |   Black box   |      Global      |     |    ✅    |       |      |      |
 | Partial dependence plots  |   Black box   |      Global      |     |    ✅    |       |      |      |
 | Accumulated local effects |   Black box   |      Global      |     |    ✅    |       |      |      |
 |   Sensitivity analysis    |   Black box   |      Global      |     |    ✅    |       |      |      |
 |  Permutation explanation  |   Black box   |      Global      |     |    ✅    |       |      |      |
 |   Feature visualization   |  Torch or TF  |      Global      |     |         |   ✅   |      |      |
 |       Feature maps        |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
+|       GPT explainer       | Black box     |     Local        |     |    ✅    |       |      |      |
 |           LIME            |   Black box   |      Local       |     |    ✅    |   ✅   | ✅   |      |
 |           SHAP            |  Black box*   |      Local       |     |    ✅    |   ✅   | ✅   |  ✅  |
-|         What-if           |  Black box    |      Local       |     |    ✅    |       |      |     |
+|          What-if          |   Black box   |      Local       |     |    ✅    |       |      |     |
 |    Integrated gradient    |  Torch or TF  |      Local       |     |    ✅    |   ✅   | ✅   |      |
 |      Counterfactual       |  Black box*   |      Local       |     |    ✅    |   ✅   | ✅   |  ✅  |
 |  Contrastive explanation  |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |   Grad-CAM, Grad-CAM++    |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |         Score-CAM         |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |         Layer-CAM         |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |      Smooth gradient      |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
@@ -103,14 +110,18 @@
 for text data. *Counterfactual* accepts black box models for tabular, text and time-series data, and PyTorch/Tensorflow models for
 image data.
 
 This [table](https://opensource.salesforce.com/OmniXAI/latest/index.html#comparison-with-competitors) 
 shows the comparison between our toolkit/library and other existing XAI toolkits/libraries
 in literature.
 
+**OmniXAI also integrates ChatGPT for generating plain text explanations given a classification/regression
+model on tabular datasets.** The generated results may not be 100% accurate, but it is worth trying this 
+explainer (we will continue improving the input prompts).
+
 ## Installation
 
 You can install ``omnixai`` from PyPI by calling ``pip install omnixai``. You may install from source by
 cloning the OmniXAI repo, navigating to the root directory, and calling
 ``pip install .``, or ``pip install -e .`` to install in editable mode. You may install additional dependencies:
 
 - **For plotting & visualization**: Calling ``pip install omnixai[plot]``, or ``pip install .[plot]`` from the
@@ -297,14 +308,30 @@
 )
 dashboard.show()                                    # Launch the dashboard
 ```
 
 After opening the Dash app in the browser, we will see a dashboard showing the explanations:
 ![alt text](https://github.com/salesforce/OmniXAI/raw/main/docs/_static/demo.gif)
 
+You can also use the GPT explainer to generate explanations in text for tabular models:
+
+```python
+explainer = TabularExplainer(
+  explainers=["gpt"],                                # The GPT explainer to apply
+  mode="classification",                             # The task type
+  data=train_data,                                   # The data for initializing the explainers
+  model=model,                                       # The ML model to explain
+  preprocess=lambda z: transformer.transform(z),     # Converts raw features into the model inputs
+  params={
+     "gpt": {"apikey": "xxxx"}
+  }                                                  # Set the OpenAI API KEY
+)
+local_explanations = explainer.explain(X=test_instances)
+```
+
 For vision tasks, the same interface is used to create explainers and generate explanations. 
 Let's take an image classification model as an example.
 
 ```python
 from omnixai.explainers.vision import VisionExplainer
 from omnixai.visualization.dashboard import Dashboard
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: omnixai Version: 1.2.5 Summary: OmniXAI: An
+Metadata-Version: 2.1 Name: omnixai Version: 1.3.0 Summary: OmniXAI: An
 Explainable AI Toolbox Home-page: https://github.com/salesforce/omnixai Author:
 Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi
 License: 3-Clause BSD Keywords: XAI Explainable AI Explanation Requires-Python:
 >=3.7,<4 Description-Content-Type: text/markdown Provides-Extra: plot Provides-
 Extra: vision Provides-Extra: nlp Provides-Extra: bentoml Provides-Extra: all
 License-File: LICENSE
 
@@ -13,17 +13,22 @@
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
 (https://opensource.salesforce.com/OmniXAI/latest/index.html) 5. [Tutorials]
 (https://opensource.salesforce.com/OmniXAI/latest/tutorials.html) 6.
 [Deployment](#deployment) 7. [Dashboard Demo](https://sfr-omnixai-
 demo.herokuapp.com/) 8. [How to Contribute](https://opensource.salesforce.com/
 OmniXAI/latest/omnixai.html#how-to-contribute) 9. [Technical Report and Citing
-OmniXAI](#technical-report-and-citing-omnixai) ## Introduction OmniXAI (short
-for Omni eXplainable AI) is a Python machine-learning library for explainable
-AI (XAI), offering omni-way explainable AI and interpretable machine learning
+OmniXAI](#technical-report-and-citing-omnixai) ## What's New The latest version
+includes an experimental GPT explainer. This explainer leverages the outcomes
+produced by SHAP and MACE to formulate the input prompt for ChatGPT.
+Subsequently, ChatGPT analyzes these results and generates the corresponding
+explanations that provide developers with a clearer understanding of the
+rationale behind the model's predictions. ## Introduction OmniXAI (short for
+Omni eXplainable AI) is a Python machine-learning library for explainable AI
+(XAI), offering omni-way explainable AI and interpretable machine learning
 capabilities to address many pain points in explaining decisions made by
 machine learning models in practice. OmniXAI aims to be a one-stop
 comprehensive library that makes explainable AI easy for data scientists, ML
 researchers and practitioners who need explanation for various types of data,
 models and explanation methods at different stages of ML process: ![alt text]
 (https://github.com/salesforce/OmniXAI/raw/main/docs/_static/ml_pipeline.png)
 OmniXAI includes a rich family of explanation methods integrated in a unified
@@ -44,45 +49,49 @@
 â | | | | | | Feature selection | NA | Global | â | | | | | | Prediction
 metrics | Black box | Global | | â | â | â | â | | Bias metrics | Black
 box | Global | | â | | | | | Partial dependence plots | Black box | Global |
 | â | | | | | Accumulated local effects | Black box | Global | | â | | | |
 | Sensitivity analysis | Black box | Global | | â | | | | | Permutation
 explanation | Black box | Global | | â | | | | | Feature visualization |
 Torch or TF | Global | | | â | | | | Feature maps | Torch or TF | Local | | |
-â | | | | LIME | Black box | Local | | â | â | â | | | SHAP | Black
-box* | Local | | â | â | â | â | | What-if | Black box | Local | | â
-| | | | | Integrated gradient | Torch or TF | Local | | â | â | â | | |
-Counterfactual | Black box* | Local | | â | â | â | â | | Contrastive
-explanation | Torch or TF | Local | | | â | | | | Grad-CAM, Grad-CAM++ |
-Torch or TF | Local | | | â | | | | Score-CAM | Torch or TF | Local | | | â
-| | | | Layer-CAM | Torch or TF | Local | | | â | | | | Smooth gradient |
-Torch or TF | Local | | | â | | | | Guided backpropagation | Torch or TF |
-Local | | | â | | | | Learning to explain | Black box | Local | | â | â |
-â | | | Linear models | Linear models | Global and Local | | â | | | | |
-Tree models | Tree models | Global and Local | | â | | | | *SHAP* accepts
-black box models for tabular data, PyTorch/Tensorflow models for image data,
-transformer models for text data. *Counterfactual* accepts black box models for
-tabular, text and time-series data, and PyTorch/Tensorflow models for image
-data. This [table](https://opensource.salesforce.com/OmniXAI/latest/
-index.html#comparison-with-competitors) shows the comparison between our
-toolkit/library and other existing XAI toolkits/libraries in literature. ##
-Installation You can install ``omnixai`` from PyPI by calling ``pip install
-omnixai``. You may install from source by cloning the OmniXAI repo, navigating
-to the root directory, and calling ``pip install .``, or ``pip install -e .``
-to install in editable mode. You may install additional dependencies: - **For
-plotting & visualization**: Calling ``pip install omnixai[plot]``, or ``pip
-install .[plot]`` from the root directory of the repo. - **For vision tasks**:
-Calling ``pip install omnixai[vision]``, or ``pip install .[vision]`` from the
-root directory of the repo. - **For NLP tasks**: Calling ``pip install omnixai
-[nlp]``, or ``pip install .[nlp]`` from the root directory of the repo. -
-**Install all the dependencies**: Calling ``pip install omnixai[all]``, or
-``pip install .[all]`` from the root directory of the repo. ## Getting Started
-For example code and an introduction to the library, see the Jupyter notebooks
-in [tutorials](https://opensource.salesforce.com/OmniXAI/latest/
-tutorials.html), and the guided walkthrough [here](https://
+â | | | | GPT explainer | Black box | Local | | â | | | | | LIME | Black
+box | Local | | â | â | â | | | SHAP | Black box* | Local | | â | â |
+â | â | | What-if | Black box | Local | | â | | | | | Integrated gradient
+| Torch or TF | Local | | â | â | â | | | Counterfactual | Black box* |
+Local | | â | â | â | â | | Contrastive explanation | Torch or TF |
+Local | | | â | | | | Grad-CAM, Grad-CAM++ | Torch or TF | Local | | | â |
+| | | Score-CAM | Torch or TF | Local | | | â | | | | Layer-CAM | Torch or TF
+| Local | | | â | | | | Smooth gradient | Torch or TF | Local | | | â | | |
+| Guided backpropagation | Torch or TF | Local | | | â | | | | Learning to
+explain | Black box | Local | | â | â | â | | | Linear models | Linear
+models | Global and Local | | â | | | | | Tree models | Tree models | Global
+and Local | | â | | | | *SHAP* accepts black box models for tabular data,
+PyTorch/Tensorflow models for image data, transformer models for text data.
+*Counterfactual* accepts black box models for tabular, text and time-series
+data, and PyTorch/Tensorflow models for image data. This [table](https://
+opensource.salesforce.com/OmniXAI/latest/index.html#comparison-with-
+competitors) shows the comparison between our toolkit/library and other
+existing XAI toolkits/libraries in literature. **OmniXAI also integrates
+ChatGPT for generating plain text explanations given a classification/
+regression model on tabular datasets.** The generated results may not be 100%
+accurate, but it is worth trying this explainer (we will continue improving the
+input prompts). ## Installation You can install ``omnixai`` from PyPI by
+calling ``pip install omnixai``. You may install from source by cloning the
+OmniXAI repo, navigating to the root directory, and calling ``pip install .``,
+or ``pip install -e .`` to install in editable mode. You may install additional
+dependencies: - **For plotting & visualization**: Calling ``pip install omnixai
+[plot]``, or ``pip install .[plot]`` from the root directory of the repo. -
+**For vision tasks**: Calling ``pip install omnixai[vision]``, or ``pip install
+.[vision]`` from the root directory of the repo. - **For NLP tasks**: Calling
+``pip install omnixai[nlp]``, or ``pip install .[nlp]`` from the root directory
+of the repo. - **Install all the dependencies**: Calling ``pip install omnixai
+[all]``, or ``pip install .[all]`` from the root directory of the repo. ##
+Getting Started For example code and an introduction to the library, see the
+Jupyter notebooks in [tutorials](https://opensource.salesforce.com/OmniXAI/
+latest/tutorials.html), and the guided walkthrough [here](https://
 opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be
 found [here](https://sfr-omnixai-demo.herokuapp.com/). Some examples: 1.
 [Tabular classification](https://github.com/salesforce/OmniXAI/blob/main/
 tutorials/tabular_classification.ipynb) 2. [Tabular regression](https://
 github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_regression.ipynb) 3.
 [Image classification](https://github.com/salesforce/OmniXAI/blob/main/
 tutorials/vision.ipynb) 4. [Text classification](https://github.com/salesforce/
@@ -207,19 +216,26 @@
 local_explanations=local_explanations, # Set the local explanations
 global_explanations=global_explanations, # Set the global explanations
 prediction_explanations=prediction_explanations, # Set the prediction metrics
 class_names=class_names, # Set class names explainer=explainer # The created
 TabularExplainer for what if analysis ) dashboard.show() # Launch the dashboard
 ``` After opening the Dash app in the browser, we will see a dashboard showing
 the explanations: ![alt text](https://github.com/salesforce/OmniXAI/raw/main/
-docs/_static/demo.gif) For vision tasks, the same interface is used to create
-explainers and generate explanations. Let's take an image classification model
-as an example. ```python from omnixai.explainers.vision import VisionExplainer
-from omnixai.visualization.dashboard import Dashboard explainer =
-VisionExplainer( explainers=["gradcam", "lime", "ig", "ce",
+docs/_static/demo.gif) You can also use the GPT explainer to generate
+explanations in text for tabular models: ```python explainer = TabularExplainer
+( explainers=["gpt"], # The GPT explainer to apply mode="classification", # The
+task type data=train_data, # The data for initializing the explainers
+model=model, # The ML model to explain preprocess=lambda z:
+transformer.transform(z), # Converts raw features into the model inputs params=
+{ "gpt": {"apikey": "xxxx"} } # Set the OpenAI API KEY ) local_explanations =
+explainer.explain(X=test_instances) ``` For vision tasks, the same interface is
+used to create explainers and generate explanations. Let's take an image
+classification model as an example. ```python from omnixai.explainers.vision
+import VisionExplainer from omnixai.visualization.dashboard import Dashboard
+explainer = VisionExplainer( explainers=["gradcam", "lime", "ig", "ce",
 "feature_visualization"], mode="classification", model=model, # An image
 classification model, e.g., ResNet50 preprocess=preprocess, # The preprocessing
 function postprocess=postprocess, # The postprocessing function params={ # Set
 the target layer for GradCAM "gradcam": {"target_layer": model.layer4[-1]}, #
 Set the objective for feature visualization "feature_visualization":
 {"objectives": [{"layer": model.layer4[-3], "type": "channel", "index": list
 (range(6))}]} }, ) # Generate explanations of GradCAM, LIME, IG and CE
```

### Comparing `omnixai-1.2.5/README.md` & `omnixai-1.3.0/omnixai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: omnixai
+Version: 1.3.0
+Summary: OmniXAI: An Explainable AI Toolbox
+Home-page: https://github.com/salesforce/omnixai
+Author: Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi
+License: 3-Clause BSD
+Keywords: XAI Explainable AI Explanation
+Requires-Python: >=3.7,<4
+Description-Content-Type: text/markdown
+Provides-Extra: plot
+Provides-Extra: vision
+Provides-Extra: nlp
+Provides-Extra: bentoml
+Provides-Extra: all
+License-File: LICENSE
+
 <p align="center">
     <br>
     <img src="https://github.com/salesforce/OmniXAI/raw/main/docs/_static/logo_small.png" width="400"/>
     <br>
 <p>
 
 # OmniXAI: A Library for Explainable AI
@@ -30,14 +47,20 @@
 4. [Documentation](https://opensource.salesforce.com/OmniXAI/latest/index.html)
 5. [Tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html)
 6. [Deployment](#deployment)
 7. [Dashboard Demo](https://sfr-omnixai-demo.herokuapp.com/)
 8. [How to Contribute](https://opensource.salesforce.com/OmniXAI/latest/omnixai.html#how-to-contribute)
 9. [Technical Report and Citing OmniXAI](#technical-report-and-citing-omnixai)
 
+## What's New
+
+The latest version includes an experimental GPT explainer. This explainer leverages the outcomes 
+produced by SHAP and MACE to formulate the input prompt for ChatGPT. Subsequently, ChatGPT 
+analyzes these results and generates the corresponding explanations that provide developers with 
+a clearer understanding of the rationale behind the model's predictions.
 
 ## Introduction
 
 OmniXAI (short for Omni eXplainable AI) is a Python machine-learning library for explainable AI (XAI), offering omni-way explainable AI and interpretable 
 machine learning capabilities to address many pain points in explaining decisions made by machine learning 
 models in practice. OmniXAI aims to be a one-stop comprehensive library that makes explainable AI easy for 
 data scientists, ML researchers and practitioners who need explanation for various types of data, models and 
@@ -63,17 +86,18 @@
 |       Bias metrics        |   Black box   |      Global      |     |    ✅    |       |      |      |
 | Partial dependence plots  |   Black box   |      Global      |     |    ✅    |       |      |      |
 | Accumulated local effects |   Black box   |      Global      |     |    ✅    |       |      |      |
 |   Sensitivity analysis    |   Black box   |      Global      |     |    ✅    |       |      |      |
 |  Permutation explanation  |   Black box   |      Global      |     |    ✅    |       |      |      |
 |   Feature visualization   |  Torch or TF  |      Global      |     |         |   ✅   |      |      |
 |       Feature maps        |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
+|       GPT explainer       | Black box     |     Local        |     |    ✅    |       |      |      |
 |           LIME            |   Black box   |      Local       |     |    ✅    |   ✅   | ✅   |      |
 |           SHAP            |  Black box*   |      Local       |     |    ✅    |   ✅   | ✅   |  ✅  |
-|         What-if           |  Black box    |      Local       |     |    ✅    |       |      |     |
+|          What-if          |   Black box   |      Local       |     |    ✅    |       |      |     |
 |    Integrated gradient    |  Torch or TF  |      Local       |     |    ✅    |   ✅   | ✅   |      |
 |      Counterfactual       |  Black box*   |      Local       |     |    ✅    |   ✅   | ✅   |  ✅  |
 |  Contrastive explanation  |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |   Grad-CAM, Grad-CAM++    |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |         Score-CAM         |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |         Layer-CAM         |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |      Smooth gradient      |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
@@ -86,14 +110,18 @@
 for text data. *Counterfactual* accepts black box models for tabular, text and time-series data, and PyTorch/Tensorflow models for
 image data.
 
 This [table](https://opensource.salesforce.com/OmniXAI/latest/index.html#comparison-with-competitors) 
 shows the comparison between our toolkit/library and other existing XAI toolkits/libraries
 in literature.
 
+**OmniXAI also integrates ChatGPT for generating plain text explanations given a classification/regression
+model on tabular datasets.** The generated results may not be 100% accurate, but it is worth trying this 
+explainer (we will continue improving the input prompts).
+
 ## Installation
 
 You can install ``omnixai`` from PyPI by calling ``pip install omnixai``. You may install from source by
 cloning the OmniXAI repo, navigating to the root directory, and calling
 ``pip install .``, or ``pip install -e .`` to install in editable mode. You may install additional dependencies:
 
 - **For plotting & visualization**: Calling ``pip install omnixai[plot]``, or ``pip install .[plot]`` from the
@@ -280,14 +308,30 @@
 )
 dashboard.show()                                    # Launch the dashboard
 ```
 
 After opening the Dash app in the browser, we will see a dashboard showing the explanations:
 ![alt text](https://github.com/salesforce/OmniXAI/raw/main/docs/_static/demo.gif)
 
+You can also use the GPT explainer to generate explanations in text for tabular models:
+
+```python
+explainer = TabularExplainer(
+  explainers=["gpt"],                                # The GPT explainer to apply
+  mode="classification",                             # The task type
+  data=train_data,                                   # The data for initializing the explainers
+  model=model,                                       # The ML model to explain
+  preprocess=lambda z: transformer.transform(z),     # Converts raw features into the model inputs
+  params={
+     "gpt": {"apikey": "xxxx"}
+  }                                                  # Set the OpenAI API KEY
+)
+local_explanations = explainer.explain(X=test_instances)
+```
+
 For vision tasks, the same interface is used to create explainers and generate explanations. 
 Let's take an image classification model as an example.
 
 ```python
 from omnixai.explainers.vision import VisionExplainer
 from omnixai.visualization.dashboard import Dashboard
```

#### html2text {}

```diff
@@ -1,22 +1,34 @@
+Metadata-Version: 2.1 Name: omnixai Version: 1.3.0 Summary: OmniXAI: An
+Explainable AI Toolbox Home-page: https://github.com/salesforce/omnixai Author:
+Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi
+License: 3-Clause BSD Keywords: XAI Explainable AI Explanation Requires-Python:
+>=3.7,<4 Description-Content-Type: text/markdown Provides-Extra: plot Provides-
+Extra: vision Provides-Extra: nlp Provides-Extra: bentoml Provides-Extra: all
+License-File: LICENSE
 
  [https://github.com/salesforce/OmniXAI/raw/main/docs/_static/logo_small.png]
 # OmniXAI: A Library for Explainable AI
     [https://img.shields.io/badge/Python-3.7,_3.8,_3.9,_3.10-blue] [PyPI]
                        [Documentation] [Downloads] [DOI]
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
 (https://opensource.salesforce.com/OmniXAI/latest/index.html) 5. [Tutorials]
 (https://opensource.salesforce.com/OmniXAI/latest/tutorials.html) 6.
 [Deployment](#deployment) 7. [Dashboard Demo](https://sfr-omnixai-
 demo.herokuapp.com/) 8. [How to Contribute](https://opensource.salesforce.com/
 OmniXAI/latest/omnixai.html#how-to-contribute) 9. [Technical Report and Citing
-OmniXAI](#technical-report-and-citing-omnixai) ## Introduction OmniXAI (short
-for Omni eXplainable AI) is a Python machine-learning library for explainable
-AI (XAI), offering omni-way explainable AI and interpretable machine learning
+OmniXAI](#technical-report-and-citing-omnixai) ## What's New The latest version
+includes an experimental GPT explainer. This explainer leverages the outcomes
+produced by SHAP and MACE to formulate the input prompt for ChatGPT.
+Subsequently, ChatGPT analyzes these results and generates the corresponding
+explanations that provide developers with a clearer understanding of the
+rationale behind the model's predictions. ## Introduction OmniXAI (short for
+Omni eXplainable AI) is a Python machine-learning library for explainable AI
+(XAI), offering omni-way explainable AI and interpretable machine learning
 capabilities to address many pain points in explaining decisions made by
 machine learning models in practice. OmniXAI aims to be a one-stop
 comprehensive library that makes explainable AI easy for data scientists, ML
 researchers and practitioners who need explanation for various types of data,
 models and explanation methods at different stages of ML process: ![alt text]
 (https://github.com/salesforce/OmniXAI/raw/main/docs/_static/ml_pipeline.png)
 OmniXAI includes a rich family of explanation methods integrated in a unified
@@ -37,45 +49,49 @@
 â | | | | | | Feature selection | NA | Global | â | | | | | | Prediction
 metrics | Black box | Global | | â | â | â | â | | Bias metrics | Black
 box | Global | | â | | | | | Partial dependence plots | Black box | Global |
 | â | | | | | Accumulated local effects | Black box | Global | | â | | | |
 | Sensitivity analysis | Black box | Global | | â | | | | | Permutation
 explanation | Black box | Global | | â | | | | | Feature visualization |
 Torch or TF | Global | | | â | | | | Feature maps | Torch or TF | Local | | |
-â | | | | LIME | Black box | Local | | â | â | â | | | SHAP | Black
-box* | Local | | â | â | â | â | | What-if | Black box | Local | | â
-| | | | | Integrated gradient | Torch or TF | Local | | â | â | â | | |
-Counterfactual | Black box* | Local | | â | â | â | â | | Contrastive
-explanation | Torch or TF | Local | | | â | | | | Grad-CAM, Grad-CAM++ |
-Torch or TF | Local | | | â | | | | Score-CAM | Torch or TF | Local | | | â
-| | | | Layer-CAM | Torch or TF | Local | | | â | | | | Smooth gradient |
-Torch or TF | Local | | | â | | | | Guided backpropagation | Torch or TF |
-Local | | | â | | | | Learning to explain | Black box | Local | | â | â |
-â | | | Linear models | Linear models | Global and Local | | â | | | | |
-Tree models | Tree models | Global and Local | | â | | | | *SHAP* accepts
-black box models for tabular data, PyTorch/Tensorflow models for image data,
-transformer models for text data. *Counterfactual* accepts black box models for
-tabular, text and time-series data, and PyTorch/Tensorflow models for image
-data. This [table](https://opensource.salesforce.com/OmniXAI/latest/
-index.html#comparison-with-competitors) shows the comparison between our
-toolkit/library and other existing XAI toolkits/libraries in literature. ##
-Installation You can install ``omnixai`` from PyPI by calling ``pip install
-omnixai``. You may install from source by cloning the OmniXAI repo, navigating
-to the root directory, and calling ``pip install .``, or ``pip install -e .``
-to install in editable mode. You may install additional dependencies: - **For
-plotting & visualization**: Calling ``pip install omnixai[plot]``, or ``pip
-install .[plot]`` from the root directory of the repo. - **For vision tasks**:
-Calling ``pip install omnixai[vision]``, or ``pip install .[vision]`` from the
-root directory of the repo. - **For NLP tasks**: Calling ``pip install omnixai
-[nlp]``, or ``pip install .[nlp]`` from the root directory of the repo. -
-**Install all the dependencies**: Calling ``pip install omnixai[all]``, or
-``pip install .[all]`` from the root directory of the repo. ## Getting Started
-For example code and an introduction to the library, see the Jupyter notebooks
-in [tutorials](https://opensource.salesforce.com/OmniXAI/latest/
-tutorials.html), and the guided walkthrough [here](https://
+â | | | | GPT explainer | Black box | Local | | â | | | | | LIME | Black
+box | Local | | â | â | â | | | SHAP | Black box* | Local | | â | â |
+â | â | | What-if | Black box | Local | | â | | | | | Integrated gradient
+| Torch or TF | Local | | â | â | â | | | Counterfactual | Black box* |
+Local | | â | â | â | â | | Contrastive explanation | Torch or TF |
+Local | | | â | | | | Grad-CAM, Grad-CAM++ | Torch or TF | Local | | | â |
+| | | Score-CAM | Torch or TF | Local | | | â | | | | Layer-CAM | Torch or TF
+| Local | | | â | | | | Smooth gradient | Torch or TF | Local | | | â | | |
+| Guided backpropagation | Torch or TF | Local | | | â | | | | Learning to
+explain | Black box | Local | | â | â | â | | | Linear models | Linear
+models | Global and Local | | â | | | | | Tree models | Tree models | Global
+and Local | | â | | | | *SHAP* accepts black box models for tabular data,
+PyTorch/Tensorflow models for image data, transformer models for text data.
+*Counterfactual* accepts black box models for tabular, text and time-series
+data, and PyTorch/Tensorflow models for image data. This [table](https://
+opensource.salesforce.com/OmniXAI/latest/index.html#comparison-with-
+competitors) shows the comparison between our toolkit/library and other
+existing XAI toolkits/libraries in literature. **OmniXAI also integrates
+ChatGPT for generating plain text explanations given a classification/
+regression model on tabular datasets.** The generated results may not be 100%
+accurate, but it is worth trying this explainer (we will continue improving the
+input prompts). ## Installation You can install ``omnixai`` from PyPI by
+calling ``pip install omnixai``. You may install from source by cloning the
+OmniXAI repo, navigating to the root directory, and calling ``pip install .``,
+or ``pip install -e .`` to install in editable mode. You may install additional
+dependencies: - **For plotting & visualization**: Calling ``pip install omnixai
+[plot]``, or ``pip install .[plot]`` from the root directory of the repo. -
+**For vision tasks**: Calling ``pip install omnixai[vision]``, or ``pip install
+.[vision]`` from the root directory of the repo. - **For NLP tasks**: Calling
+``pip install omnixai[nlp]``, or ``pip install .[nlp]`` from the root directory
+of the repo. - **Install all the dependencies**: Calling ``pip install omnixai
+[all]``, or ``pip install .[all]`` from the root directory of the repo. ##
+Getting Started For example code and an introduction to the library, see the
+Jupyter notebooks in [tutorials](https://opensource.salesforce.com/OmniXAI/
+latest/tutorials.html), and the guided walkthrough [here](https://
 opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be
 found [here](https://sfr-omnixai-demo.herokuapp.com/). Some examples: 1.
 [Tabular classification](https://github.com/salesforce/OmniXAI/blob/main/
 tutorials/tabular_classification.ipynb) 2. [Tabular regression](https://
 github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_regression.ipynb) 3.
 [Image classification](https://github.com/salesforce/OmniXAI/blob/main/
 tutorials/vision.ipynb) 4. [Text classification](https://github.com/salesforce/
@@ -200,19 +216,26 @@
 local_explanations=local_explanations, # Set the local explanations
 global_explanations=global_explanations, # Set the global explanations
 prediction_explanations=prediction_explanations, # Set the prediction metrics
 class_names=class_names, # Set class names explainer=explainer # The created
 TabularExplainer for what if analysis ) dashboard.show() # Launch the dashboard
 ``` After opening the Dash app in the browser, we will see a dashboard showing
 the explanations: ![alt text](https://github.com/salesforce/OmniXAI/raw/main/
-docs/_static/demo.gif) For vision tasks, the same interface is used to create
-explainers and generate explanations. Let's take an image classification model
-as an example. ```python from omnixai.explainers.vision import VisionExplainer
-from omnixai.visualization.dashboard import Dashboard explainer =
-VisionExplainer( explainers=["gradcam", "lime", "ig", "ce",
+docs/_static/demo.gif) You can also use the GPT explainer to generate
+explanations in text for tabular models: ```python explainer = TabularExplainer
+( explainers=["gpt"], # The GPT explainer to apply mode="classification", # The
+task type data=train_data, # The data for initializing the explainers
+model=model, # The ML model to explain preprocess=lambda z:
+transformer.transform(z), # Converts raw features into the model inputs params=
+{ "gpt": {"apikey": "xxxx"} } # Set the OpenAI API KEY ) local_explanations =
+explainer.explain(X=test_instances) ``` For vision tasks, the same interface is
+used to create explainers and generate explanations. Let's take an image
+classification model as an example. ```python from omnixai.explainers.vision
+import VisionExplainer from omnixai.visualization.dashboard import Dashboard
+explainer = VisionExplainer( explainers=["gradcam", "lime", "ig", "ce",
 "feature_visualization"], mode="classification", model=model, # An image
 classification model, e.g., ResNet50 preprocess=preprocess, # The preprocessing
 function postprocess=postprocess, # The postprocessing function params={ # Set
 the target layer for GradCAM "gradcam": {"target_layer": model.layer4[-1]}, #
 Set the objective for feature visualization "feature_visualization":
 {"objectives": [{"layer": model.layer4[-3], "type": "channel", "index": list
 (range(6))}]} }, ) # Generate explanations of GradCAM, LIME, IG and CE
```

### Comparing `omnixai-1.2.5/docs/conf.py` & `omnixai-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `omnixai-1.2.5/omnixai/data/base.py` & `omnixai-1.3.0/omnixai/data/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The base class for all data types.
 """
```

### Comparing `omnixai-1.2.5/omnixai/data/image.py` & `omnixai-1.3.0/omnixai/data/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The class for image data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/data/multi_inputs.py` & `omnixai-1.3.0/omnixai/data/multi_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The class for multiple inputs.
 """
```

### Comparing `omnixai-1.2.5/omnixai/data/tabular.py` & `omnixai-1.3.0/omnixai/data/tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The class for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/data/text.py` & `omnixai-1.3.0/omnixai/data/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The class for text data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/data/timeseries.py` & `omnixai-1.3.0/omnixai/data/timeseries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The class for time series data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/deployment/bentoml/omnixai.py` & `omnixai-1.3.0/omnixai/deployment/bentoml/omnixai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from __future__ import annotations
 
 import json
```

### Comparing `omnixai-1.2.5/omnixai/explainers/base.py` & `omnixai-1.3.0/omnixai/explainers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The base classes for the supported explainers.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/data/__init__.py` & `omnixai-1.3.0/omnixai/explainers/data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from .auto import DataAnalyzer
 from .imbalance import ImbalanceAnalyzer
 from .correlation import CorrelationAnalyzer
```

### Comparing `omnixai-1.2.5/omnixai/explainers/data/auto.py` & `omnixai-1.3.0/omnixai/explainers/data/auto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from typing import Collection, Dict
 
 from ...data.tabular import Tabular
```

### Comparing `omnixai-1.2.5/omnixai/explainers/data/chi_square.py` & `omnixai-1.3.0/omnixai/explainers/data/chi_square.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The class for computing chi-squared stats between each non-negative feature and target.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/data/correlation.py` & `omnixai-1.3.0/omnixai/explainers/data/correlation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The class for feature correlation analysis.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/data/imbalance.py` & `omnixai-1.3.0/omnixai/explainers/data/imbalance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The class for checking feature imbalances.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/data/mutual_info.py` & `omnixai-1.3.0/omnixai/explainers/data/mutual_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The class for estimating mutual information.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/nlp/__init__.py` & `omnixai-1.3.0/omnixai/explainers/nlp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from .auto import NLPExplainer
 from .agnostic.lime import LimeText
 from .agnostic.shap import ShapText
```

### Comparing `omnixai-1.2.5/omnixai/explainers/nlp/agnostic/l2x.py` & `omnixai-1.3.0/omnixai/explainers/nlp/agnostic/l2x.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The L2X explainer for NLP tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/nlp/agnostic/lime.py` & `omnixai-1.3.0/omnixai/explainers/nlp/agnostic/lime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The LIME explainer for text classification.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/nlp/agnostic/shap.py` & `omnixai-1.3.0/omnixai/explainers/nlp/agnostic/shap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The SHAP explainer for text classification.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/nlp/auto.py` & `omnixai-1.3.0/omnixai/explainers/nlp/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from typing import Collection, Callable, Any, Dict
 
 from ...data.text import Text
```

### Comparing `omnixai-1.2.5/omnixai/explainers/nlp/counterfactual/polyjuice.py` & `omnixai-1.3.0/omnixai/explainers/nlp/counterfactual/polyjuice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The NLP counterfactual explainer based on the Polyjuice model.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/nlp/specific/ig.py` & `omnixai-1.3.0/omnixai/explainers/nlp/specific/ig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The integrated-gradient explainer for NLP tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/prediction/auto.py` & `omnixai-1.3.0/omnixai/explainers/prediction/auto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The prediction analysis for classification and regression.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/ranking/agnostic/permutation.py` & `omnixai-1.3.0/omnixai/explainers/ranking/agnostic/permutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Feature Permutation Ranking Explainer for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/ranking/agnostic/validity.py` & `omnixai-1.3.0/omnixai/explainers/ranking/agnostic/validity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Ranking Explainer for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/ranking/counterfactual/mace.py` & `omnixai-1.3.0/omnixai/explainers/ranking/counterfactual/mace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The Model-Agnostic Counterfactual Explanation (MACE) for ranking tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/__init__.py` & `omnixai-1.3.0/omnixai/explainers/tabular/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from .auto import TabularExplainer
 from .agnostic.lime import LimeTabular
 from .agnostic.shap import ShapTabular
 from .agnostic.pdp import PartialDependenceTabular
 from .agnostic.ale import ALE
 from .agnostic.sensitivity import SensitivityAnalysisTabular
 from .agnostic.L2X.l2x import L2XTabular
 from .agnostic.permutation import PermutationImportance
 from .agnostic.shap_global import GlobalShapTabular
 from .agnostic.bias import BiasAnalyzer
+from .agnostic.gpt import GPTExplainer
 from .counterfactual.mace.mace import MACEExplainer
 from .counterfactual.ce import CounterfactualExplainer
 from .counterfactual.knn import KNNCounterfactualExplainer
 from .specific.ig import IntegratedGradientTabular
 from .specific.linear import LinearRegression
 from .specific.linear import LogisticRegression
 from .specific.decision_tree import TreeClassifier
@@ -32,14 +33,15 @@
     "PartialDependenceTabular",
     "ALE",
     "SensitivityAnalysisTabular",
     "L2XTabular",
     "PermutationImportance",
     "GlobalShapTabular",
     "BiasAnalyzer",
+    "GPTExplainer",
     "MACEExplainer",
     "CounterfactualExplainer",
     "KNNCounterfactualExplainer",
     "LinearRegression",
     "LogisticRegression",
     "TreeRegressor",
     "TreeClassifier",
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/agnostic/L2X/l2x.py` & `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/l2x.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The L2X explainer for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/agnostic/L2X/utils.py` & `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/L2X/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import torch
 import torch.nn as nn
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/agnostic/ale.py` & `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/ale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The accumulated local effects plots for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/agnostic/bias.py` & `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/bias.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The model bias analyzer for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/agnostic/lime.py` & `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/lime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The LIME explainer for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/agnostic/pdp.py` & `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/pdp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The partial dependence plots for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/agnostic/permutation.py` & `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/permutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The permutation feature importance explanation for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/agnostic/sensitivity.py` & `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/sensitivity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Morris sensitivity analysis for tabular data
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/agnostic/shap.py` & `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/shap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The SHAP explainer for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/agnostic/shap_global.py` & `omnixai-1.3.0/omnixai/explainers/tabular/agnostic/shap_global.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The SHAP explainer for global feature importance.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/auto.py` & `omnixai-1.3.0/omnixai/explainers/tabular/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 import pandas as pd
 from typing import Collection, Callable, Any, Dict
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/base.py` & `omnixai-1.3.0/omnixai/explainers/tabular/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import sklearn
 import numpy as np
 import pandas as pd
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/ce.py` & `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/ce.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The basic counterfactual explainer for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/knn.py` & `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/knn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The KNN-based counterfactual explainer for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/diversify.py` & `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/diversify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 import pandas as pd
 from typing import Callable
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/gld.py` & `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/gld.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 import pandas as pd
 from collections import deque
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/greedy.py` & `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/greedy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 from typing import Dict, Callable
 from .....data.tabular import Tabular
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/mace.py` & `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/mace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The Model-Agnostic Counterfactual Explanation (MACE) for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/refine.py` & `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/refine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import pandas as pd
 from typing import Dict, Callable, Union
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/retrieval.py` & `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/retrieval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 import pandas as pd
 from collections import defaultdict, Counter
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/counterfactual/mace/rl.py` & `omnixai-1.3.0/omnixai/explainers/tabular/counterfactual/mace/rl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 import pandas as pd
 from typing import Dict, Callable
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/specific/decision_tree.py` & `omnixai-1.3.0/omnixai/explainers/tabular/specific/decision_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The explainable tree-based models.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/specific/ig.py` & `omnixai-1.3.0/omnixai/explainers/tabular/specific/ig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The integrated-gradient explainer for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/specific/linear.py` & `omnixai-1.3.0/omnixai/explainers/tabular/specific/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The explainable linear models.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/tabular/specific/shap_tree.py` & `omnixai-1.3.0/omnixai/explainers/tabular/specific/shap_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The tree-specific SHAP explainer for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/timeseries/__init__.py` & `omnixai-1.3.0/omnixai/explainers/timeseries/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from .auto import TimeseriesExplainer
 from .agnostic.shap import ShapTimeseries
 from .counterfactual.ce import CounterfactualExplainer
```

### Comparing `omnixai-1.2.5/omnixai/explainers/timeseries/agnostic/shap.py` & `omnixai-1.3.0/omnixai/explainers/timeseries/agnostic/shap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The SHAP explainer for time series tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/timeseries/auto.py` & `omnixai-1.3.0/omnixai/explainers/timeseries/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from typing import Collection, Callable, Any, Dict
 
 from ...data.timeseries import Timeseries
```

### Comparing `omnixai-1.2.5/omnixai/explainers/timeseries/counterfactual/ce.py` & `omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/ce.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The basic counterfactual explainer for time series tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/timeseries/counterfactual/mace.py` & `omnixai-1.3.0/omnixai/explainers/timeseries/counterfactual/mace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The Model-Agnostic Counterfactual Explanation (MACE) designed for time series tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/__init__.py` & `omnixai-1.3.0/omnixai/explainers/vision/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from .auto import VisionExplainer
 from .agnostic.lime import LimeImage
 from .agnostic.shap import ShapImage
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/agnostic/l2x.py` & `omnixai-1.3.0/omnixai/explainers/vision/agnostic/l2x.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The L2X explainer for image data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/agnostic/lime.py` & `omnixai-1.3.0/omnixai/explainers/vision/agnostic/lime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The LIME explainer for image classification.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/agnostic/pdp.py` & `omnixai-1.3.0/omnixai/explainers/vision/agnostic/pdp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The partial dependence plots for vision tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/agnostic/shap.py` & `omnixai-1.3.0/omnixai/explainers/vision/agnostic/shap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The SHAP explainer for vision tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/auto.py` & `omnixai-1.3.0/omnixai/explainers/vision/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from typing import Collection, Callable, Any, Dict
 
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/counterfactual/ce.py` & `omnixai-1.3.0/omnixai/explainers/vision/counterfactual/ce.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The counterfactual explainer for image classification.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/cem.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/cem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The contrastive explainer for image classification.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/pytorch/feature_maps.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/feature_maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import torch.nn as nn
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/pytorch/optimizer.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import torch
 import torchvision
 import torch.nn as nn
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/pytorch/preprocess.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/pytorch/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import torch
 import torchvision
 from packaging import version
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/tf/optimizer.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import itertools
 import numpy as np
 import tensorflow as tf
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/tf/preprocess.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/tf/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 import tensorflow as tf
 from omnixai.preprocessing.base import TransformBase
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/utils.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import itertools
 import numpy as np
 from typing import Union, List, Any
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/feature_visualization/visualizer.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/feature_visualization/visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The feature visualizer for vision models.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/gradcam/gradcam.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/gradcam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The Grad-CAM methods for vision tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/gradcam/pytorch/gradcam.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/pytorch/gradcam.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 from typing import Callable
 from abc import abstractmethod
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/gradcam/tf/gradcam.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/gradcam/tf/gradcam.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 from typing import Callable
 from abc import abstractmethod
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/guided_bp.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/guided_bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from typing import Callable
 from omnixai.utils.misc import is_tf_available, is_torch_available
 from omnixai.explainers.base import ExplainerBase
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/ig.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/ig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The integrated-gradient explainer for vision tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/pytorch/scorecam.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/pytorch/scorecam.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 from scipy.special import softmax
 from typing import Callable
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/scorecam.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/scorecam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The Score-CAM methods for vision tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/tf/scorecam.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/tf/scorecam.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 from scipy.special import softmax
 from typing import Callable
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/scorecam/utils.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/scorecam/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import numpy as np
 from omnixai.data.image import Image
 from omnixai.preprocessing.image import Resize
 
 
 class ScoreCAMMixin:
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/smoothgrad.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/smoothgrad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from typing import Callable
 from omnixai.utils.misc import is_tf_available, is_torch_available
 from omnixai.explainers.base import ExplainerBase
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision/specific/utils.py` & `omnixai-1.3.0/omnixai/explainers/vision/specific/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 from omnixai.utils.misc import is_tf_available, is_torch_available
 from omnixai.data.image import Image
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision_language/specific/gradcam/gradcam.py` & `omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/gradcam.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The Grad-CAM methods for vision-language models.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision_language/specific/gradcam/pytorch/gradcam.py` & `omnixai-1.3.0/omnixai/explainers/vision_language/specific/gradcam/pytorch/gradcam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import inspect
 import numpy as np
 from typing import Callable
```

### Comparing `omnixai-1.2.5/omnixai/explainers/vision_language/specific/ig.py` & `omnixai-1.3.0/omnixai/explainers/vision_language/specific/ig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The integrated-gradient explainer for vision-language models.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/base.py` & `omnixai-1.3.0/omnixai/explanations/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import dill
 import numpy as np
 from abc import abstractmethod
@@ -293,7 +293,71 @@
         return plotly.offline.iplot(self._plotly_figure(index, class_names=class_names, **kwargs))
 
     @classmethod
     def from_dict(cls, d):
         self = cls.__new__(PredictedResults)
         self.results = d["results"]
         return self
+
+
+class PlainText(ExplanationBase):
+    """
+    The class for plain text explanations.
+    """
+
+    def __init__(self, explanations=None):
+        """
+        :param explanations: The explanation results for initializing ``FeatureImportance``,
+            which is optional.
+        """
+        super().__init__()
+        self.explanations = [] if explanations is None else explanations
+
+    def __repr__(self):
+        return repr(self.explanations)
+
+    def __getitem__(self, i: int):
+        assert i < len(self.explanations)
+        return PlainText(explanations=[self.explanations[i]])
+
+    def add(self, instance, text, **kwargs):
+        """
+        Adds the generated explanation corresponding to one instance.
+
+        :param instance: The instance to explain.
+        :param text: The text explanation of the given instance.
+        """
+        e = {"instance": instance, "text": text}
+        e.update(kwargs)
+        self.explanations.append(e)
+
+    def get_explanations(self, index=None):
+        """
+        Gets the generated explanations.
+
+        :param index: The index of an explanation result stored in ``PlainText``.
+            When ``index`` is None, the function returns a list of all the explanations.
+        :return: The explanation for one specific instance (a dict)
+            or the explanations for all the instances (a list of dicts).
+            Each dict has the following format: `{"instance": the input instance,
+            "text": the corresponding explanations in plain text}`.
+        :rtype: Union[Dict, List]
+        """
+        return self.explanations if index is None else self.explanations[index]
+
+    def plot(self, **kwargs):
+        raise NotImplementedError
+
+    def plotly_plot(self, **kwargs):
+        raise NotImplementedError
+
+    def ipython_plot(self, **kwargs):
+        raise NotImplementedError
+
+    @classmethod
+    def from_dict(cls, d):
+        import pandas as pd
+        explanations = []
+        for e in d["explanations"]:
+            e["instance"] = pd.DataFrame.from_dict(e["instance"])
+            explanations.append(e)
+        return PlainText(explanations=explanations)
```

### Comparing `omnixai-1.2.5/omnixai/explanations/image/contrast.py` & `omnixai-1.3.0/omnixai/explanations/image/contrast.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Contrastive explanations for vision tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/image/counterfactual.py` & `omnixai-1.3.0/omnixai/explanations/image/counterfactual.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Counterfactual explanations for vision tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/image/mask.py` & `omnixai-1.3.0/omnixai/explanations/image/mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Image mask explanations for vision tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/image/pixel_importance.py` & `omnixai-1.3.0/omnixai/explanations/image/pixel_importance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Pixel importance explanations for vision tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/image/plain.py` & `omnixai-1.3.0/omnixai/explanations/image/plain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Plain image explanations for vision tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/prediction/confusion.py` & `omnixai-1.3.0/omnixai/explanations/prediction/confusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The confusion matrix.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/prediction/cumulative.py` & `omnixai-1.3.0/omnixai/explanations/prediction/cumulative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The cumulative gains.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/prediction/lift.py` & `omnixai-1.3.0/omnixai/explanations/prediction/lift.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The lift curves.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/prediction/metrics.py` & `omnixai-1.3.0/omnixai/explanations/prediction/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The metrics for classification and regression.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/prediction/pr.py` & `omnixai-1.3.0/omnixai/explanations/prediction/pr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The precision recall curves.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/prediction/residual.py` & `omnixai-1.3.0/omnixai/explanations/prediction/residual.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The regression residual plot.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/prediction/roc.py` & `omnixai-1.3.0/omnixai/explanations/prediction/roc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The ROC curves.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/tabular/ale.py` & `omnixai-1.3.0/omnixai/explanations/tabular/ale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Accumulated local effects plots.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/tabular/bias.py` & `omnixai-1.3.0/omnixai/explanations/tabular/bias.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The bias analysis results for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/tabular/correlation.py` & `omnixai-1.3.0/omnixai/explanations/tabular/correlation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Feature correlation analysis.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/tabular/counterfactual.py` & `omnixai-1.3.0/omnixai/explanations/tabular/counterfactual.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Counterfactual explanations.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/tabular/feature_importance.py` & `omnixai-1.3.0/omnixai/explanations/tabular/feature_importance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Feature importance explanations.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/tabular/imbalance.py` & `omnixai-1.3.0/omnixai/explanations/tabular/imbalance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Feature imbalance plots.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/tabular/linear.py` & `omnixai-1.3.0/omnixai/explanations/tabular/linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Explanations for linear models.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/tabular/pdp.py` & `omnixai-1.3.0/omnixai/explanations/tabular/pdp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Partial dependence plots.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/tabular/sensitivity.py` & `omnixai-1.3.0/omnixai/explanations/tabular/sensitivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Morris sensitivity analysis.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/tabular/tree.py` & `omnixai-1.3.0/omnixai/explanations/tabular/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Explanations for tree-based models.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/tabular/validity.py` & `omnixai-1.3.0/omnixai/explanations/tabular/validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Validity ranking explanation explanations.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/text/word_importance.py` & `omnixai-1.3.0/omnixai/explanations/text/word_importance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Word/token importance explanations for NLP tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/timeseries/counterfactual.py` & `omnixai-1.3.0/omnixai/explanations/timeseries/counterfactual.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Counterfactual explanations for time series tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/explanations/timeseries/feature_importance.py` & `omnixai-1.3.0/omnixai/explanations/timeseries/feature_importance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 Feature importance explanations for time series tasks.
 """
```

### Comparing `omnixai-1.2.5/omnixai/preprocessing/base.py` & `omnixai-1.3.0/omnixai/preprocessing/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The base class for all the transforms.
 """
```

### Comparing `omnixai-1.2.5/omnixai/preprocessing/encode.py` & `omnixai-1.3.0/omnixai/preprocessing/encode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The pre-processing functions for categorical and continuous-valued features.
 """
```

### Comparing `omnixai-1.2.5/omnixai/preprocessing/fill.py` & `omnixai-1.3.0/omnixai/preprocessing/fill.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The pre-processing functions for filling NaNs and missing values.
 """
```

### Comparing `omnixai-1.2.5/omnixai/preprocessing/image.py` & `omnixai-1.3.0/omnixai/preprocessing/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The transformations for image data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/preprocessing/normalize.py` & `omnixai-1.3.0/omnixai/preprocessing/normalize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The pre-processing functions for continuous-valued features.
 """
```

### Comparing `omnixai-1.2.5/omnixai/preprocessing/pipeline.py` & `omnixai-1.3.0/omnixai/preprocessing/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The pipeline for multiple pre-processing transforms.
 """
```

### Comparing `omnixai-1.2.5/omnixai/preprocessing/tabular.py` & `omnixai-1.3.0/omnixai/preprocessing/tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The pre-processing function for tabular data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/preprocessing/text.py` & `omnixai-1.3.0/omnixai/preprocessing/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The pre-processing functions for text data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/sampler/tabular.py` & `omnixai-1.3.0/omnixai/sampler/tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The class for re-sampling training data.
 """
```

### Comparing `omnixai-1.2.5/omnixai/tests/data/test_image.py` & `omnixai-1.3.0/omnixai/tests/data/test_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import torchvision
```

### Comparing `omnixai-1.2.5/omnixai/tests/data/test_multi.py` & `omnixai-1.3.0/omnixai/tests/data/test_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 from PIL import Image as PilImage
```

### Comparing `omnixai-1.2.5/omnixai/tests/data/test_tabular.py` & `omnixai-1.3.0/omnixai/tests/data/test_tabular.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import pandas as pd
```

### Comparing `omnixai-1.2.5/omnixai/tests/data/test_text.py` & `omnixai-1.3.0/omnixai/tests/data/test_text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 from omnixai.data.text import Text
```

### Comparing `omnixai-1.2.5/omnixai/tests/data/test_timeseries.py` & `omnixai-1.3.0/omnixai/tests/data/test_timeseries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import pandas as pd
 from omnixai.data.timeseries import Timeseries
```

### Comparing `omnixai-1.2.5/omnixai/tests/deployment/bentoml/api_server.py` & `omnixai-1.3.0/omnixai/tests/deployment/bentoml/api_server.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import uvicorn
 import socket
 import click
 from bentoml._internal.log import configure_server_logging
 from bentoml._internal.context import component_context
 from omnixai.deployment.bentoml.omnixai import init_service
```

### Comparing `omnixai-1.2.5/omnixai/tests/deployment/bentoml/nlp/model.py` & `omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import torch
 import torch.nn as nn
```

### Comparing `omnixai-1.2.5/omnixai/tests/deployment/bentoml/nlp/request.py` & `omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import requests
 from requests_toolbelt.multipart.encoder import MultipartEncoder
```

### Comparing `omnixai-1.2.5/omnixai/tests/deployment/bentoml/nlp/test.py` & `omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from omnixai.data.text import Text
 from omnixai.deployment.bentoml.omnixai import init_service
```

### Comparing `omnixai-1.2.5/omnixai/tests/deployment/bentoml/nlp/train.py` & `omnixai-1.3.0/omnixai/tests/deployment/bentoml/nlp/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import pandas as pd
 import torch
 import torch.nn as nn
```

### Comparing `omnixai-1.2.5/omnixai/tests/deployment/bentoml/tabular/request.py` & `omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import requests
```

### Comparing `omnixai-1.2.5/omnixai/tests/deployment/bentoml/tabular/test.py` & `omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import numpy as np
 from omnixai.data.tabular import Tabular
```

### Comparing `omnixai-1.2.5/omnixai/tests/deployment/bentoml/tabular/train.py` & `omnixai-1.3.0/omnixai/tests/deployment/bentoml/tabular/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import sklearn
 import sklearn.datasets
```

### Comparing `omnixai-1.2.5/omnixai/tests/deployment/bentoml/vision/request.py` & `omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/deployment/bentoml/vision/save.py` & `omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/save.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import torch
 from torchvision import models, transforms
```

### Comparing `omnixai-1.2.5/omnixai/tests/deployment/bentoml/vision/test.py` & `omnixai-1.3.0/omnixai/tests/deployment/bentoml/vision/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 from PIL import Image as PilImage
 from omnixai.preprocessing.image import Resize
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/L2X/test_l2x.py` & `omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import torch
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/L2X/test_l2x_image_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_image_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import torch
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/L2X/test_l2x_tabular_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_tabular_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pprint
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/L2X/test_l2x_tabular_regression.py` & `omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_tabular_regression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import pprint
 from omnixai.utils.misc import set_random_seed
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/L2X/test_l2x_text_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/L2X/test_l2x_text_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ale/test_ale_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/ale/test_ale_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pprint
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ale/test_ale_regression.py` & `omnixai-1.3.0/omnixai/tests/explainers/ale/test_ale_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import pprint
 from omnixai.utils.misc import set_random_seed
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/bias/test_bias_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/bias/test_bias_classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 from omnixai.utils.misc import set_random_seed
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/bias/test_bias_regression.py` & `omnixai-1.3.0/omnixai/tests/explainers/bias/test_bias_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 from omnixai.utils.misc import set_random_seed
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ce/test_ce_imagenet.py` & `omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_imagenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ce/test_ce_tabular.py` & `omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import torch
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ce/test_ce_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_tf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import tensorflow as tf
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ce/test_ce_timeseries.py` & `omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_timeseries.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import os
 import unittest
 import numpy as np
 from omnixai.utils.misc import set_random_seed
 from omnixai.data.timeseries import Timeseries
 from omnixai.explainers.timeseries.counterfactual.ce import CounterfactualExplainer
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ce/test_ce_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/ce/test_ce_torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import torch
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/cem/cem_optimizer_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/cem/cem_optimizer_tf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import tensorflow as tf
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/cem/cem_optimizer_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/cem/cem_optimizer_torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import torch
 import torch.nn as nn
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/cem/test_cem_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/cem/test_cem_tf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import tensorflow as tf
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/cem/test_cem_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/cem/test_cem_torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import torch
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/data/test_chi2.py` & `omnixai-1.3.0/omnixai/tests/explainers/data/test_chi2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/data/test_correlation.py` & `omnixai-1.3.0/omnixai/tests/explainers/data/test_correlation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/data/test_imbalance.py` & `omnixai-1.3.0/omnixai/tests/explainers/data/test_imbalance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/data/test_mutual.py` & `omnixai-1.3.0/omnixai/tests/explainers/data/test_mutual.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/decision_tree/test_tree_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/decision_tree/test_tree_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pprint
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/decision_tree/test_tree_regression.py` & `omnixai-1.3.0/omnixai/tests/explainers/decision_tree/test_tree_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import pprint
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/example.py` & `omnixai-1.3.0/omnixai/tests/explainers/example.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import matplotlib.pyplot as plt
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/explainer_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/explainer_tf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 from tensorflow.keras.applications import vgg16
 from omnixai.explainers.vision.specific.feature_visualization.tf.optimizer import \
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/explainer_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/explainer_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import torch
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/feature_explainer.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_explainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import torch
 import unittest
 from torchvision import models
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/feature_map_explainer_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_map_explainer_tf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/feature_map_explainer_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/feature_map_explainer_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import torch
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_tf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import tensorflow as tf
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_feature_optimizer_torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import torch.nn as nn
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_fft.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fft.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import torch
 import tensorflow as tf
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_tf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import tensorflow as tf
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_fv_preprocess_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_map_extractor_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_map_extractor_tf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import tensorflow as tf
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/feature_visualization/test_map_extractor_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/feature_visualization/test_map_extractor_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import torch
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/gradcam/test_gradcam_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_gradcam_tf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/gradcam/test_gradcam_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_gradcam_torch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/gradcam/test_layercam_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_layercam_tf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/gradcam/test_layercam_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/gradcam/test_layercam_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/gradcam/vlm_gradcam_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/gradcam/vlm_gradcam_torch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import os
 import torch
 import unittest
 import numpy as np
 from PIL import Image as PilImage
 from omnixai.data.text import Text
 from omnixai.data.image import Image
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/guided_bp/test_guided_bp_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/guided_bp/test_guided_bp_tf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/guided_bp/test_guided_bp_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/guided_bp/test_guided_bp_torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ig/nlp_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/ig/nlp_tf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import pandas as pd
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ig/nlp_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/ig/nlp_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ig/test_compute_integrated_gradients.py` & `omnixai-1.3.0/omnixai/tests/explainers/ig/test_compute_integrated_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import torch
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ig/test_ig_image.py` & `omnixai-1.3.0/omnixai/tests/explainers/ig/test_ig_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ig/test_ig_tabular.py` & `omnixai-1.3.0/omnixai/tests/explainers/ig/test_ig_tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import pprint
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/knn/test_ce_knn.py` & `omnixai-1.3.0/omnixai/tests/explainers/knn/test_ce_knn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pandas as pd
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/lime/test_lime_image_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_image_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/lime/test_lime_tabular_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_tabular_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pprint
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/lime/test_lime_tabular_regression.py` & `omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_tabular_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import pprint
 from omnixai.utils.misc import set_random_seed
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/lime/test_lime_text_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/lime/test_lime_text_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pprint
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/linear/test_linear_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/linear/test_linear_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pprint
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/linear/test_linear_regression.py` & `omnixai-1.3.0/omnixai/tests/explainers/linear/test_linear_regression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import pandas as pd
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/mace/test_mace.py` & `omnixai-1.3.0/omnixai/tests/explainers/mace/test_mace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pandas as pd
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/mace/test_mace_timeseries.py` & `omnixai-1.3.0/omnixai/tests/visualization/dashboard_timeseries.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import os
 import unittest
 import numpy as np
 import pandas as pd
-from omnixai.utils.misc import set_random_seed
 from omnixai.data.timeseries import Timeseries
-from omnixai.explainers.timeseries.counterfactual.mace import MACEExplainer
+from omnixai.explainers.timeseries import TimeseriesExplainer
+from omnixai.visualization.dashboard import Dashboard
 
 
 def load_timeseries():
-    data_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "../../datasets")
+    data_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "../datasets")
     df = pd.read_csv(os.path.join(data_dir, "timeseries.csv"))
     df["timestamp"] = pd.to_datetime(df["timestamp"], unit='s')
     df = df.rename(columns={"horizontal": "values"})
     df = df.set_index("timestamp")
     df = df.drop(columns=["anomaly"])
     return df
 
@@ -23,29 +29,35 @@
     def _detector(ts: Timeseries):
         anomaly_scores = np.sum((ts.values > threshold).astype(int))
         return anomaly_scores / ts.shape[0]
 
     return _detector
 
 
-class TestMACETimeseries(unittest.TestCase):
+class TestDashboard(unittest.TestCase):
 
     def setUp(self) -> None:
         df = load_timeseries()
         self.train_df = df.iloc[:9150]
         self.test_df = df.iloc[9150:9300]
         self.detector = train_detector(self.train_df)
         print(self.detector(Timeseries.from_pd(self.test_df)))
 
     def test(self):
-        set_random_seed()
-        explainer = MACEExplainer(
-            training_data=Timeseries.from_pd(self.train_df),
-            predict_function=self.detector,
-            threshold=0.001
+        explainers = TimeseriesExplainer(
+            explainers=["shap", "mace"],
+            mode="anomaly_detection",
+            data=Timeseries.from_pd(self.train_df),
+            model=self.detector,
+            preprocess=None,
+            postprocess=None,
+            params={"mace": {"threshold": 0.001}}
         )
-        explanations = explainer.explain(Timeseries.from_pd(self.test_df))
-        fig = explanations.plotly_plot()
+        test_instance = Timeseries.from_pd(self.test_df)
+        local_explanations = explainers.explain(test_instance)
+        print(local_explanations)
+        dashboard = Dashboard(instances=test_instance, local_explanations=local_explanations)
+        dashboard.show()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/mace/test_ranking.py` & `omnixai-1.3.0/omnixai/tests/explainers/mace/test_ranking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pandas as pd
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/mace/test_retrieval.py` & `omnixai-1.3.0/omnixai/tests/explainers/mace/test_retrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pandas as pd
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/mace/test_rl_optimizer.py` & `omnixai-1.3.0/omnixai/tests/explainers/mace/test_rl_optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/pdp/pdp_image.py` & `omnixai-1.3.0/omnixai/tests/explainers/pdp/pdp_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/pdp/test_tabular_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/pdp/test_tabular_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pprint
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/pdp/test_tabular_regression.py` & `omnixai-1.3.0/omnixai/tests/explainers/pdp/test_tabular_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import pprint
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/permutation/test_permutation_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/permutation/test_permutation_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 from omnixai.utils.misc import set_random_seed
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/permutation/test_permutation_regression.py` & `omnixai-1.3.0/omnixai/tests/explainers/prediction/test_regression_metric.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
-from omnixai.utils.misc import set_random_seed
-from omnixai.explainers.tabular import PermutationImportance
+from omnixai.explainers.prediction import PredictionAnalyzer
 from omnixai.tests.explainers.tasks import TabularRegression
+from omnixai.explanations.base import ExplanationBase
 
 
-class TestPDPTabular(unittest.TestCase):
-    def test(self):
-        set_random_seed()
+class TestRegressionMetrics(unittest.TestCase):
+
+    def test_regression_metric(self):
         task = TabularRegression().train_boston()
         predict_function = lambda z: task.model.predict(task.transform.transform(z))
-        explainer = PermutationImportance(
-            training_data=task.train_data, predict_function=predict_function, mode="regression"
+
+        explainer = PredictionAnalyzer(
+            predict_function=predict_function,
+            test_data=task.test_data,
+            test_targets=task.test_targets,
+            mode="regression"
         )
-        explanations = explainer.explain(X=task.test_data, y=task.test_targets)
+        explanations = explainer._metric()
+        print(explanations.get_explanations())
         explanations.plotly_plot()
+        explanations.plot()
+
+        s = explanations.to_json()
+        e = ExplanationBase.from_json(s)
+        self.assertEqual(s, e.to_json())
+        e.plotly_plot()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/polyjuice/polyjuice_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/polyjuice/polyjuice_classification.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import unittest
 import transformers
 import numpy as np
 
 from omnixai.data.text import Text
 from omnixai.explainers.nlp.counterfactual.polyjuice import Polyjuice
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/prediction/test_classification_metrics.py` & `omnixai-1.3.0/omnixai/tests/explainers/prediction/test_confusion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,51 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import unittest
 import numpy as np
 from sklearn import svm, datasets
 from sklearn.model_selection import train_test_split
 
 from omnixai.explainers.prediction import PredictionAnalyzer
 from omnixai.explanations.base import ExplanationBase
 
 
-class TestClassificationMetrics(unittest.TestCase):
+class TestConfusionMatrix(unittest.TestCase):
 
-    def test_classification_metric(self):
+    def setUp(self) -> None:
         iris = datasets.load_iris()
         x = iris.data
         y = iris.target
 
         random_state = np.random.RandomState(0)
         n_samples, n_features = x.shape
         x = np.c_[x, random_state.randn(n_samples, 20 * n_features)]
 
         x_train, x_test, y_train, y_test = \
             train_test_split(x, y, test_size=0.5, random_state=0)
         classifier = svm.SVC(kernel="linear", probability=True, random_state=0)
         classifier.fit(x_train, y_train)
 
+        self.x_test = x_test
+        self.y_test = y_test
+        self.classifier = classifier
+
+    def test_confusion(self):
         explainer = PredictionAnalyzer(
             mode="classification",
-            predict_function=lambda z: classifier.predict_proba(z),
-            test_data=x_test,
-            test_targets=y_test
+            predict_function=lambda x: self.classifier.predict_proba(x),
+            test_data=self.x_test,
+            test_targets=self.y_test
         )
-        explanations = explainer._metric()
-        print(explanations.get_explanations())
-        explanations.plotly_plot()
+        explanations = explainer._confusion_matrix()
+        explanations.plotly_plot(class_names=["a", "b", "c"])
         explanations.plot(class_names=["a", "b", "c"])
 
         s = explanations.to_json()
         e = ExplanationBase.from_json(s)
         self.assertEqual(s, e.to_json())
         e.plotly_plot()
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/prediction/test_regression_metric.py` & `omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_regression.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,40 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import unittest
-from omnixai.explainers.prediction import PredictionAnalyzer
+import pprint
+from omnixai.utils.misc import set_random_seed
+from omnixai.explainers.tabular import ShapTabular
 from omnixai.tests.explainers.tasks import TabularRegression
-from omnixai.explanations.base import ExplanationBase
 
 
-class TestRegressionMetrics(unittest.TestCase):
-
-    def test_regression_metric(self):
+class TestShapTabular(unittest.TestCase):
+    def test_explain(self):
         task = TabularRegression().train_boston()
         predict_function = lambda z: task.model.predict(task.transform.transform(z))
 
-        explainer = PredictionAnalyzer(
+        set_random_seed()
+        explainer = ShapTabular(
+            training_data=task.train_data,
             predict_function=predict_function,
-            test_data=task.test_data,
-            test_targets=task.test_targets,
-            mode="regression"
+            mode="regression",
+            ignored_features=None,
+            nsamples=100
         )
-        explanations = explainer._metric()
-        print(explanations.get_explanations())
-        explanations.plotly_plot()
-        explanations.plot()
-
-        s = explanations.to_json()
-        e = ExplanationBase.from_json(s)
-        self.assertEqual(s, e.to_json())
-        e.plotly_plot()
+
+        i = 25
+        test_x = task.test_data.iloc(i)
+        explanations = explainer.explain(test_x, nsamples=100)
+        for e in explanations.get_explanations():
+            print(e["instance"])
+            pprint.pprint(list(zip(e["features"], e["values"], e["scores"])))
+            self.assertEqual(e["features"][0], "RM")
+            self.assertEqual(e["features"][1], "LSTAT")
+            self.assertEqual(e["features"][2], "B")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ranking/test_perm_ranking.py` & `omnixai-1.3.0/omnixai/tests/explainers/ranking/test_perm_ranking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pandas as pd
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/ranking/test_validity_ranking.py` & `omnixai-1.3.0/omnixai/tests/explainers/ranking/test_validity_ranking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 from omnixai.explainers.ranking.agnostic.validity import ValidityRankingExplainer
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/scorecam/scorecam_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/scorecam/scorecam_torch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/scorecam/test_scorecam_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/scorecam/test_scorecam_tf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/sensitivity/test_sa_tabular.py` & `omnixai-1.3.0/omnixai/tests/explainers/sensitivity/test_sa_tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import pprint
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/shap/shap_image_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/shap/shap_image_tf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import tensorflow as tf
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/shap/shap_image_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/shap/shap_image_torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import torch
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/shap/shap_merlion.py` & `omnixai-1.3.0/omnixai/tests/explainers/shap/shap_merlion.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import unittest
 import pandas as pd
 from datetime import datetime
 from typing import List
 from merlion.utils.time_series import TimeSeries as merlion_timeSeries
 from omnixai.data.timeseries import Timeseries as omnixai_timeSeries
 from merlion.models.defaults import DefaultForecasterConfig, DefaultForecaster
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/shap/shap_text.py` & `omnixai-1.3.0/omnixai/tests/explainers/shap/shap_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import transformers
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/shap/test_shap_tabular_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pprint
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/shap/test_shap_tabular_global.py` & `omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_tabular_global.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pprint
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/shap/test_shap_tabular_regression.py` & `omnixai-1.3.0/omnixai/tests/preprocessing/test_encode.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
-import pprint
-from omnixai.utils.misc import set_random_seed
-from omnixai.explainers.tabular import ShapTabular
-from omnixai.tests.explainers.tasks import TabularRegression
-
-
-class TestShapTabular(unittest.TestCase):
-    def test_explain(self):
-        task = TabularRegression().train_boston()
-        predict_function = lambda z: task.model.predict(task.transform.transform(z))
-
-        set_random_seed()
-        explainer = ShapTabular(
-            training_data=task.train_data,
-            predict_function=predict_function,
-            mode="regression",
-            ignored_features=None,
-            nsamples=100
-        )
-
-        i = 25
-        test_x = task.test_data.iloc(i)
-        explanations = explainer.explain(test_x, nsamples=100)
-        for e in explanations.get_explanations():
-            print(e["instance"])
-            pprint.pprint(list(zip(e["features"], e["values"], e["scores"])))
-            self.assertEqual(e["features"][0], "RM")
-            self.assertEqual(e["features"][1], "LSTAT")
-            self.assertEqual(e["features"][2], "B")
+import numpy as np
+from omnixai.preprocessing.encode import *
+
+
+class TestEncode(unittest.TestCase):
+    def test_KBins(self):
+        n_bins = 5
+        x = np.random.rand(10, 5)
+        s = KBins(n_bins=n_bins).fit(x)
+        y = s.transform(x)
+        z = s.invert(y)
+
+        self.assertEqual(np.sum(np.abs(np.min(y, axis=0))), 0)
+        self.assertEqual(np.mean(np.abs(np.max(y, axis=0))), n_bins - 1)
+
+    def test_OneHot(self):
+        x = [["Male", 1], ["Female", 3], ["Female", 2]]
+        s = OneHot().fit(x)
+        y = s.transform(x)
+        z = s.invert(y)
+
+        self.assertCountEqual(y.shape, (3, 5))
+        self.assertCountEqual(z.shape, (3, 2))
+        for i in range(3):
+            self.assertCountEqual(z[i], x[i])
+
+    def test_Ordinal(self):
+        x = [["Male", 1], ["Female", 3], ["Female", 2]]
+        s = Ordinal().fit(x)
+        y = s.transform(x)
+        z = s.invert(y)
+
+        self.assertCountEqual(y.shape, (3, 2))
+        self.assertCountEqual(z.shape, (3, 2))
+        for i in range(3):
+            self.assertCountEqual(z[i], x[i])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/shap/test_shap_timeseries.py` & `omnixai-1.3.0/omnixai/tests/explainers/shap/test_shap_timeseries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import os
 import unittest
 import numpy as np
 from omnixai.utils.misc import set_random_seed
 from omnixai.data.timeseries import Timeseries
 from omnixai.explainers.timeseries.agnostic.shap import ShapTimeseries
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/shap_tree/shaptree_classification.py` & `omnixai-1.3.0/omnixai/tests/explainers/shap_tree/shaptree_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import pprint
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/shap_tree/shaptree_regression.py` & `omnixai-1.3.0/omnixai/tests/explainers/shap_tree/shaptree_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import pprint
 import xgboost
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/smoothgrad/test_smooth_grad_tf.py` & `omnixai-1.3.0/omnixai/tests/explainers/smoothgrad/test_smooth_grad_tf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/smoothgrad/test_smooth_grad_torch.py` & `omnixai-1.3.0/omnixai/tests/explainers/smoothgrad/test_smooth_grad_torch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/explainers/tasks.py` & `omnixai-1.3.0/omnixai/tests/explainers/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import dill
 import sklearn
```

### Comparing `omnixai-1.2.5/omnixai/tests/preprocessing/test_encode.py` & `omnixai-1.3.0/omnixai/tests/preprocessing/test_normalize.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,34 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
-from omnixai.preprocessing.encode import *
+from omnixai.preprocessing.normalize import *
 
 
-class TestEncode(unittest.TestCase):
-    def test_KBins(self):
-        n_bins = 5
+class TestNormalize(unittest.TestCase):
+    def test_standard(self):
         x = np.random.rand(10, 5)
-        s = KBins(n_bins=n_bins).fit(x)
+        s = Standard().fit(x)
         y = s.transform(x)
         z = s.invert(y)
 
-        self.assertEqual(np.sum(np.abs(np.min(y, axis=0))), 0)
-        self.assertEqual(np.mean(np.abs(np.max(y, axis=0))), n_bins - 1)
-
-    def test_OneHot(self):
-        x = [["Male", 1], ["Female", 3], ["Female", 2]]
-        s = OneHot().fit(x)
-        y = s.transform(x)
-        z = s.invert(y)
+        self.assertLess(np.sum(np.abs(np.sum(y, axis=0))), 1e-6)
+        self.assertLess(np.sum(np.abs(x - z)), 1e-6)
 
-        self.assertCountEqual(y.shape, (3, 5))
-        self.assertCountEqual(z.shape, (3, 2))
-        for i in range(3):
-            self.assertCountEqual(z[i], x[i])
-
-    def test_Ordinal(self):
-        x = [["Male", 1], ["Female", 3], ["Female", 2]]
-        s = Ordinal().fit(x)
+    def test_minmax(self):
+        x = np.random.rand(10, 5)
+        s = MinMax().fit(x)
         y = s.transform(x)
         z = s.invert(y)
 
-        self.assertCountEqual(y.shape, (3, 2))
-        self.assertCountEqual(z.shape, (3, 2))
-        for i in range(3):
-            self.assertCountEqual(z[i], x[i])
+        self.assertEqual(np.sum(np.abs(np.min(y, axis=0))), 0)
+        self.assertEqual(np.mean(np.abs(np.max(y, axis=0))), 1)
+        self.assertLess(np.sum(np.abs(x - z)), 1e-6)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `omnixai-1.2.5/omnixai/tests/preprocessing/test_fill.py` & `omnixai-1.3.0/omnixai/tests/preprocessing/test_fill.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 from omnixai.preprocessing.fill import *
```

### Comparing `omnixai-1.2.5/omnixai/tests/preprocessing/test_image_transform.py` & `omnixai-1.3.0/omnixai/tests/preprocessing/test_image_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import torchvision
```

### Comparing `omnixai-1.2.5/omnixai/tests/preprocessing/test_pipeline.py` & `omnixai-1.3.0/omnixai/tests/preprocessing/test_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/preprocessing/test_tabular_transform.py` & `omnixai-1.3.0/omnixai/tests/preprocessing/test_tabular_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import pandas as pd
```

### Comparing `omnixai-1.2.5/omnixai/tests/preprocessing/test_text_transform.py` & `omnixai-1.3.0/omnixai/tests/preprocessing/test_text_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 from omnixai.data.text import Text
 from omnixai.preprocessing.text import Tfidf, Word2Id
```

### Comparing `omnixai-1.2.5/omnixai/tests/sampler/test_sampler.py` & `omnixai-1.3.0/omnixai/tests/sampler/test_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/utils/json/test_counterfactual.py` & `omnixai-1.3.0/omnixai/tests/utils/json/test_counterfactual.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import unittest
 import pandas as pd
 from omnixai.explanations.tabular.counterfactual import CFExplanation, ExplanationBase
 
 
 class TestCF(unittest.TestCase):
```

### Comparing `omnixai-1.2.5/omnixai/tests/utils/json/test_feature_importance.py` & `omnixai-1.3.0/omnixai/tests/utils/json/test_feature_importance.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import unittest
 import pandas as pd
 from omnixai.explanations.tabular.feature_importance import FeatureImportance, ExplanationBase
 
 
 class TestFeatureImportance(unittest.TestCase):
```

### Comparing `omnixai-1.2.5/omnixai/tests/utils/json/test_prediction.py` & `omnixai-1.3.0/omnixai/tests/utils/json/test_prediction.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import unittest
 import numpy as np
 from omnixai.explanations.base import PredictedResults, ExplanationBase
 
 
 class TestPrediction(unittest.TestCase):
```

### Comparing `omnixai-1.2.5/omnixai/tests/utils/test_explanation_utils.py` & `omnixai-1.3.0/omnixai/tests/utils/test_explanation_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import unittest
 import numpy as np
 import pandas as pd
 from omnixai.explanations.utils import np_to_json, json_to_np, \
     pd_to_json, json_to_pd
```

### Comparing `omnixai-1.2.5/omnixai/tests/utils/test_segmentation.py` & `omnixai-1.3.0/omnixai/tests/utils/test_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/visualization/dashboard_da.py` & `omnixai-1.3.0/omnixai/tests/visualization/dashboard_da.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import numpy as np
```

### Comparing `omnixai-1.2.5/omnixai/tests/visualization/dashboard_image.py` & `omnixai-1.3.0/omnixai/tests/visualization/dashboard_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/visualization/dashboard_image_compare.py` & `omnixai-1.3.0/omnixai/tests/visualization/dashboard_image_compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import json
 import unittest
```

### Comparing `omnixai-1.2.5/omnixai/tests/visualization/dashboard_tabular.py` & `omnixai-1.3.0/omnixai/tests/visualization/dashboard_tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import os
 import unittest
 import sklearn
```

### Comparing `omnixai-1.2.5/omnixai/tests/visualization/dashboard_tabular_regression.py` & `omnixai-1.3.0/omnixai/tests/visualization/dashboard_tabular_regression.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import unittest
 import numpy as np
 import pandas as pd
 import sklearn
 import sklearn.ensemble
 from sklearn.datasets import fetch_california_housing
```

### Comparing `omnixai-1.2.5/omnixai/tests/visualization/dashboard_text.py` & `omnixai-1.3.0/omnixai/tests/visualization/dashboard_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import unittest
 import numpy as np
 import transformers
```

### Comparing `omnixai-1.2.5/omnixai/tests/visualization/dashboard_text_imdb.py` & `omnixai-1.3.0/omnixai/tests/visualization/dashboard_text_imdb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import unittest
 import numpy as np
 import pandas as pd
 import torch
 import torch.nn as nn
 import sklearn
```

### Comparing `omnixai-1.2.5/omnixai/utils/misc.py` & `omnixai-1.3.0/omnixai/utils/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import sys
 import inspect
 import importlib.util
```

### Comparing `omnixai-1.2.5/omnixai/utils/segmentation.py` & `omnixai-1.3.0/omnixai/utils/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import numpy as np
 from PIL import Image as PilImage
 from skimage.segmentation import quickshift, felzenszwalb, slic
```

### Comparing `omnixai-1.2.5/omnixai/visualization/assets/Acumin-BdPro.otf` & `omnixai-1.3.0/omnixai/visualization/assets/Acumin-BdPro.otf`

 * *Files identical despite different names*

### Comparing `omnixai-1.2.5/omnixai/visualization/assets/base.css` & `omnixai-1.3.0/omnixai/visualization/assets/base.css`

 * *Files identical despite different names*

### Comparing `omnixai-1.2.5/omnixai/visualization/assets/logo_small.png` & `omnixai-1.3.0/omnixai/visualization/assets/logo_small.png`

 * *Files identical despite different names*

### Comparing `omnixai-1.2.5/omnixai/visualization/assets/modal.css` & `omnixai-1.3.0/omnixai/visualization/assets/modal.css`

 * *Files identical despite different names*

### Comparing `omnixai-1.2.5/omnixai/visualization/assets/styles.css` & `omnixai-1.3.0/omnixai/visualization/assets/styles.css`

 * *Files identical despite different names*

### Comparing `omnixai-1.2.5/omnixai/visualization/assets/xai.css` & `omnixai-1.3.0/omnixai/visualization/assets/xai.css`

 * *Files identical despite different names*

### Comparing `omnixai-1.2.5/omnixai/visualization/callbacks/data_exp.py` & `omnixai-1.3.0/omnixai/visualization/callbacks/data_exp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import dash
 import copy
 import json
```

### Comparing `omnixai-1.2.5/omnixai/visualization/callbacks/global_exp.py` & `omnixai-1.3.0/omnixai/visualization/callbacks/global_exp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import dash
 import copy
 import json
```

### Comparing `omnixai-1.2.5/omnixai/visualization/callbacks/local_exp.py` & `omnixai-1.3.0/omnixai/visualization/callbacks/local_exp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import dash
 import copy
 import json
```

### Comparing `omnixai-1.2.5/omnixai/visualization/callbacks/prediction_exp.py` & `omnixai-1.3.0/omnixai/visualization/callbacks/prediction_exp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import dash
 import copy
 import json
```

### Comparing `omnixai-1.2.5/omnixai/visualization/callbacks/whatif_exp.py` & `omnixai-1.3.0/omnixai/visualization/callbacks/whatif_exp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import dash
 import copy
 import json
 import omnixai.visualization.state as board
 from dash import Input, Output, State, callback
 from ..pages.whatif_exp import create_result_column
```

### Comparing `omnixai-1.2.5/omnixai/visualization/dashboard.py` & `omnixai-1.3.0/omnixai/visualization/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 """
 The OmniXAI dashboard.
 """
```

### Comparing `omnixai-1.2.5/omnixai/visualization/layout.py` & `omnixai-1.3.0/omnixai/visualization/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from dash import dcc
 from dash import html
```

### Comparing `omnixai-1.2.5/omnixai/visualization/pages/data_exp.py` & `omnixai-1.3.0/omnixai/visualization/pages/data_exp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from dash import dcc
 from dash import html
 from .utils import create_explanation_layout
```

### Comparing `omnixai-1.2.5/omnixai/visualization/pages/global_exp.py` & `omnixai-1.3.0/omnixai/visualization/pages/global_exp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from dash import dcc
 from dash import html
 from .utils import create_explanation_layout
```

### Comparing `omnixai-1.2.5/omnixai/visualization/pages/local_exp.py` & `omnixai-1.3.0/omnixai/visualization/pages/local_exp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from dash import dcc
 from dash import html
 from .utils import create_explanation_layout
```

### Comparing `omnixai-1.2.5/omnixai/visualization/pages/prediction_exp.py` & `omnixai-1.3.0/omnixai/visualization/pages/prediction_exp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from dash import dcc
 from dash import html
 from .utils import create_explanation_layout
```

### Comparing `omnixai-1.2.5/omnixai/visualization/pages/utils.py` & `omnixai-1.3.0/omnixai/visualization/pages/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from dash import html
 from collections import OrderedDict
 from omnixai.explanations.base import DashFigure
```

### Comparing `omnixai-1.2.5/omnixai/visualization/pages/whatif_exp.py` & `omnixai-1.3.0/omnixai/visualization/pages/whatif_exp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from dash import dcc
 from dash import html
 from ..plot import plot_one_instance
```

### Comparing `omnixai-1.2.5/omnixai/visualization/plot.py` & `omnixai-1.3.0/omnixai/visualization/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 import base64
 from io import BytesIO
 from dash import dash_table, html, dcc
```

### Comparing `omnixai-1.2.5/omnixai/visualization/state.py` & `omnixai-1.3.0/omnixai/visualization/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+#
+# Copyright (c) 2023 salesforce.com, inc.
+# All rights reserved.
+# SPDX-License-Identifier: BSD-3-Clause
+# For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
+#
 import numpy as np
 from collections import OrderedDict
 from ..data.tabular import Tabular
 
 
 class State:
     views = ["local", "global", "prediction", "data"]
```

### Comparing `omnixai-1.2.5/omnixai.egg-info/PKG-INFO` & `omnixai-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: omnixai
-Version: 1.2.5
-Summary: OmniXAI: An Explainable AI Toolbox
-Home-page: https://github.com/salesforce/omnixai
-Author: Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi
-License: 3-Clause BSD
-Keywords: XAI Explainable AI Explanation
-Requires-Python: >=3.7,<4
-Description-Content-Type: text/markdown
-Provides-Extra: plot
-Provides-Extra: vision
-Provides-Extra: nlp
-Provides-Extra: bentoml
-Provides-Extra: all
-License-File: LICENSE
-
 <p align="center">
     <br>
     <img src="https://github.com/salesforce/OmniXAI/raw/main/docs/_static/logo_small.png" width="400"/>
     <br>
 <p>
 
 # OmniXAI: A Library for Explainable AI
@@ -47,14 +30,20 @@
 4. [Documentation](https://opensource.salesforce.com/OmniXAI/latest/index.html)
 5. [Tutorials](https://opensource.salesforce.com/OmniXAI/latest/tutorials.html)
 6. [Deployment](#deployment)
 7. [Dashboard Demo](https://sfr-omnixai-demo.herokuapp.com/)
 8. [How to Contribute](https://opensource.salesforce.com/OmniXAI/latest/omnixai.html#how-to-contribute)
 9. [Technical Report and Citing OmniXAI](#technical-report-and-citing-omnixai)
 
+## What's New
+
+The latest version includes an experimental GPT explainer. This explainer leverages the outcomes 
+produced by SHAP and MACE to formulate the input prompt for ChatGPT. Subsequently, ChatGPT 
+analyzes these results and generates the corresponding explanations that provide developers with 
+a clearer understanding of the rationale behind the model's predictions.
 
 ## Introduction
 
 OmniXAI (short for Omni eXplainable AI) is a Python machine-learning library for explainable AI (XAI), offering omni-way explainable AI and interpretable 
 machine learning capabilities to address many pain points in explaining decisions made by machine learning 
 models in practice. OmniXAI aims to be a one-stop comprehensive library that makes explainable AI easy for 
 data scientists, ML researchers and practitioners who need explanation for various types of data, models and 
@@ -80,17 +69,18 @@
 |       Bias metrics        |   Black box   |      Global      |     |    ✅    |       |      |      |
 | Partial dependence plots  |   Black box   |      Global      |     |    ✅    |       |      |      |
 | Accumulated local effects |   Black box   |      Global      |     |    ✅    |       |      |      |
 |   Sensitivity analysis    |   Black box   |      Global      |     |    ✅    |       |      |      |
 |  Permutation explanation  |   Black box   |      Global      |     |    ✅    |       |      |      |
 |   Feature visualization   |  Torch or TF  |      Global      |     |         |   ✅   |      |      |
 |       Feature maps        |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
+|       GPT explainer       | Black box     |     Local        |     |    ✅    |       |      |      |
 |           LIME            |   Black box   |      Local       |     |    ✅    |   ✅   | ✅   |      |
 |           SHAP            |  Black box*   |      Local       |     |    ✅    |   ✅   | ✅   |  ✅  |
-|         What-if           |  Black box    |      Local       |     |    ✅    |       |      |     |
+|          What-if          |   Black box   |      Local       |     |    ✅    |       |      |     |
 |    Integrated gradient    |  Torch or TF  |      Local       |     |    ✅    |   ✅   | ✅   |      |
 |      Counterfactual       |  Black box*   |      Local       |     |    ✅    |   ✅   | ✅   |  ✅  |
 |  Contrastive explanation  |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |   Grad-CAM, Grad-CAM++    |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |         Score-CAM         |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |         Layer-CAM         |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
 |      Smooth gradient      |  Torch or TF  |      Local       |     |         |   ✅   |      |      |
@@ -103,14 +93,18 @@
 for text data. *Counterfactual* accepts black box models for tabular, text and time-series data, and PyTorch/Tensorflow models for
 image data.
 
 This [table](https://opensource.salesforce.com/OmniXAI/latest/index.html#comparison-with-competitors) 
 shows the comparison between our toolkit/library and other existing XAI toolkits/libraries
 in literature.
 
+**OmniXAI also integrates ChatGPT for generating plain text explanations given a classification/regression
+model on tabular datasets.** The generated results may not be 100% accurate, but it is worth trying this 
+explainer (we will continue improving the input prompts).
+
 ## Installation
 
 You can install ``omnixai`` from PyPI by calling ``pip install omnixai``. You may install from source by
 cloning the OmniXAI repo, navigating to the root directory, and calling
 ``pip install .``, or ``pip install -e .`` to install in editable mode. You may install additional dependencies:
 
 - **For plotting & visualization**: Calling ``pip install omnixai[plot]``, or ``pip install .[plot]`` from the
@@ -297,14 +291,30 @@
 )
 dashboard.show()                                    # Launch the dashboard
 ```
 
 After opening the Dash app in the browser, we will see a dashboard showing the explanations:
 ![alt text](https://github.com/salesforce/OmniXAI/raw/main/docs/_static/demo.gif)
 
+You can also use the GPT explainer to generate explanations in text for tabular models:
+
+```python
+explainer = TabularExplainer(
+  explainers=["gpt"],                                # The GPT explainer to apply
+  mode="classification",                             # The task type
+  data=train_data,                                   # The data for initializing the explainers
+  model=model,                                       # The ML model to explain
+  preprocess=lambda z: transformer.transform(z),     # Converts raw features into the model inputs
+  params={
+     "gpt": {"apikey": "xxxx"}
+  }                                                  # Set the OpenAI API KEY
+)
+local_explanations = explainer.explain(X=test_instances)
+```
+
 For vision tasks, the same interface is used to create explainers and generate explanations. 
 Let's take an image classification model as an example.
 
 ```python
 from omnixai.explainers.vision import VisionExplainer
 from omnixai.visualization.dashboard import Dashboard
```

#### html2text {}

```diff
@@ -1,29 +1,27 @@
-Metadata-Version: 2.1 Name: omnixai Version: 1.2.5 Summary: OmniXAI: An
-Explainable AI Toolbox Home-page: https://github.com/salesforce/omnixai Author:
-Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi
-License: 3-Clause BSD Keywords: XAI Explainable AI Explanation Requires-Python:
->=3.7,<4 Description-Content-Type: text/markdown Provides-Extra: plot Provides-
-Extra: vision Provides-Extra: nlp Provides-Extra: bentoml Provides-Extra: all
-License-File: LICENSE
 
  [https://github.com/salesforce/OmniXAI/raw/main/docs/_static/logo_small.png]
 # OmniXAI: A Library for Explainable AI
     [https://img.shields.io/badge/Python-3.7,_3.8,_3.9,_3.10-blue] [PyPI]
                        [Documentation] [Downloads] [DOI]
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
 (https://opensource.salesforce.com/OmniXAI/latest/index.html) 5. [Tutorials]
 (https://opensource.salesforce.com/OmniXAI/latest/tutorials.html) 6.
 [Deployment](#deployment) 7. [Dashboard Demo](https://sfr-omnixai-
 demo.herokuapp.com/) 8. [How to Contribute](https://opensource.salesforce.com/
 OmniXAI/latest/omnixai.html#how-to-contribute) 9. [Technical Report and Citing
-OmniXAI](#technical-report-and-citing-omnixai) ## Introduction OmniXAI (short
-for Omni eXplainable AI) is a Python machine-learning library for explainable
-AI (XAI), offering omni-way explainable AI and interpretable machine learning
+OmniXAI](#technical-report-and-citing-omnixai) ## What's New The latest version
+includes an experimental GPT explainer. This explainer leverages the outcomes
+produced by SHAP and MACE to formulate the input prompt for ChatGPT.
+Subsequently, ChatGPT analyzes these results and generates the corresponding
+explanations that provide developers with a clearer understanding of the
+rationale behind the model's predictions. ## Introduction OmniXAI (short for
+Omni eXplainable AI) is a Python machine-learning library for explainable AI
+(XAI), offering omni-way explainable AI and interpretable machine learning
 capabilities to address many pain points in explaining decisions made by
 machine learning models in practice. OmniXAI aims to be a one-stop
 comprehensive library that makes explainable AI easy for data scientists, ML
 researchers and practitioners who need explanation for various types of data,
 models and explanation methods at different stages of ML process: ![alt text]
 (https://github.com/salesforce/OmniXAI/raw/main/docs/_static/ml_pipeline.png)
 OmniXAI includes a rich family of explanation methods integrated in a unified
@@ -44,45 +42,49 @@
 â | | | | | | Feature selection | NA | Global | â | | | | | | Prediction
 metrics | Black box | Global | | â | â | â | â | | Bias metrics | Black
 box | Global | | â | | | | | Partial dependence plots | Black box | Global |
 | â | | | | | Accumulated local effects | Black box | Global | | â | | | |
 | Sensitivity analysis | Black box | Global | | â | | | | | Permutation
 explanation | Black box | Global | | â | | | | | Feature visualization |
 Torch or TF | Global | | | â | | | | Feature maps | Torch or TF | Local | | |
-â | | | | LIME | Black box | Local | | â | â | â | | | SHAP | Black
-box* | Local | | â | â | â | â | | What-if | Black box | Local | | â
-| | | | | Integrated gradient | Torch or TF | Local | | â | â | â | | |
-Counterfactual | Black box* | Local | | â | â | â | â | | Contrastive
-explanation | Torch or TF | Local | | | â | | | | Grad-CAM, Grad-CAM++ |
-Torch or TF | Local | | | â | | | | Score-CAM | Torch or TF | Local | | | â
-| | | | Layer-CAM | Torch or TF | Local | | | â | | | | Smooth gradient |
-Torch or TF | Local | | | â | | | | Guided backpropagation | Torch or TF |
-Local | | | â | | | | Learning to explain | Black box | Local | | â | â |
-â | | | Linear models | Linear models | Global and Local | | â | | | | |
-Tree models | Tree models | Global and Local | | â | | | | *SHAP* accepts
-black box models for tabular data, PyTorch/Tensorflow models for image data,
-transformer models for text data. *Counterfactual* accepts black box models for
-tabular, text and time-series data, and PyTorch/Tensorflow models for image
-data. This [table](https://opensource.salesforce.com/OmniXAI/latest/
-index.html#comparison-with-competitors) shows the comparison between our
-toolkit/library and other existing XAI toolkits/libraries in literature. ##
-Installation You can install ``omnixai`` from PyPI by calling ``pip install
-omnixai``. You may install from source by cloning the OmniXAI repo, navigating
-to the root directory, and calling ``pip install .``, or ``pip install -e .``
-to install in editable mode. You may install additional dependencies: - **For
-plotting & visualization**: Calling ``pip install omnixai[plot]``, or ``pip
-install .[plot]`` from the root directory of the repo. - **For vision tasks**:
-Calling ``pip install omnixai[vision]``, or ``pip install .[vision]`` from the
-root directory of the repo. - **For NLP tasks**: Calling ``pip install omnixai
-[nlp]``, or ``pip install .[nlp]`` from the root directory of the repo. -
-**Install all the dependencies**: Calling ``pip install omnixai[all]``, or
-``pip install .[all]`` from the root directory of the repo. ## Getting Started
-For example code and an introduction to the library, see the Jupyter notebooks
-in [tutorials](https://opensource.salesforce.com/OmniXAI/latest/
-tutorials.html), and the guided walkthrough [here](https://
+â | | | | GPT explainer | Black box | Local | | â | | | | | LIME | Black
+box | Local | | â | â | â | | | SHAP | Black box* | Local | | â | â |
+â | â | | What-if | Black box | Local | | â | | | | | Integrated gradient
+| Torch or TF | Local | | â | â | â | | | Counterfactual | Black box* |
+Local | | â | â | â | â | | Contrastive explanation | Torch or TF |
+Local | | | â | | | | Grad-CAM, Grad-CAM++ | Torch or TF | Local | | | â |
+| | | Score-CAM | Torch or TF | Local | | | â | | | | Layer-CAM | Torch or TF
+| Local | | | â | | | | Smooth gradient | Torch or TF | Local | | | â | | |
+| Guided backpropagation | Torch or TF | Local | | | â | | | | Learning to
+explain | Black box | Local | | â | â | â | | | Linear models | Linear
+models | Global and Local | | â | | | | | Tree models | Tree models | Global
+and Local | | â | | | | *SHAP* accepts black box models for tabular data,
+PyTorch/Tensorflow models for image data, transformer models for text data.
+*Counterfactual* accepts black box models for tabular, text and time-series
+data, and PyTorch/Tensorflow models for image data. This [table](https://
+opensource.salesforce.com/OmniXAI/latest/index.html#comparison-with-
+competitors) shows the comparison between our toolkit/library and other
+existing XAI toolkits/libraries in literature. **OmniXAI also integrates
+ChatGPT for generating plain text explanations given a classification/
+regression model on tabular datasets.** The generated results may not be 100%
+accurate, but it is worth trying this explainer (we will continue improving the
+input prompts). ## Installation You can install ``omnixai`` from PyPI by
+calling ``pip install omnixai``. You may install from source by cloning the
+OmniXAI repo, navigating to the root directory, and calling ``pip install .``,
+or ``pip install -e .`` to install in editable mode. You may install additional
+dependencies: - **For plotting & visualization**: Calling ``pip install omnixai
+[plot]``, or ``pip install .[plot]`` from the root directory of the repo. -
+**For vision tasks**: Calling ``pip install omnixai[vision]``, or ``pip install
+.[vision]`` from the root directory of the repo. - **For NLP tasks**: Calling
+``pip install omnixai[nlp]``, or ``pip install .[nlp]`` from the root directory
+of the repo. - **Install all the dependencies**: Calling ``pip install omnixai
+[all]``, or ``pip install .[all]`` from the root directory of the repo. ##
+Getting Started For example code and an introduction to the library, see the
+Jupyter notebooks in [tutorials](https://opensource.salesforce.com/OmniXAI/
+latest/tutorials.html), and the guided walkthrough [here](https://
 opensource.salesforce.com/OmniXAI/latest/index.html). A dashboard demo can be
 found [here](https://sfr-omnixai-demo.herokuapp.com/). Some examples: 1.
 [Tabular classification](https://github.com/salesforce/OmniXAI/blob/main/
 tutorials/tabular_classification.ipynb) 2. [Tabular regression](https://
 github.com/salesforce/OmniXAI/blob/main/tutorials/tabular_regression.ipynb) 3.
 [Image classification](https://github.com/salesforce/OmniXAI/blob/main/
 tutorials/vision.ipynb) 4. [Text classification](https://github.com/salesforce/
@@ -207,19 +209,26 @@
 local_explanations=local_explanations, # Set the local explanations
 global_explanations=global_explanations, # Set the global explanations
 prediction_explanations=prediction_explanations, # Set the prediction metrics
 class_names=class_names, # Set class names explainer=explainer # The created
 TabularExplainer for what if analysis ) dashboard.show() # Launch the dashboard
 ``` After opening the Dash app in the browser, we will see a dashboard showing
 the explanations: ![alt text](https://github.com/salesforce/OmniXAI/raw/main/
-docs/_static/demo.gif) For vision tasks, the same interface is used to create
-explainers and generate explanations. Let's take an image classification model
-as an example. ```python from omnixai.explainers.vision import VisionExplainer
-from omnixai.visualization.dashboard import Dashboard explainer =
-VisionExplainer( explainers=["gradcam", "lime", "ig", "ce",
+docs/_static/demo.gif) You can also use the GPT explainer to generate
+explanations in text for tabular models: ```python explainer = TabularExplainer
+( explainers=["gpt"], # The GPT explainer to apply mode="classification", # The
+task type data=train_data, # The data for initializing the explainers
+model=model, # The ML model to explain preprocess=lambda z:
+transformer.transform(z), # Converts raw features into the model inputs params=
+{ "gpt": {"apikey": "xxxx"} } # Set the OpenAI API KEY ) local_explanations =
+explainer.explain(X=test_instances) ``` For vision tasks, the same interface is
+used to create explainers and generate explanations. Let's take an image
+classification model as an example. ```python from omnixai.explainers.vision
+import VisionExplainer from omnixai.visualization.dashboard import Dashboard
+explainer = VisionExplainer( explainers=["gradcam", "lime", "ig", "ce",
 "feature_visualization"], mode="classification", model=model, # An image
 classification model, e.g., ResNet50 preprocess=preprocess, # The preprocessing
 function postprocess=postprocess, # The postprocessing function params={ # Set
 the target layer for GradCAM "gradcam": {"target_layer": model.layer4[-1]}, #
 Set the objective for feature visualization "feature_visualization":
 {"objectives": [{"layer": model.layer4[-3], "type": "channel", "index": list
 (range(6))}]} }, ) # Generate explanations of GradCAM, LIME, IG and CE
```

### Comparing `omnixai-1.2.5/omnixai.egg-info/SOURCES.txt` & `omnixai-1.3.0/omnixai.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 omnixai/explainers/ranking/counterfactual/mace.py
 omnixai/explainers/tabular/__init__.py
 omnixai/explainers/tabular/auto.py
 omnixai/explainers/tabular/base.py
 omnixai/explainers/tabular/agnostic/__init__.py
 omnixai/explainers/tabular/agnostic/ale.py
 omnixai/explainers/tabular/agnostic/bias.py
+omnixai/explainers/tabular/agnostic/gpt.py
 omnixai/explainers/tabular/agnostic/lime.py
 omnixai/explainers/tabular/agnostic/pdp.py
 omnixai/explainers/tabular/agnostic/permutation.py
 omnixai/explainers/tabular/agnostic/sensitivity.py
 omnixai/explainers/tabular/agnostic/shap.py
 omnixai/explainers/tabular/agnostic/shap_global.py
 omnixai/explainers/tabular/agnostic/L2X/__init__.py
@@ -221,14 +222,15 @@
 omnixai/tests/explainers/feature_visualization/test_feature_optimizer_tf.py
 omnixai/tests/explainers/feature_visualization/test_feature_optimizer_torch.py
 omnixai/tests/explainers/feature_visualization/test_fft.py
 omnixai/tests/explainers/feature_visualization/test_fv_preprocess_tf.py
 omnixai/tests/explainers/feature_visualization/test_fv_preprocess_torch.py
 omnixai/tests/explainers/feature_visualization/test_map_extractor_tf.py
 omnixai/tests/explainers/feature_visualization/test_map_extractor_torch.py
+omnixai/tests/explainers/gpt/gpt_explainer_classification.py
 omnixai/tests/explainers/gradcam/test_gradcam_tf.py
 omnixai/tests/explainers/gradcam/test_gradcam_torch.py
 omnixai/tests/explainers/gradcam/test_layercam_tf.py
 omnixai/tests/explainers/gradcam/test_layercam_torch.py
 omnixai/tests/explainers/gradcam/vlm_gradcam_torch.py
 omnixai/tests/explainers/guided_bp/test_guided_bp_tf.py
 omnixai/tests/explainers/guided_bp/test_guided_bp_torch.py
```

### Comparing `omnixai-1.2.5/omnixai.egg-info/requires.txt` & `omnixai-1.3.0/omnixai.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-numpy>=1.17
+numpy<1.24,>=1.17
 pandas>=1.1.0
 scikit-learn<1.2,>=0.24
 scipy>=1.5.0
 scikit-image>=0.17.2
 matplotlib
 pillow<10.0
 lime
 shap>=0.40.0
 SALib
 hnswlib>=0.5.0
 dill
 tqdm
 wheel
 packaging
-ipython!=8.7.0
+ipython>=8.10.0
 tabulate
 statsmodels>=0.10.1
+openai
 
 [all]
 plotly>=4
 dash>=2.0
 dash_bootstrap_components>=1.0
 jupyter-dash>=0.4
 torch>=1.7
```

### Comparing `omnixai-1.2.5/setup.py` & `omnixai-1.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022 salesforce.com, inc.
+# Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause
 #
 from setuptools import setup, find_namespace_packages
 
 extras_require = {
@@ -17,42 +17,43 @@
     "nlp": ["nltk>=3.4.5", "polyjuice_nlp"],
     "bentoml": ["bentoml>=1.0.0"],
 }
 extras_require["all"] = sum(extras_require.values(), [])
 
 setup(
     name="omnixai",
-    version="1.2.5",
+    version="1.3.0",
     author="Wenzhuo Yang, Hung Le, Tanmay Shivprasad Laud, Silvio Savarese, Steven C.H. Hoi",
     description="OmniXAI: An Explainable AI Toolbox",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="XAI Explainable AI Explanation",
     url="https://github.com/salesforce/omnixai",
     license="3-Clause BSD",
     packages=find_namespace_packages(include="omnixai.*"),
     package_dir={"omnixai": "omnixai"},
     package_data={"omnixai": ["visualization/assets/*"]},
     install_requires=[
-        "numpy>=1.17",
+        "numpy>=1.17,<1.24",
         "pandas>=1.1.0",
         "scikit-learn>=0.24,<1.2",
         "scipy>=1.5.0",
         "scikit-image>=0.17.2",
         "matplotlib",
         "pillow<10.0",
         "lime",
         "shap>=0.40.0",
         "SALib",
         "hnswlib>=0.5.0",
         "dill",
         "tqdm",
         "wheel",
         "packaging",
-        "ipython!=8.7.0",
+        "ipython>=8.10.0",
         "tabulate",
         "statsmodels>=0.10.1",
+        "openai"
     ],
     extras_require=extras_require,
     python_requires=">=3.7,<4",
     zip_safe=False,
 )
```

