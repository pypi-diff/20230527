# Comparing `tmp/autogluon.tabular-0.7.1b20230526.tar.gz` & `tmp/autogluon.tabular-0.7.1b20230527.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-0.7.1b20230526.tar", last modified: Fri May 26 09:04:09 2023, max compression
+gzip compressed data, was "autogluon.tabular-0.7.1b20230527.tar", last modified: Sat May 27 09:04:03 2023, max compression
```

## Comparing `autogluon.tabular-0.7.1b20230526.tar` & `autogluon.tabular-0.7.1b20230527.tar`

### file list

```diff
@@ -1,175 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.215872 autogluon.tabular-0.7.1b20230526/
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-26 09:04:09.215872 autogluon.tabular-0.7.1b20230526/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:04:09.215872 autogluon.tabular-0.7.1b20230526/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.195872 autogluon.tabular-0.7.1b20230526/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.195872 autogluon.tabular-0.7.1b20230526/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.199872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.199872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.199872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47558 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.199872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.199872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.199872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.199872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25059 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.203872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.207872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.207872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.207872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.207872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.207872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.207872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.207872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.207872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/mxnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/mxnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/mxnet/embednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/mxnet/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    37284 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_mxnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.211872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.211872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.211872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.211872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.211872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.211872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.211872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.211872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   248806 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.211872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.211872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.215872 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-26 09:03:32.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 09:04:09.000000 autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:09.199872 autogluon.tabular-0.7.1b20230526/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-26 09:04:09.000000 autogluon.tabular-0.7.1b20230526/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-26 09:04:09.000000 autogluon.tabular-0.7.1b20230526/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:04:09.000000 autogluon.tabular-0.7.1b20230526/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 09:04:09.000000 autogluon.tabular-0.7.1b20230526/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-26 09:04:09.000000 autogluon.tabular-0.7.1b20230526/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 09:04:09.000000 autogluon.tabular-0.7.1b20230526/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:04:09.000000 autogluon.tabular-0.7.1b20230526/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.459000 autogluon.tabular-0.7.1b20230527/
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-27 09:04:03.459000 autogluon.tabular-0.7.1b20230527/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:04:03.459000 autogluon.tabular-0.7.1b20230527/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.443000 autogluon.tabular-0.7.1b20230527/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.443000 autogluon.tabular-0.7.1b20230527/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.447000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.447000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.447000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47558 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.447000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.447000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.447000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.447000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.447000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.447000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25059 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.451001 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   248865 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.455000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.459000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.459000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-27 09:03:34.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-27 09:04:03.000000 autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:04:03.447000 autogluon.tabular-0.7.1b20230527/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-27 09:04:03.000000 autogluon.tabular-0.7.1b20230527/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-27 09:04:03.000000 autogluon.tabular-0.7.1b20230527/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:04:03.000000 autogluon.tabular-0.7.1b20230527/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 09:04:03.000000 autogluon.tabular-0.7.1b20230527/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-27 09:04:03.000000 autogluon.tabular-0.7.1b20230527/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 09:04:03.000000 autogluon.tabular-0.7.1b20230527/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:04:03.000000 autogluon.tabular-0.7.1b20230527/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-0.7.1b20230526/PKG-INFO` & `autogluon.tabular-0.7.1b20230527/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.1b20230526
+Version: 0.7.1b20230527
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.7.1b20230526/setup.py` & `autogluon.tabular-0.7.1b20230527/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/learner/default_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from .lgb.lgb_model import LGBModel
 from .catboost.catboost_model import CatBoostModel
 from .xgboost.xgboost_model import XGBoostModel
 from .rf.rf_model import RFModel
 from .xt.xt_model import XTModel
 from .knn.knn_model import KNNModel
 from .lr.lr_model import LinearModel
-from .tabular_nn.mxnet.tabular_nn_mxnet import TabularNeuralNetMxnetModel
 from .tabular_nn.torch.tabular_nn_torch import TabularNeuralNetTorchModel
 from .fastainn.tabular_nn_fastai import NNFastAiTabularModel
 from .fasttext.fasttext_model import FastTextModel
 from .text_prediction.text_prediction_v1_model import TextPredictorModel
 from .image_prediction.image_predictor import ImagePredictorModel
 from .imodels.imodels_models import RuleFitModel, BoostedRulesModel, GreedyTreeModel, HSTreeModel, \
     FigsModel, _IModelsModel
```

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 """ Default (fixed) hyperparameter values used in Tabular Neural Network models.
-    MXNet vs Torch backend frameworks use slightly different hyperparameters.
     A value of None typically indicates an adaptive value for the hyperparameter will be chosen based on the data.
 """
 
 from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE
 
 
 def get_fixed_params(framework):
     """ Parameters that currently cannot be searched during HPO """
     fixed_params = {
         # 'seed_value': 0,  # random seed for reproducibility (set = None to ignore)
     }
-    mxnet_fixed_params = {
-        'num_epochs': 500,  # maximum number of epochs (passes over full dataset) for training NN
-        'epochs_wo_improve': 20,  # we terminate training if validation performance hasn't improved in the last 'epochs_wo_improve' # of epochs
-        # TODO: Epochs could take a very long time, we may want smarter logic than simply # of epochs without improvement (slope, difference in score, etc.)
-        'max_layer_width': 2056,  # maximum number of hidden units in network layer (integer > 0)
-        # Does not need to be searched by default
-    }
     pytorch_fixed_params = {
         'num_epochs': 500,  # maximum number of epochs (passes over full dataset) for training NN
         'epochs_wo_improve': 20,  # we terminate training if validation performance hasn't improved in the last 'epochs_wo_improve' # of epochs
     }
-    return merge_framework_params(framework=framework, shared_params=fixed_params, mxnet_params=mxnet_fixed_params, pytorch_params=pytorch_fixed_params)
+    return merge_framework_params(framework=framework, shared_params=fixed_params, pytorch_params=pytorch_fixed_params)
 
 
 def get_hyper_params(framework):
     """ Parameters that currently can be tuned during HPO """
     hyper_params = {
         ## Hyperparameters for neural net architecture:
         'activation': 'relu',  # Activation function
-        # Options for mxnet: ['relu', 'softrelu', 'tanh', 'softsign'], options for pytorch: ['relu', 'elu', 'tanh']
+        # Options: ['relu', 'softrelu', 'tanh', 'softsign'], options for pytorch: ['relu', 'elu', 'tanh']
         'embedding_size_factor': 1.0,  # scaling factor to adjust size of embedding layers (float > 0)
         # Options: range[0.01 - 100] on log-scale
         'embed_exponent': 0.56,  # exponent used to determine size of embedding layers based on # categories.
         'max_embedding_dim': 100,  # maximum size of embedding layer for a single categorical feature (int > 0).
         ## Regression-specific hyperparameters:
         'y_range': None,  # Tuple specifying whether Y is constrained to (min_y, max_y). Can be = (-np.inf, np.inf).
         # If None, inferred based on training labels. Note: MUST be None for classification tasks!
@@ -54,49 +46,26 @@
         'proc.max_category_levels': 100,  # maximum number of allowed levels per categorical feature
         # Options: [10, 100, 200, 300, 400, 500, 1000, 10000]
         'proc.skew_threshold': 0.99,  # numerical features whose absolute skewness is greater than this receive special power-transform preprocessing. Choose big value to avoid using power-transforms
         # Options: [0.2, 0.3, 0.5, 0.8, 0.9, 0.99, 0.999, 1.0, 10.0, 100.0]
         'use_ngram_features': False,  # If False, will drop automatically generated ngram features from language features. This results in worse model quality but far faster inference and training times.
         # Options: [True, False]
     }
-    mxnet_hyper_params = {
-        'layers': None,  # List of widths (num_units) for each hidden layer (Note: only specifies hidden layers. These numbers are not absolute, they will also be scaled based on number of training examples and problem type)
-        # Options: List of lists that are manually created
-        'network_type': 'widedeep',  # Type of neural net used to produce predictions
-        # Options: ['widedeep', 'feedforward']
-        'numeric_embed_dim': None,  # Size of joint embedding for all numeric+one-hot features.
-        # Options: integer values between 10-10000
-        'batch_size': 512,  # batch-size used for NN training
-        # Options: [32, 64, 128, 256, 512, 1024, 2048]
-        'use_batchnorm': True,  # whether or not to utilize batch normalization
-        # Options: [True, False]
-        'clip_gradient': 100.0,  # gradient clipping threshold (float > 0)
-        # Options: [1, 10, 100, 1000]
-        'momentum': 0.9,  # momentum which is only used for SGD optimizer
-        'loss_function': None,  # MXNet loss function minimized during training
-        'lr_scheduler': None,  # If not None, string specifying what type of learning rate scheduler to use (may override learning_rate).
-        # Options: [None, 'cosine', 'step', 'poly', 'constant']
-        # Below are hyperparameters specific to the LR scheduler (only used if lr_scheduler != None). For more info, see: https://gluon-cv.mxnet.io/api/utils.html#gluoncv.utils.LRScheduler
-        'base_lr': 3e-5,  # smallest LR (float > 0)
-        'target_lr': 1.0,  # largest LR (float > 0)
-        'lr_decay': 0.1,  # step factor used to decay LR (float in (0,1))
-        'warmup_epochs': 10,  # number of epochs at beginning of training in which LR is linearly ramped up (float > 1).
-    }
     pytorch_hyper_params = {
         'num_layers': 4,  # number of layers
         # Options: [2, 3, 4, 5]
         'hidden_size': 128,  # number of hidden units in each layer
         # Options: [128, 256, 512]
         'max_batch_size': 512,  # maximum batch-size, actual batch size may be slightly smaller.
         'use_batchnorm': False,  # whether or not to utilize batch normalization
         # Options: [True, False]
         'loss_function': 'auto',  # Pytorch loss function minimized during training
         # Example options for regression: nn.MSELoss(), nn.L1Loss()
     }
-    return merge_framework_params(framework=framework, shared_params=hyper_params, mxnet_params=mxnet_hyper_params, pytorch_params=pytorch_hyper_params)
+    return merge_framework_params(framework=framework, shared_params=hyper_params, pytorch_params=pytorch_hyper_params)
 
 
 def get_quantile_hyper_params(framework):
     """ Parameters that currently can be searched during HPO """
     hyper_params = get_hyper_params(framework)
     new_hyper_params = {
         'gamma': 5.0,  # margin loss weight which helps ensure noncrossing quantile estimates
@@ -139,15 +108,13 @@
     if framework != 'pytorch':
         raise ValueError("Only pytorch tabular neural network is currently supported for quantile regression.")
     params = get_fixed_params(framework)
     params.update(get_quantile_hyper_params(framework))
     return params
 
 
-def merge_framework_params(framework, shared_params, mxnet_params, pytorch_params):
-    if framework == 'mxnet':
-        shared_params.update(mxnet_params)
-    elif framework == 'pytorch':
+def merge_framework_params(framework, shared_params, pytorch_params):
+    if framework == 'pytorch':
         shared_params.update(pytorch_params)
     else:
-        raise ValueError("framework must be 'pytorch' or 'mxnet'")
+        raise ValueError("framework must be 'pytorch'")
     return shared_params
```

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """ Default (fixed) hyperparameter search spaces used in Tabular Neural Network models.
-    MXNet vs Torch backend frameworks use slightly different hyperparameters.
 """
 from autogluon.common import space
 
 from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE
 
 from .parameters import merge_framework_params
 
@@ -15,28 +14,21 @@
         'dropout_prob': space.Categorical(0.1, 0.0, 0.5, 0.2, 0.3, 0.4),
         'embedding_size_factor': space.Categorical(1.0, 0.5, 1.5, 0.7, 0.6, 0.8, 0.9, 1.1, 1.2, 1.3, 1.4),
         'proc.embed_min_categories': space.Categorical(4, 3, 10, 100, 1000),
         'proc.impute_strategy': space.Categorical('median', 'mean', 'most_frequent'),
         'proc.max_category_levels': space.Categorical(100, 10, 20, 200, 300, 400, 500, 1000, 10000),
         'proc.skew_threshold': space.Categorical(0.99, 0.2, 0.3, 0.5, 0.8, 0.9, 0.999, 1.0, 10.0, 100.0),
     }
-    mxnet_params = {
-        'use_batchnorm': space.Categorical(True, False),
-        'layers': space.Categorical(None, [200, 100], [256], [100, 50], [200, 100, 50], [1024], [32], [300, 150]),
-        'network_type': space.Categorical('widedeep', 'feedforward'),
-        'activation': space.Categorical('relu', 'softrelu'),
-        'batch_size': space.Categorical(512, 1024, 2056, 128),
-    }
     pytorch_params = {
         'use_batchnorm': space.Categorical(False, True),
         'num_layers': space.Categorical(2, 3, 4),
         'hidden_size': space.Categorical(128, 256, 512),
         'activation': space.Categorical('relu', 'elu'),
     }
-    params = merge_framework_params(framework=framework, shared_params=params, mxnet_params=mxnet_params, pytorch_params=pytorch_params)
+    params = merge_framework_params(framework=framework, shared_params=params, pytorch_params=pytorch_params)
     if problem_type == QUANTILE:
         problem_params =  get_searchspace_quantile(framework)
     elif problem_type == BINARY:
         problem_params = get_searchspace_binary(framework)
     elif problem_type == MULTICLASS:
         problem_params = get_searchspace_multiclass(framework, num_classes=num_classes)
     elif problem_type == REGRESSION:
@@ -53,21 +45,18 @@
     return {}
 
 
 def get_searchspace_regression(framework):
     params = {
         'weight_decay': space.Real(1e-12, 1.0, default=1e-6, log=True),
     }
-    mxnet_params = {
-        'activation': space.Categorical('relu', 'softrelu', 'tanh'),
-    }
     pytorch_params = {
         'activation': space.Categorical('relu', 'elu', 'tanh'),
     }
-    return merge_framework_params(framework=framework, shared_params=params, mxnet_params=mxnet_params, pytorch_params=pytorch_params)
+    return merge_framework_params(framework=framework, shared_params=params, pytorch_params=pytorch_params)
 
 
 def get_searchspace_quantile(framework):
     if framework != 'pytorch':
         raise ValueError("Only pytorch tabular neural network is currently supported for quantile regression.")
     params = {
         'activation': space.Categorical('relu', 'elu', 'tanh'),
```

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/mxnet/embednet.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,213 +1,258 @@
+import logging
+import torch
+import torch.nn as nn
 import numpy as np
-import mxnet as mx
-from mxnet import nd, gluon
 
-from ..utils.nn_architecture_utils import get_embed_sizes
+from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE
 
+from ..utils.nn_architecture_utils import get_embed_sizes
 
-class NumericBlock(gluon.HybridBlock):
-    """ Single Dense layer that jointly embeds all numeric and one-hot features """
-    def __init__(self, params, **kwargs):
-        super(NumericBlock, self).__init__(**kwargs)
-        with self.name_scope():
-            self.body = gluon.nn.Dense(params['numeric_embed_dim'], activation=params['activation'])
-            
-    def hybrid_forward(self, F, x):
-        return self.body(x)
-
-
-class EmbedBlock(gluon.HybridBlock):
-    """ Used to embed a single embedding feature. """
-    def __init__(self, embed_dim, num_categories, **kwargs):
-        super(EmbedBlock, self).__init__(**kwargs)
-        with self.name_scope():
-            self.body = gluon.nn.Embedding(input_dim=num_categories, output_dim=embed_dim,
-                                           weight_initializer=mx.init.Orthogonal(scale=0.1, rand_type='uniform')) # for Xavier-style: scale = np.sqrt(3/float(embed_dim))
-    
-    def hybrid_forward(self, F, x):
-        return self.body(x)
-
-
-class FeedforwardBlock(gluon.HybridBlock):
-    """ Standard Feedforward layers """
-    def __init__(self, params, num_net_outputs, **kwargs):
-        super(FeedforwardBlock, self).__init__(**kwargs)
-        layers = params['layers']
-        with self.name_scope():
-            self.body = gluon.nn.HybridSequential()
-            if params['use_batchnorm']:
-                 self.body.add(gluon.nn.BatchNorm())
-            if params['dropout_prob'] > 0:
-                self.body.add(gluon.nn.Dropout(params['dropout_prob']))
-            for i in range(len(layers)):
-                layer_width = layers[i]
-                if layer_width < 1 or int(layer_width) != layer_width:
-                    raise ValueError("layers must be ints >= 1")
-                self.body.add(gluon.nn.Dense(layer_width, activation=params['activation']))
-                if params['use_batchnorm']:
-                    self.body.add(gluon.nn.BatchNorm())
-                if params['dropout_prob'] > 0:
-                    self.body.add(gluon.nn.Dropout(params['dropout_prob']))
-            self.body.add(gluon.nn.Dense(num_net_outputs, activation=None))
-    
-    def hybrid_forward(self, F, x):
-        return self.body(x)
+logger = logging.getLogger(__name__)
 
 
-class WideAndDeepBlock(gluon.HybridBlock):
-    """ Standard feedforward layers with a single skip connection from output directly to input (ie. deep and wide network).
+class EmbedNet(nn.Module):
     """
-    def __init__(self, params, num_net_outputs, **kwargs):
-        super(WideAndDeepBlock, self).__init__(**kwargs)
-        self.deep = FeedforwardBlock(params, num_net_outputs, **kwargs)
-        with self.name_scope(): # Skip connection, ie. wide network branch
-            self.wide = gluon.nn.Dense(num_net_outputs, activation=None)
-    
-    def hybrid_forward(self, F, x):
-        return self.deep(x) + self.wide(x)
-
-
-class EmbedNet(gluon.Block): # TODO: hybridize?
-    """ Gluon net with input layers to handle numerical data & categorical embeddings
-        which are concatenated together after input layer and then passed into feedforward network.
-        If architecture_desc != None, then we assume EmbedNet has already been previously created,
-        and we create a new EmbedNet based on the provided architecture description 
-        (thus ignoring train_dataset, params, num_net_outputs). 
+    y_range: Used specifically for regression. = None for classification.
     """
-    def __init__(self, train_dataset=None, params=None, num_net_outputs=None, architecture_desc=None, ctx=None, **kwargs):
-        if (architecture_desc is None) and (train_dataset is None or params is None or num_net_outputs is None):
-            raise ValueError("train_dataset, params, num_net_outputs cannot = None if architecture_desc=None")
-        super(EmbedNet, self).__init__(**kwargs)
-        if architecture_desc is None: # Adpatively specify network architecture based on training dataset
+    def __init__(self,
+                 problem_type,
+                 num_net_outputs=None,
+                 quantile_levels=None,
+                 train_dataset=None,
+                 architecture_desc=None,
+                 device=None,
+                 **kwargs):
+        if (architecture_desc is None) and (train_dataset is None):
+            raise ValueError("train_dataset cannot = None if architecture_desc=None")
+        super().__init__()
+        self.problem_type = problem_type
+        if self. problem_type == QUANTILE:
+            self.register_buffer('quantile_levels', torch.Tensor(quantile_levels).float().reshape(1, -1))
+        self.device = torch.device('cpu') if device is None else device
+        if architecture_desc is None:
+            params = self._set_params(**kwargs)
+            # adpatively specify network architecture based on training dataset
             self.from_logits = False
-            self.has_vector_features = train_dataset.has_vector_features()
-            self.has_embed_features = train_dataset.num_embed_features() > 0
+            self.has_vector_features = train_dataset.has_vector_features
+            self.has_embed_features = train_dataset.has_embed_features
             if self.has_embed_features:
                 num_categs_per_feature = train_dataset.getNumCategoriesEmbeddings()
                 embed_dims = get_embed_sizes(train_dataset, params, num_categs_per_feature)
-        else: # Ignore train_dataset, params, etc. Recreate architecture based on description:
+            if self.has_vector_features:
+                vector_dims = train_dataset.data_list[train_dataset.vectordata_index].shape[-1]
+        else:
+            # ignore train_dataset, params, etc. Recreate architecture based on description:
             self.architecture_desc = architecture_desc
             self.has_vector_features = architecture_desc['has_vector_features']
             self.has_embed_features = architecture_desc['has_embed_features']
             self.from_logits = architecture_desc['from_logits']
-            num_net_outputs = architecture_desc['num_net_outputs']
             params = architecture_desc['params']
             if self.has_embed_features:
                 num_categs_per_feature = architecture_desc['num_categs_per_feature']
                 embed_dims = architecture_desc['embed_dims']
-        
-        # Define neural net parameters:
-        if self.has_vector_features:
-            self.numeric_block = NumericBlock(params)
+            if self.has_vector_features:
+                vector_dims = architecture_desc['vector_dims']
+        # init input size
+        input_size = 0
+
+        # define embedding layer:
         if self.has_embed_features:
-            self.embed_blocks = gluon.nn.HybridSequential()
+            self.embed_blocks = nn.ModuleList()
             for i in range(len(num_categs_per_feature)):
-                self.embed_blocks.add(EmbedBlock(embed_dims[i], num_categs_per_feature[i]))
-        if params['network_type'] == 'feedforward':
-            self.output_block = FeedforwardBlock(params, num_net_outputs)
-        elif params['network_type'] == 'widedeep':
-            self.output_block = WideAndDeepBlock(params, num_net_outputs)
-        else:
-            raise ValueError("unknown network_type specified: %s" % params['network_type'])
-        
-        y_range = params['y_range'] # Used specifically for regression. = None for classification.
-        self.y_constraint = None # determines if Y-predictions should be constrained
-        if y_range is not None:
-            if y_range[0] == -np.inf and y_range[1] == np.inf:
-                self.y_constraint = None # do not worry about Y-range in this case
-            elif y_range[0] >= 0 and y_range[1] == np.inf:
-                self.y_constraint = 'nonnegative'
-            elif y_range[0] == -np.inf and y_range[1] <= 0:
-                self.y_constraint = 'nonpositive'
-            else:
-                self.y_constraint = 'bounded'
-            self.y_lower = nd.array(params['y_range'][0]).reshape(1,)
-            self.y_upper = nd.array(params['y_range'][1]).reshape(1,)
-            if ctx is not None:
-                self.y_lower = self.y_lower.as_in_context(ctx)
-                self.y_upper = self.y_upper.as_in_context(ctx)
-            self.y_span = self.y_upper - self.y_lower
-        
-        if architecture_desc is None: # Save Architecture description
-            self.architecture_desc = {'has_vector_features': self.has_vector_features, 
-                                  'has_embed_features': self.has_embed_features,
-                                  'params': params, 'num_net_outputs': num_net_outputs,
-                                  'from_logits': self.from_logits}
+                self.embed_blocks.append(nn.Embedding(num_embeddings=num_categs_per_feature[i],
+                                                      embedding_dim=embed_dims[i]))
+                input_size += embed_dims[i]
+
+        # update input size
+        if self.has_vector_features:
+            input_size += vector_dims
+
+        # activation
+        act_fn = nn.Identity()
+        if params['activation'] == 'elu':
+            act_fn = nn.ELU()
+        elif params['activation'] == 'relu':
+            act_fn = nn.ReLU()
+        elif params['activation'] == 'tanh':
+            act_fn = nn.Tanh()
+
+        layers = []
+        if params['use_batchnorm']:
+            layers.append(nn.BatchNorm1d(input_size))
+        layers.append(nn.Linear(input_size, params['hidden_size']))
+        layers.append(act_fn)
+        for _ in range(params['num_layers'] - 1):
+            if params['use_batchnorm']:
+                layers.append(nn.BatchNorm1d(params['hidden_size']))
+            layers.append(nn.Dropout(params['dropout_prob']))
+            layers.append(nn.Linear(params['hidden_size'], params['hidden_size']))
+            layers.append(act_fn)
+        layers.append(nn.Linear(params['hidden_size'], num_net_outputs))
+        self.main_block = nn.Sequential(*layers)
+
+        if self.problem_type in [REGRESSION, QUANTILE]:  # set range for output
+            y_range = params['y_range']  # Used specifically for regression. = None for classification.
+            self.y_constraint = None  # determines if Y-predictions should be constrained
+            if y_range is not None:
+                if y_range[0] == -np.inf and y_range[1] == np.inf:
+                    self.y_constraint = None  # do not worry about Y-range in this case
+                elif y_range[0] >= 0 and y_range[1] == np.inf:
+                    self.y_constraint = 'nonnegative'
+                elif y_range[0] == -np.inf and y_range[1] <= 0:
+                    self.y_constraint = 'nonpositive'
+                else:
+                    self.y_constraint = 'bounded'
+                self.y_lower = y_range[0]
+                self.y_upper = y_range[1]
+                self.y_span = self.y_upper - self.y_lower
+
+        if self.problem_type == QUANTILE:
+            self.alpha = params['alpha']  # for huber loss
+        if self.problem_type == SOFTCLASS:
+            self.log_softmax = torch.nn.LogSoftmax(dim=1)
+        if self.problem_type in [BINARY, MULTICLASS, SOFTCLASS]:
+            self.softmax = torch.nn.Softmax(dim=1)
+        if architecture_desc is None:  # Save Architecture description
+            self.architecture_desc = {'has_vector_features': self.has_vector_features,
+                                      'has_embed_features': self.has_embed_features,
+                                      'params': params, 'num_net_outputs': num_net_outputs,
+                                      'from_logits': self.from_logits}
             if self.has_embed_features:
                 self.architecture_desc['num_categs_per_feature'] = num_categs_per_feature
                 self.architecture_desc['embed_dims'] = embed_dims
+            if self.has_vector_features:
+                self.architecture_desc['vector_dims'] = vector_dims
+
+    def _set_params(self,
+                    num_layers=4,
+                    hidden_size=128,
+                    activation='relu',
+                    use_batchnorm=False,
+                    dropout_prob=0.1,
+                    y_range=None,
+                    alpha=0.01,
+                    max_embedding_dim=100,
+                    embed_exponent=0.56,
+                    embedding_size_factor=1.0):
+        return dict(
+            num_layers=num_layers,
+            hidden_size=hidden_size,
+            activation=activation,
+            use_batchnorm=use_batchnorm,
+            dropout_prob=dropout_prob,
+            y_range=y_range,
+            alpha=alpha,
+            max_embedding_dim=max_embedding_dim,
+            embed_exponent=embed_exponent,
+            embedding_size_factor=embedding_size_factor,
+        )
+
+    def init_params(self):
+        for layer in self.children():
+            if hasattr(layer, 'reset_parameters'):
+                layer.reset_parameters()
 
     def forward(self, data_batch):
+        input_data = []
+        input_offset = 0
         if self.has_vector_features:
-            numerical_data = data_batch['vector'] # NDArray
-            numerical_activations = self.numeric_block(numerical_data)
-            input_activations = numerical_activations
+            input_data.append(data_batch[0].to(self.device))
+            input_offset += 1
         if self.has_embed_features:
-            embed_data = data_batch['embed'] # List
+            embed_data = data_batch[input_offset]
+            for i in range(len(self.embed_blocks)):
+                input_data.append(self.embed_blocks[i](embed_data[i].to(self.device)))
 
-            # TODO: Remove below lines or write logic to switch between using these lines and the multithreaded version once multithreaded version is optimized
-            embed_activations = self.embed_blocks[0](embed_data[0])
-            for i in range(1, len(self.embed_blocks)):
-                embed_activations = nd.concat(embed_activations,
-                                              self.embed_blocks[i](embed_data[i]), dim=2)
-
-            # TODO: Optimize below to perform better before using
-            # lock = threading.Lock()
-            # results = {}
-            #
-            # def _worker(i, results, embed_block, embed_data, is_recording, is_training, lock):
-            #     if is_recording:
-            #         with mx.autograd.record(is_training):
-            #             output = embed_block(embed_data)
-            #     else:
-            #         output = embed_block(embed_data)
-            #     output.wait_to_read()
-            #     with lock:
-            #         results[i] = output
-            #
-            # is_training = mx.autograd.is_training()
-            # is_recording = mx.autograd.is_recording()
-            # threads = [threading.Thread(target=_worker,
-            #                     args=(i, results, embed_block, embed_data,
-            #                           is_recording, is_training, lock),
-            #                     )
-            #    for i, (embed_block, embed_data) in
-            #    enumerate(zip(self.embed_blocks, embed_data))]
-            #
-            # for thread in threads:
-            #     thread.start()
-            # for thread in threads:
-            #     thread.join()
-            #
-            # embed_activations = []
-            # for i in range(len(results)):
-            #     output = results[i]
-            #     embed_activations.append(output)
-            #
-            # #embed_activations = []
-            # #for i in range(len(self.embed_blocks)):
-            # #    embed_activations.append(self.embed_blocks[i](embed_data[i]))
-            # embed_activations = nd.concat(*embed_activations, dim=2)
-            embed_activations = embed_activations.flatten()
-            if not self.has_vector_features:
-                input_activations = embed_activations
-            else:
-                input_activations = nd.concat(embed_activations, input_activations)
-        if self.y_constraint is None:
-            return self.output_block(input_activations)
+        if len(input_data) > 1:
+            input_data = torch.cat(input_data, dim=1)
         else:
-            unscaled_pred = self.output_block(input_activations)
-            if self.y_constraint == 'nonnegative':
-                return self.y_lower + nd.abs(unscaled_pred)
-            elif self.y_constraint == 'nonpositive':
-                return self.y_upper - nd.abs(unscaled_pred)
+            input_data = input_data[0]
+
+        output_data = self.main_block(input_data)
+        if self.problem_type in [REGRESSION, QUANTILE]:  # output with y-range
+            if self.y_constraint is None:
+                return output_data
             else:
-                """
-                print("unscaled_pred",unscaled_pred)
-                print("nd.sigmoid(unscaled_pred)", nd.sigmoid(unscaled_pred))
-                print("self.y_span", self.y_span)
-                print("self.y_lower", self.y_lower)
-                print("self.y_lower.shape", self.y_lower.shape)
-                print("nd.sigmoid(unscaled_pred).shape", nd.sigmoid(unscaled_pred).shape)
-                """
-                return nd.sigmoid(unscaled_pred) * self.y_span + self.y_lower
+                if self.y_constraint == 'nonnegative':
+                    return self.y_lower + torch.abs(output_data)
+                elif self.y_constraint == 'nonpositive':
+                    return self.y_upper - torch.abs(output_data)
+                else:
+                    return torch.sigmoid(output_data) * self.y_span + self.y_lower
+        elif self.problem_type == SOFTCLASS:
+            return self.log_softmax(output_data)  # KLDivLoss takes in log-probabilities as predictions.
+        else:
+            return output_data
+
+    def huber_pinball_loss(self, input_data, target_data):
+        error_data = target_data.contiguous().reshape(-1, 1) - input_data
+        if self.alpha == 0.0:
+            loss_data = torch.max(self.quantile_levels * error_data, (self.quantile_levels - 1) * error_data)
+            return loss_data.mean()
+
+        loss_data = torch.where(torch.abs(error_data) < self.alpha,
+                                0.5 * error_data * error_data,
+                                self.alpha * (torch.abs(error_data) - 0.5 * self.alpha))
+        loss_data /= self.alpha
+        scale = torch.where(error_data >= 0,
+                            torch.ones_like(error_data) * self.quantile_levels,
+                            torch.ones_like(error_data) * (1 - self.quantile_levels))
+        loss_data *= scale
+        return loss_data.mean()
+
+    def margin_loss(self, input_data, margin_scale=0.0001):
+        # number of samples
+        batch_size, num_quantiles = input_data.size()
+
+        # compute margin loss (batch_size x num_net_outputs(above) x num_net_outputs(below))
+        error_data = input_data.unsqueeze(1) - input_data.unsqueeze(2)
+
+        # margin data (num_quantiles x num_quantiles)
+        margin_data = self.quantile_levels.permute(1, 0) - self.quantile_levels
+        margin_data = torch.tril(margin_data, -1) * margin_scale
+
+        # compute accumulated margin
+        loss_data = torch.tril(error_data + margin_data, diagonal=-1)
+        loss_data = loss_data.relu()
+        loss_data = loss_data.sum() / float(batch_size * (num_quantiles * num_quantiles - num_quantiles) * 0.5)
+        return loss_data
+
+    def quantile_loss(self, predict_data, target_data, margin):
+        if margin > 0.0:
+            m_loss = self.margin_loss(predict_data)
+        else:
+            m_loss = 0.0
+        h_loss = self.huber_pinball_loss(predict_data, target_data).mean()
+        return h_loss + margin * m_loss
+
+    def compute_loss(self, data_batch, loss_function=None, gamma=None):
+        # train mode
+        self.train()
+        predict_data = self(data_batch)
+        target_data = data_batch[-1].to(self.device)
+        if self.problem_type in [BINARY, MULTICLASS]:
+            target_data = target_data.type(torch.long)  # Windows default int type is int32. Need to explicit convert to Long.
+        if self.problem_type == QUANTILE:
+            return self.quantile_loss(predict_data, target_data, margin=gamma)
+        if self.problem_type == SOFTCLASS:
+            return loss_function(predict_data, target_data)
+        else:
+            target_data = target_data.flatten()
+            if self.problem_type == REGRESSION:
+                predict_data = predict_data.flatten()
+            return loss_function(predict_data, target_data)
+
+
+    def predict(self, input_data):
+        self.eval()
+        with torch.no_grad():
+            predict_data = self(input_data)
+            if self.problem_type == QUANTILE:
+                predict_data = torch.sort(predict_data, -1)[0]  # sorting ensures monotonicity of quantile estimates
+            elif self.problem_type in [BINARY, MULTICLASS, SOFTCLASS]:
+                predict_data = self.softmax(predict_data)  # convert NN output to probability
+            elif self.problem_type == REGRESSION:
+                predict_data = predict_data.flatten()
+            if self.problem_type == BINARY:
+                predict_data = predict_data[:,1]
+            return predict_data.data.cpu().numpy()
```

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_dataset.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,157 +1,177 @@
+import os
 import logging
-from collections import OrderedDict
+
+import torch
 import numpy as np
-import pandas as pd
-import mxnet as mx
 
-from autogluon.core.utils.loaders import load_pkl
-from autogluon.core.utils.savers import save_pkl
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS
+from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE
+
+logger = logging.getLogger(__name__)
 
-logger = logging.getLogger(__name__)  # TODO: Currently unused
 
+class TabularTorchDataset(torch.utils.data.IterableDataset):
+    """
+        This class follows the structure of TabularNNDataset in tabular_nn_dataset.py,
 
-class TabularNNDataset:
-    """ Class for preprocessing & storing/feeding data batches used by tabular data neural networks. Assumes entire dataset can be loaded into numpy arrays.
-        Original Data table may contain numerical and categorical fields.
+        Class for preprocessing & storing/feeding data batches used by pytorch neural networks for tabular data.
+        Assumes entire dataset can be loaded into numpy arrays.
+        Original data table may contain numeric and categorical fields and missing values.
 
         Attributes:
-            dataset (mxnet.gluon.data.dataset): Contains the raw data (use dataset._data to access).
-                                                Different indices in this list correspond to different types of inputs to the neural network (each is 2D ND array)
-                                                All vector-valued (continuous & one-hot) features are concatenated together into a single index of the dataset.
-            data_desc (list[str]): Describes the data type of each index of dataset (options: 'vector','embed_<featname>')
-            dataloader (mxnet.gluon.data.DataLoader): Loads batches of data from dataset for neural net training and inference.
+            data_list (list[np.array]): Contains the raw data. Different indices in this list correspond to different
+                                        types of inputs to the neural network (each is 2D array). All vector-valued
+                                        (continuous & one-hot) features are concatenated together into a single index
+                                        of the dataset.
+            data_desc (list[str]): Describes the data type of each index of dataset
+                                   (options: 'vector','embed_<featname>')
             embed_indices (list): which columns in dataset correspond to embed features (order matters!)
-            vecfeature_col_map (dict): maps vector_feature_name ->  columns of dataset._data[vector] array that contain the data for this feature
-            feature_dataindex_map (dict): maps feature_name -> i such that dataset._data[i] = data array for this feature. Cannot be used for vector-valued features, instead use vecfeature_col_map
-            feature_groups (dict): maps feature_type (ie. 'vector' or 'embed') to list of feature names of this type (empty list if there are no features of this type)
-            vectordata_index (int): describes which element of the dataset._data list holds the vector data matrix (access via self.dataset._data[self.vectordata_index]); None if no vector features
-            label_index (int): describing which element of the dataset._data list holds labels (access via self.dataset._data[self.label_index].asnumpy()); None if no labels
+            vecfeature_col_map (dict): maps vector_feature_name ->  columns of dataset._data[vector] array that
+                                       contain the data for this feature
+            feature_dataindex_map (dict): maps feature_name -> i such that dataset._data[i] = data array for
+                                          this feature. Cannot be used for vector-valued features,
+                                          instead use vecfeature_col_map
+            feature_groups (dict): maps feature_type (ie. 'vector' or 'embed') to list of feature
+                                   names of this type (empty list if there are no features of this type)
+            vectordata_index (int): describes which element of the dataset._data list holds the vector data matrix
+                                    (access via self.data_list[self.vectordata_index]); None if no vector features
+            label_index (int): describing which element of the dataset._data list holds labels
+                               (access via self.data_list[self.label_index]); None if no labels
             num_categories_per_embedfeature (list): Number of categories for each embedding feature (order matters!)
             num_examples (int): number of examples in this dataset
-            num_features (int): number of features (we only consider original variables as features, so num_features may not correspond to dimensionality of the data eg in the case of one-hot encoding)
-            num_classes (int): number of classes (only used for multiclass classification)
-
-        Note: Default numerical data-type is converted to float32 (as well as labels in regression).
+            num_features (int): number of features (we only consider original variables as features, so num_features
+                                may not correspond to dimensionality of the data eg in the case of one-hot encoding)
+        Note: Default numerical data-type is converted to float32.
     """
+    # hard-coded names for files. This file contains pickled torch.util.data.Dataset object
+    DATAOBJ_SUFFIX = '_tabdataset_torch.pt'
 
-    DATAOBJ_SUFFIX = '_tabNNdataset.pkl' # hard-coded names for files. This file contains pickled TabularNNDataset object
-    DATAVALUES_SUFFIX = '_tabNNdata.npz' # This file contains raw data values as data_list of NDArrays
-
-    def __init__(self, processed_array, feature_arraycol_map, feature_type_map, batch_size, num_dataloading_workers, problem_type,
-                 labels=None, is_test=True):
+    def __init__(self, processed_array, feature_arraycol_map, feature_type_map, problem_type, labels=None):
         """ Args:
-                processed_array: 2D numpy array returned by preprocessor. Contains raw data of all features as columns
-                feature_arraycol_map (OrderedDict): Mapsfeature-name -> list of column-indices in processed_array corresponding to this feature
-                feature_type_map (OrderedDict): Maps feature-name -> feature_type string (options: 'vector', 'embed')
-                labels (pd.Series): list of labels (y) if available
-                batch_size (int): number of examples to put in each mini-batch
-                num_dataloading_workers (int): number of threads to devote to loading mini-batches of data rather than model-training
+            processed_array: 2D numpy array returned by preprocessor. Contains raw data of all features as columns
+            feature_arraycol_map (OrderedDict): Mapsfeature-name -> list of column-indices in processed_array
+                                                corresponding to this feature
+            feature_type_map (OrderedDict): Maps feature-name -> feature_type string
+                                            (options: 'vector', 'embed')
+            problem_type (str): what prediction task this data is used for.
+            labels (pd.Series): list of labels (y) if available
         """
-        self.dataset = None
-        self.dataloader = None
         self.problem_type = problem_type
         self.num_examples = processed_array.shape[0]
-        self.num_features = len(feature_arraycol_map) # number of features (!=dim(processed_array) because some features may be vector-valued, eg one-hot)
-        self.batch_size = min(self.num_examples, batch_size)
-        self.is_test = is_test
-        self.num_dataloading_workers = num_dataloading_workers
-        last_batch_size = self.num_examples % self.batch_size
-        if last_batch_size == 0:
-            last_batch_size = self.batch_size
-        # TODO: The code fixes the crash on mxnet gluon interpreting a single value in a batch incorrectly.
-        #  Comment out to see crash if data would have single row as final batch on test prediction (such as 1025 rows for batch size 512)
-        if (self.num_examples != 1) and self.is_test and (last_batch_size == 1):
-            init_batch_size = self.batch_size
-            while last_batch_size == 1:
-                self.batch_size = self.batch_size + 1
-                last_batch_size = self.num_examples % self.batch_size
-                if last_batch_size == 0:
-                    last_batch_size = self.batch_size
-                if self.batch_size > init_batch_size+10:
-                    # Hard set to avoid potential infinite loop, don't think its mathematically possible to reach this code however.
-                    self.batch_size = self.num_examples
-                    last_batch_size = 0
-
+        self.num_features = len(feature_arraycol_map)
         if feature_arraycol_map.keys() != feature_type_map.keys():
             raise ValueError("feature_arraycol_map and feature_type_map must share same keys")
-        self.feature_groups = {'vector': [], 'embed': []} # maps feature_type -> list of feature_names (order is preserved in list)
+        self.feature_groups = {'vector': [], 'embed': []}
         self.feature_type_map = feature_type_map
         for feature in feature_type_map:
             if feature_type_map[feature] == 'vector':
                 self.feature_groups['vector'].append(feature)
             elif feature_type_map[feature] == 'embed':
                 self.feature_groups['embed'].append(feature)
             else:
                 raise ValueError("unknown feature type: %s" % feature)
-
-        if not self.is_test and labels is None:
-            raise ValueError("labels must be provided when is_test = False")
         if labels is not None and len(labels) != self.num_examples:
             raise ValueError("number of labels and training examples do not match")
 
-        data_list = [] # stores all data of each feature-type in list used to construct MXNet dataset. Each index of list = 2D NDArray.
-        self.label_index = None # int describing which element of the dataset._data list holds labels
-        self.data_desc = [] # describes feature-type of each index of data_list
-        self.vectordata_index = None # int describing which element of the dataset._data list holds the vector data matrix
-        self.vecfeature_col_map = {} # maps vector_feature_name ->  columns of dataset._data[vector] array that contain data for this feature
-        self.feature_dataindex_map = {} # maps feature_name -> i such that dataset._data[i] = data array for this feature. Cannot be used for vector-valued features, instead use: self.vecfeature_col_map
+        self.data_desc = []
+        self.data_list = []
+        self.label_index = None
+        self.vectordata_index = None
+        self.vecfeature_col_map = {}
+        self.feature_dataindex_map = {}
+        self.num_classes = None
 
+        # numerical data
         if len(self.feature_groups['vector']) > 0:
-            vector_inds = [] # columns of processed_array corresponding to vector data
+            vector_inds = []
             for feature in feature_type_map:
                 if feature_type_map[feature] == 'vector':
-                    current_last_ind = len(vector_inds) # current last index of the vector datamatrix
+                    current_last_ind = len(vector_inds)
                     vector_inds += feature_arraycol_map[feature]
-                    new_last_ind = len(vector_inds) # new last index of the vector datamatrix
+                    new_last_ind = len(vector_inds)
                     self.vecfeature_col_map[feature] = list(range(current_last_ind, new_last_ind))
-            data_list.append(mx.nd.array(processed_array[:,vector_inds], dtype='float32')) # Matrix of data from all vector features
-            self.data_desc.append("vector")
-            self.vectordata_index = len(data_list) - 1
+            self.data_list.append(processed_array[:, vector_inds].astype('float32'))
+            self.data_desc.append('vector')
+            self.vectordata_index = len(self.data_list) - 1
 
+        # embedding data
         if len(self.feature_groups['embed']) > 0:
             for feature in feature_type_map:
                 if feature_type_map[feature] == 'embed':
                     feature_colind = feature_arraycol_map[feature]
-                    data_list.append(mx.nd.array(processed_array[:,feature_colind], dtype='int32')) # array of ints with data for this embedding feature
-                    self.data_desc.append("embed")
-                    self.feature_dataindex_map[feature]  = len(data_list)-1
+                    self.data_list.append(processed_array[:, feature_colind].astype('int64').flatten())
+                    self.data_desc.append('embed')
+                    self.feature_dataindex_map[feature] = len(self.data_list) - 1
 
-        self.num_classes = None
+        # output (target) data
         if labels is not None:
             labels = np.array(labels)
             self.data_desc.append("label")
-            self.label_index = len(data_list) # To access data labels, use: self.dataset._data[self.label_index]
-            self.num_classes = None
+            self.label_index = len(self.data_list)
             if self.problem_type == SOFTCLASS:
                 self.num_classes = labels.shape[1]
-                data_list.append(mx.nd.array(labels))
+                self.data_list.append(labels.astype('float32'))
             else:
-                if self.problem_type == REGRESSION and labels.dtype != np.float32:
-                    labels = labels.astype('float32') # Convert to proper float-type if not already
+                if self.problem_type in [REGRESSION, QUANTILE] and labels.dtype != np.float32:
+                    labels = labels.astype('float32')  # Convert to proper float-type if not already
                 elif self.problem_type in [BINARY, MULTICLASS]:
                     self.num_classes = len(set(labels))
-                data_list.append(mx.nd.array(labels.reshape(len(labels),1)))
+                    labels = labels.astype('long')
+                self.data_list.append(labels.reshape(-1, 1))
 
-        self.embed_indices = [i for i in range(len(self.data_desc)) if 'embed' in self.data_desc[i]] # list of indices of embedding features in self.dataset, order matters!
+        self.embed_indices = [i for i in range(len(self.data_desc)) if 'embed' in self.data_desc[i]]
         self.num_categories_per_embed_feature = None
-        self.generate_dataset_and_dataloader(data_list=data_list)
-        if not self.is_test:
-            self.num_categories_per_embedfeature = self.getNumCategoriesEmbeddings()
-
-    def generate_dataset_and_dataloader(self, data_list):
-        self.dataset = mx.gluon.data.dataset.ArrayDataset(*data_list)  # Access ith embedding-feature via: self.dataset._data[self.data_desc.index('embed_'+str(i))].asnumpy()
-        self.dataloader = mx.gluon.data.DataLoader(
-            self.dataset,
-            self.batch_size,
-            shuffle=not self.is_test,
-            last_batch='keep' if self.is_test else 'rollover',
-            num_workers=0,
-        )  # no need to shuffle test data
+        self.num_categories_per_embedfeature = self.getNumCategoriesEmbeddings()
+
+        self.has_vector_features = self.vectordata_index is not None
+        self.has_embed_features = len(self.feature_groups['embed']) > 0
+
+    def __iter__(self):
+        """
+        Iterate through the iterable dataset, and return a subsample of it.
+
+        This overrides the `__iter__` function in IterableDataset.
+        This is typically useful when we are using :class:`torch.utils.data.DataLoader` to
+        load the dataset.
+
+        Returns a tuple containing (vector_features, embed_features, label).
+        The length of the tuple depends on `has_vector_features` and `has_embed_feautures` attribute.
+        """
+        idxarray = np.arange(self.num_examples)
+        if self.shuffle:
+            np.random.shuffle(idxarray)
+        indices = range(0, self.num_examples, self.batch_size)
+        for idx_start in indices:
+            # Drop last batch
+            if self.drop_last and (idx_start + self.batch_size) > self.num_examples:
+                break
+            idx = range(idx_start, min(self.num_examples, idx_start + self.batch_size))
+
+            # Shuffle the index array to reorder the output sequence.
+            # This should be consistent across different features (vector, embed and label).
+            if self.shuffle:
+                idx = idxarray[idx]
+
+            # Generate a tuple that contains (vector_features, embed_features, label).
+            # The length of the tuple depends on `has_vector_features`, `has_embed_feautures`, and
+            # whether the label has been provided.
+            output_list = []
+            if self.has_vector_features:
+                output_list.append(self.data_list[self.vectordata_index][idx])
+            if self.has_embed_features:
+                output_embed = []
+                for i in self.embed_indices:
+                    output_embed.append(self.data_list[i][idx])
+                output_list.append(output_embed)
+            if self.label_index is not None:
+                output_list.append(self.data_list[self.label_index][idx])
+            yield tuple(output_list)
+
+    def __len__(self):
+        return self.num_examples
 
     def has_vector_features(self):
         """ Returns boolean indicating whether this dataset contains vector features """
         return self.vectordata_index is not None
 
     def num_embed_features(self):
         """ Returns number of embed features in this dataset """
@@ -160,18 +180,15 @@
     def num_vector_features(self):
         """ Number of vector features (each onehot feature counts = 1, regardless of how many categories) """
         return len(self.feature_groups['vector'])
 
     def get_labels(self):
         """ Returns numpy array of labels for this dataset """
         if self.label_index is not None:
-            if self.problem_type == SOFTCLASS:
-                return self.dataset._data[self.label_index].asnumpy()
-            else:
-                return self.dataset._data[self.label_index].asnumpy().flatten()
+            return self.data_list[self.label_index]
         else:
             return None
 
     def getNumCategoriesEmbeddings(self):
         """ Returns number of categories for each embedding feature.
             Should only be applied to training data.
             If training data feature contains unique levels 1,...,n-1, there are actually n categories,
@@ -185,111 +202,51 @@
             for i in range(num_embed_feats):
                 feat_i = self.feature_groups['embed'][i]
                 feat_i_data = self.get_feature_data(feat_i).flatten().tolist()
                 num_categories_i = len(set(feat_i_data)) # number of categories for ith feature
                 num_categories_per_embedfeature[i] = num_categories_i + 1 # to account for unknown test-time categories
             return num_categories_per_embedfeature
 
-    def get_feature_data(self, feature, asnumpy=True):
+    def get_feature_data(self, feature):
         """ Returns all data for this feature.
             Args:
                 feature (str): name of feature of interest (in processed dataframe)
-                asnumpy (bool): should we return 2D numpy array or MXNet NDarray
-        """
-        nonvector_featuretypes = set(['embed'])
-        if feature not in self.feature_type_map:
-            raise ValueError("unknown feature encountered: %s" % feature)
-        if self.feature_type_map[feature] == 'vector':
-            vector_datamatrix = self.dataset._data[self.vectordata_index] # does not work for one-hot...
-            feature_data = vector_datamatrix[:, self.vecfeature_col_map[feature]]
-        elif self.feature_type_map[feature] in nonvector_featuretypes:
-            feature_idx = self.feature_dataindex_map[feature]
-            feature_data = self.dataset._data[feature_idx]
-        else:
-            raise ValueError("Unknown feature specified: " % feature)
-        if asnumpy:
-            return feature_data.asnumpy()
-        else:
-            return feature_data
-
-    def get_feature_batch(self, feature, data_batch, asnumpy=False):
-        """ Returns part of this batch corresponding to data from a single feature
-            Args:
-                data_batch (nd.array): the batch of data as provided by self.dataloader
-            Returns:
-
         """
         nonvector_featuretypes = set(['embed'])
         if feature not in self.feature_type_map:
             raise ValueError("unknown feature encountered: %s" % feature)
         if self.feature_type_map[feature] == 'vector':
-            vector_datamatrix = data_batch[self.vectordata_index]
+            vector_datamatrix = self.data_list[self.vectordata_index]
             feature_data = vector_datamatrix[:, self.vecfeature_col_map[feature]]
         elif self.feature_type_map[feature] in nonvector_featuretypes:
             feature_idx = self.feature_dataindex_map[feature]
-            feature_data = data_batch[feature_idx]
+            feature_data = self.data_list[feature_idx]
         else:
             raise ValueError("Unknown feature specified: " % feature)
-        if asnumpy:
-            return feature_data.asnumpy()
-        else:
-            return feature_data
-
-    def format_batch_data(self, data_batch, ctx):
-        """ Partitions data from this batch into different data types.
-            Args:
-                data_batch (nd.array): the batch of data as provided by self.dataloader
-            Returns:
-                formatted_batch (dict): {'vector': array of vector_datamatrix,
-                                         'embed': list of embedding features' batch data,
-                                         'label': array of labels}
-                                        where each key in dict may be missing.
-        """
-        if not isinstance(data_batch, list):
-            data_batch = [data_batch] # Need to convert to list if dimension was dropped during batching
-
-        if len(data_batch[0].shape) == 1:
-            data_batch[0] = data_batch[0].expand_dims(axis=0)
-        formatted_batch = {}
-        if self.has_vector_features(): # None if there is no vector data
-            formatted_batch['vector'] = data_batch[self.vectordata_index].as_in_context(ctx)
-        if self.num_embed_features() > 0:
-            formatted_batch['embed'] = []
-            for i in self.embed_indices:
-                formatted_batch['embed'].append(data_batch[i].as_in_context(ctx))
-        if self.label_index is not None: # is None if there are no labels
-            formatted_batch['label'] = data_batch[self.label_index].as_in_context(ctx)
-
-        return formatted_batch
-
-    def mask_features_batch(self, features, mask_value, data_batch):
-        """ Returns new batch where all values of the indicated features have been replaced by the provided mask_value.
-            Args:
-                features (list[str]): list of feature names that should be masked.
-                mask_value (float): value of mask which original feature values should be replaced by. If None, we replace by mean/mode/unknown
-                data_batch (nd.array): the batch of data as provided by self.dataloader
-            Returns:
-                new_batch (nd.array): batch of masked data in same format as data_batch
-        """
-        return None # TODO
+        return feature_data
 
     def save(self, file_prefix=""):
         """ Additional naming changes will be appended to end of file_prefix (must contain full absolute path) """
         dataobj_file = file_prefix + self.DATAOBJ_SUFFIX
-        datalist_file = file_prefix + self.DATAVALUES_SUFFIX
-        data_list = self.dataset._data
-        self.dataset = None  # Avoid pickling these
-        self.dataloader = None
-        save_pkl.save(path=dataobj_file, object=self)
-        mx.nd.save(datalist_file, data_list)
-        logger.debug("TabularNN Dataset saved to files: \n %s \n %s" % (dataobj_file, datalist_file))
+        if not os.path.exists(os.path.dirname(dataobj_file)):
+            os.makedirs(os.path.dirname(dataobj_file))
+        torch.save(self, dataobj_file)
+        logger.debug("TabularPyTorchDataset Dataset saved to a file: \n %s" % dataobj_file)
 
     @classmethod
     def load(cls, file_prefix=""):
         """ Additional naming changes will be appended to end of file_prefix (must contain full absolute path) """
         dataobj_file = file_prefix + cls.DATAOBJ_SUFFIX
-        datalist_file = file_prefix + cls.DATAVALUES_SUFFIX
-        dataset: TabularNNDataset = load_pkl.load(path=dataobj_file)
-        data_list = mx.nd.load(datalist_file)
-        dataset.generate_dataset_and_dataloader(data_list=data_list)
-        logger.debug("TabularNN Dataset loaded from files: \n %s \n %s" % (dataobj_file, datalist_file))
+        dataset: TabularTorchDataset = torch.load(dataobj_file)
+        logger.debug("TabularNN Dataset loaded from a file: \n %s" % dataobj_file)
         return dataset
+
+    def build_loader(self, batch_size, num_workers, is_test=False):
+        def worker_init_fn(worker_id):
+            np.random.seed(np.random.get_state()[1][0] + worker_id)
+        self.batch_size = batch_size
+        self.shuffle = False if is_test else True
+        self.drop_last = False if is_test else True
+        loader = torch.utils.data.DataLoader(self, num_workers=num_workers,
+                                             batch_size=None, # no collation
+                                             worker_init_fn=worker_init_fn)
+        return loader
```

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_mxnet.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,621 +1,696 @@
-""" MXNet neural networks for tabular data containing numerical, categorical, and text fields.
-    First performs neural network specific pre-processing of the data.
-    Contains separate input modules which are applied to different columns of the data depending on the type of values they contain:
-    - Numeric columns are passed through single Dense layer (binary categorical variables are treated as numeric)
-    - Categorical columns are passed through separate Embedding layers
-    Vectors produced by different input layers are then concatenated and passed to multi-layer MLP model with problem_type determined output layer.
-    Hyperparameters are passed as dict params, including options for preprocessing stages.
-"""
 import json
 import logging
 import os
 import random
 import time
 import warnings
-from collections import OrderedDict
-
 import numpy as np
 import pandas as pd
 
+from typing import Dict, Union
+
 from autogluon.common.features.types import R_BOOL, R_INT, R_FLOAT, R_CATEGORY, S_TEXT_NGRAM, S_TEXT_AS_CATEGORY
-from autogluon.common.utils.try_import import try_import_mxboard, try_import_mxnet
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS
+from autogluon.common.utils.resource_utils import ResourceManager
+from autogluon.common.utils.try_import import try_import_torch
+from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE
+from autogluon.core.hpo.constants import RAY_BACKEND
 from autogluon.core.utils.exceptions import TimeLimitExceeded
 from autogluon.core.models.abstract.abstract_nn_model import AbstractNeuralNetworkModel
 
+from ..compilers.native import TabularNeuralNetTorchNativeCompiler
+from ..compilers.onnx import TabularNeuralNetTorchOnnxCompiler
 from ..hyperparameters.parameters import get_default_param
 from ..hyperparameters.searchspaces import get_default_searchspace
 from ..utils.data_preprocessor import create_preprocessor, get_feature_arraycol_map, get_feature_type_map
-from ..utils.nn_architecture_utils import infer_y_range, get_default_layers, default_numeric_embed_dim
+from ..utils.nn_architecture_utils import infer_y_range
 
-warnings.filterwarnings("ignore", module='sklearn.preprocessing')  # sklearn processing n_quantiles warning
 logger = logging.getLogger(__name__)
-EPS = 1e-10  # small number
-_has_warned_mxnet_deprecation = False
-
-
-# TODO: Gets stuck after inferring feature types near infinitely in nyc-jiashenliu-515k-hotel-reviews-data-in-europe dataset, 70 GB of memory, c5.9xlarge
-#  Suspect issue is coming from embeddings due to text features with extremely large categorical counts.
-class TabularNeuralNetMxnetModel(AbstractNeuralNetworkModel):
-    """ Class for neural network models that operate on tabular data.
-        These networks use different types of input layers to process different types of data in various columns.
-
-        Attributes:
-            _types_of_features (dict): keys = 'continuous', 'skewed', 'onehot', 'embed'; values = column-names of Dataframe corresponding to the features of this type
-            feature_arraycol_map (OrderedDict): maps feature-name -> list of column-indices in df corresponding to this feature
-        self.feature_type_map (OrderedDict): maps feature-name -> feature_type string (options: 'vector', 'embed')
-        processor (sklearn.ColumnTransformer): scikit-learn preprocessor object.
 
-        Note: This model always assumes higher values of self.eval_metric indicate better performance.
 
+# TODO: QuantileTransformer in pipelines accounts for majority of online inference time
+class TabularNeuralNetTorchModel(AbstractNeuralNetworkModel):
+    """
+    PyTorch neural network models for classification/regression with tabular data.
     """
 
     # Constants used throughout this class:
-    # model_internals_file_name = 'model-internals.pkl' # store model internals here
-    unique_category_str = '!missing!' # string used to represent missing values and unknown categories for categorical features. Should not appear in the dataset
-    params_file_name = 'net.params' # Stores parameters of final network
-    temp_file_name = 'temp_net.params' # Stores temporary network parameters (eg. during the course of training)
+    unique_category_str = np.nan  # string used to represent missing values and unknown categories for categorical features.
+    temp_file_name = 'temp_model.pt'  # Stores temporary network parameters (eg. during the course of training)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        """
-        TabularNeuralNetMxnetModel object.
-
-        Parameters
-        ----------
-        path (str): file-path to directory where to save files associated with this model
-        name (str): name used to refer to this model
-        problem_type (str): what type of prediction problem is this model used for
-        eval_metric (func): function used to evaluate performance (Note: we assume higher = better)
-        hyperparameters (dict): various hyperparameters for neural network and the NN-specific data processing
-        features (list): List of predictive features to use, other features are ignored by the model.
-        """
         self.feature_arraycol_map = None
         self.feature_type_map = None
         self.features_to_drop = []  # may change between different bagging folds. TODO: consider just removing these from self._features_internal
         self.processor = None  # data processor
-        self.summary_writer = None
-        self.ctx = None
-        self.batch_size = None
         self.num_dataloading_workers = None
-        self.num_dataloading_workers_inference = 0
-        self.params_post_fit = None
-        self.num_net_outputs = None
         self._architecture_desc = None
         self.optimizer = None
-        self.verbosity = None
+        self.device = None
+        self.max_batch_size = None
+        self._num_cpus_infer = None
 
     def _set_default_params(self):
         """ Specifies hyperparameter values to use by default """
-        default_params = get_default_param(problem_type=self.problem_type, framework='mxnet')
+        default_params = get_default_param(problem_type=self.problem_type, framework='pytorch')
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     def _get_default_auxiliary_params(self) -> dict:
         default_auxiliary_params = super()._get_default_auxiliary_params()
         extra_auxiliary_params = dict(
             valid_raw_types=[R_BOOL, R_INT, R_FLOAT, R_CATEGORY],
             ignored_type_group_special=[S_TEXT_NGRAM, S_TEXT_AS_CATEGORY],
         )
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
     def _get_default_searchspace(self):
-        return get_default_searchspace(problem_type=self.problem_type, framework='mxnet')
+        return get_default_searchspace(problem_type=self.problem_type, framework='pytorch')
 
-    def set_net_defaults(self, train_dataset, params):
-        """ Sets dataset-adaptive default values to use for our neural network """
+    def _get_num_net_outputs(self):
         if self.problem_type in [MULTICLASS, SOFTCLASS]:
-            self.num_net_outputs = train_dataset.num_classes
-        elif self.problem_type == REGRESSION:
-            self.num_net_outputs = 1
-            if params['y_range'] is None:
-                params['y_range'] = infer_y_range(y_vals=train_dataset.dataset._data[train_dataset.label_index].asnumpy(), y_range_extend=params['y_range_extend'])
+            return self.num_classes
         elif self.problem_type == BINARY:
-            self.num_net_outputs = 2
+            return 2
+        elif self.problem_type == REGRESSION:
+            return 1
+        elif self.problem_type == QUANTILE:
+            return len(self.quantile_levels)
         else:
-            raise ValueError("unknown problem_type specified: %s" % self.problem_type)
+            raise ValueError(f'Unknown problem_type: {self.problem_type}')
+
+    def _get_device(self, num_gpus):
+        import torch
+        if num_gpus is not None and num_gpus >= 1:
+            if torch.cuda.is_available():
+                device = torch.device("cuda")
+                logger.log(15, "Training on GPU")
+                if num_gpus > 1:
+                    logger.warning(f"{self.__class__.__name__} not yet able to use more than 1 GPU. 'num_gpus' is set to >1, but we will be using only 1 GPU.")
+            else:
+                device = torch.device("cpu")
+                logger.log(15, "Training on CPU")
+        else:
+            device = torch.device("cpu")
+            logger.log(15, "Training on CPU")
+        return device
+
+    def _set_net_defaults(self, train_dataset, params):
+        params = params.copy()
+        y_range_extend = params.pop('y_range_extend', None)
+        """ Sets dataset-adaptive default values to use for our neural network """
+        if self.problem_type in [REGRESSION, QUANTILE]:
+            if params['y_range'] is None:
+                params['y_range'] = infer_y_range(y_vals=train_dataset.data_list[train_dataset.label_index], y_range_extend=y_range_extend)
+        return params
 
-        if params['layers'] is None:  # Use default choices for MLP architecture
-            params['layers'] = get_default_layers(problem_type=self.problem_type, num_net_outputs=self.num_net_outputs, max_layer_width=params['max_layer_width'])
+    def _get_default_loss_function(self):
+        import torch
+        if self.problem_type == REGRESSION:
+            return torch.nn.L1Loss()  # or torch.nn.MSELoss()
+        elif self.problem_type in [BINARY, MULTICLASS]:
+            return torch.nn.CrossEntropyLoss()
+        elif self.problem_type == SOFTCLASS:
+            return torch.nn.KLDivLoss()  # compares log-probability prediction vs probability target.
+
+    @staticmethod
+    def _prepare_params(params):
+        params = params.copy()
+
+        processor_param_keys = {'proc.embed_min_categories', 'proc.impute_strategy', 'proc.max_category_levels', 'proc.skew_threshold', 'use_ngram_features'}
+        processor_kwargs = {k: v for k, v in params.items() if k in processor_param_keys}
+        for key in processor_param_keys:
+            params.pop(key, None)
+
+        optimizer_param_keys = {'optimizer', 'learning_rate', 'weight_decay'}
+        optimizer_kwargs = {k: v for k, v in params.items() if k in optimizer_param_keys}
+        for key in optimizer_param_keys:
+            params.pop(key, None)
+
+        fit_param_keys = {'num_epochs', 'epochs_wo_improve'}
+        fit_kwargs = {k: v for k, v in params.items() if k in fit_param_keys}
+        for key in fit_param_keys:
+            params.pop(key, None)
+
+        loss_param_keys = {'loss_function', 'gamma'}
+        loss_kwargs = {k: v for k, v in params.items() if k in loss_param_keys}
+        for key in loss_param_keys:
+            params.pop(key, None)
 
-        if train_dataset.has_vector_features() and params['numeric_embed_dim'] is None:  # Use default choices for numeric embedding size
-            params['numeric_embed_dim'] = default_numeric_embed_dim(train_dataset=train_dataset, max_layer_width=params['max_layer_width'], first_layer_width=params['layers'][0])
-        return
+        return processor_kwargs, optimizer_kwargs, fit_kwargs, loss_kwargs, params
 
     def _fit(self, X, y, X_val=None, y_val=None,
-             time_limit=None, sample_weight=None, num_cpus=1, num_gpus=0, reporter=None, **kwargs):
-        """ X (pd.DataFrame): training data features (not necessarily preprocessed yet)
-            X_val (pd.DataFrame): test data features (should have same column names as Xtrain)
-            y (pd.Series):
-            y_val (pd.Series): are pandas Series
-            kwargs: Can specify amount of compute resources to utilize (num_cpus, num_gpus).
-        """
+             time_limit=None, sample_weight=None, num_cpus=1, num_gpus=0, reporter=None, verbosity=2, **kwargs):
+        try_import_torch()
+        import torch
+        torch.set_num_threads(num_cpus)
+        from .tabular_torch_dataset import TabularTorchDataset
+
         start_time = time.time()
-        try_import_mxnet()
-        import mxnet as mx
-        self.verbosity = kwargs.get('verbosity', 2)
-        global _has_warned_mxnet_deprecation
-        if not _has_warned_mxnet_deprecation:
-            _has_warned_mxnet_deprecation = True
-            logger.log(30, '\tWARNING: TabularNeuralNetMxnetModel (alias "NN" & "NN_MXNET") has been deprecated in v0.4.0.\n'
-                           '\t\tStarting in v0.6.0, calling TabularNeuralNetMxnetModel will raise an exception.\n'
-                           '\t\tConsider instead using TabularNeuralNetTorchModel via "NN_TORCH".')
+
+        params = self._get_model_params()
+
+        processor_kwargs, optimizer_kwargs, fit_kwargs, loss_kwargs, params = self._prepare_params(params=params)
+
+        seed_value = params.pop('seed_value', 0)
+
+        self._num_cpus_infer = params.pop('_num_cpus_infer', 1)
+        if seed_value is not None:  # Set seeds
+            random.seed(seed_value)
+            np.random.seed(seed_value)
+            torch.manual_seed(seed_value)
 
         if sample_weight is not None:  # TODO: support
-            logger.log(15, "sample_weight not yet supported for TabularNeuralNetModel, this model will ignore them in training.")
+            logger.log(15, f"sample_weight not yet supported for {self.__class__.__name__},"
+                           " this model will ignore them in training.")
 
-        params = self._get_model_params()
         if num_cpus is not None:
             self.num_dataloading_workers = max(1, int(num_cpus/2.0))
         else:
             self.num_dataloading_workers = 1
         if self.num_dataloading_workers == 1:
-            self.num_dataloading_workers = 0  # 0 is always faster and uses less memory than 1
-        self.batch_size = params['batch_size']
-        train_dataset, val_dataset = self.generate_datasets(X=X, y=y, params=params, X_val=X_val, y_val=y_val)
-        logger.log(15, "Training data for neural network has: %d examples, %d features (%d vector, %d embedding)" %
-                   (train_dataset.num_examples, train_dataset.num_features, len(train_dataset.feature_groups['vector']), len(train_dataset.feature_groups['embed'])
-                  ))
-        # self._save_preprocessor()  # TODO: should save these things for hyperparam tuning. Need one HP tuner for network-specific HPs, another for preprocessing HPs.
+            self.num_dataloading_workers = 0  # TODO: verify 0 is typically faster and uses less memory than 1 in pytorch
+        self.num_dataloading_workers = 0  # TODO: >0 crashes on MacOS
+        self.max_batch_size = params.pop('max_batch_size', 512)
+        batch_size = params.pop('batch_size', None)
+        if batch_size is None:
+            if isinstance(X, TabularTorchDataset):
+                batch_size = min(int(2 ** (3 + np.floor(np.log10(len(X))))), self.max_batch_size)
+            else:
+                batch_size = min(int(2 ** (3 + np.floor(np.log10(X.shape[0])))), self.max_batch_size)
 
-        if num_gpus is not None and num_gpus >= 1:
-            self.ctx = mx.gpu()  # Currently cannot use more than 1 GPU
-        else:
-            self.ctx = mx.cpu()
-        self.get_net(train_dataset, params=params)
+        train_dataset, val_dataset = self._generate_datasets(X=X, y=y, params=processor_kwargs, X_val=X_val, y_val=y_val)
+        logger.log(15, f"Training data for {self.__class__.__name__} has: "
+                       f"{train_dataset.num_examples} examples, {train_dataset.num_features} features "
+                       f"({len(train_dataset.feature_groups['vector'])} vector, {len(train_dataset.feature_groups['embed'])} embedding)")
+
+        self.device = self._get_device(num_gpus=num_gpus)
+
+        self._get_net(train_dataset, params=params)
+        self.optimizer = self._init_optimizer(**optimizer_kwargs)
 
         if time_limit is not None:
             time_elapsed = time.time() - start_time
             time_limit_orig = time_limit
             time_limit = time_limit - time_elapsed
-            if time_limit <= time_limit_orig * 0.4:  # if 60% of time was spent preprocessing, likely not enough time to train model
-                raise TimeLimitExceeded
 
-        self.train_net(train_dataset=train_dataset, params=params, val_dataset=val_dataset, initialize=True, setup_trainer=True, time_limit=time_limit, reporter=reporter)
-        self.params_post_fit = params
-        """
-        # TODO: if we don't want to save intermediate network parameters, need to do something like saving in temp directory to clean up after training:
-        with make_temp_directory() as temp_dir:
-            save_callback = SaveModelCallback(self.model, monitor=self.metric, mode=save_callback_mode, name=self.name)
-            with progress_disabled_ctx(self.model) as model:
-                original_path = model.path
-                model.path = Path(temp_dir)
-                model.fit_one_cycle(self.epochs, self.lr, callbacks=save_callback)
-
-                # Load the best one and export it
-                model.load(self.name)
-                print(f'Model validation metrics: {model.validate()}')
-                model.path = original_path
-        """
-
-    def get_net(self, train_dataset, params):
-        """ Creates a Gluon neural net and context for this dataset.
-            Also sets up trainer/optimizer as necessary.
-        """
-        from .embednet import EmbedNet
-        self.set_net_defaults(train_dataset, params)
-        self.model = EmbedNet(train_dataset=train_dataset, params=params, num_net_outputs=self.num_net_outputs, ctx=self.ctx)
+            # if 60% of time was spent preprocessing, likely not enough time to train model
+            if time_limit <= time_limit_orig * 0.4:
+                raise TimeLimitExceeded
 
-        # TODO: Below should not occur until at time of saving
+        # train network
+        self._train_net(train_dataset=train_dataset,
+                        loss_kwargs=loss_kwargs,
+                        batch_size=batch_size,
+                        val_dataset=val_dataset,
+                        time_limit=time_limit,
+                        reporter=reporter,
+                        verbosity=verbosity,
+                        **fit_kwargs)
+
+    def _get_net(self, train_dataset, params):
+        from .torch_network_modules import EmbedNet
+
+        # set network params
+        params = self._set_net_defaults(train_dataset, params)
+        self.model = EmbedNet(problem_type=self.problem_type, num_net_outputs=self._get_num_net_outputs(), quantile_levels=self.quantile_levels,
+                              train_dataset=train_dataset, device=self.device, **params)
+        self.model = self.model.to(self.device)
         if not os.path.exists(self.path):
             os.makedirs(self.path)
 
-    def train_net(self, train_dataset, params, val_dataset=None, initialize=True, setup_trainer=True, time_limit=None, reporter=None):
-        """ Trains neural net on given train dataset, early stops based on test_dataset.
-            Args:
-                train_dataset (TabularNNDataset): training data used to learn network weights
-                val_dataset (TabularNNDataset): validation data used for hyperparameter tuning
-                initialize (bool): set = False to continue training of a previously trained model, otherwise initializes network weights randomly
-                setup_trainer (bool): set = False to reuse the same trainer from a previous training run, otherwise creates new trainer from scratch
-        """
+    def _train_net(self,
+                   train_dataset,
+                   loss_kwargs,
+                   batch_size,
+                   num_epochs,
+                   epochs_wo_improve,
+                   val_dataset=None,
+                   time_limit=None,
+                   reporter=None,
+                   verbosity=2):
+        import torch
         start_time = time.time()
-        import mxnet as mx
-        logger.log(15, "Training neural network for up to %s epochs..." % params['num_epochs'])
-        seed_value = params.get('seed_value', 0)
-        if seed_value is not None:  # Set seeds
-            random.seed(seed_value)
-            np.random.seed(seed_value)
-            mx.random.seed(seed_value)
-        if initialize:  # Initialize the weights of network
-            logging.debug("initializing neural network...")
-            self.model.collect_params().initialize(ctx=self.ctx)
-            self.model.hybridize()
-            logging.debug("initialized")
-        if setup_trainer:
-            # Also setup mxboard to monitor training if visualizer has been specified:
-            visualizer = self.params_aux.get('visualizer', 'none')
-            if visualizer == 'tensorboard' or visualizer == 'mxboard':
-                try_import_mxboard()
-                from mxboard import SummaryWriter
-                self.summary_writer = SummaryWriter(logdir=self.path, flush_secs=5, verbose=False)
-            self.optimizer = self.setup_trainer(params=params, train_dataset=train_dataset)
-        best_val_metric = -np.inf  # higher = better
-        val_metric = None
-        best_val_epoch = 0
-        val_improve_epoch = 0  # most recent epoch where validation-score strictly improved
-        num_epochs = params['num_epochs']
+        logging.debug("initializing neural network...")
+        self.model.init_params()
+        logging.debug("initialized")
+        train_dataloader = train_dataset.build_loader(batch_size, self.num_dataloading_workers, is_test=False)
+
+        if isinstance(loss_kwargs.get('loss_function', 'auto'), str) and loss_kwargs.get('loss_function', 'auto') == 'auto':
+            loss_kwargs['loss_function'] = self._get_default_loss_function()
+
         if val_dataset is not None:
             y_val = val_dataset.get_labels()
+            if y_val.ndim == 2 and y_val.shape[1] == 1:
+                y_val = y_val.flatten()
         else:
             y_val = None
 
-        if params['loss_function'] is None:
-            if self.problem_type == REGRESSION:
-                params['loss_function'] = mx.gluon.loss.L1Loss()
-            elif self.problem_type == SOFTCLASS:
-                params['loss_function'] = mx.gluon.loss.SoftmaxCrossEntropyLoss(sparse_label=False, from_logits=self.model.from_logits)
-            else:
-                params['loss_function'] = mx.gluon.loss.SoftmaxCrossEntropyLoss(from_logits=self.model.from_logits)
+        if verbosity <= 1:
+            verbose_eval = False
+        else:
+            verbose_eval = True
 
-        loss_func = params['loss_function']
-        epochs_wo_improve = params['epochs_wo_improve']
-        loss_scaling_factor = 1.0  # we divide loss by this quantity to stabilize gradients
-
-        rescale_losses = {mx.gluon.loss.L1Loss: 'std', mx.gluon.loss.HuberLoss: 'std', mx.gluon.loss.L2Loss: 'var'}  # dict of loss names where we should rescale loss, value indicates how to rescale.
-        loss_torescale = [key for key in rescale_losses if isinstance(loss_func, key)]
-        if loss_torescale:
-            loss_torescale = loss_torescale[0]
-            if rescale_losses[loss_torescale] == 'std':
-                loss_scaling_factor = np.std(train_dataset.get_labels())/5.0 + EPS  # std-dev of labels
-            elif rescale_losses[loss_torescale] == 'var':
-                loss_scaling_factor = np.var(train_dataset.get_labels())/5.0 + EPS  # variance of labels
-            else:
-                raise ValueError("Unknown loss-rescaling type %s specified for loss_func==%s" % (rescale_losses[loss_torescale], loss_func))
+        logger.log(15, "Neural network architecture:")
+        logger.log(15, str(self.model))
 
-        if self.verbosity <= 1:
-            verbose_eval = -1  # Print losses every verbose epochs, Never if -1
-        elif self.verbosity == 2:
-            verbose_eval = 50
-        elif self.verbosity == 3:
-            verbose_eval = 10
-        else:
-            verbose_eval = 1
+        net_filename = os.path.join(self.path, self.temp_file_name)
+        if num_epochs == 0:
+            # use dummy training loop that stops immediately
+            # useful for using NN just for data preprocessing / debugging
+            logger.log(20, "Not training Tabular Neural Network since num_updates == 0")
 
-        net_filename = self.path + self.temp_file_name
-        if num_epochs == 0:  # use dummy training loop that stops immediately (useful for using NN just for data preprocessing / debugging)
-            logger.log(20, "Not training Neural Net since num_epochs == 0.  Neural network architecture is:")
-            for batch_idx, data_batch in enumerate(train_dataset.dataloader):
-                data_batch = train_dataset.format_batch_data(data_batch, self.ctx)
-                with mx.autograd.record():
-                    output = self.model(data_batch)
-                    labels = data_batch['label']
-                    loss = loss_func(output, labels) / loss_scaling_factor
-                    # print(str(mx.nd.mean(loss).asscalar()), end="\r")  # prints per-batch losses
-                loss.backward()
-                self.optimizer.step(labels.shape[0])
+            # for each batch
+            for batch_idx, data_batch in enumerate(train_dataloader):
                 if batch_idx > 0:
                     break
-            self.model.save_parameters(net_filename)
-            logger.log(15, "untrained Neural Net saved to file")
+                loss = self.model.compute_loss(data_batch, **loss_kwargs)
+                self.optimizer.zero_grad()
+                loss.backward()
+                self.optimizer.step()
+
+            os.makedirs(os.path.dirname(self.path), exist_ok=True)
+            torch.save(self.model, net_filename)
+            logger.log(15, "Untrained Tabular Neural Network saved to file")
             return
 
+        # start training loop:
+        logger.log(15, f"Training tabular neural network for up to {num_epochs} epochs...")
+        total_updates = 0
+        num_updates_per_epoch = max(round(len(train_dataset) / batch_size) + 1, 1)
+        update_to_check_time = min(10, max(1, int(num_updates_per_epoch/10)))
+        do_update = True
+        epoch = 0
+        best_epoch = 0
+        best_val_metric = -np.inf  # higher = better
+        best_val_update = 0
+        val_improve_epoch = 0  # most recent epoch where validation-score strictly improved
         start_fit_time = time.time()
         if time_limit is not None:
             time_limit = time_limit - (start_fit_time - start_time)
+            if time_limit <= 0:
+                raise TimeLimitExceeded
+        while do_update:
+            time_start_epoch = time.time()
+            total_train_loss = 0.0
+            total_train_size = 0.0
+            for batch_idx, data_batch in enumerate(train_dataloader):
+                # forward
+                loss = self.model.compute_loss(data_batch, **loss_kwargs)
+                total_train_loss += loss.item()
+                total_train_size += 1
 
-        # Training Loop:
-        for e in range(num_epochs):
-            if e == 0:  # special actions during first epoch:
-                logger.log(15, "Neural network architecture:")
-                logger.log(15, str(self.model))
-            cumulative_loss = 0
-            for batch_idx, data_batch in enumerate(train_dataset.dataloader):
-                data_batch = train_dataset.format_batch_data(data_batch, self.ctx)
-                with mx.autograd.record():
-                    output = self.model(data_batch)
-                    labels = data_batch['label']
-                    loss = loss_func(output, labels) / loss_scaling_factor
-                    # print(str(mx.nd.mean(loss).asscalar()), end="\r")  # prints per-batch losses
+                # update
+                self.optimizer.zero_grad()
                 loss.backward()
-                self.optimizer.step(labels.shape[0])
-                cumulative_loss += loss.sum()
-            train_loss = cumulative_loss/float(train_dataset.num_examples)  # training loss this epoch
+                self.optimizer.step()
+                total_updates += 1
+
+                # time limit
+                if time_limit is not None:
+                    time_cur = time.time()
+                    update_cur = batch_idx + 1
+                    if epoch == 0 and update_cur == update_to_check_time:
+                        time_elapsed_epoch = time_cur - time_start_epoch
+                        estimated_time = time_elapsed_epoch / update_cur * num_updates_per_epoch
+                        if estimated_time > time_limit:
+                            logger.log(30, f"\tNot enough time to train first epoch. "
+                                           f"(Time Required: {round(estimated_time, 2)}s, Time Left: {round(time_limit, 2)}s)")
+                            raise TimeLimitExceeded
+                    time_elapsed = time_cur - start_fit_time
+                    if time_limit < time_elapsed:
+                        logger.log(15, f"\tRan out of time, stopping training early. (Stopped on Update {total_updates} (Epoch {epoch}))")
+                        do_update = False
+                        break
+
+            if not do_update:
+                break
+
+            epoch += 1
+
+            # validation
             if val_dataset is not None:
-                # FIXME: Switch to adaptive ES
-                val_metric = self.score(X=val_dataset, y=y_val, metric=self.stopping_metric)
+                # compute validation score
+                val_metric = self.score(X=val_dataset, y=y_val, metric=self.stopping_metric, _reset_threads=False)
                 if np.isnan(val_metric):
-                    if e == 0:
-                        raise RuntimeError("NaNs encountered in TabularNeuralNetModel training. Features/labels may be improperly formatted or NN weights may have diverged.")
+                    if best_epoch == 0:
+                        raise RuntimeError(f"NaNs encountered in {self.__class__.__name__} training. "
+                                           "Features/labels may be improperly formatted, "
+                                           "or NN weights may have diverged.")
                     else:
-                        logger.warning("Warning: NaNs encountered in TabularNeuralNetModel training. Reverting model to last checkpoint without NaNs.")
+                        logger.warning(f"Warning: NaNs encountered in {self.__class__.__name__} training. "
+                                       "Reverting model to last checkpoint without NaNs.")
                         break
-                if (val_metric >= best_val_metric) or (e == 0):
+
+                # update best validation
+                if (val_metric >= best_val_metric) or best_epoch == 0:
                     if val_metric > best_val_metric:
-                        val_improve_epoch = e
+                        val_improve_epoch = epoch
                     best_val_metric = val_metric
-                    best_val_epoch = e
-                    # Until functionality is added to restart training from a particular epoch, there is no point in saving params without test_dataset
-                    self.model.save_parameters(net_filename)
-            else:
-                best_val_epoch = e
-            if val_dataset is not None:
-                if verbose_eval > 0 and e % verbose_eval == 0:
-                    logger.log(15, "Epoch %s.  Train loss: %s, Val %s: %s" %
-                      (e, train_loss.asscalar(), self.stopping_metric.name, val_metric))
-                if self.summary_writer is not None:
-                    self.summary_writer.add_scalar(tag='val_'+self.stopping_metric.name,
-                                                   value=val_metric, global_step=e)
-            else:
-                if verbose_eval > 0 and e % verbose_eval == 0:
-                    logger.log(15, "Epoch %s.  Train loss: %s" % (e, train_loss.asscalar()))
-            if self.summary_writer is not None:
-                self.summary_writer.add_scalar(tag='train_loss', value=train_loss.asscalar(), global_step=e)  # TODO: do we want to keep mxboard support?
-            if reporter is not None:
-                # TODO: Ensure reporter/scheduler properly handle None/nan values after refactor
-                if val_dataset is not None and (not np.isnan(val_metric)):  # TODO: This might work without the if statement
-                    # epoch must be number of epochs done (starting at 1)
-                    reporter(epoch=e + 1,
+                    os.makedirs(os.path.dirname(self.path), exist_ok=True)
+                    torch.save(self.model, net_filename)
+                    best_epoch = epoch
+                    best_val_update = total_updates
+                if verbose_eval:
+                    logger.log(15, f"Epoch {epoch} (Update {total_updates}).\t"
+                                   f"Train loss: {round(total_train_loss / total_train_size, 4)}, "
+                                   f"Val {self.stopping_metric.name}: {round(val_metric, 4)}, "
+                                   f"Best Epoch: {best_epoch}")
+
+                if reporter is not None:
+                    reporter(epoch=total_updates,
                              validation_performance=val_metric,  # Higher val_metric = better
-                             train_loss=float(train_loss.asscalar()),
+                             train_loss=total_train_loss / total_train_size,
                              eval_metric=self.eval_metric.name,
                              greater_is_better=self.eval_metric.greater_is_better)
-            if e - val_improve_epoch > epochs_wo_improve:
-                break  # early-stop if validation-score hasn't strictly improved in `epochs_wo_improve` consecutive epochs
+
+                # no improvement
+                if epoch - val_improve_epoch >= epochs_wo_improve:
+                    break
+
+            if epoch >= num_epochs:
+                break
+
             if time_limit is not None:
                 time_elapsed = time.time() - start_fit_time
-                time_epoch_average = time_elapsed / (e+1)
+                time_epoch_average = time_elapsed / (epoch+1)
                 time_left = time_limit - time_elapsed
                 if time_left < time_epoch_average:
-                    logger.log(20, f"\tRan out of time, stopping training early. (Stopping on epoch {e})")
+                    logger.log(20, f"\tRan out of time, stopping training early. (Stopping on epoch {epoch})")
                     break
 
+        if epoch == 0:
+            raise AssertionError('0 epochs trained!')
+
+        # revert back to best model
         if val_dataset is not None:
-            self.model.load_parameters(net_filename)  # Revert back to best model
+            logger.log(15, f"Best model found on Epoch {best_epoch} (Update {best_val_update}). Val {self.stopping_metric.name}: {best_val_metric}")
             try:
+                self.model = torch.load(net_filename)
                 os.remove(net_filename)
             except FileNotFoundError:
                 pass
-        if val_dataset is None:
-            logger.log(15, "Best model found in epoch %d" % best_val_epoch)
-        else:  # evaluate one final time:
-            final_val_metric = self.score(X=val_dataset, y=y_val, metric=self.stopping_metric)
-            if np.isnan(final_val_metric):
-                final_val_metric = -np.inf
-            logger.log(15, "Best model found in epoch %d. Val %s: %s" %
-                  (best_val_epoch, self.stopping_metric.name, final_val_metric))
-        self.params_trained['num_epochs'] = best_val_epoch + 1
-        return
+        else:
+            logger.log(15, f"Best model found on Epoch {best_epoch} (Update {best_val_update}).")
+        self.params_trained['batch_size'] = batch_size
+        self.params_trained['num_epochs'] = best_epoch
 
     def _predict_proba(self, X, **kwargs):
         """ To align predict with abstract_model API.
             Preprocess here only refers to feature processing steps done by all AbstractModel objects,
             not tabularNN-specific preprocessing steps.
             If X is not DataFrame but instead TabularNNDataset object, we can still produce predictions,
             but cannot use preprocess in this case (needs to be already processed).
         """
-        from .tabular_nn_dataset import TabularNNDataset
-        if isinstance(X, TabularNNDataset):
-            return self._predict_tabular_data(new_data=X, process=False, predict_proba=True)
+        from .tabular_torch_dataset import TabularTorchDataset
+        if isinstance(X, TabularTorchDataset):
+            return self._predict_tabular_data(new_data=X, process=False)
         elif isinstance(X, pd.DataFrame):
             X = self.preprocess(X, **kwargs)
-            return self._predict_tabular_data(new_data=X, process=True, predict_proba=True)
+            return self._predict_tabular_data(new_data=X, process=True)
         else:
-            raise ValueError("X must be of type pd.DataFrame or TabularNNDataset, not type: %s" % type(X))
+            raise ValueError("X must be of type pd.DataFrame or TabularTorchDataset, not type: %s" % type(X))
 
-    def _predict_tabular_data(self, new_data, process=True, predict_proba=True):  # TODO ensure API lines up with tabular.Model class.
-        """ Specific TabularNN method to produce predictions on new (unprocessed) data.
-            Returns 1D numpy array unless predict_proba=True and task is multi-class classification (not binary).
-            Args:
-                new_data (pd.Dataframe or TabularNNDataset): new data to make predictions on.
-                If you want to make prediction for just a single row of new_data, pass in: new_data.iloc[[row_index]]
-                process (bool): should new data be processed (if False, new_data must be TabularNNDataset)
-                predict_proba (bool): should we output class-probabilities (not used for regression)
-        """
-        from .tabular_nn_dataset import TabularNNDataset
-        import mxnet as mx
+    def _predict_tabular_data(self, new_data, process=True):
+        from .tabular_torch_dataset import TabularTorchDataset
         if process:
-            new_data = self.process_test_data(new_data, batch_size=self.batch_size, num_dataloading_workers=self.num_dataloading_workers_inference, labels=None)
-        if not isinstance(new_data, TabularNNDataset):
-            raise ValueError("new_data must of of type TabularNNDataset if process=False")
-        if self.problem_type == REGRESSION or not predict_proba:
-            preds = mx.nd.zeros((new_data.num_examples,1))
-        else:
-            preds = mx.nd.zeros((new_data.num_examples, self.num_net_outputs))
-        i = 0
-        for batch_idx, data_batch in enumerate(new_data.dataloader):
-            data_batch = new_data.format_batch_data(data_batch, self.ctx)
-            preds_batch = self.model(data_batch)
-            batch_size = len(preds_batch)
-            if self.problem_type != REGRESSION:
-                if not predict_proba: # need to take argmax
-                    preds_batch = mx.nd.argmax(preds_batch, axis=1, keepdims=True)
-                else: # need to take softmax
-                    preds_batch = mx.nd.softmax(preds_batch, axis=1)
-            preds[i:(i+batch_size)] = preds_batch
-            i = i+batch_size
-        if self.problem_type == REGRESSION or not predict_proba:
-            return preds.asnumpy().flatten()  # return 1D numpy array
-        elif self.problem_type == BINARY and predict_proba:
-            return preds[:,1].asnumpy()  # for binary problems, only return P(Y==+1)
+            new_data = self._process_test_data(new_data)
+        if not isinstance(new_data, TabularTorchDataset):
+            raise ValueError("new_data must of of type TabularTorchDataset if process=False")
+        val_dataloader = new_data.build_loader(self.max_batch_size, self.num_dataloading_workers, is_test=True)
+        preds_dataset = []
+        for data_batch in val_dataloader:
+            preds_batch = self.model.predict(data_batch)
+            preds_dataset.append(preds_batch)
+        preds_dataset = np.concatenate(preds_dataset, 0)
+        return preds_dataset
 
-        return preds.asnumpy()  # return 2D numpy array
+    def _generate_datasets(self, X, y, params, X_val=None, y_val=None):
+        from .tabular_torch_dataset import TabularTorchDataset
 
-    def generate_datasets(self, X, y, params, X_val=None, y_val=None):
         impute_strategy = params['proc.impute_strategy']
         max_category_levels = params['proc.max_category_levels']
         skew_threshold = params['proc.skew_threshold']
         embed_min_categories = params['proc.embed_min_categories']
         use_ngram_features = params['use_ngram_features']
 
-        from .tabular_nn_dataset import TabularNNDataset
-        if isinstance(X, TabularNNDataset):
+        if isinstance(X, TabularTorchDataset):
             train_dataset = X
         else:
             X = self.preprocess(X)
-            train_dataset = self.process_train_data(
-                df=X, labels=y, batch_size=self.batch_size, num_dataloading_workers=self.num_dataloading_workers,
-                impute_strategy=impute_strategy, max_category_levels=max_category_levels, skew_threshold=skew_threshold, embed_min_categories=embed_min_categories, use_ngram_features=use_ngram_features,
-            )
+            train_dataset = self._process_train_data(df=X, labels=y,
+                                                     impute_strategy=impute_strategy,
+                                                     max_category_levels=max_category_levels,
+                                                     skew_threshold=skew_threshold,
+                                                     embed_min_categories=embed_min_categories,
+                                                     use_ngram_features=use_ngram_features)
         if X_val is not None:
-            if isinstance(X_val, TabularNNDataset):
+            if isinstance(X_val, TabularTorchDataset):
                 val_dataset = X_val
             else:
                 X_val = self.preprocess(X_val)
-                val_dataset = self.process_test_data(df=X_val, labels=y_val, batch_size=self.batch_size, num_dataloading_workers=self.num_dataloading_workers_inference)
+                val_dataset = self._process_test_data(df=X_val, labels=y_val)
         else:
             val_dataset = None
         return train_dataset, val_dataset
 
-    def process_test_data(self, df, batch_size, num_dataloading_workers, labels=None):
+    def _process_test_data(self, df, labels=None):
         """ Process train or test DataFrame into a form fit for neural network models.
-        Args:
-            df (pd.DataFrame): Data to be processed (X)
-            labels (pd.Series): labels to be processed (y)
-            test (bool): Is this test data where each datapoint should be processed separately using predetermined preprocessing steps.
-                         Otherwise preprocessor uses all data to determine properties like best scaling factors, number of categories, etc.
-        Returns:
-            Dataset object
+            Args:
+                df (pd.DataFrame): Data to be processed (X)
+                labels (pd.Series): labels to be processed (y)
+            Returns:
+                Dataset object
         """
-        from .tabular_nn_dataset import TabularNNDataset
-        warnings.filterwarnings("ignore", module='sklearn.preprocessing') # sklearn processing n_quantiles warning
+        from .tabular_torch_dataset import TabularTorchDataset
+
+        # sklearn processing n_quantiles warning
+        warnings.filterwarnings("ignore", module='sklearn.preprocessing')
         if labels is not None and len(labels) != len(df):
             raise ValueError("Number of examples in Dataframe does not match number of labels")
         if (self.processor is None or self._types_of_features is None
            or self.feature_arraycol_map is None or self.feature_type_map is None):
             raise ValueError("Need to process training data before test data")
         if self.features_to_drop:
             drop_cols = [col for col in df.columns if col in self.features_to_drop]
             if drop_cols:
                 df = df.drop(columns=drop_cols)
 
-        df = self.processor.transform(df) # 2D numpy array. self.feature_arraycol_map, self.feature_type_map have been previously set while processing training data.
-        return TabularNNDataset(df, self.feature_arraycol_map, self.feature_type_map,
-                                batch_size=batch_size, num_dataloading_workers=num_dataloading_workers,
-                                problem_type=self.problem_type, labels=labels, is_test=True)
-
-    def process_train_data(self, df, batch_size, num_dataloading_workers, impute_strategy, max_category_levels, skew_threshold, embed_min_categories, use_ngram_features, labels):
-        """ Preprocess training data and create self.processor object that can be used to process future data.
-            This method should only be used once per TabularNeuralNetModel object, otherwise will produce Warning.
-
-        # TODO no label processing for now
-        # TODO: add time/ngram features
-        # TODO: no filtering of data-frame columns based on statistics, e.g. categorical columns with all unique variables or zero-variance features.
-                This should be done in default_learner class for all models not just TabularNeuralNetModel...
-        """
-        from .tabular_nn_dataset import TabularNNDataset
-        warnings.filterwarnings("ignore", module='sklearn.preprocessing')  # sklearn processing n_quantiles warning
+        # self.feature_arraycol_map, self.feature_type_map have been previously set while processing training data.
+        df = self.processor.transform(df)
+        return TabularTorchDataset(df, self.feature_arraycol_map, self.feature_type_map, self.problem_type, labels)
+
+    def _process_train_data(self, df, impute_strategy, max_category_levels, skew_threshold,
+                            embed_min_categories, use_ngram_features, labels):
+        from .tabular_torch_dataset import TabularTorchDataset
+
+        # sklearn processing n_quantiles warning
+        warnings.filterwarnings("ignore", module='sklearn.preprocessing')
         if labels is None:
             raise ValueError("Attempting process training data without labels")
         if len(labels) != len(df):
             raise ValueError("Number of examples in Dataframe does not match number of labels")
 
-        self._types_of_features, df = self._get_types_of_features(df, skew_threshold=skew_threshold, embed_min_categories=embed_min_categories, use_ngram_features=use_ngram_features)  # dict with keys: : 'continuous', 'skewed', 'onehot', 'embed', values = column-names of df
+        # dict with keys: : 'continuous', 'skewed', 'onehot', 'embed', values = column-names of df
+        self._types_of_features, df = self._get_types_of_features(df, skew_threshold=skew_threshold,
+                                                                  embed_min_categories=embed_min_categories,
+                                                                  use_ngram_features=use_ngram_features)
         logger.log(15, "Tabular Neural Network treats features as the following types:")
         logger.log(15, json.dumps(self._types_of_features, indent=4))
         logger.log(15, "\n")
         if self.processor is not None:
-            Warning("Attempting to process training data for TabularNeuralNetModel, but previously already did this.")
-        self.processor = create_preprocessor(impute_strategy=impute_strategy, max_category_levels=max_category_levels, unique_category_str=self.unique_category_str, continuous_features=self._types_of_features['continuous'],
-                                   skewed_features=self._types_of_features['skewed'], onehot_features=self._types_of_features['onehot'], embed_features=self._types_of_features['embed'], bool_features=self._types_of_features['bool'])
-        df = self.processor.fit_transform(df) # 2D numpy array
-        self.feature_arraycol_map = get_feature_arraycol_map(processor=self.processor, max_category_levels=max_category_levels)  # OrderedDict of feature-name -> list of column-indices in df corresponding to this feature
+            Warning(f"Attempting to process training data for {self.__class__.__name__}, but previously already did this.")
+        self.processor = create_preprocessor(
+            impute_strategy=impute_strategy,
+            max_category_levels=max_category_levels,
+            unique_category_str=self.unique_category_str,
+            continuous_features=self._types_of_features['continuous'],
+            skewed_features=self._types_of_features['skewed'],
+            onehot_features=self._types_of_features['onehot'],
+            embed_features=self._types_of_features['embed'],
+            bool_features=self._types_of_features['bool']
+        )
+        df = self.processor.fit_transform(df)
+        # OrderedDict of feature-name -> list of column-indices in df corresponding to this feature
+        self.feature_arraycol_map = get_feature_arraycol_map(processor=self.processor, max_category_levels=max_category_levels)
         num_array_cols = np.sum([len(self.feature_arraycol_map[key]) for key in self.feature_arraycol_map])  # should match number of columns in processed array
         if num_array_cols != df.shape[1]:
-            raise ValueError("Error during one-hot encoding data processing for neural network. Number of columns in df array does not match feature_arraycol_map.")
+            raise ValueError("Error during one-hot encoding data processing for neural network. "
+                             "Number of columns in df array does not match feature_arraycol_map.")
 
-        self.feature_type_map = get_feature_type_map(feature_arraycol_map=self.feature_arraycol_map, types_of_features=self._types_of_features)  # OrderedDict of feature-name -> feature_type string (options: 'vector', 'embed')
-        return TabularNNDataset(df, self.feature_arraycol_map, self.feature_type_map,
-                                batch_size=batch_size, num_dataloading_workers=num_dataloading_workers,
-                                problem_type=self.problem_type, labels=labels, is_test=False)
-
-    def setup_trainer(self, params, train_dataset=None):
-        """ Set up optimizer needed for training.
-            Network must first be initialized before this.
-        """
-        import mxnet as mx
-        optimizer_opts = {'learning_rate': params['learning_rate'], 'wd': params['weight_decay'], 'clip_gradient': params['clip_gradient']}
-        if 'lr_scheduler' in params and params['lr_scheduler'] is not None:
-            if train_dataset is None:
-                raise ValueError("train_dataset cannot be None when lr_scheduler is specified.")
-            base_lr = params.get('base_lr', 1e-6)
-            target_lr = params.get('target_lr', 1.0)
-            warmup_epochs = params.get('warmup_epochs', 10)
-            lr_decay = params.get('lr_decay', 0.1)
-            lr_mode = params['lr_scheduler']
-            num_batches = train_dataset.num_examples // params['batch_size']
-            lr_decay_epoch = [max(warmup_epochs, int(params['num_epochs']/3)), max(warmup_epochs+1, int(params['num_epochs']/2)),
-                              max(warmup_epochs+2, int(2*params['num_epochs']/3))]
-            from .lr_scheduler import LRSequential, LRScheduler
-            lr_scheduler = LRSequential([
-                LRScheduler('linear', base_lr=base_lr, target_lr=target_lr, nepochs=warmup_epochs, iters_per_epoch=num_batches),
-                LRScheduler(lr_mode, base_lr=target_lr, target_lr=base_lr, nepochs=params['num_epochs'] - warmup_epochs,
-                            iters_per_epoch=num_batches, step_epoch=lr_decay_epoch, step_factor=lr_decay, power=2)
-            ])
-            optimizer_opts['lr_scheduler'] = lr_scheduler
-        if params['optimizer'] == 'sgd':
-            if 'momentum' in params:
-                optimizer_opts['momentum'] = params['momentum']
-            optimizer = mx.gluon.Trainer(self.model.collect_params(), 'sgd', optimizer_opts)
-        elif params['optimizer'] == 'adam':  # TODO: Can we try AdamW?
-            optimizer = mx.gluon.Trainer(self.model.collect_params(), 'adam', optimizer_opts)
+        # OrderedDict of feature-name -> feature_type string (options: 'vector', 'embed')
+        self.feature_type_map = get_feature_type_map(feature_arraycol_map=self.feature_arraycol_map, types_of_features=self._types_of_features)
+        return TabularTorchDataset(df, self.feature_arraycol_map, self.feature_type_map, self.problem_type, labels)
+
+    def _init_optimizer(self, optimizer, learning_rate, weight_decay):
+        """
+        Set up optimizer needed for training.
+        Network must first be initialized before this.
+        """
+        import torch
+
+        if optimizer == 'sgd':
+            optimizer = torch.optim.SGD(params=self.model.parameters(),
+                                        lr=learning_rate,
+                                        weight_decay=weight_decay)
+        elif optimizer == 'adam':
+            optimizer = torch.optim.Adam(params=self.model.parameters(),
+                                         lr=learning_rate,
+                                         weight_decay=weight_decay)
         else:
-            raise ValueError("Unknown optimizer specified: %s" % params['optimizer'])
+            raise ValueError(f"Unknown optimizer specified: {optimizer}")
         return optimizer
 
-    def get_info(self):
-        info = super().get_info()
-        info['hyperparameters_post_fit'] = self.params_post_fit
-        return info
-
     def reduce_memory_size(self, remove_fit=True, requires_save=True, **kwargs):
         super().reduce_memory_size(remove_fit=remove_fit, requires_save=requires_save, **kwargs)
         if remove_fit and requires_save:
             self.optimizer = None
 
     def _get_default_stopping_metric(self):
         return self.eval_metric
+    
+    def _get_maximum_resources(self) -> Dict[str, Union[int, float]]:
+        # torch model trains slower when utilizing virtual cores and this issue scale up when the number of cpu cores increases
+        return {
+            "num_cpus": ResourceManager.get_cpu_count_psutil(logical=False)
+        }
+
+    def _get_default_resources(self):
+        # logical=False is faster in training
+        num_cpus = ResourceManager.get_cpu_count_psutil(logical=False)
+        num_gpus = 0
+        return num_cpus, num_gpus
 
     def save(self, path: str = None, verbose=True) -> str:
+        import torch
+        # Save on CPU to ensure the model can be loaded on a box without GPU
         if self.model is not None:
-            self._architecture_desc = self.model.architecture_desc
-        temp_model = self.model
-        temp_sw = self.summary_writer
-        self.model = None
-        self.summary_writer = None
-        path_final = super().save(path=path, verbose=verbose)
-        self.model = temp_model
-        self.summary_writer = temp_sw
-        self._architecture_desc = None
-
-        # Export model
+            self.model = self.model.to(torch.device("cpu"))
+        path = super().save(path, verbose)
+        # Put the model back to the device after the save
         if self.model is not None:
-            params_filepath = path_final + self.params_file_name
-            # TODO: Don't use os.makedirs here, have save_parameters function in tabular_nn_model that checks if local path or S3 path
-            os.makedirs(os.path.dirname(path_final), exist_ok=True)
-            self.model.save_parameters(params_filepath)
-        return path_final
+            self.model.to(self.device)
+        return path
 
     @classmethod
     def load(cls, path: str, reset_paths=True, verbose=True):
-        model: TabularNeuralNetMxnetModel = super().load(path=path, reset_paths=reset_paths, verbose=verbose)
-        if model._architecture_desc is not None:
-            from .embednet import EmbedNet
-            model.model = EmbedNet(architecture_desc=model._architecture_desc, ctx=model.ctx)  # recreate network from architecture description
-            model._architecture_desc = None
-            # TODO: maybe need to initialize/hybridize?
-            model.model.load_parameters(model.path + model.params_file_name, ctx=model.ctx)
-            model.summary_writer = None
-        return model
-
-    def _more_tags(self):
-        # `can_refit_full=True` because num_epochs is communicated at end of `_fit`: `self.params_trained['num_epochs'] = best_val_epoch + 1`
-        return {'can_refit_full': True}
-
-
+        """
+        Loads the model from disk to memory.
+        The loaded model will be on the same device it was trained on (cuda/mps);
+        if the device is it's not available (trained on GPU, deployed on CPU),
+        then `cpu` will be used.
 
-""" General TODOs:
+        Parameters
+        ----------
+        path : str
+            Path to the saved model, minus the file name.
+            This should generally be a directory path ending with a '/' character (or appropriate path separator value depending on OS).
+            The model file is typically located in path + cls.model_file_name.
+        reset_paths : bool, default True
+            Whether to reset the self.path value of the loaded model to be equal to path.
+            It is highly recommended to keep this value as True unless accessing the original self.path value is important.
+            If False, the actual valid path and self.path may differ, leading to strange behaviour and potential exceptions if the model needs to load any other files at a later time.
+        verbose : bool, default True
+            Whether to log the location of the loaded file.
+
+        Returns
+        -------
+        model : cls
+            Loaded model object.
+        """
+        import torch
+
+        model: TabularNeuralNetTorchModel = super().load(path=path, reset_paths=reset_paths, verbose=verbose)
+
+        # Put the model on the same device it was train on (GPU/MPS) if it is available; otherwise use CPU
+        if model.model is not None:
+            original_device_type = model.device.type
+            if 'cuda' in original_device_type:
+                # cuda: nvidia GPU
+                device = torch.device(original_device_type if torch.cuda.is_available() else 'cpu')
+            elif 'mps' in original_device_type:
+                # mps: Apple Silicon
+                device = torch.device(original_device_type if torch.backends.mps.is_available() else 'cpu')
+            else:
+                device = torch.device(original_device_type)
 
-- Automatically decrease batch-size if memory issue arises
+            if verbose and (original_device_type != device.type):
+                logger.log(15, f'Model is trained on {original_device_type}, but the device is not available - loading on {device.type}')
 
-- Retrain final NN on full dataset (train+val). How to ensure stability here?
-- OrdinalEncoder class in sklearn currently cannot handle rare categories or unknown ones at test-time, so we have created our own Encoder in category_encoders.py
-There is open PR in sklearn to address this: https://github.com/scikit-learn/scikit-learn/pull/13833/files
-Currently, our code uses category_encoders package (BSD license) instead: https://github.com/scikit-learn-contrib/categorical-encoding
-Once PR is merged into sklearn, may want to switch: category_encoders.Ordinal -> sklearn.preprocessing.OrdinalEncoder in preprocess_train_data()
+            model.device = device
+            model.model = model.model.to(model.device)
+            model.model.device = model.device
+
+        # Compiled models handling
+        if hasattr(model, '_compiler') and model._compiler and model._compiler.name != 'native':
+            model.model.eval()
+            model.processor = model._compiler.load(path=model.path)
+        return model
+    
+    def _get_hpo_backend(self):
+        """Choose which backend(Ray or Custom) to use for hpo"""
+        return RAY_BACKEND
+
+    def get_minimum_resources(self, is_gpu_available=False):
+        minimum_resources = {
+            'num_cpus': 1,
+        }
+        if is_gpu_available:
+            # Our custom implementation does not support partial GPU. No gpu usage according to nvidia-smi when the `num_gpus` passed to fit is fractional`
+            minimum_resources['num_gpus'] = 1
+        return minimum_resources
 
-- Save preprocessed data so that we can do HPO of neural net hyperparameters more efficiently, while also doing HPO of preprocessing hyperparameters?
-      Naive full HPO method requires redoing preprocessing in each trial even if we did not change preprocessing hyperparameters.
-      Alternative is we save each preprocessed dataset & corresponding TabularNeuralNetModel object with its unique param names in the file. Then when we try a new HP-config, we first try loading from file if one exists.
+    def _more_tags(self):
+        # `can_refit_full=True` because batch_size and num_epochs is communicated at end of `_fit`:
+        #  self.params_trained['batch_size'] = batch_size
+        #  self.params_trained['num_epochs'] = best_epoch
+        return {'can_refit_full': True}
 
-"""
+    def _valid_compilers(self):
+        return [TabularNeuralNetTorchNativeCompiler,
+                TabularNeuralNetTorchOnnxCompiler]
+
+    def _default_compiler(self):
+        return TabularNeuralNetTorchNativeCompiler
+
+    def _get_input_types(self, batch_size=None):
+        input_types = []
+        for f in self._features:
+            input_types.append((f, [batch_size, 1]))
+        return input_types
+
+    def compile(self, compiler_configs=None):
+        """
+        Compile the trained model for faster inference.
+
+        This completely overrides the compile() in AbstractModel, since we won't
+        overwrite self.model in the compilation process.
+        Instead, self.processor would be converted from sklearn ColumnTransformer
+        to its alternative counterpart.
+        """
+        assert self.is_fit(), "The model must be fit before calling the compile method."
+        if compiler_configs is None:
+            compiler_configs = {}
+        # Take self.max_batch_size as default batch size, instead of None in AbstractModel
+        batch_size = compiler_configs.get("batch_size", self.max_batch_size)
+        compiler_configs.update(batch_size=batch_size)
+        super().compile(compiler_configs)
+
+    def _compile(self, **kwargs):
+        """
+        Take the compiler to perform actual compilation.
+
+        This overrides the _compile() in AbstractModel, since we won't
+        overwrite self.model in the compilation process.
+        Instead, self.processor would be converted from sklearn ColumnTransformer
+        to TabularNeuralNetTorchOnnxTransformer.
+        """
+        from sklearn.compose._column_transformer import ColumnTransformer
+
+        input_types = kwargs.get('input_types', self._get_input_types(batch_size=self.max_batch_size))
+        assert isinstance(self.processor, ColumnTransformer), f"unexpected processor type {type(self.processor)}, " \
+            "expecting processor type to be sklearn.compose._column_transformer.ColumnTransformer"
+        self.processor = self._compiler.compile(model=(self.processor, self.model),
+                                                path=self.path,
+                                                input_types=input_types)
```

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/predictor/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from autogluon.common.utils.file_utils import get_directory_size, get_directory_size_per_file
 from autogluon.common.utils.log_utils import set_logger_verbosity
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.utils import setup_outputdir, get_autogluon_metadata, compare_autogluon_metadata, check_saved_predictor_version
 from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE, AUTO_WEIGHT, BALANCE_WEIGHT, PSEUDO_MODEL_SUFFIX, PROBLEM_TYPES_CLASSIFICATION
 from autogluon.core.data.label_cleaner import LabelCleanerMulticlassToBinary
 from autogluon.core.dataset import TabularDataset
+from autogluon.core.problem_type import problem_type_info
 from autogluon.core.pseudolabeling.pseudolabeling import filter_pseudo, filter_ensemble_pseudo
 from autogluon.core.scheduler.scheduler_factory import scheduler_factory
 from autogluon.core.trainer import AbstractTrainer
 from autogluon.core.utils import get_pred_from_proba_df
 from autogluon.core.utils import plot_performance_vs_trials, plot_summary_of_models, plot_tabular_models
 from autogluon.core.utils.decorators import apply_presets
 from autogluon.core.utils.loaders import load_pkl, load_str
@@ -384,15 +385,15 @@
             Determines the hyperparameters used by the models.
             If `str` is passed, will use a preset hyperparameter configuration.
                 Valid `str` options: ['default', 'light', 'very_light', 'toy', 'multimodal']
                     'default': Default AutoGluon hyperparameters intended to maximize accuracy without significant regard to inference time or disk usage.
                     'light': Results in smaller models. Generally will make inference speed much faster and disk usage much lower, but with worse accuracy.
                     'very_light': Results in much smaller models. Behaves similarly to 'light', but in many cases with over 10x less disk usage and a further reduction in accuracy.
                     'toy': Results in extremely small models. Only use this when prototyping, as the model quality will be severely reduced.
-                    'multimodal': [EXPERIMENTAL] Trains a multimodal transformer model alongside tabular models. Requires that some text columns appear in the data, a GPU, and CUDA-enabled MXNet.
+                    'multimodal': [EXPERIMENTAL] Trains a multimodal transformer model alongside tabular models. Requires that some text columns appear in the data and GPU.
                         When combined with 'best_quality' `presets` option, this can achieve extremely strong results in multimodal data tables that contain columns with text in addition to numeric/categorical columns.
                 Reference `autogluon/tabular/configs/hyperparameter_configs.py` for information on the hyperparameters associated with each preset.
             Keys are strings that indicate which model types to train.
                 Stable model options include:
                     'GBM' (LightGBM)
                     'CAT' (CatBoost)
                     'XGB' (XGBoost)
@@ -1153,15 +1154,15 @@
         -----------
         unlabeled_data: Extra unlabeled data (could be the test data) to assign pseudolabels to
             and incorporate as extra training data.
         max_iter: int, default = 5
             Maximum allowed number of iterations, where in each iteration, the data are pseudolabeled
             by the current predictor and the predictor is refit including the pseudolabled data in its training set.
         return_pred_proba: bool, default = False
-            Transductive learning setting, will return predictive probabiliteis of unlabeled_data
+            Transductive learning setting, will return predictive probabilities of unlabeled_data
         use_ensemble: bool, default = False
             If True will use ensemble pseudo labeling algorithm if False will use best model
             pseudo labeling method
         fit_ensemble: bool, default = False
             If True will fit weighted ensemble on final best models. Fitting weighted ensemble will be done after fitting
             of models is completed unless otherwise specified. If False will not fit weighted ensemble on final best
             models.
@@ -1195,16 +1196,20 @@
                 if self.problem_type in PROBLEM_TYPES_CLASSIFICATION:
                     test_pseudo_idxes_true, y_pred_proba, y_pred = filter_ensemble_pseudo(predictor=self,
                                                                                           unlabeled_data=X_test)
                 else:
                     test_pseudo_idxes_true, y_pred = filter_ensemble_pseudo(predictor=self, unlabeled_data=X_test)
                     y_pred_proba = y_pred.copy()
             else:
-                y_pred_proba = self.predict_proba(data=X_test, as_multiclass=True)
-                y_pred = get_pred_from_proba_df(y_pred_proba, problem_type=self.problem_type)
+                if self.can_predict_proba:
+                    y_pred_proba = self.predict_proba(data=X_test, as_multiclass=True)
+                    y_pred = get_pred_from_proba_df(y_pred_proba, problem_type=self.problem_type)
+                else:
+                    y_pred = self.predict(data=X_test)
+                    y_pred_proba = y_pred
                 test_pseudo_idxes_true = filter_pseudo(y_pred_proba_og=y_pred_proba, problem_type=self.problem_type)
 
             if return_pred_prob:
                 if i == 0:
                     y_pred_proba_og = y_pred_proba
                 else:
                     y_pred_proba_og.loc[test_pseudo_idxes_true.index] = y_pred_proba.loc[test_pseudo_idxes_true.index]
@@ -1241,15 +1246,18 @@
             else:
                 # Cut down X_test to not include pseudo labeled data
                 X_test = X_test.loc[test_pseudo_idxes[~test_pseudo_idxes].index]
                 previous_score = current_score
 
         if fit_ensemble and not fit_ensemble_every_iter:
             self._fit_weighted_ensemble_pseudo()
-            y_pred_proba_og = self.predict_proba(unlabeled_data)
+            if self.can_predict_proba:
+                y_pred_proba_og = self.predict_proba(unlabeled_data)
+            else:
+                y_pred_proba_og = self.predict(unlabeled_data)
 
         if return_pred_prob:
             return self, y_pred_proba_og
         else:
             return self
 
     def fit_pseudolabel(self, pseudo_data: pd.DataFrame, max_iter: int = 5, return_pred_prob: bool = False,
@@ -1334,15 +1342,15 @@
                            **fit_extra_kwargs)
 
             if fit_ensemble:
                 logger.log(15, 'Fitting weighted ensemble model using best models')
                 self.fit_weighted_ensemble()
 
             if return_pred_prob:
-                y_pred_proba = self.predict_proba(pseudo_data)
+                y_pred_proba = self.predict_proba(pseudo_data) if self.can_predict_proba else self.predict(pseudo_data)
                 return self, y_pred_proba
             else:
                 return self
         else:
             logger.log(20, 'Given test_data for pseudo labeling did not contain labels. '
                            'AutoGluon will assign pseudo labels to data and use it for extra training data...')
             return self._run_pseudolabeling(unlabeled_data=pseudo_data, max_iter=max_iter,
@@ -1374,19 +1382,18 @@
         -------
         Array of predictions, one corresponding to each row in given dataset. Either :class:`np.ndarray` or :class:`pd.Series` depending on `as_pandas` argument.
         """
         self._assert_is_fit('predict')
         data = self.__get_dataset(data)
         return self._learner.predict(X=data, model=model, as_pandas=as_pandas, transform_features=transform_features)
 
-    # TODO: v0.8: Error if called with self.problem_type='regression' or 'quantile'
     def predict_proba(self, data, model=None, as_pandas=True, as_multiclass=True, transform_features=True):
         """
         Use trained models to produce predicted class probabilities rather than class-labels (if task is classification).
-        If `predictor.problem_type` is regression, this functions identically to `predict`, returning the same output.
+        If `predictor.problem_type` is regression or quantile, this will raise an AssertionError.
 
         Parameters
         ----------
         data : str or :class:`TabularDataset` or :class:`pd.DataFrame`
             The data to make predictions for. Should contain same column names as training dataset and follow same format
             (may contain extra columns that won't be used by Predictor, including the label-column itself).
             If str is passed, `data` will be loaded using the str value as the file path.
@@ -1411,42 +1418,29 @@
         Returns
         -------
         Array of predicted class-probabilities, corresponding to each row in the given data.
         May be a :class:`np.ndarray` or :class:`pd.DataFrame` / :class:`pd.Series` depending on `as_pandas` and `as_multiclass` arguments and the type of prediction problem.
         For binary classification problems, the output contains for each datapoint the predicted probabilities of the negative and positive classes, unless you specify `as_multiclass=False`.
         """
         self._assert_is_fit('predict_proba')
-        data = self.__get_dataset(data)
         if not self.can_predict_proba:
-            warnings.warn(
-                f'Calling `predictor.predict_proba` when problem_type={self.problem_type} will raise an AssertionError starting in AutoGluon v0.8. '
-                'Please call `predictor.predict` instead. You can check the value of `predictor.can_predict_proba` to tell if predict_proba is valid.',
-                category=FutureWarning
-            )
+            raise AssertionError(f'`predictor.predict_proba` is not supported when problem_type="{self.problem_type}". '
+                                 f'Please call `predictor.predict` instead. '
+                                 f'You can check the value of `predictor.can_predict_proba` to tell if predict_proba is valid.')
+        data = self.__get_dataset(data)
         return self._learner.predict_proba(X=data, model=model, as_pandas=as_pandas, as_multiclass=as_multiclass, transform_features=transform_features)
 
-    # TODO: Ensure this is correct as new problem_types are added.
-    #  Consider making problem_type a class object to be able to look this up easier.
-    @property
-    def _is_classification(self) -> bool:
-        """
-        Return True if problem_type is classification, otherwise return False.
-        Raises an AssertionError if `self.problem_type` is None.
-        """
-        assert self.problem_type is not None, "problem_type cannot be None when determining if the predictor is solving a classification problem"
-        return self.problem_type not in [REGRESSION, QUANTILE]
-
     @property
     def can_predict_proba(self) -> bool:
         """
         Return True if predictor can return prediction probabilities via `.predict_proba`, otherwise return False.
         Raises an AssertionError if called before fitting.
         """
         self._assert_is_fit('can_predict_proba')
-        return self._is_classification
+        return problem_type_info.can_predict_proba(problem_type=self.problem_type)
 
     def evaluate(self, data, model=None, silent=False, auxiliary_metrics=True, detailed_report=False) -> dict:
         """
         Report the predictive performance evaluated over a given dataset.
         This is basically a shortcut for: `pred_proba = predict_proba(data); evaluate_predictions(data[label], pred_proba)`.
 
         Parameters
@@ -1700,14 +1694,18 @@
             If False (advanced), will return prediction probabilities in AutoGluon's internal format.
 
         Returns
         -------
         Dictionary with model names as keys and model prediction probabilities as values.
         """
         self._assert_is_fit('predict_proba_multi')
+        if not self.can_predict_proba:
+            raise AssertionError(f'`predictor.predict_proba_multi` is not supported when problem_type="{self.problem_type}". '
+                                 f'Please call `predictor.predict_multi` instead. '
+                                 f'You can check the value of `predictor.can_predict_proba` to tell if predict_proba_multi is valid.')
         data = self.__get_dataset(data, allow_nan=True)
         return self._learner.predict_proba_multi(X=data,
                                                  models=models,
                                                  as_pandas=as_pandas,
                                                  as_multiclass=as_multiclass,
                                                  transform_features=transform_features,
                                                  inverse_transform=inverse_transform)
@@ -2855,15 +2853,15 @@
         time_limit : int, default = None
             Approximately how long (in seconds) the distillation process should run for.
             If None, no time-constraint will be enforced allowing the distilled models to fully train.
         hyperparameters : dict or str, default = None
             Specifies which models to use as students and what hyperparameter-values to use for them.
             Same as `hyperparameters` argument of `fit()`.
             If = None, then student models will use the same hyperparameters from `fit()` used to produce this Predictor.
-            Note: distillation is currently only supported for ['GBM','NN_MXNET','NN_TORCH','RF','CAT'] student models, other models and their hyperparameters are ignored here.
+            Note: distillation is currently only supported for ['GBM','NN_TORCH','RF','CAT'] student models, other models and their hyperparameters are ignored here.
         holdout_frac : float
             Same as `holdout_frac` argument of :meth:`TabularPredictor.fit`.
         teacher_preds : str, default = 'soft'
             What form of teacher predictions to distill from (teacher refers to the most accurate AutoGluon ensemble-predictor).
             If None, we only train with original labels (no data augmentation).
             If 'hard', labels are hard teacher predictions given by: `teacher.predict()`
             If 'soft', labels are soft teacher predictions given by: `teacher.predict_proba()`
```

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from autogluon.core.constants import AG_ARGS, AG_ARGS_FIT, AG_ARGS_ENSEMBLE, BINARY, MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE
 from autogluon.core.models import AbstractModel, GreedyWeightedEnsembleModel, StackerEnsembleModel, SimpleWeightedEnsembleModel, DummyModel
 from autogluon.core.trainer.utils import process_hyperparameters
 
 from .presets_custom import get_preset_custom
 from ...models import LGBModel, CatBoostModel, XGBoostModel, RFModel, XTModel, KNNModel, LinearModel,\
-    TabularNeuralNetMxnetModel, TabularNeuralNetTorchModel, NNFastAiTabularModel, FastTextModel, TextPredictorModel, \
+    TabularNeuralNetTorchModel, NNFastAiTabularModel, FastTextModel, TextPredictorModel, \
     ImagePredictorModel, VowpalWabbitModel, \
     RuleFitModel, GreedyTreeModel, HSTreeModel, FigsModel, BoostedRulesModel, MultiModalPredictorModel, FTTransformerModel
 from ...models.tab_transformer.tab_transformer_model import TabTransformerModel
 
 logger = logging.getLogger(__name__)
 
 # Higher values indicate higher priority, priority dictates the order models are trained for a given level.
@@ -23,15 +23,14 @@
     RF=80,
     CAT=70,
     XT=60,
     FASTAI=50,
     XGB=40,
     LR=30,
     NN_TORCH=25,
-    NN_MXNET=20,
     VW=10,
     FASTTEXT=0,
     AG_TEXT_NN=0,
     AG_IMAGE_NN=0,
     AG_AUTOMM=0,
     TRANSF=0,
     custom=0,
@@ -49,15 +48,14 @@
     MULTICLASS: dict(
         FASTAI=95,
     ),
 }
 
 DEFAULT_SOFTCLASS_PRIORITY = dict(
     GBM=100,
-    NN_MXNET=90,
     RF=80,
     CAT=60,
     custom=0,
 )
 
 DEFAULT_CUSTOM_MODEL_PRIORITY = 0
 
@@ -67,15 +65,14 @@
 MODEL_TYPES = dict(
     RF=RFModel,
     XT=XTModel,
     KNN=KNNModel,
     GBM=LGBModel,
     CAT=CatBoostModel,
     XGB=XGBoostModel,
-    NN_MXNET=TabularNeuralNetMxnetModel,
     NN_TORCH=TabularNeuralNetTorchModel,
     LR=LinearModel,
     FASTAI=NNFastAiTabularModel,
     TRANSF=TabTransformerModel,
     AG_TEXT_NN=TextPredictorModel,
     AG_IMAGE_NN=ImagePredictorModel,
     AG_AUTOMM=MultiModalPredictorModel,
@@ -99,15 +96,14 @@
 DEFAULT_MODEL_NAMES = {
     RFModel: 'RandomForest',
     XTModel: 'ExtraTrees',
     KNNModel: 'KNeighbors',
     LGBModel: 'LightGBM',
     CatBoostModel: 'CatBoost',
     XGBoostModel: 'XGBoost',
-    TabularNeuralNetMxnetModel: 'NeuralNetMXNet',
     TabularNeuralNetTorchModel: 'NeuralNetTorch',
     LinearModel: 'LinearModel',
     NNFastAiTabularModel: 'NeuralNetFastAI',
     TabTransformerModel: 'Transformer',
     TextPredictorModel: 'TextPredictor',
     ImagePredictorModel: 'ImagePredictor',
     MultiModalPredictorModel: 'MultiModalPredictor',
@@ -183,34 +179,19 @@
 
     level_key = level if level in hyperparameters.keys() else 'default'
     if level_key not in hyperparameters.keys() and level_key == 'default':
         hyperparameters = {'default': hyperparameters}
     hp_level = hyperparameters[level_key]
     model_cfg_priority_dict = defaultdict(list)
     model_type_list = list(hp_level.keys())
-    if 'NN' in model_type_list:
-        # TODO: Remove in v0.7.0
-        logger.log(30, '\tWARNING: "NN" model has been deprecated in v0.4.0 and renamed to "NN_MXNET". '
-                       'Starting in v0.6.0, specifying "NN" or "NN_MXNET" will raise an exception. Consider instead specifying "NN_TORCH".')
     for model_type in model_type_list:
-        if problem_type == QUANTILE:
-            if model_type not in DEFAULT_QUANTILE_MODEL:
-                if model_type == 'NN_MXNET' and 'NN_TORCH' in DEFAULT_QUANTILE_MODEL and 'NN_TORCH' not in model_type_list:
-                    model_type = 'NN_TORCH'
-                    hp_level['NN_TORCH'] = hp_level.pop('NN_MXNET')
-                    logger.log(15, "Quantile regression must use NN_TORCH instead of NN_MXNET, switching NN_MXET -> NN_TORCH.")
-                else:
-                    continue
         models_of_type = hp_level[model_type]
         if not isinstance(models_of_type, list):
             models_of_type = [models_of_type]
         model_cfgs_to_process = []
-        if model_type == 'NN':
-            # TODO: Remove in v0.6.0
-            model_type = 'NN_MXNET'
         for model_cfg in models_of_type:
             if model_type in invalid_type_set:
                 logger.log(20, f"\tFound '{model_type}' model in hyperparameters, but '{model_type}' is present in `excluded_model_types` and will be removed.")
                 continue  # Don't include excluded models
             if isinstance(model_cfg, str):
                 if model_type == 'AG_TEXT_NN' or model_type == 'AG_AUTOMM':
                     model_cfgs_to_process.append({})
@@ -373,17 +354,16 @@
         model_init = model_type(**model_init_kwargs)
 
     return model_init
 
 
 # TODO: v0.1 cleanup and avoid hardcoded logic with model names
 def get_preset_models_softclass(hyperparameters, invalid_model_names: list = None, **kwargs):
-    # TODO v0.1: This import depends on mxnet, consider refactoring to avoid mxnet
     from autogluon.core.metrics.softclass_metrics import soft_log_loss
-    model_types_standard = ['GBM', 'NN_MXNET', 'NN_TORCH', 'CAT', 'ENS_WEIGHTED']
+    model_types_standard = ['GBM', 'NN_TORCH', 'CAT', 'ENS_WEIGHTED']
     hyperparameters = copy.deepcopy(hyperparameters)
 
     hyperparameters_standard = {key: hyperparameters[key] for key in hyperparameters if key in model_types_standard}
     hyperparameters_rf = {key: hyperparameters[key] for key in hyperparameters if key == 'RF'}
 
     # Swap RF criterion for MSE:
     if 'RF' in hyperparameters_rf:
@@ -393,14 +373,14 @@
             rf_params[i].update(rf_newparams)
         rf_params = [j for n, j in enumerate(rf_params) if j not in rf_params[(n+1):]]  # Remove duplicates which may arise after overwriting criterion
         hyperparameters_standard['RF'] = rf_params
     models, model_args_fit = get_preset_models(problem_type=SOFTCLASS, eval_metric=soft_log_loss,
                                                hyperparameters=hyperparameters_standard,
                                                default_priorities=DEFAULT_SOFTCLASS_PRIORITY, invalid_model_names=invalid_model_names, **kwargs)
     if len(models) == 0:
-        raise ValueError("At least one of the following model-types must be present in hyperparameters: ['GBM','CAT','NN_MXNET','RF'], "
+        raise ValueError("At least one of the following model-types must be present in hyperparameters: ['GBM','CAT','RF'], "
                          "These are the only supported models for softclass prediction problems. "
                          "Softclass problems are also not yet supported for fit() with per-stack level hyperparameters.")
     for model in models:
         model.normalize_pred_probas = True  # FIXME: Do we need to do this for child models too?
 
     return models, model_args_fit
```

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from .presets import get_preset_models, get_preset_models_softclass
 
 logger = logging.getLogger(__name__)
 
 # Higher values indicate higher priority, priority dictates the order models are trained (which matters if time runs out).
 DEFAULT_DISTILL_PRIORITY = dict(
     GBM=100,
-    NN_MXNET=90,
     CAT=80,
     RF=70,
     custom=0,
 )
 
 
 def get_preset_models_distillation(path, problem_type, eval_metric, hyperparameters,
@@ -25,25 +24,20 @@
     if level_key not in hyperparameters.keys() and level_key == 'default':
         hyperparameters = {'default': hyperparameters}
     hyperparameters = hyperparameters[level_key]
     if problem_type == BINARY:  # convert to regression in distillation
         eval_metric = mean_squared_error
         # Constrain output-range of NN:
         nn_outputrange = {'y_range': (0.0,1.0), 'y_range_extend': 0.0}
-        if 'NN_MXNET' in hyperparameters:
-            nn_hyperparameters = hyperparameters['NN_MXNET']
-        else:
-            nn_hyperparameters = None
+        nn_hyperparameters = None
         if isinstance(nn_hyperparameters, list):
             for i in range(len(nn_hyperparameters)):
                 nn_hyperparameters[i].update(nn_outputrange)
         elif nn_hyperparameters is not None:
             nn_hyperparameters.update(nn_outputrange)
-        if 'NN_MXNET' in hyperparameters:
-            hyperparameters['NN_MXNET'] = nn_hyperparameters
         # Swap RF criterion for MSE:
         rf_newparams = {'criterion': 'squared_error', 'ag_args': {'name_suffix': 'MSE'}}
         if 'RF' in hyperparameters:
             rf_hyperparameters = hyperparameters['RF']
         else:
             rf_hyperparameters = None
         if isinstance(rf_hyperparameters, list):
```

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-0.7.1b20230527/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-0.7.1b20230527/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.1b20230526
+Version: 0.7.1b20230527
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-0.7.1b20230527/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -88,19 +88,14 @@
 src/autogluon/tabular/models/tabular_nn/__init__.py
 src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
 src/autogluon/tabular/models/tabular_nn/compilers/native.py
 src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
 src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
 src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
 src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-src/autogluon/tabular/models/tabular_nn/mxnet/__init__.py
-src/autogluon/tabular/models/tabular_nn/mxnet/embednet.py
-src/autogluon/tabular/models/tabular_nn/mxnet/lr_scheduler.py
-src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_dataset.py
-src/autogluon/tabular/models/tabular_nn/mxnet/tabular_nn_mxnet.py
 src/autogluon/tabular/models/tabular_nn/torch/__init__.py
 src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
 src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
 src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
 src/autogluon/tabular/models/tabular_nn/utils/__init__.py
 src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
 src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
```

### Comparing `autogluon.tabular-0.7.1b20230526/src/autogluon.tabular.egg-info/requires.txt` & `autogluon.tabular-0.7.1b20230527/src/autogluon.tabular.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 numpy<1.27,>=1.21
 scipy<1.12,>=1.5.4
 pandas<1.6,>=1.4.1
 scikit-learn<1.3,>=1.0
 networkx<3.0,>=2.3
-autogluon.core==0.7.1b20230526
-autogluon.features==0.7.1b20230526
+autogluon.core==0.7.1b20230527
+autogluon.features==0.7.1b20230527
 
 [all]
-autogluon.core[all]==0.7.1b20230526
-xgboost<1.8,>=1.6
+fastai<2.8,>=2.3.1
 torch<1.14,>=1.9
-lightgbm<3.4,>=3.3
 catboost<1.2,>=1.1
-fastai<2.8,>=2.3.1
+xgboost<1.8,>=1.6
+lightgbm<3.4,>=3.3
+autogluon.core[all]==0.7.1b20230527
 
 [catboost]
 catboost<1.2,>=1.1
 
 [fastai]
 torch<1.14,>=1.9
 fastai<2.8,>=2.3.1
@@ -24,15 +24,15 @@
 [imodels]
 imodels<1.4.0,>=1.3.10
 
 [lightgbm]
 lightgbm<3.4,>=3.3
 
 [ray]
-autogluon.core[all]==0.7.1b20230526
+autogluon.core[all]==0.7.1b20230527
 
 [skex]
 scikit-learn-intelex<2023.1,>=2021.7
 
 [skl2onnx]
 skl2onnx<1.14.0,>=1.13.0
 onnxruntime-gpu<1.14.0,>=1.13.0
```

