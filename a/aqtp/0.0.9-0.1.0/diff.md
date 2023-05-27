# Comparing `tmp/aqtp-0.0.9.tar.gz` & `tmp/aqtp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/private/tmp/aqt/aqt/aqt/dist/tmp0hb08w5f/aqtp-0.0.9.tar", last modified: Thu Jun 30 23:08:12 2022, max compression
+gzip compressed data, was "aqtp-0.1.0.tar", last modified: Sat May 27 01:21:40 2023, max compression
```

## Comparing `aqtp-0.0.9.tar` & `aqtp-0.1.0.tar`

### file list

```diff
@@ -1,174 +1,188 @@
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      664 2022-06-30 23:08:12.000000 aqtp-0.0.9/PKG-INFO
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    11358 2022-06-30 23:05:31.000000 aqtp-0.0.9/LICENSE
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/__init__.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/__init__.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/utils/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    10129 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/pandas_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    23689 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/report_utils_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     3451 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/summary_utils_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    20428 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/report_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     6742 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/hparams_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     4307 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/tfevent_utils_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/__init__.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     2538 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/summary_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1045 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/common.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     7640 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/config_schema_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    10538 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/config_schema_utils_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     4810 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/analysis_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    10192 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/pandas_utils_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     5109 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/analysis_utils_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     6640 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/utils/tfevent_utils.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/jax/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    24151 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/compute_cost_utils_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     2570 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/hlo_utils_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     4644 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/test_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    47255 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/quantization_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     8221 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/get_bounds.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     9777 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/stats_tag_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     3340 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/train_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    25450 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/flax_attention_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     6897 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/fp_cast.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     7689 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/fp_cast_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     5917 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/primitives.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    63597 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/flax_layers_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    58822 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/quantization.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1654 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/shape_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    11341 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/get_bounds_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/__init__.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     3106 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/quant_config.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    17467 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/compute_cost_utils.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/jax/flax/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/flax/__init__.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     5671 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/flax/struct.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      995 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/utils.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     9773 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/models_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1963 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/check_config_util.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     7928 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/train_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     8129 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/input_pipeline.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     7345 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/models.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    15474 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/pokebnn.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     2547 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/train_test.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs_script/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     6856 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     9525 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     3119 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/pokebnn_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/__init__.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/paper/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1230 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1231 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1439 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      853 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      855 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     7142 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/base_config.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      925 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1390 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/__init__.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      855 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1514 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1440 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1439 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      925 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1383 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1025 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1232 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    19732 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/train.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     2130 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/hparams_config.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     5749 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     2423 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     9798 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/stats.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     3449 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/hlo_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     3065 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/train_utils_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    39123 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/flax_layers.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     3284 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    38042 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/models_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    23300 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    33379 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/models.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    10508 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/train_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    11800 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    25395 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     7056 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/bleu.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     3953 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/predict.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     3939 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/__init__.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1000 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1175 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      954 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1042 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1244 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1002 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1056 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1041 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1002 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1006 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      954 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1101 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1060 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1069 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      954 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1193 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1000 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1069 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     6278 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1018 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      995 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1099 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1096 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1099 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1096 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1925 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1014 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    50024 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/train.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    15170 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/decode.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    11082 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      577 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    12798 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     5228 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    10461 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/stats_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    35159 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/flax_attention.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     6508 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/primitives_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     6060 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax_legacy/jax/stats_tag.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/tensorflow/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    18757 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/tensorflow/aqt_matmul_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     8158 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/tensorflow/aqt_conv2d.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    21343 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/tensorflow/aqt_tensor.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      576 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/tensorflow/__init__.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     4443 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/tensorflow/aqt_conv2d_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     7831 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/tensorflow/aqt_tensor_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     3372 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/tensorflow/aqt_ops.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     6822 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/tensorflow/aqt_einsum.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    17226 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/tensorflow/aqt_einsum_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    17312 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/tensorflow/aqt_matmul.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqt/jax/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    13472 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax/aqt_dot_general_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     8156 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax/aqt_dot_general.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    13086 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax/aqt_conv_general.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     2690 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax/aqt_utils.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    11381 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax/aqt_conv_general_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)    17183 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax/aqt_tensor.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      576 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax/__init__.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     3949 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax/aqt_tensor_test.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1021 2022-06-30 23:05:31.000000 aqtp-0.0.9/aqt/jax/aqt_ops.py
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     1852 2022-06-30 23:06:36.000000 aqtp-0.0.9/setup.py
-drwxr-xr-x   0 jihwanlee (763707) wheel        (0)        0 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqtp.egg-info/
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      664 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqtp.egg-info/PKG-INFO
--rw-r--r--   0 jihwanlee (763707) wheel        (0)        1 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqtp.egg-info/not-zip-safe
--rw-r--r--   0 jihwanlee (763707) wheel        (0)     7845 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqtp.egg-info/SOURCES.txt
--rw-r--r--   0 jihwanlee (763707) wheel        (0)      132 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqtp.egg-info/requires.txt
--rw-r--r--   0 jihwanlee (763707) wheel        (0)        4 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqtp.egg-info/top_level.txt
--rw-r--r--   0 jihwanlee (763707) wheel        (0)        1 2022-06-30 23:08:12.000000 aqtp-0.0.9/aqtp.egg-info/dependency_links.txt
--rw-r--r--   0 jihwanlee (763707) wheel        (0)       38 2022-06-30 23:08:12.000000 aqtp-0.0.9/setup.cfg
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.976766 aqtp-0.1.0/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    11358 2023-05-27 00:40:35.000000 aqtp-0.1.0/LICENSE
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1753 2023-05-27 01:21:40.976766 aqtp-0.1.0/PKG-INFO
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1133 2023-05-27 01:21:13.000000 aqtp-0.1.0/README.md
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.956766 aqtp-0.1.0/aqt/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/__init__.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.960766 aqtp-0.1.0/aqt/common/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      576 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     4354 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/aqt_common.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    14652 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/aqt_config.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    13928 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/aqt_config_schedule_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     5177 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/aqt_config_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    15655 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/emulated_floating_points.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     5730 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/emulation_utils.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.960766 aqtp-0.1.0/aqt/jax/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      576 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    13641 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_conv_general.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    12151 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_conv_general_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     8861 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_dot_general.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    14977 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_dot_general_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     3783 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_matmul.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     3293 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_matmul_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1083 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_ops.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    17734 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_tensor.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     4766 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_tensor_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     2705 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_utils.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.960766 aqtp-0.1.0/aqt/jax_legacy/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/__init__.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.964766 aqtp-0.1.0/aqt/jax_legacy/jax/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    17225 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/compute_cost_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    24127 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/compute_cost_utils_test.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.964766 aqtp-0.1.0/aqt/jax_legacy/jax/flax/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     5671 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax/struct.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    35186 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax_attention.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    25400 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax_attention_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    42938 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax_layers.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    75454 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax_layers_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     6897 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/fp_cast.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     7689 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/fp_cast_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     9842 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/get_bounds.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    11477 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/get_bounds_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     3477 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/hlo_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     2570 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/hlo_utils_test.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.964766 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1963 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/check_config_util.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     7382 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/base_config.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      853 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1230 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1439 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1231 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      855 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      855 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      925 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1439 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1440 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1390 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1514 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1383 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1025 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      925 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1232 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     6856 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     9732 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     2423 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     2130 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/hparams_config.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     8129 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/input_pipeline.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     7345 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/models.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     9773 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/models_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    15474 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/pokebnn.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     3119 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/pokebnn_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     5749 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    19735 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     2611 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train_benchmark.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     2547 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     7921 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     5854 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/primitives.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     6508 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/primitives_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     3927 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/quant_config.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    63692 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/quantization.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    45534 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/quantization_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1654 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/shape_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    22858 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/sparsity.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    23122 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/sparsity_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     9798 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/stats.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     6060 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/stats_tag.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     9777 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/stats_tag_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    10461 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/stats_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     4644 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/test_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     5436 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/train_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     6301 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/train_utils_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      995 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/utils.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     7056 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/bleu.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    15134 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/decode.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    12107 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    11082 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    13257 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     6573 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.972766 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1069 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1069 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1056 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1041 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1006 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1193 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      954 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1000 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1101 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1002 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      954 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1000 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1042 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1002 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      954 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1060 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1175 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1244 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.972766 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1096 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1099 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1014 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1096 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1099 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1018 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      995 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1925 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    23300 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    33379 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/models.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    38051 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/models_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     4055 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/predict.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    51615 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     5666 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    10503 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     3939 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    25395 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     3284 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.972766 aqtp-0.1.0/aqt/jax_legacy/utils/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     4810 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/analysis_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     5109 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/analysis_utils_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1045 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/common.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     8505 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/config_schema_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    11978 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/config_schema_utils_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     6807 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/hparams_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    10180 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/pandas_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    10192 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/pandas_utils_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    20428 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/report_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    23689 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/report_utils_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     2538 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/summary_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     3451 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/summary_utils_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     6640 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/tfevent_utils.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     4307 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/tfevent_utils_test.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.976766 aqtp-0.1.0/aqt/tensorflow/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      576 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/__init__.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    11332 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_conv2d.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     6495 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_conv2d_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     6945 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_einsum.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    19276 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_einsum_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    24040 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_matmul.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    14193 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_matmul_test.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     3423 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_ops.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)    25108 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_tensor.py
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     8386 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_tensor_test.py
+drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.976766 aqtp-0.1.0/aqtp.egg-info/
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1753 2023-05-27 01:21:40.000000 aqtp-0.1.0/aqtp.egg-info/PKG-INFO
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     8230 2023-05-27 01:21:40.000000 aqtp-0.1.0/aqtp.egg-info/SOURCES.txt
+-rw-r--r--   0 lew      (84645) primarygroup (89939)        1 2023-05-27 01:21:40.000000 aqtp-0.1.0/aqtp.egg-info/dependency_links.txt
+-rw-r--r--   0 lew      (84645) primarygroup (89939)        1 2023-05-27 01:04:56.000000 aqtp-0.1.0/aqtp.egg-info/not-zip-safe
+-rw-r--r--   0 lew      (84645) primarygroup (89939)      132 2023-05-27 01:21:40.000000 aqtp-0.1.0/aqtp.egg-info/requires.txt
+-rw-r--r--   0 lew      (84645) primarygroup (89939)        4 2023-05-27 01:21:40.000000 aqtp-0.1.0/aqtp.egg-info/top_level.txt
+-rw-r--r--   0 lew      (84645) primarygroup (89939)       38 2023-05-27 01:21:40.976766 aqtp-0.1.0/setup.cfg
+-rw-r--r--   0 lew      (84645) primarygroup (89939)     1852 2023-05-27 01:21:34.000000 aqtp-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aqtp-0.0.9/LICENSE` & `aqtp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/__init__.py` & `aqtp-0.1.0/aqt/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/pandas_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/pandas_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 
   if sort_by_args is not None:
     by = [tup[0] for tup in sort_by_args]
     ascending = [tup[1] for tup in sort_by_args]
     df = df.sort_values(by=by, ascending=ascending)
 
   df = df.reset_index(drop=True)
-  return df
+  return df  # pytype: disable=bad-return-type  # typed-pandas
 
 
 def boxplot_with_group_by_sorted_by_median(df: pd.DataFrame,
                                            column_to_plot: str,
                                            by: Union[str, List[str]]):
   """Returns a box plot for dataframe column, after group by operation.
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/report_utils_test.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/report_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/summary_utils_test.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/summary_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/report_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/report_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/hparams_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/hparams_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,16 @@
 import json
 import os
 import typing
 from typing import Any, Dict, Optional, Type, TypeVar
 
 from aqt.jax_legacy.jax import quant_config
 from aqt.jax_legacy.jax import quantization
+from aqt.jax_legacy.jax import sparsity
 from aqt.jax_legacy.jax.flax import struct as flax_struct
-
-
 import dacite
 import jax
 import ml_collections
 
 
 T = TypeVar('T')
 
@@ -104,14 +103,15 @@
   # to convert from a string into an enum. The classes of all enum values which
   # are stored in a TrainingHParams instance (directly or indirectly) should be
   # listed here. See https://github.com/konradhalas/dacite#casting.
   enum_classes = [
       quantization.QuantOps.ActHParams.InputDistribution,
       quantization.QuantType,
       quant_config.QuantGranularity,
+      sparsity.SparseType,
   ]
   data_dict = _convert_lists_to_tuples(data_dict)
   return dacite.from_dict(
       data_class=dataclass_name,
       data=data_dict,
       config=dacite.Config(cast=enum_classes))
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/tfevent_utils_test.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/tfevent_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/summary_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/common.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/common.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/config_schema_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/config_schema_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,16 @@
       parent_config,
       [
           "weight_prec",
           "weight_quant_granularity",
           "quant_type",
           "quant_act",
           "weight_half_shift",
+          "act_sparsity",
+          "weight_sparsity",
       ])
   config.lock()
   return config
 
 
 def get_conv_config(
     parent_config: ml_collections.ConfigDict) -> ml_collections.ConfigDict:
@@ -159,21 +161,36 @@
       "exp_max": int_ph(),
       "sig_bits": int_ph()
   })
   config.lock()
   return config
 
 
+def get_sparse_config(use_unstructured: bool) -> ml_collections.ConfigDict:
+  """Returns a sparse ConfigDict based on sparsity type argument."""
+  prune_rate = float_ph() if use_unstructured else (int_ph(), int_ph())
+  config = ml_collections.ConfigDict({
+      "type": str_ph(),
+      "prune_rate": prune_rate,
+      "smallest": bool_ph(),
+      "order": str_ph(),
+      "absolute": bool_ph(),
+      "structure_decay": bool_ph(),
+      "sparse_ste": bool_ph()
+  })
+  config.lock()
+  return config
 
 
 # TODO(shivaniagrawal): base config should be more generic and only model
 # specific configs should be updated.
 def get_base_config(
     use_auto_acts: bool,
     fp_quant: bool,
+    use_unstructured: bool = False,
 ) -> ml_collections.ConfigDict:
   """Return a base ConfigDict for AQT; does not have model specific fields."""
   if use_auto_acts:
     bounds = ml_collections.ConfigDict({
         "initial_bound": float_ph(),
         "stddev_coeff": float_ph(),
         "absdev_coeff": float_ph(),
@@ -187,23 +204,25 @@
     })
   else:
     bounds = float_ph()
   if fp_quant:
     prec = get_fp_quant_config()
   else:
     prec = int_ph()
+  sparsity = get_sparse_config(use_unstructured)
   base_config = ml_collections.ConfigDict({
       "metadata": {
           "description": "Base configuration",
           "hyper_str": str_ph(),
       },
       "weight_decay": float_ph(),
       "activation_bound_update_freq": int_ph(),
       "activation_bound_start_step": int_ph(),
       "prec": prec,
+      "sparsity": sparsity,
       "half_shift": bool_ph(),
       "quant_type": str_ph(),
       "quant_act": {
           "bounds": bounds,
           # TODO(shivaniagrawal): The input distribution is really an intrinsic
           # model property and shouldn't be part of the model configuration.
           # Update the hparam dataclasses to eliminate the input_distribution
@@ -212,13 +231,17 @@
       },
       "weight_quant_granularity": str_ph()
   })
 
   set_default_reference(
       base_config, base_config, "weight_prec", parent_field="prec")
   set_default_reference(base_config.quant_act, base_config, "prec")
+  set_default_reference(
+      base_config, base_config, "act_sparsity", parent_field="sparsity")
+  set_default_reference(
+      base_config, base_config, "weight_sparsity", parent_field="sparsity")
 
   set_default_reference(
       base_config, base_config, "weight_half_shift", parent_field="half_shift")
   set_default_reference(base_config.quant_act, base_config, "half_shift")
 
   return base_config
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/config_schema_utils_test.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/config_schema_utils_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -162,14 +162,37 @@
             'sig_bits': 2
         }
     }
     # Test that this sets the weight and activation to 4 as well.
     self.assertEqual(config.weight_prec.to_dict(), expected_prec_dict)
     self.assertEqual(config.quant_act.prec.to_dict(), expected_prec_dict)
 
+  @parameterized.parameters(
+      dict(use_unstructured=True), dict(use_unstructured=False))
+  def test_sparsity_propagates(self, use_unstructured):
+    config = config_schema_utils.get_base_config(
+        use_auto_acts=True, fp_quant=False, use_unstructured=use_unstructured)
+
+    prune_rate = 0.2 if use_unstructured else (1, 2)
+
+    expected_sparse_dict = {
+        'type': 'unstructured',
+        'prune_rate': prune_rate,
+        'smallest': True,
+        'absolute': False,
+        'order': 'C',
+        'structure_decay': False,
+        'sparse_ste': False
+    }
+
+    config.sparsity.update(expected_sparse_dict)
+
+    # Test that this sets the weight and activation to 4 as well.
+    self.assertEqual(config.weight_sparsity.to_dict(), expected_sparse_dict)
+    self.assertEqual(config.act_sparsity.to_dict(), expected_sparse_dict)
 
   def test_auto_acts_parameter(self):
     # If use_auto_acts is False, then the bounds should be a single scalar that
     # specifies the fixed bound; 'None' by default.
     config = config_schema_utils.get_base_config(
         use_auto_acts=False, fp_quant=False)
     self.assertIsNone(config.quant_act.bounds)
@@ -184,19 +207,21 @@
     with self.assertRaises(TypeError):
       config.quant_act.bounds = 1.0
 
   @parameterized.parameters(
       dict(use_auto_acts=True, fp_quant=False),
       dict(use_auto_acts=False, fp_quant=False),
       dict(use_auto_acts=False, fp_quant=True),
+      dict(use_auto_acts=False, fp_quant=True, use_unstructured=True),
   )
   def test_schema_matches_expected(
       self,
       use_auto_acts,
       fp_quant,
+      use_unstructured=False,
   ):
     # This tests that the schema of the configdict returned by 'base_config',
     # once all references are resolved, matches an expected schema. 'Schema'
     # here means the names and structure of fields at each level of the
     # configuration hierarchy. A value of 'None' in the expected schemas defined
     # below indicates a real configuration would have a concrete scalar value
     # there.
@@ -234,14 +259,24 @@
     else:
       quant_act_schema = {
           'bounds': None,
           'input_distribution': None,
           'prec': prec,
           'half_shift': None,
       }
+    prune_rate = None if use_unstructured else [None, None]
+    sparsity = {
+        'type': None,
+        'prune_rate': prune_rate,
+        'smallest': None,
+        'order': None,
+        'absolute': None,
+        'structure_decay': None,
+        'sparse_ste': None
+    }
     expected_top_level_schema = {
         'metadata': {
             'description': None,
             'hyper_str': None
         },
         'weight_decay': None,
         'activation_bound_update_freq': None,
@@ -249,19 +284,24 @@
         'prec': prec,
         'half_shift': None,
         'weight_prec': prec,
         'weight_half_shift': None,
         'quant_type': None,
         'quant_act': quant_act_schema,
         'weight_quant_granularity': None,
+        'sparsity': sparsity,  # Top level sparsity value, sets both weight and
+        # activation sparsity,
+        'weight_sparsity': sparsity,
+        'act_sparsity': sparsity,
     }
 
     config = config_schema_utils.get_base_config(
         use_auto_acts=use_auto_acts,
         fp_quant=fp_quant,
+        use_unstructured=use_unstructured,
     )
     # This round-trip conversion from JSON forces all references to resolve to
     # concrete values.
     config_reified = json.loads(config.to_json())
 
     # This test is not interested in checking the specific values of fields in
     # the configuration, but only that the schema of the hierarchies
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/analysis_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/pandas_utils_test.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/pandas_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/analysis_utils_test.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/analysis_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/utils/tfevent_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/tfevent_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/compute_cost_utils_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/compute_cost_utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,27 +129,27 @@
           prec=lhs_prec,
           half_shift=False)
       rhs_act_hparams = QuantOps.ActHParams(
           input_distribution='symmetric',
           bounds=get_bounds_hyper,
           prec=rhs_prec,
           half_shift=False)
-      lhs_get_bounds_params = get_bounds.GetBounds.Params(
+      lhs_bounds_params = get_bounds.GetBounds.Params(
           update_stats=False, update_bounds=False, module_name='lhs')
-      rhs_get_bounds_params = get_bounds.GetBounds.Params(
+      rhs_bounds_params = get_bounds.GetBounds.Params(
           update_stats=False, update_bounds=False, module_name='rhs')
       output = quantization.quantized_dynamic_dot_general(
           lhs_act=lhs_act,
           rhs_act=rhs_act,
           lhs_act_hparams=lhs_act_hparams,
           rhs_act_hparams=rhs_act_hparams,
           dot_dimension_numbers=(((1,), (0,)), ((), ())),
           quant_type=QuantType.AQT,
-          lhs_get_bounds_params=lhs_get_bounds_params,
-          rhs_get_bounds_params=rhs_get_bounds_params)
+          lhs_bounds_params=lhs_bounds_params,
+          rhs_bounds_params=rhs_bounds_params)
       return output
 
   @parameterized.named_parameters(
       # TestModelWith1Dense
       dict(
           testcase_name='single_dense_layer_bfloat16',
           modelclass=TestModelWith1Dense,
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/hlo_utils_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/hlo_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/test_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/test_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/quantization_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/quantization_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,15 +199,15 @@
       hparams: QuantOps.ActHParams
 
       @nn.compact
       def __call__(self, inputs):
         return QuantOps.create_input_ops(
             inputs,
             hparams=hparams,
-            get_bounds_params=GetBounds.Params(
+            bounds_params=GetBounds.Params(
                 update_stats=False, update_bounds=False))
 
     test_module = TestModule(hparams=hparams)
     state = test_module.init(jax.random.PRNGKey(0), inputs=inputs)
     act_quant_op = test_module.apply(state, inputs=inputs)
 
     act_scaled = (inputs * act_quant_op._scale).astype(inputs.dtype)
@@ -379,15 +379,15 @@
     _ = QuantOps.create_inputs_fake_quant(
         inputs=inputs,
         hparams=QuantOps.ActHParams(
             input_distribution=QuantOps.ActHParams.InputDistribution.SYMMETRIC,
             bounds=bounds,
             prec=8.0,
             half_shift=False),
-        get_bounds_params=GetBounds.Params(
+        bounds_params=GetBounds.Params(
             update_stats=False,
             update_bounds=False,
             expected_bounds_shape=expected_inputs_scale_shape))
 
   @parameterized.named_parameters(
       dict(testcase_name='prec_2',
            prec=2), dict(testcase_name='prec_4', prec=4),
@@ -437,25 +437,25 @@
     act_scale = 8.
     scaled_activations = activations * act_scale
 
     bounds = 6.
 
     activations = QuantOps.create_inputs_fake_quant(
         inputs=activations,
-        get_bounds_params=GetBounds.Params(
+        bounds_params=GetBounds.Params(
             update_stats=False, update_bounds=False),
         hparams=QuantOps.ActHParams(
             input_distribution=QuantOps.ActHParams.InputDistribution.SYMMETRIC,
             bounds=bounds,
             prec=prec,
             half_shift=False))
 
     scaled_activations = QuantOps.create_inputs_fake_quant(
         inputs=scaled_activations,
-        get_bounds_params=GetBounds.Params(
+        bounds_params=GetBounds.Params(
             update_stats=False, update_bounds=False),
         hparams=QuantOps.ActHParams(
             input_distribution=QuantOps.ActHParams.InputDistribution.SYMMETRIC,
             bounds=bounds * act_scale,
             prec=prec,
             half_shift=False))
     onp.testing.assert_array_equal(activations * act_scale, scaled_activations)
@@ -493,15 +493,15 @@
     # Integer activations within upper_bound and upper_bound == 2^i s.t. i<prec
     # quantizes correctly.
     upper_bound = 2**(prec - 3)
     activations = random.randint(random.PRNGKey(0), (10, 1), 0, upper_bound)
 
     rescaled_activations = QuantOps.create_inputs_fake_quant(
         inputs=activations,
-        get_bounds_params=GetBounds.Params(
+        bounds_params=GetBounds.Params(
             update_stats=False, update_bounds=False),
         hparams=QuantOps.ActHParams(
             input_distribution=QuantOps.ActHParams.InputDistribution.POSITIVE,
             bounds=upper_bound,
             prec=prec,
             half_shift=False))
     onp.testing.assert_array_equal(activations, rescaled_activations)
@@ -513,15 +513,15 @@
   def test_int_symmetric_act_quantization(self, prec):
     # Integer activations within bounds and abs(bounds) == 2^(prec -1) - 1
     # quantizes correctly.
     bounds = 2**(prec - 1) - 1
     activations = random.randint(random.PRNGKey(0), (10, 1), -bounds, bounds)
     rescaled_activations = QuantOps.create_inputs_fake_quant(
         inputs=activations,
-        get_bounds_params=GetBounds.Params(
+        bounds_params=GetBounds.Params(
             update_stats=False, update_bounds=False),
         hparams=QuantOps.ActHParams(
             input_distribution=QuantOps.ActHParams.InputDistribution.SYMMETRIC,
             bounds=bounds,
             prec=prec,
             half_shift=False))
 
@@ -582,15 +582,15 @@
       hparams: quantization.QuantOps.ActHParams
 
       @nn.compact
       def __call__(self, inputs):
         return quantization.QuantOps.create_inputs_fake_quant(
             inputs,
             hparams=hparams,
-            get_bounds_params=GetBounds.Params(
+            bounds_params=GetBounds.Params(
                 update_stats=True, update_bounds=False))
 
     test_module = TestModule(hparams=hparams)
     state = test_module.init(jax.random.PRNGKey(0), inputs=inputs)
     inputs_after_fake_quant, _ = test_module.apply(
         state, inputs=inputs, mutable=True)
     onp.testing.assert_array_equal(inputs, inputs_after_fake_quant)
@@ -667,15 +667,15 @@
 
     def quantized_matmul(quant_type):
       return quantization.quantized_dot(
           w=self.rhs,
           act=self.lhs,
           weight_params=weight_params,
           act_hparams=act_params,
-          get_bounds_params=None,
+          bounds_params=None,
           quant_type=quant_type,
           prefer_int8_to_int32_dot=True)
 
     aqt_result = quantized_matmul(QuantType.AQT)
     fakequant_result = quantized_matmul(QuantType.FAKE_QUANT)
     onp.testing.assert_allclose(
         aqt_result,
@@ -747,15 +747,15 @@
 
     def quantized_matmul(quant_type):
       return quantization.quantized_dot_general(
           w=self.rhs,
           act=lhs_ndims_3,
           weight_params=weight_params,
           act_hparams=act_params,
-          get_bounds_params=None,
+          bounds_params=None,
           quant_type=quant_type,
           dimension_numbers=(((lhs_ndims_3.ndim - 1,), (0,)), ((), ())),
           prefer_int8_to_int32_dot=True)
 
     aqt_result = quantized_matmul(QuantType.AQT)
     self.assertEqual(aqt_result.shape, (4, 3, 4))
 
@@ -783,15 +783,15 @@
   @parameterized.parameters(
       dict(act_distribution='symmetric', prefer_int8_to_int32_dot=True, prec=4),
       dict(act_distribution='symmetric', prefer_int8_to_int32_dot=True, prec=8),
       dict(act_distribution='positive', prefer_int8_to_int32_dot=True, prec=4),
       dict(act_distribution='positive', prefer_int8_to_int32_dot=True, prec=8),
       dict(
           act_distribution='symmetric', prefer_int8_to_int32_dot=False, prec=4))
-  @mock.patch.object(jax.lax, 'dot_general')
+  @mock.patch.object(jax.lax, 'dot_general', wraps=jax.lax.dot_general)
   def test_lax_dot_has_integer_inputs_in_quantized_dot(self, mock_dot_general,
                                                        act_distribution,
                                                        prefer_int8_to_int32_dot,
                                                        prec):
     weight_params = QuantOps.WeightParams(
         prec=prec, axis=(0,), half_shift=False)
     act_params = QuantOps.ActHParams(
@@ -812,15 +812,15 @@
     # compile the arms to lax.cond and so using a mock will work fine.
     with jax.disable_jit():
       quantization.quantized_dot(
           w=self.rhs,
           act=act,
           weight_params=weight_params,
           act_hparams=act_params,
-          get_bounds_params=None,
+          bounds_params=None,
           quant_type=QuantType.AQT,
           prefer_int8_to_int32_dot=prefer_int8_to_int32_dot)
     act_inputs, weight_inputs = mock_dot_general.call_args[0]
     self.assert_is_integer_in_range(
         act_inputs, prec=prec, distribution=act_distribution)
     self.assert_is_integer_in_range(
         weight_inputs, prec=prec, distribution='symmetric')
@@ -847,42 +847,20 @@
     act = self.lhs.astype(input_dtype)
     w = self.rhs.astype(input_dtype)
     output = quantization.quantized_dot(
         w=w,
         act=act,
         weight_params=weight_params,
         act_hparams=act_params,
-        get_bounds_params=None,
+        bounds_params=None,
         quant_type=quant_type,
         prefer_int8_to_int32_dot=True)
     self.assertEqual(output.dtype, input_dtype)
 
   @parameterized.parameters(
-      dict(quant_type=quantization.QuantType.AQT),
-      dict(quant_type=quantization.QuantType.FAKE_QUANT))
-  def test_quantized_dot_raises_with_mixed_dtype(self, quant_type):
-    weight_params = QuantOps.WeightParams(prec=4, axis=(0,), half_shift=False)
-    act_params = QuantOps.ActHParams(
-        input_distribution='symmetric',
-        bounds=jnp.array([[3.0, 1.5]]),
-        prec=4,
-        half_shift=False)
-    act = self.lhs.astype(jnp.bfloat16)
-    w = self.rhs.astype(jnp.float32)
-    with self.assertRaises(TypeError):
-      quantization.quantized_dot(
-          w=w,
-          act=act,
-          weight_params=weight_params,
-          act_hparams=act_params,
-          get_bounds_params=None,
-          quant_type=quant_type,
-          prefer_int8_to_int32_dot=True)
-
-  @parameterized.parameters(
       itertools.product(
           (jnp.bfloat16, jnp.float32), (4, None),
           (quantization.QuantType.AQT, quantization.QuantType.FAKE_QUANT)))
   def test_dynamic_quantized_dot_general_has_correct_dtype(
       self, input_dtype, act_prec, quant_type):
     lhs_params = QuantOps.ActHParams(
         input_distribution='symmetric',
@@ -897,38 +875,20 @@
     lhs_act = self.lhs.astype(input_dtype)
     rhs_act = self.rhs.astype(input_dtype)
     output = quantization.quantized_dynamic_dot_general(
         lhs_act=lhs_act,
         rhs_act=rhs_act,
         lhs_act_hparams=lhs_params,
         rhs_act_hparams=rhs_params,
-        lhs_get_bounds_params=None,
-        rhs_get_bounds_params=None,
+        lhs_bounds_params=None,
+        rhs_bounds_params=None,
         dot_dimension_numbers=(((1,), (0,)), ((), ())),
         quant_type=quant_type)
     self.assertEqual(output.dtype, input_dtype)
 
-  def test_dynamic_quantized_dot_general_raises_with_mixed_dtype(self):
-    lhs_params = QuantOps.ActHParams(
-        input_distribution='symmetric', bounds=2.0, prec=4, half_shift=False)
-    rhs_params = QuantOps.ActHParams(
-        input_distribution='symmetric', bounds=1.5, prec=4, half_shift=False)
-    lhs_act = self.lhs.astype(jnp.bfloat16)
-    rhs_act = self.rhs.astype(jnp.float32)
-    with self.assertRaises(TypeError):
-      quantization.quantized_dynamic_dot_general(
-          lhs_act=lhs_act,
-          rhs_act=rhs_act,
-          lhs_act_hparams=lhs_params,
-          rhs_act_hparams=rhs_params,
-          lhs_get_bounds_params=None,
-          rhs_get_bounds_params=None,
-          dot_dimension_numbers=(((1,), (0,)), ((), ())),
-          quant_type=QuantType.AQT)
-
   @parameterized.parameters(
       dict(lhs_prec=16, rhs_prec=16), dict(lhs_prec=None, rhs_prec=16),
       dict(lhs_prec=16, rhs_prec=None), dict(lhs_prec=None, rhs_prec=None))
   def test_quantized_dynamic_dot_general(self, lhs_prec, rhs_prec):
     lhs_bounds = 2.0
     rhs_bounds = 1.5
     lhs_params = QuantOps.ActHParams(
@@ -944,16 +904,16 @@
 
     def quantized_matmul(quant_type):
       return quantization.quantized_dynamic_dot_general(
           lhs_act=self.lhs,
           rhs_act=self.rhs,
           lhs_act_hparams=lhs_params,
           rhs_act_hparams=rhs_params,
-          lhs_get_bounds_params=None,
-          rhs_get_bounds_params=None,
+          lhs_bounds_params=None,
+          rhs_bounds_params=None,
           dot_dimension_numbers=(((1,), (0,)), ((), ())),
           quant_type=quant_type)
 
     aqt_result = quantized_matmul(QuantType.AQT)
     fakequant_result = quantized_matmul(QuantType.FAKE_QUANT)
     onp.testing.assert_allclose(
         aqt_result,
@@ -985,27 +945,27 @@
             prec=8,
             half_shift=False)
         rhs_params = QuantOps.ActHParams(
             input_distribution='symmetric',
             bounds=rhs_get_bounds,
             prec=8,
             half_shift=False)
-        lhs_get_bounds_params = get_bounds.GetBounds.Params(
+        lhs_bounds_params = get_bounds.GetBounds.Params(
             update_stats=True, update_bounds=False, module_name='lhs')
-        rhs_get_bounds_params = get_bounds.GetBounds.Params(
+        rhs_bounds_params = get_bounds.GetBounds.Params(
             update_stats=True, update_bounds=False, module_name='rhs')
         out = quantization.quantized_dynamic_dot_general(
             lhs_act=lhs,
             rhs_act=rhs,
             lhs_act_hparams=lhs_params,
             rhs_act_hparams=rhs_params,
             dot_dimension_numbers=(((1,), (0,)), ((), ())),
             quant_type=QuantType.AQT,
-            lhs_get_bounds_params=lhs_get_bounds_params,
-            rhs_get_bounds_params=rhs_get_bounds_params)
+            lhs_bounds_params=lhs_bounds_params,
+            rhs_bounds_params=rhs_bounds_params)
         return out
 
     lhs = jnp.array([[2.0]])
     rhs = jnp.array([[3.0]])
     module = TestModule()
     state = module.init(jax.random.PRNGKey(0), lhs, rhs)
     out, _ = module.apply(state, lhs, rhs, mutable=True)
@@ -1040,16 +1000,16 @@
     if rhs_distribution == 'positive':
       rhs_act = jnp.abs(rhs_act)
     quantization.quantized_dynamic_dot_general(
         lhs_act=lhs_act,
         rhs_act=rhs_act,
         lhs_act_hparams=lhs_params,
         rhs_act_hparams=rhs_params,
-        lhs_get_bounds_params=None,
-        rhs_get_bounds_params=None,
+        lhs_bounds_params=None,
+        rhs_bounds_params=None,
         dot_dimension_numbers=(((1,), (0,)), ((), ())),
         quant_type=QuantType.AQT)
     lhs_inputs, rhs_inputs = mock_dot_general.call_args[0]
     self.assert_is_integer_in_range(
         lhs_inputs, prec=4, distribution=lhs_distribution)
     self.assert_is_integer_in_range(
         rhs_inputs, prec=4, distribution=rhs_distribution)
@@ -1062,31 +1022,31 @@
     w = jnp.array([[-4.99]])
     res = quantization.quantized_dot(
         w=w,
         act=act,
         quant_type=quantization.QuantType.AQT,
         weight_params=weight_params,
         act_hparams=act_hparams,
-        get_bounds_params=None,
+        bounds_params=None,
         prefer_int8_to_int32_dot=True)
     onp.testing.assert_allclose(res, act * w)
 
   def test_quantized_dynamic_dot_general_no_quant(self):
     act_hparams = QuantOps.ActHParams(
         input_distribution='symmetric', bounds=-1.0, prec=4, half_shift=False)
     lhs_act = jnp.array([[-5.0]])
     rhs_act = jnp.array([[-4.99]])
     res = quantization.quantized_dynamic_dot_general(
         lhs_act=lhs_act,
         rhs_act=rhs_act,
         quant_type=quantization.QuantType.AQT,
         lhs_act_hparams=act_hparams,
         rhs_act_hparams=act_hparams,
-        lhs_get_bounds_params=None,
-        rhs_get_bounds_params=None,
+        lhs_bounds_params=None,
+        rhs_bounds_params=None,
         dot_dimension_numbers=(((1,), (0,)), ((), ())))
     onp.testing.assert_allclose(res, lhs_act * rhs_act)
 
 
 class QuantizedDotFakeQuantTest(parameterized.TestCase):
 
   def setUp(self):
@@ -1120,36 +1080,36 @@
     weight_params = QuantOps.WeightParams(
         prec=weight_prec, axis=None, half_shift=False)
     act_hparams = QuantOps.ActHParams(  # pylint: disable=g-long-ternary
         bounds=6.,
         prec=act_prec,
         input_distribution=QuantOps.ActHParams.InputDistribution.SYMMETRIC,
         half_shift=False) if act_prec else None
-    get_bounds_params = GetBounds.Params(
+    bounds_params = GetBounds.Params(
         update_stats=False, update_bounds=False)
 
     quantization.quantized_dot(
         w=self.weight,
         act=self.act,
         quant_type=strategy,
         weight_params=weight_params,
         act_hparams=act_hparams,
-        get_bounds_params=get_bounds_params,
+        bounds_params=bounds_params,
         prefer_int8_to_int32_dot=True)
 
     quantized_type = strategy.to_jax_type()
 
     mock_w_fq.assert_called_with(
         mock.ANY,
         weight_params=weight_params,
         quantized_type=quantized_type,
         fake_dependency=mock.ANY)
     if act_hparams:
       mock_act_fq.assert_called_with(
-          mock.ANY, hparams=act_hparams, get_bounds_params=get_bounds_params)
+          mock.ANY, hparams=act_hparams, bounds_params=bounds_params)
     else:
       mock_act_fq.assert_not_called()
 
 
 class QuantizedDynamicDotGeneralTest(parameterized.TestCase):
 
   def setUp(self):
@@ -1174,52 +1134,52 @@
   @mock.patch.object(QuantOps, 'create_inputs_fake_quant')
   def test_quantized_dynamic_dot_general_should_call_inputs_quantization(
       self,
       mock_act_fq,
       lhs_act_prec,
       rhs_act_prec,
       strategy=QuantType.FAKE_QUANT):
-    mock_act_fq.side_effect = lambda inputs, hparams, get_bounds_params: inputs
+    mock_act_fq.side_effect = lambda inputs, hparams, bounds_params: inputs
 
     # pylint: disable=g-long-ternary
     lhs_act_hparams = QuantOps.ActHParams(
         bounds=6.,
         prec=lhs_act_prec,
         input_distribution=QuantOps.ActHParams.InputDistribution.SYMMETRIC,
         half_shift=False) if lhs_act_prec else None
     rhs_act_hparams = QuantOps.ActHParams(
         bounds=6.,
         prec=rhs_act_prec,
         input_distribution=QuantOps.ActHParams.InputDistribution.SYMMETRIC,
         half_shift=False) if rhs_act_prec else None
     # pylint: enable=g-long-ternary
 
-    get_bounds_params = GetBounds.Params(
+    bounds_params = GetBounds.Params(
         update_stats=False, update_bounds=False)
 
     quantization.quantized_dynamic_dot_general(
         lhs_act=self.lhs_act,
         rhs_act=self.rhs_act,
         quant_type=strategy,
         dot_dimension_numbers=self.dimension_numbers,
         lhs_act_hparams=lhs_act_hparams,
-        lhs_get_bounds_params=get_bounds_params,
+        lhs_bounds_params=bounds_params,
         rhs_act_hparams=rhs_act_hparams,
-        rhs_get_bounds_params=get_bounds_params,
+        rhs_bounds_params=bounds_params,
     )
     calls = []
     for prec in [lhs_act_prec, rhs_act_prec]:
       if prec is not None:
         act_hparams = QuantOps.ActHParams(
             bounds=6., prec=prec, input_distribution=mock.ANY, half_shift=False)
         calls.append(
             mock.call(
                 mock.ANY,
                 hparams=act_hparams,
-                get_bounds_params=get_bounds_params))
+                bounds_params=bounds_params))
     self.assertLen(calls, mock_act_fq.call_count)
     mock_act_fq.assert_has_calls(calls, any_order=True)
 
 
 class QuantizedSumTest(parameterized.TestCase):
 
   @parameterized.parameters(
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/get_bounds.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/get_bounds.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,26 +12,96 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Functions to get bounds of activation/input using its statistics."""
 
 import dataclasses
 import typing
-from typing import Optional, Tuple, Union
+from typing import Iterable, Optional, Tuple, Union
+
+from aqt.jax_legacy.jax import primitives
 from aqt.jax_legacy.jax import quant_config
 from aqt.jax_legacy.jax import shape_utils
 from aqt.jax_legacy.jax.flax import struct as flax_struct
 from aqt.jax_legacy.jax.stats import Stats
 from flax import linen as nn
 from jax import lax
 import jax.numpy as jnp
 
 dataclass = flax_struct.dataclass if not typing.TYPE_CHECKING else dataclasses.dataclass
 
 
+class DynamicBounds(nn.Module):
+  """Get Bounds of activation using statistics.
+
+  Attributes:
+    hyper: hyperparamater to compute bound from statistics.
+  """
+
+  @dataclass
+  class Hyper:
+    """Hyperparameters for DynamicBounds."""
+    granularity: quant_config.QuantGranularity
+    # Clipping coefficient applied during dynamic quantization.
+    # E.g. if it is 0.9 then dynamic scale will be reduced by 10%.
+    clipping_coeff: float = 1.0
+
+  @dataclass
+  class Params:
+    """Parameters for act quantiztaion using get_bounds."""
+    # Axis along which to quantize activations.
+    quant_axis: Optional[Iterable[int]] = None
+    # Optional shape to verify if bounds shape is expected. Defaults to None.
+    expected_bounds_shape: Union[None, int, Tuple[int, ...]] = None
+    # Optional name of the get_bounds module.
+    module_name: Optional[str] = None
+
+  hyper: Hyper
+
+  @nn.compact
+  def __call__(
+      self,
+      x: jnp.ndarray,
+      *,
+      bounds_params: Params,
+  ) -> jnp.ndarray:
+    """Compute the input batch statistics.
+
+    Args:
+      x: the input to get bounds from using statistics.
+      bounds_params: parameters to compute input's statistics and bounds.
+
+    Returns:
+      Bound value (same shape as inputs).
+    """
+
+    x = jnp.asarray(x, jnp.float32)
+
+    hyper = self.hyper
+
+    if bounds_params.quant_axis is not None:
+      quant_axis = bounds_params.quant_axis
+    else:
+      if hyper.granularity == quant_config.QuantGranularity.PER_TENSOR:
+        # Equivalently, this could be written as
+        # quant_axis = tuple(range(x.ndim))
+        quant_axis = None
+      elif hyper.granularity == quant_config.QuantGranularity.PER_CHANNEL:
+        # Quantize by aggregating activation statistics across all dimensions of
+        # the activation tensor EXCEPT the batch dimension. Also known as per
+        # example statistics
+        quant_axis = tuple(range(1, x.ndim))
+      else:
+        raise ValueError(f'Unknown granularity {hyper.granularity}')
+
+    abs_max_x = primitives.max_abs_weights(x, axis=quant_axis)
+
+    return abs_max_x * self.hyper.clipping_coeff
+
+
 class GetBounds(nn.Module):
   """Get Bounds of activation using statistics.
 
   Attributes:
     hyper: hyperparamater to compute bound from statistics.
   """
 
@@ -71,22 +141,14 @@
     cams_coeff: Optional[float] = None
     cams_stddev_coeff: Optional[float] = None
     mean_of_max_coeff: Optional[float] = None
     fixed_bound: Optional[float] = None
     # whether to use old or new code to compute the bound
     use_old_code: bool = True
 
-    # Whether to use dynamic quantization.
-    # It will dynamically quantize the tensor in training and inference modes.
-    dynamic: bool = False
-
-    # Clipping coefficient applied during dynamic quantization.
-    # E.g. if it is 0.9 then dynamic scale will be reduced by 10%.
-    clipping_coeff: float = 1.0
-
   @dataclass
   class Params:
     """Parameters for act quantiztaion using get_bounds."""
     update_stats: bool  # Whether to update statistics.
     update_bounds: bool  # Whether to update bounds.
     # The axis name used to combine batch statistics from multiple devices.
     # See `jax.pmap` for a description of axis names. Defaults to None.
@@ -141,21 +203,14 @@
       # this aggregates activation statistics separately for each feature, where
       # for each feature it aggregates over all unmasked tokens in all examples.
       quant_axis = tuple(range(x.ndim - 1))
       stats_shape = (1,) * (x.ndim - 1) + (x.shape[-1],)
     else:
       raise ValueError(f'Unknown granularity {hyper.granularity}')
 
-    if hyper.dynamic:
-      abs_max_x = jnp.max(jnp.abs(x), axis=quant_axis)
-
-      # If dynamic quantization is applied then
-      # there is no need to do stats computation.
-      return abs_max_x * hyper.clipping_coeff
-
     stats_state = self.variable('get_bounds', 'stats', Stats.stats_initializer,
                                 stats_shape)
 
     def bound_initializer(shape):
       return hyper.initial_bound * jnp.ones(shape)
 
     bounds = self.variable('get_bounds', 'bounds', bound_initializer,
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/stats_tag_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/stats_tag_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/flax_attention_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/flax_attention_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                    softmax_recip_lin(1.0, a21, [a11, a21]),
                    softmax_recip_lin(1.0, a22, [a12, a22])
                ]]),
       ),
   )
   def test_custom_softmax_vs_mock(self, input_tensor, norm_dims,
                                   softmax_hparams, expected_output):
-    dtype = jax._src.numpy.lax_numpy.float32
+    dtype = jnp.float32
     output = flax_attention.softmax(
         input_tensor, norm_dims, dtype, softmax_hparams,
         quant_config.DynamicContext(update_bounds=False, quantize_acts=False))
     self.assertAllClose(expected_output, output, atol=1e-6)
 
   # # Test modified softmax vs original softmax.
   random_input = onp.random.rand(16, 16, 2, 2)
@@ -197,15 +197,15 @@
               reciprocal_hparams=None,
               quant_hparams=flax_attention.SoftmaxQuantHParams(
                   reduction_prec=None,
                   prec=QuantOps.FloatQuant.FloatPrec(
                       exp_min=-2**7, exp_max=2**7, sig_bits=23))),
       ))
   def test_softmax_vs_original(self, input_tensor, softmax_hparams):
-    dtype = jax._src.numpy.lax_numpy.float32
+    dtype = jnp.float32
     norm_dims = (0,)
     input_tensor = jnp.array(input_tensor)
     output = flax_attention.softmax(
         input_tensor, norm_dims, dtype, softmax_hparams,
         quant_config.DynamicContext(update_bounds=False, quantize_acts=True))
     expected_output = flax_attention.softmax(
         input_tensor, norm_dims, dtype, SoftmaxHParams(None, None, None),
@@ -645,15 +645,15 @@
   )
   @unittest.mock.patch.object(QuantOps, 'create_inputs_fake_quant')
   def test_self_attention_act_quant_should_call_quant_ops(
       self, mock_inputs_fake_quant, attn_act_q, attn_act_k, attn_act_probs,
       attn_act_v, update_bounds, paxis_name, train):
 
     mock_inputs_fake_quant.side_effect = (
-        lambda inputs, hparams, get_bounds_params: inputs)
+        lambda inputs, hparams, bounds_params: inputs)
 
     rng = random.PRNGKey(0)
     x = jnp.ones((4, 3, 7))
     hparams = self.construct_hparams(attn_act_q, attn_act_k, attn_act_probs,
                                      attn_act_v)
     sa_module = flax_attention.SelfAttentionAqt(
         hparams=hparams,
@@ -675,15 +675,15 @@
     calls = []
     for hparam in [attn_act_q, attn_act_k, attn_act_probs, attn_act_v]:
       if hparam is not None:
         calls.append(
             unittest.mock.call(
                 unittest.mock.ANY,
                 hparams=hparam,
-                get_bounds_params=get_bounds.GetBounds.Params(
+                bounds_params=get_bounds.GetBounds.Params(
                     update_stats=train,
                     update_bounds=update_bounds,
                     paxis_name=paxis_name,
                     mask=unittest.mock.ANY,
                     module_name=unittest.mock.ANY)))
     mock_inputs_fake_quant.assert_has_calls(calls, any_order=True)
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/fp_cast.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/fp_cast.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/fp_cast_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/fp_cast_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/primitives.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/primitives.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Primitives for neural network quantization implemented in jax."""
 from typing import Any, Iterable, Optional, TypeVar
 
 import jax
-from jax.interpreters.xla import DeviceArray
 import jax.numpy as jnp
 
 # Custom type for bounds for type hinting
 BoundsT = TypeVar('BoundsT', float, jnp.ndarray)
 
 jnp_dtype = Any  # type of jax dtype; b/164524367 use more specific type.
 
@@ -51,33 +50,33 @@
   def ste(primals, tangents):
     return jax_function(primals[0]), tangents[0]
 
   jax_function.defjvp(ste)
 
 
 @jax.custom_jvp
-def floor_with_gradient(x: DeviceArray) -> DeviceArray:
+def floor_with_gradient(x: jax.Array) -> jax.Array:
   """Floor with Straight-Through-Estimator gradient."""
   return jnp.floor(x)
 
 
 add_straight_through_estimator(floor_with_gradient)
 
 
 @jax.custom_jvp
-def round_with_gradient(x: DeviceArray) -> DeviceArray:
+def round_with_gradient(x: jax.Array) -> jax.Array:
   """Round with Straight-Through-Estimator gradient."""
   return jnp.floor(x + jnp.array(0.5))
 
 
 add_straight_through_estimator(round_with_gradient)
 
 
-def round_and_clip_to_signed_int(x: DeviceArray, *, prec: int, dtype: jnp_dtype,
-                                 half_shift: bool) -> DeviceArray:
+def round_and_clip_to_signed_int(x: jax.Array, *, prec: int, dtype: jnp_dtype,
+                                 half_shift: bool) -> jax.Array:
   """Round and clip x to range of signed type with precision 'prec'.
 
   Requires prec <= 24.
 
   Args:
     x: The argument to be quantized.
     prec: The target precision for quantization.
@@ -104,17 +103,17 @@
     # TODO(lew): Use the formula for better gradients. Needs a sweep though.
     # bound = 2**(prec - 1) - 0.5 - epsilon
     x = jnp.clip(x, a_min=-bound, a_max=bound).astype(dtype)
     x = round_with_gradient(x)
   return x
 
 
-def floor_and_clip_to_unsigned_int(x: DeviceArray, *, prec: int,
+def floor_and_clip_to_unsigned_int(x: jax.Array, *, prec: int,
                                    dtype: jnp_dtype,
-                                   half_shift: bool) -> DeviceArray:
+                                   half_shift: bool) -> jax.Array:
   """Floor-and-clip x to range of unsigned type with precision 'prec'.
 
   Requires prec <= 24.
 
   Args:
     x: The argument to be quantized.
     prec: The target precision for quantization.
@@ -144,15 +143,15 @@
       # the scaling factor back. So we need to return a nonzero value that
       # makes inputs rounded to zero.
       return 2**(prec - 1.0) - 1.0 if prec > 1 else 0.25
   else:  # prec < 1
     raise ValueError('prec value should be >= 1.')
 
 
-def max_abs_weights(x: DeviceArray,
+def max_abs_weights(x: jax.Array,
                     *,
                     axis: Optional[Iterable[int]] = None) -> BoundsT:
   """Computes the maximum of the absolute value of weights along the axis."""
   abs_max_x = jnp.max(jnp.abs(x), axis=axis, keepdims=True)
   return abs_max_x
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/flax_layers_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/flax_layers_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,26 +31,23 @@
 from aqt.jax_legacy.jax import shape_utils
 from aqt.jax_legacy.jax import test_utils
 from aqt.jax_legacy.jax.quantization import QuantOps
 from aqt.jax_legacy.jax.quantization import QuantType
 import flax
 from flax import linen as nn
 from flax import traverse_util
-from flax.core import frozen_dict
 import jax
 from jax import config
 from jax import dtypes
 from jax import lax
 from jax import random
 from jax.nn import initializers
 import jax.numpy as jnp
 import numpy as onp
 
-from google3.nlp.nlx.infrastructure.flaxformer import sharding
-
 
 FLAGS = flags.FLAGS
 
 # fp-1-4-3
 #    1: sign
 #    4: number of exponent-bits, (bias = 11), range: -11, ..., 4
 #    3: number of significand-bits (excluding hidden-bit)
@@ -100,23 +97,23 @@
     params_axes: Axis annotations, typically under state["params_axes"].
 
   Returns:
     A pytree with params info.
   """
   params = filter_out_metadata(params)
   params_axes = filter_out_metadata(params_axes)
-  params = frozen_dict.unfreeze(params)  # pytype: disable=wrong-arg-types
+  params = flax.core.unfreeze(params)  # pytype: disable=wrong-arg-types
 
   def remove_axes_suffix(ks):
     if not ks[-1].endswith('_axes'):
       raise ValueError(
           f'Param axes name should end with `_axes`, found {ks[-1]}')
     return tuple(ks[:-1]) + (ks[-1][:-len('_axes')],)
 
-  params_axes = frozen_dict.unfreeze(params_axes)  # pytype: disable=wrong-arg-types
+  params_axes = flax.core.unfreeze(params_axes)  # pytype: disable=wrong-arg-types
   flatten_axes = {
       remove_axes_suffix(ks): v
       for ks, v in traverse_util.flatten_dict(params_axes).items()
   }
   params_axes = traverse_util.unflatten_dict(flatten_axes)
 
   def _create_entry(param, param_axes):
@@ -258,15 +255,15 @@
     full_range_integer_weights = random.randint(
         self.rng_key, kernel_size + (input_dim, num_features), minval,
         maxval + 1)
 
     # manually set one value in each output dim of weights to be exactly maxval
     full_range_integer_weights = (
         full_range_integer_weights.at[0, 0, :].set(maxval))
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = full_range_integer_weights
     state = flax.core.freeze(state)
     outputs = model.apply(state, inputs)
 
     dimension_numbers = nn.linear._conv_dimension_numbers(inputs.shape)  # pylint: disable=protected-access
     exp_outputs = lax.conv_general_dilated(
         inputs,
@@ -305,15 +302,15 @@
         maxval + 1)
     # manually set one value in each output dim of weights to be exactly maxval
     full_range_integer_weights = (
         full_range_integer_weights.at[0, 0, :].set(maxval))
 
     # (batch_size, spatial_dim, spatial_dim, num_features)
     float_scale = jax.random.uniform(self.rng_key, (1, 1, 1, num_features))
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = full_range_integer_weights * float_scale
     state = flax.core.freeze(state)
     outputs = model.apply(state, inputs)
     dimension_numbers = nn.linear._conv_dimension_numbers(inputs.shape)  # pylint: disable=protected-access
     exp_outputs = lax.conv_general_dilated(
         inputs,
         jnp.asarray(state['params']['kernel'], jnp.float32), (1, 1),
@@ -363,15 +360,15 @@
         kernel_size,
         weight_prec=weight_prec,
         weight_half_shift=False)
 
     weights = random.uniform(
         self.rng_key, shape=kernel_size + (input_dim, num_features))
     weight_scale = weight_scale[jnp.newaxis, jnp.newaxis, jnp.newaxis, :]
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = weights
     outputs_without_scaling = model.apply(flax.core.freeze(state), inputs)
     state['params']['kernel'] = jnp.multiply(weights, weight_scale)
     outputs_with_scaling = model.apply(flax.core.freeze(state), inputs)
 
     onp.testing.assert_array_equal(outputs_without_scaling * weight_scale,
                                    outputs_with_scaling)
@@ -381,15 +378,15 @@
     input_dim = 3
     inputs = random.uniform(self.rng_key, shape=(1, 32, 32, input_dim))
     kernel_size = (3, 3)
     model, state = self.init_model_with_1_layer(
         inputs, num_features, kernel_size, weight_prec=1)
     weights = random.uniform(
         self.rng_key, shape=kernel_size + (input_dim, num_features))
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = weights
     outputs = model.apply(flax.core.freeze(state), inputs)
     onp.testing.assert_array_equal(outputs, onp.zeros(
         (1, 32, 32, num_features)))
 
   @parameterized.named_parameters(
       dict(
@@ -510,32 +507,36 @@
   def init_model_with_1_layer(self,
                               inputs,
                               num_features,
                               kernel_init=flax_layers.default_kernel_init,
                               weight_prec=None,
                               quant_act=None,
                               weight_half_shift=False,
-                              kernel_axis_names=None):
+                              kernel_axis_names=None,
+                              train=False,
+                              possibly_use_quantized_vars=False,
+                              quant_type=QuantType.FAKE_QUANT):
     """Create and initialize a flax model with a single DenseAqt layer."""
     dynamic_context = quant_config.DynamicContext(
         update_bounds=False, collect_acts_stats=False)
     layer_kwargs = {
         'kernel_init': kernel_init,
         'features': num_features,
         'use_bias': False,
         'dynamic_context': dynamic_context,
         'paxis_name': 'batch',
-        'train': False,
+        'train': train,
         'dtype': jnp.float32,
-        'kernel_axis_names': kernel_axis_names
+        'kernel_axis_names': kernel_axis_names,
+        'possibly_use_quantized_vars': possibly_use_quantized_vars
     }
     layer_kwargs['hparams'] = flax_layers.DenseAqt.HParams(
         weight_prec=weight_prec,
         quant_act=quant_act,
-        quant_type=QuantType.FAKE_QUANT,
+        quant_type=quant_type,
         weight_quant_granularity=quant_config.QuantGranularity.PER_CHANNEL,
         weight_half_shift=weight_half_shift)
 
     dense_module = flax_layers.DenseAqt(**layer_kwargs)
     initial_state = dense_module.init(
         self.rng_key, jnp.zeros(inputs.shape), padding_mask=None)
     return dense_module, initial_state
@@ -663,15 +664,15 @@
 
     full_range_integer_weights = random.randint(self.rng_key,
                                                 (input_dim, num_features),
                                                 minval, maxval + 1)
 
     # manually set one value in each output dim of weights to be exactly maxval
     full_range_integer_weights = full_range_integer_weights.at[0, :].set(maxval)
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = full_range_integer_weights
     state = flax.core.freeze(state)
     outputs = model.apply(state, inputs, padding_mask=None)
     exp_outputs = jnp.matmul(inputs, state['params']['kernel'])
     onp.testing.assert_array_equal(outputs, exp_outputs)
 
   @parameterized.named_parameters(
@@ -703,15 +704,15 @@
                                                 (input_dim, num_features),
                                                 minval, maxval + 1)
 
     # manually set one value in each output dim of weights to be exactly maxval
     full_range_integer_weights = full_range_integer_weights.at[0, :].set(maxval)
 
     float_scale = jax.random.uniform(self.rng_key, (1, num_features))
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = full_range_integer_weights * float_scale
     state = flax.core.freeze(state)
     outputs = model.apply(state, inputs, padding_mask=None)
     exp_outputs = jnp.matmul(inputs, state['params']['kernel'])
     # TODO(wanglisa): Determine how much noise is expected for following test.
     # We know that the noise should be proportional to the square root of
     # input_dim and inversely proportional to 2**weight_prec.
@@ -741,15 +742,15 @@
   def test_float_weights_should_give_close_output(self, weight_prec):
     inputs = random.uniform(self.rng_key, shape=(2, 3))
     model, state = self.init_model_with_1_layer(
         inputs, num_features=4, weight_prec=weight_prec)
     float_weights = jnp.linspace(-1 / 3, 1 / 3, num=12).reshape((3, 4))
 
     exp_output_without_quant = jnp.matmul(inputs, float_weights)
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = float_weights
     state = flax.core.freeze(state)
     outputs_with_quant = model.apply(state, inputs, padding_mask=None)
     onp.testing.assert_raises(AssertionError, onp.testing.assert_array_equal,
                               outputs_with_quant, exp_output_without_quant)
     test_utils.assert_all_close_prec(exp_output_without_quant,
                                      outputs_with_quant, weight_prec)
@@ -786,33 +787,33 @@
     # also scale the output exactly by the same scale.
 
     inputs = random.uniform(self.rng_key, shape=(2, 3))
     model, state = self.init_model_with_1_layer(
         inputs, num_features=4, weight_prec=weight_prec)
     weights = random.uniform(self.rng_key, shape=(3, 4))
     weight_scale = weight_scale[jnp.newaxis, :]
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = weights
     state = flax.core.freeze(state)
     outputs_without_scaling = model.apply(state, inputs, padding_mask=None)
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = jnp.multiply(weights, weight_scale)
     state = flax.core.freeze(state)
     outputs_with_scaling = model.apply(state, inputs, padding_mask=None)
 
     onp.testing.assert_array_equal(outputs_without_scaling * weight_scale,
                                    outputs_with_scaling)
 
   def test_1_bit_makes_all_weight_equal_to_zero(self):
     inputs = random.uniform(self.rng_key, shape=(2, 3))
     model, state = self.init_model_with_1_layer(
         inputs, num_features=4, weight_prec=1)
     weights = random.uniform(
         self.rng_key, shape=state['params']['kernel'].shape)
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = weights
     state = flax.core.freeze(state)
     outputs = model.apply(state, inputs, padding_mask=None)
     onp.testing.assert_array_equal(outputs, onp.zeros((2, 4)))
 
   # TODO(shivaniagrawal): change mock tests to check for QuantOps than
   # primitives.
@@ -1053,14 +1054,62 @@
         dtype=jnp.float32)
     x = jnp.ones((2, 2))
     state = layer.init(self.rng_key, x, padding_mask=None)
     layer.apply(state, x, padding_mask=None)
     weight_params = mock_quantized_dot_general.call_args[1]['weight_params']
     self.assertEqual(weight_params.axis, axis)
 
+  @parameterized.named_parameters(
+      dict(
+          testcase_name='train_quant',
+          train=True,
+          possibly_use_quantized_vars=True,
+          param_info={
+              'kernel': ['float32', 'embed=3', 'mlp=3'],
+              'qkernel': ['float32', 'embed=3', 'mlp=3'],
+              'qscale': ['float32', 'embed_qscale=1', 'mlp=3']
+          }),
+      dict(
+          testcase_name='inference_quant',
+          train=False,
+          possibly_use_quantized_vars=True,
+          param_info={
+              'qkernel': ['int8', 'embed=3', 'mlp=3'],
+              'qscale': ['float32', 'embed_qscale=1', 'mlp=3']
+          }),
+      dict(
+          testcase_name='train_without_quant',
+          train=True,
+          possibly_use_quantized_vars=False,
+          param_info={'kernel': ['float32', 'embed=3', 'mlp=3']}),
+      dict(
+          testcase_name='inference_without_quant',
+          train=True,
+          possibly_use_quantized_vars=False,
+          param_info={'kernel': ['float32', 'embed=3', 'mlp=3']}),
+  )
+  def test_train_inference_differentiation(self, train,
+                                           possibly_use_quantized_vars,
+                                           param_info):
+    num_features = 3
+    inputs = random.uniform(self.rng_key, shape=(2, 3))
+
+    _, state = self.init_model_with_1_layer(
+        inputs,
+        num_features=num_features,
+        weight_prec=8,
+        train=train,
+        possibly_use_quantized_vars=possibly_use_quantized_vars,
+        kernel_axis_names=('embed', 'mlp'),
+        quant_type=QuantType.AQT)
+
+    self.assertDictEqual(
+        param_dtypes_shapes_axes(state['params'], state['params_axes']),
+        param_info)
+
 
 class EmbedLayerTest(parameterized.TestCase):
   """Tests for AQT Embed layer."""
 
   # TODO(shivaniagrawal): we are not raising error on jax rank
   # promotion. For EmbedAqt tests; in AQT style inputs and output are not be
   # of same shape; require more work to avoid rank promotion.
@@ -1312,51 +1361,50 @@
   def tearDown(self):
     config.update('jax_numpy_rank_promotion', 'warn')
     super(DenseGeneralAqtTest, self).tearDown()
 
   def init_model_with_1_layer(self,
                               inputs,
                               num_features,
-                              axis=(1,),
+                              axis=-1,
                               kernel_init=flax_layers.default_kernel_init,
                               weight_prec=None,
                               weight_half_shift=False,
+                              quant_act=None,
+                              train=False,
                               kernel_axis_names=None,
-                              reshape_kernel=True):
+                              reshape_kernel=True,
+                              possibly_use_quantized_vars=False):
     """Create and initialize a flax model with a single DenseAqt layer."""
     layer_kwargs = {
         'kernel_init': kernel_init,
         'features': num_features,
         'axis': axis,
         'use_bias': False,
-        'train': False,
+        'train': train,
         'dtype': jnp.float32,
         'kernel_axis_names': kernel_axis_names,
         'reshape_kernel': reshape_kernel,
+        'possibly_use_quantized_vars': possibly_use_quantized_vars,
     }
     layer_kwargs['hparams'] = flax_layers.DenseGeneralAqt.HParams(
         weight_prec=weight_prec,
-        quant_act=None,
+        quant_act=quant_act,
         weight_quant_granularity=quant_config.QuantGranularity.PER_CHANNEL,
         weight_half_shift=weight_half_shift)
 
     dense_module = flax_layers.DenseGeneralAqt(**layer_kwargs)
     initial_state = dense_module.init(self.rng_key, jnp.zeros(inputs.shape))
     return dense_module, initial_state
 
+  # DenseGeneral does not support fq version, hence fp quantization isn't
+  # supported either
   @parameterized.named_parameters(
       dict(testcase_name='float', weight_prec=None),
-      dict(
-          testcase_name='quant_fp143_scaled',
-          weight_prec=fp143_scaled,
-      ),
-      dict(
-          testcase_name='quant_fp143',
-          weight_prec=fp143_unscaled,
-      ),
+
       dict(testcase_name='quant_8bit', weight_prec=8),
       dict(testcase_name='quant_4bit', weight_prec=4),
       dict(testcase_name='quant_4bit_no_reshape', weight_prec=4, reshape=False),
       dict(testcase_name='quant_2bit', weight_prec=2),
   )
   def test_ones_weights_should_give_precise_output(self,
                                                    weight_prec,
@@ -1428,22 +1476,63 @@
 
     full_range_integer_weights = random.randint(self.rng_key,
                                                 (input_dim, num_features),
                                                 minval, maxval + 1)
 
     # manually set one value in each output dim of weights to be exactly maxval
     full_range_integer_weights = full_range_integer_weights.at[0, :].set(maxval)
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = full_range_integer_weights
     state = flax.core.freeze(state)
     outputs = model.apply(state, inputs)
     exp_outputs = jnp.matmul(inputs, state['params']['kernel'])
     onp.testing.assert_array_equal(outputs, exp_outputs)
 
   @parameterized.named_parameters(
+      dict(
+          testcase_name='densegeneral_quant_8bit',
+          weight_prec=8,
+          expected_output=[[-0.08770747, -0.00193817, 0.08321345, 0.16902271],
+                           [-0.2838632, -0.1654416, -0.04855134, 0.06976502]]),
+      dict(
+          testcase_name='densegeneral_quant_4bit',
+          weight_prec=4,
+          expected_output=[[-0.09499891, -0.016027, 0.09432255, 0.17474438],
+                           [-0.29012504, -0.17881386, -0.02733358,
+                            0.08016007]]),
+      dict(
+          testcase_name='densegeneral_quant_2bit',
+          weight_prec=2,
+          expected_output=[[-0.19150016, 0.0456724, 0.0456724, 0.24732196],
+                           [-0.29805943, -0.12025267, -0.12025267,
+                            0.15108395]]),
+  )
+  def test_float_weights_regression_test(self, weight_prec, expected_output):
+    inputs = random.uniform(self.rng_key, shape=(2, 3))
+    model, state = self.init_model_with_1_layer(
+        inputs, num_features=4, weight_prec=weight_prec)
+    float_weights = jnp.linspace(-1 / 3, 1 / 3, num=12).reshape((3, 4))
+
+    exp_output_without_quant = jnp.matmul(inputs, float_weights)
+    state = flax.core.unfreeze(state)
+    state['params']['kernel'] = float_weights
+    state = flax.core.freeze(state)
+    outputs_with_quant = model.apply(state, inputs)
+    onp.testing.assert_raises(AssertionError, onp.testing.assert_array_equal,
+                              outputs_with_quant, exp_output_without_quant)
+    onp.testing.assert_allclose(outputs_with_quant, expected_output, rtol=1e-5)
+    onp.testing.assert_allclose(
+        exp_output_without_quant,
+        [[-0.08814345, -0.00231601, 0.0835114, 0.16933881],
+         [-0.2836182, -0.16580023, -0.04798227, 0.06983571]],
+        rtol=1e-5)
+    test_utils.assert_all_close_prec(exp_output_without_quant,
+                                     outputs_with_quant, weight_prec)
+
+  @parameterized.named_parameters(
       # TODO(shivaniagrawal): this test is flaky and fails with rtol=0.0004
       # with given rtol=0.0001
       # dict(
       #     testcase_name='dense_quant_8bit',
       #     layer_class=flax_layers.DenseAqt,
       #     weight_prec=8),
       dict(testcase_name='dense_quant_4bit', weight_prec=4),
@@ -1468,15 +1557,15 @@
                                                 (input_dim, num_features),
                                                 minval, maxval + 1)
 
     # manually set one value in each output dim of weights to be exactly maxval
     full_range_integer_weights = full_range_integer_weights.at[0, :].set(maxval)
 
     float_scale = jax.random.uniform(self.rng_key, (1, num_features))
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = full_range_integer_weights * float_scale
     state = flax.core.freeze(state)
     outputs = model.apply(state, inputs)
     exp_outputs = jnp.matmul(inputs, state['params']['kernel'])
     # TODO(wanglisa): Determine how much noise is expected for following test.
     # We know that the noise should be proportional to the square root of
     # input_dim and inversely proportional to 2**weight_prec.
@@ -1485,19 +1574,35 @@
     tol_const = 8e-04
     onp.testing.assert_allclose(
         outputs,
         exp_outputs,
         rtol=jnp.sqrt(input_dim) * 2**(-weight_prec) * tol_const)
 
   @parameterized.named_parameters(
-      dict(
-          testcase_name='dense_quant_fp143_scaled',
-          weight_prec=fp143_scaled,
-          weight_scale=onp.array([1, 2, 4, 8]),
-      ),
+      dict(testcase_name='dense_quant_4bit', weight_prec=4),
+      dict(testcase_name='dense_quant_2bit', weight_prec=2),
+  )
+  def test_float_weights_should_give_close_output(self, weight_prec):
+    inputs = random.uniform(self.rng_key, shape=(2, 3))
+    model, state = self.init_model_with_1_layer(
+        inputs, num_features=4, weight_prec=weight_prec)
+    float_weights = jnp.linspace(-1 / 3, 1 / 3, num=12).reshape((3, 4))
+
+    exp_output_without_quant = jnp.matmul(inputs, float_weights)
+    state = flax.core.unfreeze(state)
+    state['params']['kernel'] = float_weights
+    state = flax.core.freeze(state)
+    outputs_with_quant = model.apply(state, inputs)
+    onp.testing.assert_raises(AssertionError, onp.testing.assert_array_equal,
+                              outputs_with_quant, exp_output_without_quant)
+
+    test_utils.assert_all_close_prec(exp_output_without_quant,
+                                     outputs_with_quant, weight_prec)
+
+  @parameterized.named_parameters(
       dict(
           testcase_name='dense_quant_8bit',
           weight_prec=8,
           weight_scale=onp.array([1, 2, 4, 8])),
       dict(
           testcase_name='dense_quant_4bit',
           weight_prec=4,
@@ -1513,59 +1618,108 @@
     # also scale the output exactly by the same scale.
 
     inputs = random.uniform(self.rng_key, shape=(2, 3))
     model, state = self.init_model_with_1_layer(
         inputs, num_features=4, axis=(1,), weight_prec=weight_prec)
     weights = random.uniform(self.rng_key, shape=(3, 4))
     weight_scale = weight_scale[jnp.newaxis, :]
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = weights
     state = flax.core.freeze(state)
     outputs_without_scaling = model.apply(state, inputs)
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = jnp.multiply(weights, weight_scale)
     state = flax.core.freeze(state)
     outputs_with_scaling = model.apply(state, inputs)
 
     onp.testing.assert_array_equal(outputs_without_scaling * weight_scale,
                                    outputs_with_scaling)
 
   def test_1_bit_makes_all_weight_equal_to_zero(self):
     inputs = random.uniform(self.rng_key, shape=(2, 3))
     model, state = self.init_model_with_1_layer(
         inputs, num_features=4, axis=(1,), weight_prec=1)
     weights = random.uniform(
         self.rng_key, shape=state['params']['kernel'].shape)
-    state = state.unfreeze()
+    state = flax.core.unfreeze(state)
     state['params']['kernel'] = weights
     state = flax.core.freeze(state)
     outputs = model.apply(state, inputs)
     onp.testing.assert_array_equal(outputs, onp.zeros((2, 4)))
 
   # TODO(shivaniagrawal): change mock tests to check for QuantOps than
   # primitives.
   @parameterized.named_parameters(
-      dict(testcase_name='dense_quant_8bit', weight_prec=8),
-      dict(testcase_name='dense_quant_4bit', weight_prec=4),
-      dict(testcase_name='dense_quant_2bit', weight_prec=2),
+      dict(
+          testcase_name='dense_weight_quant_8bit',
+          weight_prec=8,
+          acts_prec=None),
+      dict(
+          testcase_name='dense_weight_quant_4bit',
+          weight_prec=4,
+          acts_prec=None),
+      dict(
+          testcase_name='dense_weight_quant_2bit',
+          weight_prec=2,
+          acts_prec=None),
+      dict(
+          testcase_name='dense_signed_input_quant_8bit',
+          weight_prec=None,
+          acts_prec=8),
+      dict(
+          testcase_name='dense_signed_input_quant_4bit',
+          weight_prec=None,
+          acts_prec=4),
+      dict(
+          testcase_name='dense_signed_input_quant_2bit',
+          weight_prec=None,
+          acts_prec=2),
+      dict(
+          testcase_name='dense_signed_input_auto_quant_8bit',
+          weight_prec=None,
+          acts_prec=8,
+          fixed_bounds=False),
+      dict(
+          testcase_name='dense_signed_input_auto_quant_4bit',
+          weight_prec=None,
+          acts_prec=4,
+          fixed_bounds=False),
   )
   @mock.patch.object(primitives, 'round_with_gradient')
   @mock.patch.object(primitives, 'floor_with_gradient')
-  def test_quantized_weights_should_call_clip_and_round(self,
-                                                        floor_with_gradient,
-                                                        round_with_gradient,
-                                                        weight_prec):
+  def test_quantized_weights_and_symmetrics_acts_should_call_clip_and_round(
+      self,
+      floor_with_gradient,
+      round_with_gradient,
+      weight_prec,
+      acts_prec,
+      fixed_bounds=False):
 
     round_with_gradient.side_effect = lambda x: x
     floor_with_gradient.side_effect = lambda x: x
 
+    if fixed_bounds:
+      bounds = 6.0
+    else:
+      bounds = get_bounds.DynamicBounds.Hyper(
+          granularity=quant_config.QuantGranularity.PER_CHANNEL)
+    quant_act = quantization.QuantOps.ActHParams(
+        input_distribution=QuantOps.ActHParams.InputDistribution.SYMMETRIC,
+        prec=acts_prec,
+        bounds=bounds,
+        half_shift=False)
     num_features = 4
     inputs = jnp.ones((2, 3), dtype=jnp.float32)
     model, state = self.init_model_with_1_layer(
-        inputs, num_features, weight_prec=weight_prec, weight_half_shift=False)
+        inputs,
+        num_features,
+        weight_prec=weight_prec,
+        weight_half_shift=False,
+        quant_act=quant_act,
+    )
 
     round_with_gradient.assert_called_with(mock.ANY)
     self.assertEqual(round_with_gradient.call_count, 1)
     floor_with_gradient.assert_not_called()
 
     round_with_gradient.reset_mock()
     floor_with_gradient.reset_mock()
@@ -1586,14 +1740,181 @@
     floor_with_gradient.side_effect = lambda x: x
     inputs = jnp.ones((2, 3), dtype=jnp.float32)
     model, state = self.init_model_with_1_layer(inputs, num_features=4)
     _ = model.apply(state, inputs)
     round_with_gradient.assert_not_called()
     floor_with_gradient.assert_not_called()
 
+  # TODO(shivaniagrawal): change mock tests to check for QuantOps than
+  # primitives.
+  @parameterized.named_parameters(
+      dict(
+          testcase_name='dense_pos_quant_8bit',
+          pos_inputs_prec=8,
+          fixed_bounds=True),
+      dict(
+          testcase_name='dense_pos_quant_4bit',
+          pos_inputs_prec=4,
+          fixed_bounds=True),
+      dict(
+          testcase_name='dense_pos_quant_8bit_auto_clip',
+          pos_inputs_prec=8,
+          fixed_bounds=False),
+      dict(
+          testcase_name='dense_pos_quant_4bit_auto_clip',
+          pos_inputs_prec=4,
+          fixed_bounds=False),
+  )
+  @mock.patch.object(primitives, 'round_with_gradient')
+  @mock.patch.object(primitives, 'floor_with_gradient')
+  def test_quantized_inputs_should_call_clip_and_round(self,
+                                                       floor_with_gradient,
+                                                       round_with_gradient,
+                                                       pos_inputs_prec,
+                                                       fixed_bounds):
+
+    round_with_gradient.side_effect = lambda x: x
+    floor_with_gradient.side_effect = lambda x: x
+    if fixed_bounds:
+      bounds = 6.0
+    else:
+      bounds = get_bounds.DynamicBounds.Hyper(
+          granularity=quant_config.QuantGranularity.PER_CHANNEL)
+    quant_act = quantization.QuantOps.ActHParams(
+        input_distribution=QuantOps.ActHParams.InputDistribution.POSITIVE,
+        prec=pos_inputs_prec,
+        bounds=bounds,
+        half_shift=False)
+    inputs = jnp.ones((2, 3), dtype=jnp.float32)
+    model, init_state = self.init_model_with_1_layer(
+        inputs,
+        num_features=4,
+        weight_prec=None,
+        quant_act=quant_act,
+        weight_half_shift=False)
+    floor_with_gradient.assert_called_with(mock.ANY)
+    self.assertEqual(floor_with_gradient.call_count, 1)
+    round_with_gradient.assert_not_called()
+
+    round_with_gradient.reset_mock()
+    floor_with_gradient.reset_mock()
+
+    model.apply(init_state, inputs)
+
+    floor_with_gradient.assert_called_with(mock.ANY)
+    self.assertEqual(floor_with_gradient.call_count, 1)
+    round_with_gradient.assert_not_called()
+
+  @parameterized.parameters(
+      dict(granularity=quant_config.QuantGranularity.PER_CHANNEL, axis=(0, 1)),
+      dict(granularity=quant_config.QuantGranularity.PER_TENSOR, axis=None))
+  @mock.patch.object(quantization, 'flaxformer_dot_general')
+  @mock.patch.object(shape_utils, 'assert_shapes_equal')
+  def test_weights_quant_granularity(self, _, mock_flaxformer_dot_general,
+                                     granularity, axis):
+    hparams = flax_layers.DenseGeneralAqt.HParams(
+        weight_prec=8,
+        quant_act=None,
+        weight_quant_granularity=granularity,
+        weight_half_shift=False)
+    layer = flax_layers.DenseGeneralAqt(
+        features=3,
+        axis=(1, 2),
+        hparams=hparams,
+        train=False,
+        use_bias=False,
+        dtype=jnp.float32)
+    x = jnp.ones((2, 3, 4))
+    state = layer.init(self.rng_key, x)
+    layer.apply(state, x)
+    weight_params = mock_flaxformer_dot_general.call_args[1]['weight_params']
+    self.assertEqual(weight_params.axis, axis)
+
+  @parameterized.parameters(
+      dict(
+          granularity=quant_config.QuantGranularity.PER_CHANNEL,
+          quant_axis=(1, 2)),
+      dict(
+          granularity=quant_config.QuantGranularity.PER_TENSOR,
+          quant_axis=None))
+  @mock.patch.object(quantization, 'flaxformer_dot_general')
+  @mock.patch.object(shape_utils, 'assert_shapes_equal')
+  def test_acts_quant_granularity(self, _, mock_flaxformer_dot_general,
+                                  granularity, quant_axis):
+    bounds = get_bounds.DynamicBounds.Hyper(granularity=granularity)
+    quant_act = quantization.QuantOps.ActHParams(
+        input_distribution=QuantOps.ActHParams.InputDistribution.POSITIVE,
+        prec=8,
+        bounds=bounds,
+        half_shift=False)
+    hparams = flax_layers.DenseGeneralAqt.HParams(
+        weight_prec=None,
+        quant_act=quant_act,
+        weight_quant_granularity=quant_config.QuantGranularity.PER_TENSOR,
+        weight_half_shift=False)
+    layer = flax_layers.DenseGeneralAqt(
+        features=2,
+        axis=(1, 2),
+        hparams=hparams,
+        train=False,
+        use_bias=False,
+        dtype=jnp.float32)
+    x = jnp.ones((2, 3, 4))
+    state = layer.init(self.rng_key, x)
+    layer.apply(state, x)
+    bounds_params = mock_flaxformer_dot_general.call_args[1]['bounds_params']
+    self.assertEqual(bounds_params.quant_axis, quant_axis)
+
+  @parameterized.named_parameters(
+      dict(
+          testcase_name='train_quant',
+          train=True,
+          possibly_use_quantized_vars=True,
+          param_info={
+              'kernel': ['float32', 'embed=3', 'mlp=3'],
+              'qkernel': ['float32', 'embed=3', 'mlp=3'],
+              'qscale': ['float32', 'embed_qscale=1', 'mlp=3']
+          }),
+      dict(
+          testcase_name='inference_quant',
+          train=False,
+          possibly_use_quantized_vars=True,
+          param_info={
+              'qkernel': ['int8', 'embed=3', 'mlp=3'],
+              'qscale': ['float32', 'embed_qscale=1', 'mlp=3']
+          }),
+      dict(
+          testcase_name='train_without_quant',
+          train=True,
+          possibly_use_quantized_vars=False,
+          param_info={'kernel': ['float32', 'embed=3', 'mlp=3']}),
+      dict(
+          testcase_name='inference_without_quant',
+          train=True,
+          possibly_use_quantized_vars=False,
+          param_info={'kernel': ['float32', 'embed=3', 'mlp=3']}),
+  )
+  def test_train_inference_differentiation(self, train,
+                                           possibly_use_quantized_vars,
+                                           param_info):
+    num_features = 3
+    inputs = random.uniform(self.rng_key, shape=(2, 3))
+
+    _, state = self.init_model_with_1_layer(
+        inputs,
+        num_features=num_features,
+        weight_prec=8,
+        train=train,
+        possibly_use_quantized_vars=possibly_use_quantized_vars,
+        kernel_axis_names=('embed', 'mlp'))
+
+    self.assertDictEqual(
+        param_dtypes_shapes_axes(state['params'], state['params_axes']),
+        param_info)
+
 
 class DenseGeneralTest(parameterized.TestCase):
 
   # pylint: disable=unused-argument
   def _mock_initializer(self, key, shape, dtype=jnp.float_, val=1.0):  # pylint: disable=g-unreachable-test-method
     return jnp.ones(shape, dtypes.canonicalize_dtype(dtype)) * val
   # pylint: enable=unused-argument
@@ -1647,18 +1968,14 @@
         bias_init=initializers.ones,
         kernel_axis_names=('a', 'b', 'c'),
     )
     y, variables = model.init_with_output(rng, x)
     # We transform the last input dimension to two output dimensions (2, 2).
     onp.testing.assert_allclose(y, onp.full((1, 2, 2), 3.))
 
-    # The output sharding dimensions have been collapsed.
-    sharding.check_params_and_axis_names_match(variables)
-    self.assertEqual(variables['params_axes']['kernel_axes'],
-                     sharding.axis_names('a', 'b * c'))
 
   def test_dense_general_two_axes(self):
     rng = random.PRNGKey(0)
     x = jnp.ones((1, 2, 2))
     model = flax_layers.DenseGeneralAqt(
         hparams=self.hparams,
         train=False,
@@ -1669,15 +1986,11 @@
         bias_init=initializers.ones,
         kernel_axis_names=('a', 'b', 'c'),
     )
     y, variables = model.init_with_output(rng, x)
     # We transform the last two input dimensions (2, 2) to one output dimension.
     onp.testing.assert_allclose(y, onp.full((1, 3), 4.))
 
-    # The input sharding dimensions have been collapsed.
-    sharding.check_params_and_axis_names_match(variables)
-    self.assertEqual(variables['params_axes']['kernel_axes'],
-                     sharding.axis_names('a * b', 'c'))
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/quantization.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/quantization.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 # 'vector unit'.
 SCALE_DTYPE = jnp.float32
 
 dataclass = flax_struct.dataclass if not typing.TYPE_CHECKING else dataclasses.dataclass
 
 # ActBounds can be an Jax array of floats with a shape that is broadcastable to
 # the shape of activation tensors.
-ActsBoundT = Union[float, jnp.ndarray, get_bounds.GetBounds.Hyper, None]
+ActsBoundT = Union[float, jnp.ndarray, get_bounds.GetBounds.Hyper,
+                   get_bounds.DynamicBounds.Hyper, None]
 
 
 @dataclass
 class _FloatQuant:
   """Parameters for floating-point quantization.
 
   Floating-point quantization refers to degraded floating-point precision
@@ -270,15 +271,15 @@
       bounds += jnp.finfo(SCALE_DTYPE).eps  # to avoid div by 0
     scale = primitives.signed_int_bound(
         prec=prec, half_shift=half_shift) / bounds
     # NOTE: stop_gradient is needed here to prevent gradient flow through scale
     # when scale is not a constant, but computed as a function of activations or
     # weights.
     scale = lax.stop_gradient(scale)
-    return cls(
+    return cls(  # pytype: disable=wrong-arg-types  # jax-ndarray
         prec=prec,
         scale=scale,
         symmetric=True,
         bounds=initial_bounds,
         half_shift=half_shift)
 
   @classmethod
@@ -297,15 +298,15 @@
     bounds = jnp.asarray(bounds, SCALE_DTYPE)
     if not DISABLE_EPSILON_IN_SCALE_FUN_FOR_TESTING:
       bounds += jnp.finfo(SCALE_DTYPE).eps  # to avoid div by 0
     scale = primitives.unsigned_int_bound(prec=prec) / bounds
     # NOTE: stop_gradient is needed here to prevent gradient flow through scale
     # when scale is not a constant, but computed as a function of activations.
     scale = lax.stop_gradient(scale)
-    return cls(
+    return cls(  # pytype: disable=wrong-arg-types  # jax-ndarray
         prec=prec,
         scale=scale,
         symmetric=False,
         bounds=initial_bounds,
         half_shift=False)  # disable half_shift for positive distribution
 
   def assert_scale_shape_is(self, *, shape: Union[int, Tuple[int, ...]]):
@@ -460,21 +461,23 @@
 
     return weight_rescaled
 
   # TODO(malmaud): rename 'input' to activation here and elsewhere in this file.
   @classmethod
   def create_input_ops(
       cls, inputs: jnp.ndarray, *, hparams: ActHParams,
-      get_bounds_params: Optional[get_bounds.GetBounds.Params]) -> 'QuantOps':
+      bounds_params: Union[get_bounds.GetBounds.Params,
+                           get_bounds.DynamicBounds.Params, None]
+  ) -> 'QuantOps':
     """Create a QuantOps that can quantize and dequantize an activation tensor.
 
     Args:
       inputs: The inputs to quantize.
       hparams: Input hyperparameter (ActHParams).
-      get_bounds_params: GetBoundsParams. Parameters for GetBounds.
+      bounds_params: BoundsParams. Parameters for GetBounds or DynamicBounds.
 
     Returns:
       Quantized and rescaled inputs using fake quant approach.
     """
 
     # TODO(shivaniagrawal): investigate why pytype allows types other than
     # ActsBoundT.
@@ -495,70 +498,86 @@
     # will cause clip_bounds will be a tensor of all '-1', which we will check
     # for in a lax.cond call below.
 
     # TODO(malmaud): Refactor code to separate bounds calculation from tracking
     # activation statistics to avoid the need to rely on special bounds values
     # when disabling quantization.
     if isinstance(hparams.bounds, get_bounds.GetBounds.Hyper):
-      if not get_bounds_params:
+      if not bounds_params and not isinstance(bounds_params,
+                                              get_bounds.GetBounds.Params):
         raise ValueError(
             'act_hparams.bounds is of type GetBounds.Hyper, user must '
-            'provide get_bounds_params, parameters for GetBounds.')
+            'provide bounds_params, parameters for GetBounds.')
       clip_bounds = get_bounds.GetBounds(
-          hyper=hparams.bounds, name=get_bounds_params.module_name)(
+          hyper=hparams.bounds, name=bounds_params.module_name)(
+              inputs,
+              bounds_params=bounds_params,
+          )
+    elif isinstance(hparams.bounds, get_bounds.DynamicBounds.Hyper):
+      if not bounds_params and not isinstance(bounds_params,
+                                              get_bounds.DynamicBounds.Params):
+        raise ValueError(
+            'act_hparams.bounds is of type DynamicBounds.Hyper, user must '
+            'provide bounds_params, parameters for DynamicBounds.')
+      clip_bounds = get_bounds.DynamicBounds(
+          hyper=hparams.bounds, name=bounds_params.module_name)(
               inputs,
-              bounds_params=get_bounds_params,
+              bounds_params=bounds_params,
           )
+
     elif isinstance(hparams.bounds, (float, jnp.ndarray)):
       clip_bounds = hparams.bounds
     else:
       assert False, (
           '%s is not a valid type for hparams.bounds, should be float, a list '
-          'of floats, or GetBounds.Hyper.' % (type(hparams.bounds)))
+          'of floats, DynamicBounds.Hyper or GetBounds.Hyper.' %
+          (type(hparams.bounds)))
 
     if isinstance(hparams.prec, _FloatQuant):
       ops = cls.create_symmetric_fp(bounds=clip_bounds, fp_quant=hparams.prec)
     elif hparams.input_distribution == cls.ActHParams.InputDistribution.SYMMETRIC:
       ops = cls.create_symmetric(
           bounds=clip_bounds, prec=hparams.prec, half_shift=hparams.half_shift)
     elif hparams.input_distribution == cls.ActHParams.InputDistribution.POSITIVE:
       ops = cls.create_positive(bounds=clip_bounds, prec=hparams.prec)
     else:
       assert False, "can't happen."
 
-    if get_bounds_params and get_bounds_params.expected_bounds_shape is not None:
+    if bounds_params and bounds_params.expected_bounds_shape is not None:
       if isinstance(hparams.bounds, get_bounds.GetBounds.Hyper):
-        ops.assert_scale_shape_is(shape=get_bounds_params.expected_bounds_shape)
+        ops.assert_scale_shape_is(shape=bounds_params.expected_bounds_shape)
       else:
         logging.info(
             'Ignoring value of argument expected_scale_shape. Scale for fixed '
             'bounds would be scalar.')
     return ops
 
   @classmethod
   def create_inputs_fake_quant(
       cls, inputs: jnp.ndarray, *, hparams: ActHParams,
-      get_bounds_params: Optional[get_bounds.GetBounds.Params]) -> jnp.ndarray:
+      bounds_params: Union[None, get_bounds.GetBounds.Params,
+                           get_bounds.DynamicBounds.Params]
+  ) -> jnp.ndarray:
     """Quantize input with fake quant approach.
 
     Args:
       inputs: The inputs to quantize.
       hparams: Input hyperparameter (ActHParams).
-      get_bounds_params: GetBoundsParams. Parameters for GetBounds.
+      bounds_params: GetBounds or DynamicBounds Params.
 
     Returns:
       Quantized and rescaled inputs using fake quant approach.
     """
 
     if hparams.bounds is None or hparams.prec is None:
       # TODO(lew): support bound-clipping without quantization
       return inputs
 
     ops = cls.create_input_ops(
-        inputs, hparams=hparams, get_bounds_params=get_bounds_params)
+        inputs, hparams=hparams, bounds_params=bounds_params)
 
     quantized_inputs = ops.fake_quant(inputs, quantized_type=SCALE_DTYPE)
     return lax.cond(ops.should_quantize(), lambda _: quantized_inputs,
                     lambda _: inputs, None)
 
   # When using GetBounds quantization (if hparams.bounds is an instance of
   # GetBounds.Hyper), if we want to disable quantization but continue to
@@ -611,15 +630,16 @@
 
 def quantized_dot(*,
                   w: jnp.ndarray,
                   act: jnp.ndarray,
                   quant_type: QuantType,
                   weight_params: QuantOps.WeightParams,
                   act_hparams: Optional[QuantOps.ActHParams],
-                  get_bounds_params: Optional[get_bounds.GetBounds.Params],
+                  bounds_params: Union[get_bounds.GetBounds.Params,
+                                       get_bounds.DynamicBounds.Params, None],
                   prefer_int8_to_int32_dot: bool,
                   dot_precision: Optional[PrecisionType] = None) -> jnp.ndarray:
   """LAX dot with optionally quantized weights and activations.
 
   Wraps LAX's `Dot
   <https://github.com/google/jax/blob/f65a327c764406db45e95048dfe09209d8ef6d37/jax/_src/lax/lax.py#L632`_
   operator.
@@ -628,16 +648,16 @@
     w: an array representing weights
     act: an array representing activations
     quant_type: quantization strategy
     weight_params: QuantOps.WeighstParams instance for describing weights
       quantization.
     act_hparams: Optional activation quantization hyperparamers; instance of
       QuantOps.ActHParams. None would mean no activation quantization.
-    get_bounds_params: Optional get bounds params for auto activation
-      quantization; instance of GetBounds.Params.
+    bounds_params: Optional bounds params for auto activation
+      quantization; instance of GetBounds.Params or DynamicBounds.Params.
     prefer_int8_to_int32_dot:  Whether to feed lax.dot inputs with an int8 dtype
       and accumulate to int32 dtype if quantizing to 8bits or 4bits. If False,
       inputs are always foating-point.
     dot_precision: Optional. Either ``None``, which means the default precision
       for the backend, or a ``lax.Precision`` enum value (``Precision.DEFAULT``,
       ``Precision.HIGH`` or ``Precision.HIGHEST``).
 
@@ -669,15 +689,15 @@
   dot_dimension_numbers = (((act.ndim - 1,), (0,)), ((), ()))
   return quantized_dot_general(
       w=w,
       act=act,
       quant_type=quant_type,
       weight_params=weight_params,
       act_hparams=act_hparams,
-      get_bounds_params=get_bounds_params,
+      bounds_params=bounds_params,
       prefer_int8_to_int32_dot=prefer_int8_to_int32_dot,
       dimension_numbers=dot_dimension_numbers,
       dot_precision=dot_precision)
 
 
 def _canonicalize_feature_axes(axis: Union[int, Tuple[int, ...]],
                                ndims: int) -> Tuple[int, ...]:
@@ -705,20 +725,62 @@
 
 
 def flaxformer_dot_general(*,
                            act: jnp.ndarray,
                            w: Optional[jnp.ndarray],
                            dimension_numbers: lax.DotDimensionNumbers,
                            weight_params: QuantOps.WeightParams,
+                           act_hparams: Optional[QuantOps.ActHParams],
+                           bounds_params: Union[None,
+                                                get_bounds.DynamicBounds.Params,
+                                                get_bounds.GetBounds.Params],
                            dot_precision: Optional[PrecisionType] = None,
+                           prefer_int8_to_int32_dot: bool = True,
                            quant_w: Optional[QuantW] = None) -> jnp.ndarray:
   """Flaxformer dot general with optionally quantized weights and activations."""
   input_dtype = act.dtype
+  is_weight_quantized = False
+  is_act_quantized = False
+  (axis, _), (_, _) = dimension_numbers
+  act_scale_shape = tuple(
+      [act.shape[dim] if dim not in axis else 1 for dim in range(0, act.ndim)])
+  if w is not None:
+    weight_scale_shape = (1,) * len(axis) + tuple(
+        [w.shape[dim] for dim in range(len(axis), w.ndim)])
+  elif quant_w is not None:
+    weight_scale_shape = (1,) * len(axis) + tuple([
+        quant_w.quantized_w.shape[dim]
+        for dim in range(len(axis), quant_w.quantized_w.ndim)
+    ])
+  else:
+    raise ValueError('Either of w or quant_w must be not None')
+
+  if act_hparams is not None and act_hparams.prec is not None:
+    is_act_quantized = True
+    # Calculate 's', the per-column scale factor on activations.
+    act_op = QuantOps.create_input_ops(
+        act, hparams=act_hparams, bounds_params=bounds_params)
+    act_quantized = act_op.to_quantized(act, dtype=input_dtype)
+
+    # Now calculate s^-1.  First we extract s, the activation scale factor,
+    # into a  variable called 'act_scale'. We extract it from 'act_op', the
+    # QuantOps instance that calculated the scale factors for the activation
+    # matrix.
+    act_scale = act_op._scale.astype(input_dtype)  # pylint: disable=protected-access
+    if act_scale.ndim == 0:
+      act_scale = act_scale * jnp.ones(act_scale_shape, act_scale.dtype)
+  else:
+    # In this case, activations are not being quantized; only weights. There
+    # is no need to absorb activation scales into the rows of the weight
+    # matrix so 'w_scaled_rows' can just be set to the original weight matrix.
+    act_quantized = act
+    act_scale = jnp.ones(act_scale_shape, act.dtype)
 
   if weight_params is not None and weight_params.prec is not None:
+    is_weight_quantized = True
     if quant_w is not None:
       weight_quantized = quant_w.quantized_w.astype(input_dtype)
       weight_scale = quant_w.scale
     else:
       # Calculate 'r' from (s^-1) * w
       weight_op = QuantOps.create_weights_ops(w, weight_params=weight_params)
       weight_scale = weight_op._scale.astype(input_dtype)  # pylint: disable=protected-access
@@ -731,49 +793,75 @@
       # TODO(malmaud): See comment on 'act_op.to_quantized' above, which
       # applies here as well.
       weight_quantized = weight_op.to_quantized(w, dtype=input_dtype)
   else:
     assert w is not None, ('w can not be None if weight quantization is not '
                            'specified.')
     weight_quantized = w
+    weight_scale = jnp.ones(weight_scale_shape, w.dtype)
 
   weight_prec = None if weight_params is None else weight_params.prec
   metadata_context = contextlib.suppress()
   if flags.FLAGS.metadata_enabled:
     metadata_context = compute_cost_utils.DotMetadataMonkeyPatch(
         lhs_prec=None, rhs_prec=weight_prec, rhs_is_weight=True)
   # Use metadata context to annotate op metadata with quantization info
 
+  # TODO(shivaniagrawal): this is duplicated code with quantized_dot that can
+  # be de-duplicated.
   # To decide whether to use an integer-domain dot operation, we first check
   # if the static quantization parameters are compatible with it by seeing if
   # they request that both inputs be quantized 8bits or less. Then check if
   # the dynamic parameters are compatible with it. ie, in a training run with
   # quantization enabled, are we past the activation start step yet.
 
   # We also do not use int8_to_int32_dot if activation has positive
   # distribution and prec=8, since we would not be able to fit uint8 range in
   # int8.
   # TODO(shivaniagrawal): A proper solution for this would be to have mixed
   # dot(uint8, int8) -> int32 in XLA.
 
+  act_prec = None if act_hparams is None else act_hparams.prec
+  act_has_symm_distribution = act_hparams is not None and (
+      act_hparams.input_distribution
+      == QuantOps.ActHParams.InputDistribution.SYMMETRIC)
+  weight_prec = None if weight_params is None else weight_params.prec
+
+  # To decide whether to use an integer-domain dot operation, we first check
+  # if the static quantization parameters are compatible with it by seeing if
+  # they request that both inputs be quantized 8bits or less. Then check if
+  # the dynamic parameters are compatible with it. ie, in a training run with
+  # quantization enabled, are we past the activation start step yet.
+
+  # We also do not use int8_to_int32_dot if activation has positive
+  # distribution and prec=8, since we would not be able to fit uint8 range in
+  # int8.
+  # TODO(shivaniagrawal): A proper solution for this would be to have mixed
+  # dot(uint8, int8) -> int32 in XLA.
+  weight_fits_in_int8 = is_weight_quantized and (weight_prec is not None and
+                                                 weight_prec <= 8)
+  # is_act_quantized might be an instance of a Jax tracer instead of a
+  # Python boolean since it is generally computed from a dynamic input to a
+  # JITted Jax function. Thus we use '&' instead of 'and'.
+  act_prec_fits_int8 = act_prec is not None and (
+      (act_prec == 8 and act_has_symm_distribution) or (act_prec < 8))
+  act_fits_in_int8 = is_act_quantized & act_prec_fits_int8
+  use_int8_to_int32_dot = prefer_int8_to_int32_dot & weight_fits_in_int8 & act_fits_in_int8
+
   with metadata_context:
     # Calculate matmul(...)
     # we are not quantizing activations yet, hence not using int8 matmul
-    out_quantized = lax.dot_general(
-        act,
+    out_quantized = dot_general_aqt(
+        act_quantized,
         weight_quantized,
         dimension_numbers=dimension_numbers,
-        precision=dot_precision)
+        dot_precision=dot_precision,
+        use_int8_to_int32_dot=use_int8_to_int32_dot)
 
-  if weight_params is not None and weight_params.prec is not None:
-    (axis, _), (_, _) = dimension_numbers
-    act_scale_shape = tuple([
-        act.shape[dim] if dim not in axis else 1 for dim in range(0, act.ndim)
-    ])
-    act_scale = jnp.ones(act_scale_shape, act.dtype)
+  if is_weight_quantized or is_act_quantized:
 
     inv_scale = lax.dot_general(
         (1 / act_scale),
         (1 / weight_scale),
         dimension_numbers=dimension_numbers,
     )
     return out_quantized * inv_scale
@@ -784,16 +872,17 @@
 # TODO(shivaniagrawal): extend it for generic dot_dimenson_numbers
 def quantized_dot_general(*,
                           w: Optional[jnp.ndarray],
                           act: jnp.ndarray,
                           quant_type: QuantType,
                           weight_params: QuantOps.WeightParams,
                           act_hparams: Optional[QuantOps.ActHParams],
-                          get_bounds_params: Optional[
-                              get_bounds.GetBounds.Params],
+                          bounds_params: Union[None,
+                                               get_bounds.GetBounds.Params,
+                                               get_bounds.DynamicBounds.Params],
                           prefer_int8_to_int32_dot: bool,
                           dimension_numbers: lax.DotDimensionNumbers,
                           dot_precision: Optional[PrecisionType] = None,
                           quant_w: Optional[QuantW] = None) -> jnp.ndarray:
   """LAX dot general with optionally quantized weights and activations.
 
   Wraps LAX's `Dot General
@@ -803,16 +892,16 @@
     w: an array representing weights
     act: an array representing activations
     quant_type: quantization strategy
     weight_params: QuantOps.WeighstParams instance for describing weights
       quantization.
     act_hparams: Optional activation quantization hyperparamers; instance of
       QuantOps.ActHParams. None would mean no activation quantization.
-    get_bounds_params: Optional get bounds params for auto activation
-      quantization; instance of GetBounds.Params.
+    bounds_params: Optional bounds params for auto activation
+      quantization; instance of GetBounds.Params or DynamicBounds.Params.
     prefer_int8_to_int32_dot:  Whether to feed lax.dot inputs with an int8 dtype
       and accumulate to int32 dtype if quantizing to 8bits or 4bits. If False,
       inputs are always foating-point.
     dimension_numbers: a tuple of tuples of the form `((lhs_contracting_dims,
       rhs_contracting_dims), (lhs_batch_dims, rhs_batch_dims))`.
     dot_precision: Optional. Either ``None``, which means the default precision
       for the backend, or a ``lax.Precision`` enum value (``Precision.DEFAULT``,
@@ -876,15 +965,15 @@
     # In this case, activations will be quantized at some point during training
     # (either now or later) and so we need to gather activation statistics by
     # calling 'QuantOps.create_input_ops', even if activations are not being
     # quantized on this particular training step (see b/174516400).
     if act_hparams is not None and act_hparams.prec is not None:
       # Calculate 's', the per-column scale factor on activations.
       act_op = QuantOps.create_input_ops(
-          act, hparams=act_hparams, get_bounds_params=get_bounds_params)
+          act, hparams=act_hparams, bounds_params=bounds_params)
       is_act_quantized = act_op.should_quantize()
       # Quantize activation matrix by computing RoundAndClip(w*s)
 
       # TODO(malmaud): We have to cast quantized activations to an fp format
       # instead of int8 since int8 matmul with int32 accumulation is not yet
       # supported in XLA (and therefore in Jax). See b/170293520. We keep
       # 'act_quantized' in whatever it's original fp format was, typically bf16
@@ -1041,15 +1130,15 @@
 
     # TODO(shivaniagrawal): HParams currently allows act_hparams to be NONE.
     # Going forward we can change act_hparams to be required field where if
     # either `prec` or `bounds` is None will result in No activation
     # quantization.
     if act_hparams:
       act = QuantOps.create_inputs_fake_quant(
-          act, hparams=act_hparams, get_bounds_params=get_bounds_params)
+          act, hparams=act_hparams, bounds_params=bounds_params)
 
     metadata_context = contextlib.suppress()
     # Use metadata context to annotate op metadata with quantization info
     act_prec = None if act_hparams is None else act_hparams.prec
     weight_prec = None if weight_params is None else weight_params.prec
 
     if flags.FLAGS.metadata_enabled:
@@ -1069,59 +1158,63 @@
   quant_type: QuantType
   weight_params: QuantOps.WeightParams
   act_hparams: Optional[QuantOps.ActHParams]
   prefer_int8_to_int32_dot: bool
   dot_precision: Optional[PrecisionType] = None
 
   # TODO(malmaud): Remove the 'padding_mask' field from 'GetBounds.Params'
-  # so that 'get_bounds_params' can be a hyperparameter of this class and
+  # so that 'bounds_params' can be a hyperparameter of this class and
   # only the padding mask will be passed as an argumen to '__call__'.
   @nn.compact
   def __call__(
       self, w: jnp.ndarray, act: jnp.ndarray,
-      get_bounds_params: Optional[get_bounds.GetBounds.Params]) -> jnp.ndarray:
+      bounds_params: Union[None, get_bounds.GetBounds.Params,
+                           get_bounds.DynamicBounds.Params]
+  ) -> jnp.ndarray:
     return quantized_dot(
         w=w,
         act=act,
-        get_bounds_params=get_bounds_params,
+        bounds_params=bounds_params,
         quant_type=self.quant_type,
         weight_params=self.weight_params,
         act_hparams=self.act_hparams,
         dot_precision=self.dot_precision,
         prefer_int8_to_int32_dot=self.prefer_int8_to_int32_dot)
 
 
 def quantized_dynamic_dot_general(
     *,
     lhs_act: jnp.ndarray,
     rhs_act: jnp.ndarray,
     quant_type: QuantType,
     lhs_act_hparams: Optional[QuantOps.ActHParams],
-    lhs_get_bounds_params: Optional[get_bounds.GetBounds.Params],
+    lhs_bounds_params: Union[None, get_bounds.GetBounds.Params,
+                             get_bounds.DynamicBounds.Params],
     rhs_act_hparams: Optional[QuantOps.ActHParams],
-    rhs_get_bounds_params: Optional[get_bounds.GetBounds.Params],
+    rhs_bounds_params: Union[None, get_bounds.GetBounds.Params,
+                             get_bounds.DynamicBounds.Params],
     dot_dimension_numbers: lax.DotDimensionNumbers,
     dot_precision: Optional[PrecisionType] = None) -> jnp.ndarray:
   """LAX dot general with optionally quantized dynamic inputs.
 
   Wraps LAX's `DotGeneral
   <https://github.com/google/jax/blob/f65a327c764406db45e95048dfe09209d8ef6d37/jax/_src/lax/lax.py#L667`_
   operator.
 
   Args:
     lhs_act: an array representing weights
     rhs_act: an array representing activations
     quant_type: quantization strategy
     lhs_act_hparams: Optional activation quantization hyperparamers for lhs act;
       instance of QuantOps.ActHParams. None means no quantization.
-    lhs_get_bounds_params: Optional get bounds params for lhs act auto
+    lhs_bounds_params: Optional get bounds params for lhs act auto
       quantization; instance of GetBounds.Params.
     rhs_act_hparams: Optional activation quantization hyperparamers for rhs act;
       instance of QuantOps.ActHParams. None means no quantization.
-    rhs_get_bounds_params: Optional get bounds params for rhs act auto
+    rhs_bounds_params: Optional get bounds params for rhs act auto
       quantization; instance of GetBounds.Params.
     dot_dimension_numbers: a tuple of tuples of the form
       `((lhs_contracting_dims, rhs_contracting_dims), (lhs_batch_dims,
       rhs_batch_dims)).
     dot_precision: Optional. Either ``None``, which means the default precision
       for the backend, or a ``lax.Precision`` enum value (``Precision.DEFAULT``,
       ``Precision.HIGH`` or ``Precision.HIGHEST``).
@@ -1148,23 +1241,24 @@
     if lhs_act.dtype != rhs_act.dtype:
       raise TypeError('Both activations must have the same dtypes, but got '
                       f'{lhs_act.dtype} and {rhs_act.dtype}')
     input_dtype = lhs_act.dtype
 
     def get_tensor_and_scale_for_act(
         act: jnp.ndarray, hparams: Optional[QuantOps.ActHParams],
-        get_bounds_params: Optional[get_bounds.GetBounds.Params]
+        bounds_params: Union[None, get_bounds.GetBounds.Params,
+                             get_bounds.DynamicBounds.Params]
     ) -> Tuple[jnp.ndarray, jnp.ndarray]:
       # We check whether activations should be quantized based on 'hparams'. If
       # so, we quantize it. If not, we return it unchanged. In either case, we
       # return a scale factor appropriate for unscaling the result of the
       # lax.dot_general.
       if hparams is not None and hparams.prec is not None:
         quant_op = QuantOps.create_input_ops(
-            act, hparams=hparams, get_bounds_params=get_bounds_params)
+            act, hparams=hparams, bounds_params=bounds_params)
 
         scale = quant_op.get_scale_for_aqt(allow_per_channel_scales=False)
         # Since only per-layer scale factors are supported, we assert that the
         # scale factors are scalars.
         shape_utils.assert_shapes_compatible(scale.shape, ())
         # TODO(malmaud): See comment on 'act_op.to_quantized' earlier in this
         # file, which applies here as well.
@@ -1181,17 +1275,17 @@
         # To avoid having a separate code path for every possibility of which of
         # the two input tensors are quantized , we implement not quantizing an
         # activation tensor by simply setting its corresponding scale factor to
         # 1.0.
         return act, jnp.array(1.0, dtype=SCALE_DTYPE)
 
     lhs_quantized, lhs_scale = get_tensor_and_scale_for_act(
-        lhs_act, lhs_act_hparams, lhs_get_bounds_params)
+        lhs_act, lhs_act_hparams, lhs_bounds_params)
     rhs_quantized, rhs_scale = get_tensor_and_scale_for_act(
-        rhs_act, rhs_act_hparams, rhs_get_bounds_params)
+        rhs_act, rhs_act_hparams, rhs_bounds_params)
 
     metadata_context = contextlib.suppress()
     # Use metadata context to annotate op metadata with quantization info
     lhs_prec = None if lhs_act_hparams is None else lhs_act_hparams.prec
     rhs_prec = None if rhs_act_hparams is None else rhs_act_hparams.prec
 
     if flags.FLAGS.metadata_enabled:
@@ -1213,23 +1307,19 @@
   elif quant_type in (QuantType.FAKE_QUANT, QuantType.FAKE_QUANT_WITH_INT):
     # TODO(shivaniagrawal): HParams currently allows act_hparams to be NONE.
     # Going forward we can change act_hparams to be required field where if
     # either `prec` or `bounds` is None will result in No activation
     # quantization.
     if lhs_act_hparams:
       lhs_act = QuantOps.create_inputs_fake_quant(
-          lhs_act,
-          hparams=lhs_act_hparams,
-          get_bounds_params=lhs_get_bounds_params)
+          lhs_act, hparams=lhs_act_hparams, bounds_params=lhs_bounds_params)
 
     if rhs_act_hparams:
       rhs_act = QuantOps.create_inputs_fake_quant(
-          rhs_act,
-          hparams=rhs_act_hparams,
-          get_bounds_params=rhs_get_bounds_params)
+          rhs_act, hparams=rhs_act_hparams, bounds_params=rhs_bounds_params)
 
     metadata_context = contextlib.suppress()
     # Use metadata context to annotate op metadata with quantization info
     lhs_prec = None if lhs_act_hparams is None else lhs_act_hparams.prec
     rhs_prec = None if rhs_act_hparams is None else rhs_act_hparams.prec
 
     if flags.FLAGS.metadata_enabled:
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/shape_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/shape_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/get_bounds_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/get_bounds_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,28 +46,24 @@
 
   def init_model(self,
                  update_bounds,
                  update_stats=True,
                  reset_stats=False,
                  use_cams=False,
                  granularity=quant_config.QuantGranularity.PER_TENSOR,
-                 ema_coeff=None,
-                 dynamic=False,
-                 clipping_coeff=1.0):
+                 ema_coeff=None):
     self.hyperparam = get_bounds.GetBounds.Hyper(
         initial_bound=self.hyperparam.initial_bound,
         stddev_coeff=self.hyperparam.stddev_coeff,
         absdev_coeff=self.hyperparam.absdev_coeff,
         mix_coeff=self.hyperparam.mix_coeff,
         reset_stats=reset_stats,
         use_cams=use_cams,
         ema_coeff=ema_coeff,
-        granularity=granularity,
-        dynamic=dynamic,
-        clipping_coeff=clipping_coeff)
+        granularity=granularity)
     gb_bounds_params = get_bounds.GetBounds.Params(
         update_bounds=update_bounds, update_stats=update_stats)
     bounds_module = get_bounds.GetBounds(hyper=self.hyperparam)
     init_state = bounds_module.init(
         self.key2, self.x, bounds_params=gb_bounds_params)
     return bounds_module, init_state, gb_bounds_params
 
@@ -273,24 +269,28 @@
           clipping_coeff=1.0,
           granularity=quant_config.QuantGranularity.PER_CHANNEL),
       dict(
           testcase_name='with clipping + per tensor bounds',
           clipping_coeff=0.5,
           granularity=quant_config.QuantGranularity.PER_TENSOR))
   def test_dynamic_bounds(self, clipping_coeff, granularity):
-    model, state, params = self.init_model(
-        False,
-        False,
-        granularity=granularity,
-        dynamic=True,
-        clipping_coeff=clipping_coeff)
+    hyperparam = get_bounds.DynamicBounds.Hyper(
+        granularity=granularity, clipping_coeff=clipping_coeff)
+    if granularity == quant_config.QuantGranularity.PER_TENSOR:
+      quant_axis = None
+    else:
+      quant_axis = (0, 1)
+    params = get_bounds.DynamicBounds.Params(quant_axis=quant_axis)
+    model = get_bounds.DynamicBounds(hyper=hyperparam)
+    state = model.init(
+        self.key2, self.x, bounds_params=params)
 
     x = jnp.array([[[2, 3], [5, 4]], [[5, 6], [7, 6]]])
     bounds = model.apply(state, x, bounds_params=params)
     if granularity == quant_config.QuantGranularity.PER_CHANNEL:
-      onp.testing.assert_allclose(bounds, jnp.array([7.0, 6.0]))
+      onp.testing.assert_allclose(bounds, jnp.array([[[7.0, 6.0]]]))
     else:
       onp.testing.assert_allclose(bounds, jnp.array(3.5))
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/flax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/quant_config.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/quant_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -58,14 +58,28 @@
 
   # This will be passed to create_weight_ops in ConvAqt
   quantize_weights: bool = flax.struct.field(default=True, pytree_node=False)
 
   # Whether to tag activations to record statistics.
   collect_acts_stats: bool = flax.struct.field(default=False, pytree_node=False)
 
+  # Whether to apply sparsity for training, this is set to True somewhere in a
+  # later stage of training.
+  # Currently we separate the update of sparsity masks for weight and
+  # activation, since during evaluation the weight sparsity mask is
+  # reused from training, while activation mask will need update
+  # (due to change of seq length).
+  # The apply_sparsity flag is shared between weight/activation sparsity,
+  # we can modify it to use two flags in the future if necessary.
+  apply_sparsity: bool = flax.struct.field(default=False, pytree_node=False)
+  update_weight_sparsity: bool = flax.struct.field(
+      default=False, pytree_node=False)
+  update_act_sparsity: bool = flax.struct.field(
+      default=False, pytree_node=False)
+  num_update_sparsity: int = flax.struct.field(default=0, pytree_node=False)
 
   # Whether to quantize activations.
   #
   # TODO(malmaud): This only applies to softmax for now. Apply it to layernorm
   # and dot operations as well.
   quantize_acts: bool = True
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/compute_cost_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/compute_cost_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from typing import Dict, Iterable, List, Optional, Tuple
 from absl import flags
 from aqt.jax_legacy.jax import hlo_utils
 from jax._src.lax import convolution as lax_convolution
 from jax._src.lax import lax
 from jax.interpreters import ad
 from jax.interpreters import batching
-from jax.interpreters import masking
 from jax.interpreters import mlir
 import numpy as onp
 # pylint: disable=g-direct-tensorflow-import
 from tensorflow.compiler.xla.service import hlo_pb2
 # pylint: enable=g-direct-tensorflow-import
 
 FLAGS = flags.FLAGS
@@ -66,15 +65,14 @@
     lax.dot_general_p = lax.standard_primitive(
         shape_rule=lax._dot_general_shape_rule,
         dtype_rule=lax._dot_general_dtype_rule,
         name=self._op_name)
     ad.defbilinear(lax.dot_general_p, lax._dot_general_transpose_lhs,
                    lax._dot_general_transpose_rhs)
     batching.primitive_batchers[lax.dot_general_p] = lax._dot_general_batch_rule
-    masking.masking_rules[lax.dot_general_p] = lax._dot_general_masking_rule
     mlir.register_lowering(lax.dot_general_p, lax._dot_general_lower)
     # pylint: enable=protected-access
 
   def __exit__(self, *exc):
     # Restore original primitive
     lax.dot_general_p = self._dot_general_p_original
 
@@ -113,16 +111,14 @@
                           expand_complex_convolutions=True),
         platform='gpu')
     ad.defbilinear(lax_convolution.conv_general_dilated_p,
                    lax_convolution._conv_general_dilated_transpose_lhs,
                    lax_convolution._conv_general_dilated_transpose_rhs)
     batching.primitive_batchers[lax_convolution.conv_general_dilated_p] = (
         lax_convolution._conv_general_dilated_batch_rule)
-    masking.masking_rules[lax_convolution.conv_general_dilated_p] = (
-        lax_convolution._conv_general_dilated_masking_rule)
     # pylint: enable=protected-access
 
   def __exit__(self, *exc):
     # Restore original primitive
     lax_convolution.conv_general_dilated_p = (
         self._conv_general_dilated_p_original)
 
@@ -209,28 +205,28 @@
 def _extract_quant_info(
     instr: hlo_pb2.HloInstructionProto) -> Tuple[int, int, bool]:
   """Extracts lhs and rhs quantization precision from op metadata."""
   if instr.opcode not in _get_supported_ops():
     raise NotImplementedError('Unexpected op detected')
   # If annotated, metadata.op_type would have the following format:
   # '[original op name]_quant_w[weight prec]_a[act prec]'
-  if 'quant' not in instr.metadata.op_type:
+  if 'quant' not in instr.metadata.op_name:
     raise NotImplementedError('Unable to parse {}'.format(
         instr.metadata.op_type))
   [(lhs_prec_str, rhs_prec_str, rhs_is_weight_str)
-  ] = re.findall('_lhs(.*)_rhs(.*)_lw(.*)', instr.metadata.op_type)
+  ] = re.findall(r'_lhs(.*)_rhs(.*)_lw(\d+)', instr.metadata.op_name)
 
   def _extract_prec(prec_str):
     if prec_str.startswith('bf'):
       prec_str = prec_str[2:]
     if prec_str.isnumeric():
       prec = int(prec_str)
     else:
       raise NotImplementedError('Unable to parse {}'.format(
-          instr.metadata.op_type))
+          instr.metadata.op_name))
     return prec
 
   lhs_prec = _extract_prec(lhs_prec_str)
   rhs_prec = _extract_prec(rhs_prec_str)
   rhs_is_weight = bool(int(rhs_is_weight_str))
   if lhs_prec <= 0 or rhs_prec <= 0:
     raise ValueError('HLO metadata precision annotatation must be a positive '
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/flax/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/flax/struct.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/flax/struct.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/utils.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/models_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/models_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/check_config_util.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/check_config_util.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/train_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 from aqt.jax_legacy.jax.imagenet import input_pipeline
 from aqt.jax_legacy.jax.imagenet import models
 from aqt.jax_legacy.jax.imagenet import pokebnn
 
 import flax
 from flax import jax_utils
 from flax import struct
-from flax.optim import dynamic_scale as dynamic_scale_lib
 from flax.training import common_utils
+from flax.training import dynamic_scale as dynamic_scale_lib
 import jax
 from jax import lax
 import jax.nn
 import jax.numpy as jnp
 import optax
 
 
@@ -139,19 +139,19 @@
       opt_state=new_opt_state,
       dynamic_scale=dynamic_scale)
 
   if dynamic_scale:
     # if is_fin == False the gradients contain Inf/NaNs and the old optimizer
     # state should be restored.
     new_state = new_state.replace(
-        opt_state=jax.tree_multimap(
+        opt_state=jax.tree_map(
             functools.partial(jnp.where, is_fin),
             new_state.opt_state,
             state.opt_state),
-        params=jax.tree_multimap(
+        params=jax.tree_map(
             functools.partial(jnp.where, is_fin),
             new_state.params,
             state.params))
     metrics['scale'] = dynamic_scale.scale
 
   return new_state, metrics
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/input_pipeline.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/models.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/pokebnn.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/pokebnn.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/train_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,16 @@
 
     dense_schema = {
         'weight_prec': None,
         'weight_quant_granularity': None,
         'quant_type': None,
         'quant_act': quant_act_schema,
         'weight_half_shift': None,
+        'weight_sparsity': sparsity_schema,
+        'act_sparsity': sparsity_schema,
     }
 
     conv_schema = {
         'weight_prec': None,
         'weight_quant_granularity': None,
         'quant_type': None,
         'quant_act': quant_act_schema,
@@ -182,14 +184,17 @@
         'act_function': None,
         'shortcut_ch_shrink_method': None,
         'shortcut_ch_expand_method': None,
         'shortcut_spatial_method': None,
         'teacher_model': None,
         'is_teacher': None,
         'seed': None,
+        'sparsity': sparsity_schema,
+        'weight_sparsity': sparsity_schema,
+        'act_sparsity': sparsity_schema,
         'lr_scheduler': {
             'warmup_epochs': None,
             'cooldown_epochs': None,
             'scheduler': None,
             'num_epochs': None,
             'endlr': None,
             'knee_lr': None,
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/pokebnn_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/pokebnn_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/base_config.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/base_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,23 @@
       "base_learning_rate": 0.1,
       "momentum": 0.9,
       "weight_decay": 0.0001,
       "activation_bound_update_freq": -1,
       "activation_bound_start_step": -1,
       "prec": None,
 
+      "sparsity": {
+          "type": "STRUCTURED_NM",
+          "prune_rate": None,
+          "order": "C",
+          "absolute": True,
+          "smallest": True,
+          "structure_decay": False,
+          "sparse_ste": False
+      },
       "quant_type": "fake_quant",
       "weight_quant_granularity": "per_channel",
       "act_function": "relu",
       "shortcut_ch_shrink_method": "none",
       "shortcut_ch_expand_method": "none",
       "shortcut_spatial_method": "none",
       "lr_scheduler": {
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/train.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 from aqt.jax_legacy.jax.imagenet.configs.paper.resnet50_w8_a8_auto import get_config as w8a8auto_paper_config
 from aqt.jax_legacy.utils import hparams_utils as os_hparams_utils
 from aqt.jax_legacy.utils import report_utils
 from aqt.jax_legacy.utils import summary_utils
 
 from flax import jax_utils
 from flax.metrics import tensorboard
-from flax.optim import dynamic_scale as dynamic_scale_lib
 from flax.training import checkpoints
 from flax.training import common_utils
+from flax.training import dynamic_scale as dynamic_scale_lib
 import jax
 from jax import random
 import jax.nn
 import jax.numpy as jnp
 from ml_collections import config_flags
 import optax
 import tensorflow.compat.v2 as tf
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/hparams_config.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/hparams_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/imagenet/configs_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/stats.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/hlo_utils.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/hlo_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     *fn_args: Arguments to fn.
     **fn_kwargs: Keyword arguments to fn.
 
   Returns:
     An HloModuleProto object.
 
   """
-  computation = jax.xla_computation(fn)(*fn_args, **fn_kwargs)
+  computation = (
+      jax.jit(fn).lower(*fn_args, **fn_kwargs).compiler_ir(dialect='hlo')
+  )
   serialized_hlo = computation.as_serialized_hlo_module_proto()
   hlo_module_proto = hlo_pb2.HloModuleProto.FromString(serialized_hlo)
   return hlo_module_proto
 
 
 def load_hlo_proto_from_model(
     model: nn.Module,  #
@@ -73,15 +75,15 @@
 def output_hlo(computation: Any, file_path: str):
   """Saves HLO for the given xla computation to given file path.
 
   The file format is determined by the file_path extension, i.e. for .txt file
   saves the hlo as text, and for .pb file save the hlo module proto binary.
 
   Args:
-    computation: wrapped jax.xla_computation
+    computation: wrapped XlaComputation
     file_path: file path to write the HLO to.
   """
   hlo_module_proto_str = computation.as_serialized_hlo_module_proto()
   hlo_txt = computation.as_hlo_text()
   output_hlo_to_file(hlo_module_proto_str, hlo_txt, file_path)
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/flax_layers.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/flax_layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,43 +27,42 @@
 from aqt.jax_legacy.jax import get_bounds
 from aqt.jax_legacy.jax import quant_config
 from aqt.jax_legacy.jax import quantization
 from aqt.jax_legacy.jax import shape_utils
 from aqt.jax_legacy.jax import stats_tag
 from aqt.jax_legacy.jax import utils
 from aqt.jax_legacy.jax.flax import struct as flax_struct
-
-
-
 from aqt.jax_legacy.jax.quantization import QuantOps
 from aqt.jax_legacy.jax.quantization import QuantType
+from aqt.jax_legacy.jax.sparsity import SparseHParams
+from aqt.jax_legacy.jax.sparsity import Sparsity
 import flax
 from flax import linen as nn
 from flax.core import frozen_dict
 from flax.linen import partitioning
 import jax
 from jax import lax
 import jax.numpy as jnp
 import numpy as np
 
 FLAGS = flags.FLAGS
 
 # Alias for initializer function.
 # Should follow the template `def init(key, shape, dtype=dtype) -> ndarray:`.
 # See flax.linen.initializers and jax.nn.initializers for more details.
-InitializerType = Callable[[jnp.ndarray, Iterable[int], Type[Any]], jnp.ndarray]
+InitializerType = Callable[[jnp.ndarray, Sequence[int], Type[Any]], jnp.ndarray]
 
 default_kernel_init = nn.initializers.lecun_normal()
 
 dataclass = flax_struct.dataclass if not typing.TYPE_CHECKING else dataclasses.dataclass
 
 Array = jnp.ndarray
 DType = jnp.dtype
 PRNGKey = jnp.ndarray
-Shape = Iterable[int]
+Shape = Sequence[int]
 Initializer = Callable[[PRNGKey, Shape, DType], Array]
 PrecisionLike = Union[None, str, lax.Precision, Tuple[str, str],
                       Tuple[lax.Precision, lax.Precision]]
 
 
 # Based on flax.linen.Dense
 class DenseAqt(nn.Module):
@@ -102,14 +101,17 @@
     # quantization will be applied.
     quant_act: Optional[QuantOps.ActHParams]
     # Quantization strategy, one of `fake_quant` or `aqt`.
     quant_type: QuantType
     weight_quant_granularity: quant_config.QuantGranularity
 
 
+    act_sparsity: Optional[SparseHParams] = None
+    weight_sparsity: Optional[SparseHParams] = None
+
   hparams: HParams
   paxis_name: Optional[str]
   features: Union[int, Tuple[int, ...]]
   train: bool
   dynamic_context: quant_config.DynamicContext
   dtype: Any
   use_bias: bool = True
@@ -149,14 +151,15 @@
     # TODO(wanglisa): Replace fake quant with AQT.
 
     if self.dynamic_context.collect_acts_stats:
       stats_tag.StatsTag(
           channel_axis=-1, name='inputs', update_stats=self.train)(
               inputs, mask=padding_mask)
     hparams = self.hparams
+
     if (hparams.weight_prec is not None and
         isinstance(hparams.weight_prec, int) and hparams.weight_prec > 8):
       raise NotImplementedError(
           'If you want to use more than 8bits for quantization, please revisit '
           'jax.lax.Precision.DEFAULT to determine whether it is still sufficient.'
       )
 
@@ -171,49 +174,70 @@
       kernel_axis_names = self.kernel_axis_names
       if len(kernel_axis_names) != len(kernel_shape):
         raise ValueError(f"Kernel axis names {kernel_axis_names} doesn't match "
                          f'kernel shape {kernel_shape}.')
 
     inputs = jnp.asarray(inputs, self.dtype)
 
-    use_quantized_vars_for_inference = self.possibly_use_quantized_vars and not self.train
-    if use_quantized_vars_for_inference:
+    # Here are 3 possible conditions:
+    #   1. not quantization: init normal kernel, quant_w = None
+    #   2. quantization and train mode: init normal kernel, quantized kernel
+    #      with bfloat16 to avoid gradient on integer and quant_w = None.
+    #   3. quantization and inference mode: no normal kernel, init quantized
+    #      kernel with int8 and quant_w = (qkernel, qscale).
+    quant_w = None
+    if (not self.possibly_use_quantized_vars) or (
+        self.possibly_use_quantized_vars and self.train):
+      kernel = partitioning.param_with_axes(
+          'kernel',
+          self.kernel_init,
+          kernel_shape,
+          axes=tuple(kernel_axis_names))
+      kernel = jnp.asarray(kernel, self.dtype)
+
+      kernel = Sparsity(
+          sparsity_hparams=hparams.weight_sparsity, name='weight_sparsity')(
+              kernel,
+              update_mask=self.dynamic_context.update_weight_sparsity,
+              apply_mask=self.dynamic_context.apply_sparsity,
+              num_update_sparsity=self.dynamic_context.num_update_sparsity)
+
+    if self.possibly_use_quantized_vars:
+      qkernel_dtype = self.dtype
+      qkernel_initializer = nn.initializers.zeros
+      if not self.train:
+        qkernel_dtype = jax.numpy.int8
+        qkernel_initializer = nn.initializers.zeros
+
       qkernel = partitioning.param_with_axes(
           'qkernel',
-          nn.initializers.zeros,
+          qkernel_initializer,
           kernel_shape,
-          jax.numpy.int8,
+          qkernel_dtype,
           axes=tuple(kernel_axis_names))
-
+      qkernel = jnp.asarray(qkernel, qkernel_dtype)
       # Initialization of scale does not matter so we are initializing with
-      # bias_init.
+      # bias_init. And here only support quantizing on first dimension.
       scale_axis_names = list(kernel_axis_names)
       scale_axis_names[0] += '_qscale'
       qscale = partitioning.param_with_axes(
           'qscale',
           self.bias_init, (1,) + features,
           axes=tuple(scale_axis_names))
       qscale = jnp.asarray(qscale, self.dtype)
-      quant_w = quantization.QuantW(qkernel, qscale)
-      kernel = None
-    else:
-      quant_w = None
-      kernel = partitioning.param_with_axes(
-          'kernel',
-          self.kernel_init,
-          kernel_shape,
-          axes=tuple(kernel_axis_names))
-      kernel = jnp.asarray(kernel, self.dtype)
-
-
-    get_bounds_params = get_bounds.GetBounds.Params(
-        update_bounds=self.dynamic_context.update_bounds,
-        update_stats=self.train,
-        paxis_name=self.paxis_name,
-        mask=padding_mask)
+      if not self.train:
+        quant_w = quantization.QuantW(qkernel, qscale)
+        kernel = None
+
+    inputs = Sparsity(
+        sparsity_hparams=hparams.act_sparsity, name='act_sparsity')(
+            inputs,
+            update_mask=self.dynamic_context.update_act_sparsity,
+            apply_mask=self.dynamic_context.apply_sparsity,
+            num_update_sparsity=self.dynamic_context.num_update_sparsity)
 
     weight_quant_granularity = hparams.weight_quant_granularity
     # kernel.shape = (channels_in, channels_out)
     if weight_quant_granularity == quant_config.QuantGranularity.PER_CHANNEL:
       # Compute scale factors by reducing over the rows of the weight matrix,
       # resulting in one scale factor per column. This results in one scale
       # factor per output channel.
@@ -231,29 +255,54 @@
         prec=hparams.weight_prec,
         half_shift=hparams.weight_half_shift,
         axis=weight_quant_axis,
         expected_scale_shape=expected_scale_shape)
 
     # TODO(wanglisa): add option to control when scale is being recomputed
 
-    # matmul
+    bounds_params = None
+    if hparams.quant_act is not None:
+      if isinstance(hparams.quant_act.bounds, get_bounds.DynamicBounds.Hyper):
+        bounds_params = get_bounds.DynamicBounds.Params(quant_axis=None)
+      elif isinstance(hparams.quant_act.bounds, get_bounds.GetBounds.Hyper):
+        bounds_params = get_bounds.GetBounds.Params(
+            update_bounds=self.dynamic_context.update_bounds,
+            update_stats=self.train,
+            paxis_name=self.paxis_name,
+            mask=padding_mask)
+
     contracting_dims = ((inputs.ndim - 1,), (0,))
     # `((lhs_contracting_dims, rhs_contracting_dims),
     batch_dims = ((), ())  # (lhs_batch_dims, rhs_batch_dims))`
-    y = quantization.quantized_dot_general(
-        act=inputs,
-        w=kernel,
-        quant_type=hparams.quant_type,
-        weight_params=weight_params,
-        act_hparams=hparams.quant_act,
-        get_bounds_params=get_bounds_params,
-        dimension_numbers=(contracting_dims, batch_dims),
-        dot_precision=self.precision,
-        prefer_int8_to_int32_dot=self.dynamic_context.prefer_int8_to_int32_dot,
-        quant_w=quant_w)
+
+    if hparams.quant_act is not None and isinstance(
+        hparams.quant_act.bounds, get_bounds.DynamicBounds.Hyper):
+      y = quantization.flaxformer_dot_general(
+          act=inputs,
+          w=kernel,
+          dimension_numbers=(contracting_dims, batch_dims),
+          weight_params=weight_params,
+          act_hparams=hparams.quant_act,
+          bounds_params=bounds_params,
+          dot_precision=self.precision,
+          quant_w=quant_w)
+
+    else:
+      y = quantization.quantized_dot_general(
+          act=inputs,
+          w=kernel,
+          quant_type=hparams.quant_type,
+          weight_params=weight_params,
+          act_hparams=hparams.quant_act,
+          bounds_params=bounds_params,
+          dimension_numbers=(contracting_dims, batch_dims),
+          dot_precision=self.precision,
+          prefer_int8_to_int32_dot=self.dynamic_context
+          .prefer_int8_to_int32_dot,
+          quant_w=quant_w)
 
     # bias
     if self.use_bias:
       bias = partitioning.param_with_axes(
           'bias',
           self.bias_init, (np.prod(features),),
           axes=(kernel_axis_names[-1],))
@@ -349,17 +398,14 @@
     features = _canonicalize_tuple(self.features)
     axis = _canonicalize_tuple(self.axis)
 
     inputs = jnp.asarray(inputs, self.dtype)
     axis = _normalize_axes(axis, inputs.ndim)
 
     hparams = self.hparams
-    if hparams.quant_act is not None:
-      raise ValueError(
-          'activation quantization is not yet supported for DenseGeneralAqt')
 
     if (hparams.weight_prec is not None and
         isinstance(hparams.weight_prec, int) and hparams.weight_prec > 8):
       raise NotImplementedError(
           'If you want to use more than 8bits for quantization, please revisit '
           'jax.lax.Precision.DEFAULT to determine whether it is still sufficient.'
       )
@@ -389,22 +435,45 @@
           return self.reshaped_kernel_axis_name_map.get(result, result)
 
         kernel_axis_names = (
             _reshaped_axis_names(kernel_axis_names[:len(axis)]),
             _reshaped_axis_names(kernel_axis_names[len(axis):]),
         )
 
-    use_quantized_vars_for_inference = self.possibly_use_quantized_vars and not self.train
-    if use_quantized_vars_for_inference:
+    # Here are 3 possible conditions:
+    #   1. not quantization: init normal kernel, quant_w = None
+    #   2. quantization and train mode: init normal kernel, quantized kernel
+    #      with bfloat16 to avoid gradient on integer and quant_w = None.
+    #   3. quantization and inference mode: no normal kernel, init quantized
+    #      kernel with int8 and quant_w = (qkernenl, qscale).
+    quant_w = None
+    if (not self.possibly_use_quantized_vars) or (
+        self.possibly_use_quantized_vars and self.train):
+      kernel = partitioning.param_with_axes(
+          'kernel',
+          self.kernel_init,
+          kernel_param_shape,
+          jnp.float32,
+          axes=tuple(kernel_axis_names))
+      kernel = jnp.asarray(kernel, self.dtype)
+      kernel = jnp.reshape(kernel, kernel_shape)
+
+    if self.possibly_use_quantized_vars:
+      qkernel_dtype = self.dtype
+      qkernel_initializer = nn.initializers.zeros
+      if not self.train:
+        qkernel_dtype = jax.numpy.int8
+        qkernel_initializer = nn.initializers.zeros
       qkernel = partitioning.param_with_axes(
           'qkernel',
-          nn.initializers.zeros,
+          qkernel_initializer,
           kernel_param_shape,
-          jax.numpy.int8,
+          qkernel_dtype,
           axes=tuple(kernel_axis_names))
+      qkernel = jnp.asarray(qkernel, qkernel_dtype)
       qkernel = jnp.reshape(qkernel, kernel_shape)
 
       # Initialization of scale does not matter so we are initializing with
       # bias_init.
       scale_axis_names = list(kernel_axis_names)
       len_contracted_dims = 1 if self.reshape_kernel else len(axis)
       for ax in range(0, len_contracted_dims):
@@ -412,56 +481,66 @@
       qscale = partitioning.param_with_axes(
           'qscale',
           self.bias_init,
           scale_param_shape,
           axes=tuple(scale_axis_names))
       qscale = jnp.asarray(qscale, self.dtype)
       qscale = jnp.reshape(qscale, scale_shape)
-      quant_w = quantization.QuantW(qkernel, qscale)
-      kernel = None
-    else:
-      quant_w = None
-      kernel = partitioning.param_with_axes(
-          'kernel',
-          self.kernel_init,
-          kernel_param_shape,
-          jnp.float32,
-          axes=tuple(kernel_axis_names))
-      kernel = jnp.asarray(kernel, self.dtype)
-      kernel = jnp.reshape(kernel, kernel_shape)
+      if not self.train:
+        quant_w = quantization.QuantW(qkernel, qscale)
+        kernel = None
 
     contract_ind = tuple(range(0, len(axis)))
 
     weight_quant_granularity = hparams.weight_quant_granularity
 
+    act_quant_axis = None
+    if hparams.quant_act:
+      if isinstance(hparams.quant_act.bounds, get_bounds.DynamicBounds.Hyper):
+        act_quant_granularity = hparams.quant_act.bounds.granularity  # pytype: disable=attribute-error  # jax-ndarray
+        if act_quant_granularity == quant_config.QuantGranularity.PER_CHANNEL:
+          act_quant_axis = tuple(axis)
+        elif act_quant_granularity == quant_config.QuantGranularity.PER_TENSOR:
+          act_quant_axis = None
+        else:
+          raise ValueError(
+              f'Invalid quantization granularity {weight_quant_granularity}.')
+      elif isinstance(hparams.quant_act.bounds, get_bounds.GetBounds.Hyper):
+        raise NotImplementedError(
+            'We do not support get_bounds for dot general.')
+
     if weight_quant_granularity == quant_config.QuantGranularity.PER_CHANNEL:
       # Compute scale factors by reducing over the rows of the weight matrix,
       # resulting in one scale factor per column. This results in one scale
       # factor per output channel.
       expected_scale_shape = (1,) * len(axis) + features
       weight_quant_axis = contract_ind
     elif weight_quant_granularity == quant_config.QuantGranularity.PER_TENSOR:
       # Compute a single scale factor for the entire weight matrix.
       expected_scale_shape = (1,) * len(kernel_shape)
       weight_quant_axis = None
     else:
       raise ValueError(
           f'Invalid quantization granularity {weight_quant_granularity}.')
 
+    bounds_params = get_bounds.DynamicBounds.Params(quant_axis=act_quant_axis)
+
     weight_params = QuantOps.WeightParams(
         prec=hparams.weight_prec,
         half_shift=hparams.weight_half_shift,
         axis=weight_quant_axis,
         expected_scale_shape=expected_scale_shape)
 
     out = quantization.flaxformer_dot_general(
         act=inputs,
         w=kernel,
         dimension_numbers=((axis, contract_ind), ((), ())),
         weight_params=weight_params,
+        act_hparams=hparams.quant_act,
+        bounds_params=bounds_params,
         dot_precision=self.precision,
         quant_w=quant_w)
 
     if self.use_bias:
       bias = partitioning.param_with_axes(
           'bias',
           self.bias_init, (np.prod(features),),
@@ -573,15 +652,15 @@
     kernel = jnp.asarray(kernel, self.dtype)
 
     # Activation quantization
     if hparams.quant_act is not None:
       inputs = QuantOps.create_inputs_fake_quant(
           inputs=inputs,
           hparams=hparams.quant_act,
-          get_bounds_params=get_bounds.GetBounds.Params(
+          bounds_params=get_bounds.GetBounds.Params(
               update_bounds=self.dynamic_context.update_bounds,
               update_stats=self.train,
               paxis_name=self.paxis_name))
 
     # Weight quantization
     if hparams.weight_prec is not None:
       kernel_reduction_axis = tuple(range(kernel.ndim - 1))
@@ -806,25 +885,25 @@
       shape_utils.assert_shapes_equal(padding_mask.shape, (batch_size, 1))
 
     embedding = self.embedding
     embedding = jnp.asarray(embedding, self.dtype)
 
     # TODO(malmaud): Remove the 'mask' field from this struct so we can
     # make this struct a hyperparameter of the EncoderAqt class.
-    get_bounds_params = get_bounds.GetBounds.Params(
+    bounds_params = get_bounds.GetBounds.Params(
         update_bounds=self.dynamic_context.update_bounds,
         update_stats=self.train,
         paxis_name=self.paxis_name,
         mask=padding_mask,
         module_name='logits')
 
     out = self.quantized_dot(
         act=query,
         w=jnp.transpose(embedding),
-        get_bounds_params=get_bounds_params)
+        bounds_params=bounds_params)
 
     return out
 
 
 # Forked from Flax LayerNorm module.
 class LayerNormAqt(nn.Module):
   """Layer normalization (https://arxiv.org/abs/1607.06450).
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/models_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/models_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -858,15 +858,15 @@
     key = jax.random.PRNGKey(0)
     # Mark the first token of the target and last token of the inputs as padding
     # tokens.
     targets = onp.array([[0, 2]])
     inputs = onp.array([[1, 0]])
     initial_state = module.init(key, inputs=inputs, targets=targets)
     # Change the embedding of the padding token.
-    initial_state = initial_state.unfreeze()
+    initial_state = flax.core.unfreeze(initial_state)
     initial_state['params']['shared_embedding']['embedding'] = initial_state[
         'params']['shared_embedding']['embedding'].at[0, :].set(10.0)
     module.train = True
     _, state1 = module.apply(
         flax.core.freeze(initial_state),
         inputs=inputs,
         targets=targets,
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/models.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/train_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                         training_state_initial.flax_state)
     with np.testing.assert_raises(AssertionError):
       np.testing.assert_array_equal(training_state.dropout_rngs,
                                     training_state_initial.dropout_rngs)
     training_state_restored = training_state_initial.restore_checkpoint(
         model_dir=ckpt_dir)
 
-    leaf_equality_tree = jax.tree_multimap(lambda x, y: jnp.all(x == y),
+    leaf_equality_tree = jax.tree_map(lambda x, y: jnp.all(x == y),
                                            training_state.flax_state,
                                            training_state_restored.flax_state)
     self.assertTrue(
         all(jax.tree_leaves(leaf_equality_tree)),
         'Training state was altered during restoration.')
 
     np.testing.assert_array_equal(training_state.dropout_rngs,
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from aqt.jax_legacy.jax.wmt_mlperf import training_hparams_generator_lib
 from aqt.jax_legacy.jax.wmt_mlperf.hparams_configs.experimental import full_model_8bit_weights_only_int8
 from aqt.jax_legacy.jax.wmt_mlperf.hparams_configs.experimental import small_model_8bit_weights_and_fixed_acts
 from aqt.jax_legacy.jax.wmt_mlperf.hparams_configs.experimental import small_model_bfloat16
 from aqt.jax_legacy.jax.wmt_mlperf.hparams_configs.leaderboard import full_model_bfloat16
 from aqt.jax_legacy.utils import hparams_utils
 from flax import serialization
+from flax.core import pop
 import jax
 import jax.numpy as jnp
 from jax.tools import jax_to_ir
 from ml_collections import config_dict
 import tensorflow.compat.v2 as tf
 
 flags.DEFINE_string(
@@ -98,16 +99,19 @@
           update_bounds=False, collect_acts_stats=False, quantize_acts=True))
   init_state = model.init(rng, jnp.ones(input_shape, jnp.float32))
 
   def _fn(state, inputs):
     return model.apply(state, inputs, mutable=False)
 
   if not use_xla_optimizations:
-    computation = jax.xla_computation(_fn)(init_state,
-                                           jnp.ones(input_shape, jnp.float32))
+    computation = (
+        jax.jit(_fn)
+        .lower(init_state, jnp.ones(input_shape, jnp.float32))
+        .compiler_ir(dialect='hlo')
+    )
     hlo_utils.output_hlo(computation, FLAGS.hlo_output)
 
   else:
 
     def _wrapped_fn(inputs):
       return _fn(init_state, inputs)
 
@@ -128,42 +132,45 @@
     layers: The number of model layers.
   """
   if FLAGS.checkpoint:
     raise app.UsageError('Checkpoints not yet supported for WMT encoder.')
 
   input_shape = (1, 32)
   rng = jax.random.PRNGKey(0)
-  model_hparams = training_hparams_generator_lib.create_base_transformer_hparams(
-      embedding_weight_prec=None,
-      attention_weight_prec=None,
-      mlp_weight_prec=None,
-      mlp_pos_inputs_prec=None,
-      mlp_pos_inputs_hyper=None,
-      mlp_signed_inputs_prec=None,
-      mlp_signed_inputs_hyper=None,
-      attention_kqv_inputs_prec=None,
-      attention_kqv_inputs_hyper=None,
-      attention_out_inputs_prec=None,
-      attention_out_inputs_hyper=None,
-      logits_inputs_prec=None,
-      logits_inputs_hyper=None,
-      logits_via_embeddings=True,
-      attention_act_q_inputs_prec=None,
-      attention_act_q_inputs_hyper=None,
-      attention_act_k_inputs_prec=None,
-      attention_act_k_inputs_hyper=None,
-      attention_act_probs_inputs_prec=None,
-      attention_act_v_inputs_prec=None,
-      attention_act_v_inputs_hyper=None,
-      num_layers=layers,
-      emb_dim=1024,
-      num_heads=1,
-      qkv_dim=1024,
-      mlp_dim=4096,
-      quant_type=QuantType.FAKE_QUANT)
+  model_hparams = (
+      training_hparams_generator_lib.create_base_transformer_hparams(
+          embedding_weight_prec=None,
+          attention_weight_prec=None,
+          mlp_weight_prec=None,
+          mlp_pos_inputs_prec=None,
+          mlp_pos_inputs_hyper=None,
+          mlp_signed_inputs_prec=None,
+          mlp_signed_inputs_hyper=None,
+          attention_kqv_inputs_prec=None,
+          attention_kqv_inputs_hyper=None,
+          attention_out_inputs_prec=None,
+          attention_out_inputs_hyper=None,
+          logits_inputs_prec=None,
+          logits_inputs_hyper=None,
+          logits_via_embeddings=True,
+          attention_act_q_inputs_prec=None,
+          attention_act_q_inputs_hyper=None,
+          attention_act_k_inputs_prec=None,
+          attention_act_k_inputs_hyper=None,
+          attention_act_probs_inputs_prec=None,
+          attention_act_v_inputs_prec=None,
+          attention_act_v_inputs_hyper=None,
+          num_layers=layers,
+          emb_dim=1024,
+          num_heads=1,
+          qkv_dim=1024,
+          mlp_dim=4096,
+          quant_type=QuantType.FAKE_QUANT,
+      )
+  )
   model = models.Encoder(
       vocab_size=32711,
       hparams=model_hparams.encoder,
       shared_embedding=None,
       use_bfloat16=False,
       emb_dim=model_hparams.emb_dim,
       num_heads=model_hparams.num_heads,
@@ -176,15 +183,19 @@
       dynamic_context=quant_config.DynamicContext(
           update_bounds=False, collect_acts_stats=False, quantize_acts=True))
   init_state = model.init(rng, jnp.ones(input_shape, jnp.float32))
 
   def _fn(state, inputs):
     return model.apply(state, inputs)
 
-  computation = jax.xla_computation(_fn)(init_state, jnp.ones(input_shape))
+  computation = (
+      jax.jit(_fn)
+      .lower(init_state, jnp.ones(input_shape))
+      .compiler_ir(dialect='hlo')
+  )
   hlo_utils.output_hlo(computation, FLAGS.hlo_output)
 
 
 def encoder_full_model_opt_8_16():
   """Generates HLO for just the encoder of full transformer bfloat16."""
   encoder_from_file(config=full_model_bfloat16.get_config())
 
@@ -246,16 +257,16 @@
       use_bfloat16=False,
       dropout_rate=0.0,
       attention_dropout_rate=0.0)
   state = jax.jit(model.init)(rng, jnp.ones(encode_shape, jnp.float32),
                               jnp.ones(decode_shape, jnp.float32))
   if FLAGS.checkpoint:
     model = _restore_from_checkpoint(model, FLAGS.checkpoint)
-  state, cache = state.pop('cache')  # pytype: disable=attribute-error
-  state, params = state.pop('params')  # pytype: disable=attribute-error
+  state, cache = pop(state, 'cache')  # pytype: disable=attribute-error
+  state, params = pop(state, 'params')  # pytype: disable=attribute-error
   input_dummy = jnp.ones(encode_shape)
   if FLAGS.checkpoint:
 
     def _with_weights(inputs):
       return predict.step(
           inputs,
           params,
@@ -264,15 +275,17 @@
           EOS_TOKEN,
           decode_length,
           transformer_kwargs=transformer_kwargs,
           hparams=model_hparams,
           dynamic_context=quant_config.DynamicContext(
               update_bounds=False, quantize_acts=True))
 
-    computation = jax.xla_computation(_with_weights)(input_dummy)
+    computation = (
+        jax.jit(_with_weights).lower(input_dummy).compiler_ir(dialect='hlo')
+    )
   else:
 
     def _without_weights(inputs, params):
       return predict.step(
           inputs,
           params,
           cache,
@@ -280,15 +293,19 @@
           EOS_TOKEN,
           decode_length,
           transformer_kwargs=transformer_kwargs,
           hparams=model_hparams,
           dynamic_context=quant_config.DynamicContext(
               update_bounds=False, quantize_acts=True))
 
-    computation = jax.xla_computation(_without_weights)(input_dummy, params)
+    computation = (
+        jax.jit(_without_weights)
+        .lower(input_dummy, params)
+        .compiler_ir(dialect='hlo')
+    )
 
   hlo_utils.output_hlo(computation, FLAGS.hlo_output)
 
 
 def transformer_32_64_big_model():
   """Generates HLO that corresponds to a bigger version of the July demo."""
   transformer(
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/bleu.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/bleu.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/predict.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,47 +49,50 @@
       train=False,
       dynamic_context=dynamic_context,
       hparams=hparams,
       should_decode=False,
       dropout_rate=0.0,
       attention_dropout_rate=0.0,
       use_bfloat16=False)
+  mutable = ['sparsity']
+  new_logits, _ = model.apply({
+      'params': params,
+      **state
+  },
+                              inputs,
+                              method=model.encode,
+                              mutable=mutable)
   encoded_inputs = decode.flat_batch_beam_expand(
-      model.apply({
-          'params': params,
-          **state
-      },
-                  inputs,
-                  method=model.encode,
-                  mutable=False), beam_size)
+      new_logits, beam_size)
 
   def tokens_ids_to_logits(flat_ids, flat_cache):
     """Token slice to logits from decoder model."""
     # --> [batch * beam, 1, vocab]
     model = models.Transformer(
         **transformer_kwargs,
         train=False,
         dynamic_context=dynamic_context,
         hparams=hparams,
         should_decode=True,
         dropout_rate=0.0,
         attention_dropout_rate=0.0,
         use_bfloat16=False)
+    mutable = ['cache']
     flat_logits, new_vars = model.apply(
         {
             'params': params,
             'cache': flat_cache,
             **state
         },
         encoded=encoded_inputs,
         src_padding_mask=src_padding_mask,
         targets=flat_ids,
         tgt_padding_mask=tgt_padding_mask,
         method=model.decode,
-        mutable=['cache'])
+        mutable=mutable)
     new_flat_cache = new_vars['cache']
 
     return flat_logits, new_flat_cache
 
   # using the above-defined single-step decoder function, run a
   # beam search over possible sequences given input encoding.
   beam_seqs, _ = decode.beam_search(
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,15 +96,25 @@
           "mlp_dim": 4096,
           "share_embeddings": True,
           "logits_via_embedding": True,
       },
       "weight_outlier_regularization_regex": "^.*kernel$",
       "weight_quant_granularity": "per_channel",
 
+      "sparsity": {
+          "type": "STRUCTURED_NM",
+          "prune_rate": None,
+          "order": "R",  # row wise sparsity
+          "absolute": True,
+          "smallest": True,
+          "structure_decay": False,
+          "sparse_ste": False
+      },
   })
+  config.act_sparsity.order = "C"
   if not fp_quant:
     config.prec = None
     config.quant_type = "aqt"
   else:
     config.prec.is_scaled = False
     config.quant_type = "fake_quant"
   layernorm_config = config_schema.get_layer_norm_config(
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/train.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from absl import flags
 from absl import logging
 
 from aqt.jax_legacy.jax import compute_cost_utils
 from aqt.jax_legacy.jax import hlo_utils
 from aqt.jax_legacy.jax import quant_config
 from aqt.jax_legacy.jax import train_utils
+
+
 from aqt.jax_legacy.jax.wmt_mlperf import bleu
 from aqt.jax_legacy.jax.wmt_mlperf import input_pipeline
 from aqt.jax_legacy.jax.wmt_mlperf import models
 from aqt.jax_legacy.jax.wmt_mlperf import predict
 
 # train_flags is imported for the side effect of flag definitions.
 # These are used both in xm_launch.py and this training executable.
@@ -63,23 +65,34 @@
 import numpy as np
 import sacrebleu
 import tensorflow.compat.v2 as tf
 import tensorflow_text as tftxt
 
 
 
+flax.config.update('flax_use_orbax_checkpointing', False)
+
 T = TypeVar('T')
 
 EOS_TOKEN = 2  # Default Sentencepiece EOS token.
 
 COMPUTE_MEMORY_COST_FILENAME = 'compute_memory_cost.json'
 
 FLAGS = flags.FLAGS
 
 
+flags.DEFINE_bool(
+    'log_sparsity_scalars',
+    default=True,
+    help=(
+        'Log `apply_sparsity`, `update_weight_sparsity` and '
+        '`update_act_sparsity`  scalars to Tensorboard'
+    ),
+)
+
 config_flags.DEFINE_config_file('hparams_config_dict', None,
                                 'Path to file defining a config dict.')
 
 flags.DEFINE_integer(
     'config_idx',
     default=None,
     help=(
@@ -158,15 +171,15 @@
       attention_dropout_rate=0.1,
       should_decode=False)
   variables = model.init(
       key,
       jnp.zeros(input_shape, jnp.float32),
       jnp.zeros(target_shape, jnp.float32),
   )
-  init_state, params = variables.pop('params')  # pytype: disable=attribute-error
+  init_state, params = flax.core.pop(variables, 'params')  # pytype: disable=attribute-error
   return params, init_state
 
 
 # TODO(malmaud): Consider bundling the optimizer parameters into their own
 # HParams class
 def create_optimizer(params, learning_rate, weight_decay, beta1, beta2, eps):
   optimizer_def = optim.Adam(
@@ -343,15 +356,15 @@
         targets,
         inputs_positions=inputs_positions,
         targets_positions=targets_positions,
         inputs_segmentation=inputs_segmentation,
         targets_segmentation=targets_segmentation,
         mutable=True,
         rngs={'dropout': dropout_rng})
-    new_state, _ = new_variables.pop('params')
+    new_state, _ = flax.core.pop(new_variables, 'params')
     loss, weight_sum = compute_weighted_cross_entropy(logits, targets, weights)
     mean_loss = loss / weight_sum
     total_loss = mean_loss
 
 
     return total_loss, (logits, new_state)
 
@@ -364,23 +377,21 @@
   new_optimizer = optimizer.apply_gradient(loss_grad, learning_rate=lr)
 
   if FLAGS.compute_train_metrics:
     metrics = compute_metrics(logits, targets, weights)
   else:
     metrics = {}
   metrics['learning_rate'] = lr
-  # Compute or_loss for logging
-  # TODO(wanglisa): Is there a way to avoid computing it twice?
-  or_loss = custom_losses.weight_outlier_regularization_loss(
-      optimizer.target,
-      weights_regex_pattern=hparams.weight_outlier_regularization_regex)
-  metrics['or_loss'] = or_loss
+  metrics['apply_sparsity'] = dynamic_context.apply_sparsity
+  metrics['num_update_sparsity'] = dynamic_context.num_update_sparsity
+  metrics['update_weight_sparsity'] = dynamic_context.update_weight_sparsity
+  metrics['update_act_sparsity'] = dynamic_context.update_act_sparsity
 
-  return new_state, new_optimizer, metrics, new_dropout_rng
 
+  return new_state, new_optimizer, metrics, new_dropout_rng
 
 # TODO(shivaniagrawal): parametrize the axis_name and use the same axis name
 # throughout Transformer model.
 p_train_step = jax.pmap(
     functools.partial(train_step),
     axis_name='batch',
     static_broadcasted_argnums=(3, 4))
@@ -471,20 +482,23 @@
 def estimate_compute_and_memory_cost(
     model_dir: str, params: Mapping[str, Any], transformer_kwargs: Mapping[str,
                                                                            Any],
     state: Mapping[str,
                    Any], hparams: training_hparams.TrainingHParams) -> None:
   """Estimate compute and memory cost of model."""
 
-  without_weights_fn, input_dummy, target_dummy, state, params = get_jax_computation_of_model(
-      params=params,
-      transformer_kwargs=transformer_kwargs,
-      state=state,
-      hparams=hparams,
-      with_weights=False)
+  without_weights_fn, input_dummy, target_dummy, state, params = (
+      get_jax_computation_of_model(
+          params=params,
+          transformer_kwargs=transformer_kwargs,
+          state=state,
+          hparams=hparams,
+          with_weights=False,
+      )
+  )
   cost_dict = compute_cost_utils.estimate_costs_of_dot_and_conv_ops_from_jax_fn(
       without_weights_fn, params, input_dummy, target_dummy, state)
 
   path = tf.io.gfile.join(model_dir, COMPUTE_MEMORY_COST_FILENAME)
   with tf.io.gfile.GFile(path, 'w') as file:
     json.dump(cost_dict, file, indent=2)
   logging.info('Estimated compute and memory costs and wrote to file')
@@ -494,28 +508,34 @@
                      params: Mapping[str, Any], state: Mapping[str, Any],
                      hparams: training_hparams.TrainingHParams):
   """Writes training HLO for given model."""
   if not FLAGS.output_hlo_filename:
     return
 
   basename, _ = os.path.splitext(FLAGS.output_hlo_filename)
-  without_weights_fn, input_dummy, target_dummy, state, model = get_jax_computation_of_model(
-      params=params,
-      transformer_kwargs=transformer_kwargs,
-      state=state,
-      hparams=hparams,
-      with_weights=False)
+  without_weights_fn, input_dummy, target_dummy, state, model = (
+      get_jax_computation_of_model(
+          params=params,
+          transformer_kwargs=transformer_kwargs,
+          state=state,
+          hparams=hparams,
+          with_weights=False,
+      )
+  )
   _write_hlo(basename, without_weights_fn, model, input_dummy, target_dummy,
              state)
-  with_weights_fn, input_dummy, target_dummy, state, model = get_jax_computation_of_model(
-      params=params,
-      transformer_kwargs=transformer_kwargs,
-      state=state,
-      hparams=hparams,
-      with_weights=True)
+  with_weights_fn, input_dummy, target_dummy, state, model = (
+      get_jax_computation_of_model(
+          params=params,
+          transformer_kwargs=transformer_kwargs,
+          state=state,
+          hparams=hparams,
+          with_weights=True,
+      )
+  )
   _write_hlo(basename + '_with_weights', with_weights_fn, input_dummy,
              target_dummy, state)
 
 
 def _write_hlo(output, fn, *fn_args, **fn_kwargs):
   """Writes HLO for the given function.
 
@@ -529,15 +549,17 @@
     *fn_args: the function's args.
     **fn_kwargs: the function's kwargs.
 
   Returns:
     None.
   """
   try:
-    computation = jax.xla_computation(fn)(*fn_args, **fn_kwargs)
+    computation = (
+        jax.jit(fn).lower(*fn_args, **fn_kwargs).compiler_ir(dialect='hlo')
+    )
     logging.info('Generated XLA computation for HLO.')
     pb_path = tf.io.gfile.join(FLAGS.model_dir, f'{output}.pb')
     if not tf.io.gfile.exists(pb_path):
       hlo_utils.output_hlo(computation, pb_path)
       logging.info('Wrote serialized proto %s file.', pb_path)
     txt_path = tf.io.gfile.join(FLAGS.model_dir, f'{output}.txt')
     if not tf.io.gfile.exists(txt_path):
@@ -559,21 +581,23 @@
       dynamic_context=dynamic_context,
       use_bfloat16=FLAGS.use_bfloat16,
       train=False,
       hparams=hparams,
       dropout_rate=0.0,
       attention_dropout_rate=0.0,
       should_decode=False)
-  logits = model.apply({
+  mutable = ['sparsity']
+  # .apply() will return a tuple if mutable is not False
+  logits, _ = model.apply({
       'params': params,
       **state
   },
-                       inputs,
-                       targets,
-                       mutable=False)
+                          inputs,
+                          targets,
+                          mutable=mutable)
   return compute_metrics(logits, targets, weights)
 
 
 p_eval_step = jax.pmap(
     eval_step, axis_name='batch', static_broadcasted_argnums=(3, 4))
 # Argument 3 is transformer_kwargs. Argument 4 is hparams.
 
@@ -815,18 +839,22 @@
 
   def restore_checkpoint(self,
                          *,
                          model_dir: str,
                          prefix: str = 'checkpoint_') -> 'TrainingState':
     """Restore TrainingState from checkpoint in model_dir."""
     unreplicated_flax_state = jax_utils.unreplicate(self.flax_state)
-    optimizer, flax_state, dropout_rngs, transformer_kwargs = checkpoints.restore_checkpoint(
-        model_dir, (self.optimizer, unreplicated_flax_state, self.dropout_rngs,
-                    self.transformer_kwargs),
-        prefix=prefix)
+    target_state = (self.optimizer, unreplicated_flax_state, self.dropout_rngs,
+                    self.transformer_kwargs)
+    try:
+      optimizer, flax_state, dropout_rngs, transformer_kwargs = (
+          checkpoints.restore_checkpoint(model_dir, target_state, prefix=prefix)
+      )
+    except ValueError:
+      optimizer, flax_state, dropout_rngs, transformer_kwargs = target_state
     flax_state = jax_utils.replicate(flax_state)
     return type(self)(
         flax_state=flax_state,
         optimizer=optimizer,
         dropout_rngs=dropout_rngs,
         transformer_kwargs=transformer_kwargs)
 
@@ -848,19 +876,27 @@
   if train:
     collect_acts_stats = FLAGS.collect_acts_stats
   else:
     collect_acts_stats = False
   dynamic_context = train_utils.get_dynamic_context_for_step(
       activation_bound_update_freq=hparams.activation_bound_update_freq,
       activation_bound_start_step=hparams.activation_bound_start_step,
+      # TODO(shivaniagrawal): make a decision on passing this via hparams.
+      sparsity_start_step=FLAGS.sparsity_start_step,
+      sparsity_update_freq=FLAGS.sparsity_update_freq,
       step=step,
       collect_acts_stats=collect_acts_stats,
       prefer_int8_to_int32_dot=hparams.prefer_int8_to_int32_dot)
   if not train:
     dynamic_context = dataclasses.replace(dynamic_context, update_bounds=False)
+    dynamic_context = dataclasses.replace(dynamic_context, apply_sparsity=True)
+    dynamic_context = dataclasses.replace(
+        dynamic_context, update_act_sparsity=True)
+    dynamic_context = dataclasses.replace(
+        dynamic_context, update_weight_sparsity=False)
   return jax_utils.replicate(dynamic_context)
 
 
 def run_train_step(*, training_state: TrainingState, step: int, batch: Any,
                    hparams: training_hparams.TrainingHParams):
   """Run a single step of training."""
   dynamic_context = get_dynamic_context(hparams, step, train=True)
@@ -905,26 +941,29 @@
   def load(cls: Type[T], random_seed: int,
            eval_dataset_list: Optional[List[str]], batch_size: int) -> T:
     """Loads all datasets used by the training loop."""
     n_devices = jax.local_device_count()
     vocab_path = FLAGS.vocab_path
     if vocab_path is None:
       vocab_path = os.path.join(FLAGS.model_dir, 'sentencepiece_model')
-    train_ds, eval_ds_dict, train_eval_ds, predict_ds_dict, encoder = input_pipeline.get_wmt_datasets(
-        n_devices=n_devices,
-        dataset_name=FLAGS.dataset_name,
-        eval_dataset_list=eval_dataset_list,
-        shard_idx=jax.host_id(),
-        shard_count=jax.host_count(),
-        data_dir=FLAGS.data_dir,
-        vocab_path=vocab_path,
-        batch_size=batch_size,
-        max_length=FLAGS.max_target_length,
-        max_eval_length=FLAGS.max_eval_target_length,
-        seed=random_seed)
+    train_ds, eval_ds_dict, train_eval_ds, predict_ds_dict, encoder = (
+        input_pipeline.get_wmt_datasets(
+            n_devices=n_devices,
+            dataset_name=FLAGS.dataset_name,
+            eval_dataset_list=eval_dataset_list,
+            shard_idx=jax.host_id(),
+            shard_count=jax.host_count(),
+            data_dir=FLAGS.data_dir,
+            vocab_path=vocab_path,
+            batch_size=batch_size,
+            max_length=FLAGS.max_target_length,
+            max_eval_length=FLAGS.max_eval_target_length,
+            seed=random_seed,
+        )
+    )
     return cls(
         train_ds=train_ds,
         eval_ds_dict=eval_ds_dict,
         train_eval_ds=train_eval_ds,
         predict_ds_dict=predict_ds_dict,
         encoder=encoder)
 
@@ -984,19 +1023,26 @@
 
   # Scan the existing checkpoints and see if any correspond to a lower loss. If
   # so, this isn't the best checkpoint so return. Otherwise, we have a new best
   # checkpoint so delete the current one and write a new one.
 
   for dir_name, _, file_names in tf.io.gfile.walk(model_dir):
     for filename in file_names:
+      if filename == 'best_checkpoint_eval_loss_tmp':
+        file_path = tf.io.gfile.join(dir_name, filename)
+        tf.io.gfile.remove(file_path)
+        return
       # This regex will match a filename like 'best_checkpoint_eval_loss_1.5'
       # and will extract '1.5' into 'current_best_loss'.
       checkpoint_match = re.match(rf'.*{prefix}(.*)$', str(filename))
       if checkpoint_match is not None:
-        current_best_loss = float(checkpoint_match.group(1))
+        current_best_loss_str = checkpoint_match.group(1)
+        if current_best_loss_str == 'tmp':
+          return
+        current_best_loss = float(current_best_loss_str)
         if loss >= current_best_loss:
           return
         else:
           file_path = tf.io.gfile.join(dir_name, filename)
           tf.io.gfile.remove(file_path)
 
   training_state.save_checkpoint(model_dir=model_dir, step=loss, prefix=prefix)
@@ -1007,15 +1053,15 @@
   state_dict_keys = []
   if FLAGS.visualize_acts_bound:
     state_dict_keys.append('bounds')
   if FLAGS.collect_acts_stats:
     # State names from googlex.positron.tensorflow.jax.aqt.stats_tag.StatsTag
     state_dict_keys.extend([
         'min_per_ch', 'max_per_ch', 'mean_per_ch', 'stddev_per_ch',
-        'absdev_per_ch', 'stddev_per_ch_uncentered', 'absdev_per_ch_uncentered'
+        'absdev_per_ch', 'stddev_per_ch_uncentered', 'absdev_per_ch_uncentered',
     ])
   return state_dict_keys
 
 
 
 
 def eval_ds_name_to_summary_dir(eval_dataset_name: str) -> str:
@@ -1104,21 +1150,24 @@
   #    checkpoint in the model directory), we resume training based on the
   #    latest saved checkpoint.
   #
   # In a typical usecase, 'restore_checkpoint_model_dir' might point to a
   # bfloat16 model directory trained to convergence and this training run will
   # perform quantization-aware finetuning of that model.
   checkpoint_model_dir = None
-  if FLAGS.restore_checkpoint_model_dir is not None and not does_checkpoint_exist(
-      FLAGS.model_dir):
+  if (
+      FLAGS.restore_checkpoint_model_dir is not None
+      and not does_checkpoint_exist(FLAGS.model_dir)
+  ):
     checkpoint_model_dir = FLAGS.restore_checkpoint_model_dir
   elif FLAGS.restore_checkpoints:
     if not FLAGS.save_checkpoints:
       raise ValueError(
-          'If restore_checkpoints is enabled, then save_checkpoints must be enabled as well.'
+          'If restore_checkpoints is enabled, then save_checkpoints must be'
+          ' enabled as well.'
       )
     checkpoint_model_dir = FLAGS.model_dir
   if checkpoint_model_dir is not None:
     logging.info('Restoring checkpoint from: %s', checkpoint_model_dir)
     training_state = training_state.restore_checkpoint(
         model_dir=checkpoint_model_dir)
     # Grab last step from the first of the optimizer replicas.
@@ -1153,16 +1202,14 @@
           hparams=hparams,
           transformer_kwargs=transformer_kwargs)
     state = jax_utils.replicate(state)
     optimizer = optimizer.replicate()
     logging.info('Replicated optimizer.')
 
   t_loop_start = time.time()
-  t_train = timer.MultiIntervalTimer()
-  t_train.Start()
   for step, batch in zip(range(start_step, num_train_steps), train_iter):
     # Shard data to devices and do a training step.
     training_state, metrics = run_train_step(
         training_state=training_state, batch=batch, step=step, hparams=hparams)
     state = training_state.flax_state
     optimizer = training_state.optimizer
     metrics_all.append(metrics)
@@ -1174,53 +1221,56 @@
     if step % FLAGS.checkpoint_freq == 0 and step > 0:
       if jax.host_id() == 0 and FLAGS.save_checkpoints:
         training_state.save_checkpoint(model_dir=FLAGS.model_dir, step=step)
 
 
     # Periodic metric handling.
     if step % eval_freq == 0:
-      t_train.Stop()
 
       # Training Metrics
       if FLAGS.compute_train_metrics:
         metrics_all = common_utils.get_metrics(metrics_all)
         state_dict_summary_all = common_utils.get_metrics(
             state_dict_summary_all)
         lr = metrics_all.pop('learning_rate').mean()
 
         metrics_sums = jax.tree_map(jnp.sum, metrics_all)
         denominator = metrics_sums.pop('denominator')
-        or_loss = metrics_sums.pop('or_loss').mean()
         summary = jax.tree_map(lambda x: x / denominator, metrics_sums)  # pylint: disable=cell-var-from-loop
         summary['learning_rate'] = lr
-        summary['or_loss'] = or_loss
+        if FLAGS.log_sparsity_scalars:
+          apply_sparsity = metrics_all.pop('apply_sparsity').mean()
+          update_weight_sparsity = metrics_all.pop(
+              'update_weight_sparsity').mean()
+          update_act_sparsity = metrics_all.pop('update_act_sparsity').mean()
+          num_update_sparsity = metrics_all.pop('num_update_sparsity').mean()
+          summary['apply_sparsity'] = apply_sparsity
+          summary['update_weight_sparsity'] = update_weight_sparsity
+          summary['update_act_sparsity'] = update_act_sparsity
+          summary['num_update_sparsity'] = num_update_sparsity
         summary['perplexity'] = jnp.clip(jnp.exp(summary['loss']), a_max=1.0e4)
         logging.info('train in step: %d, loss: %.4f', step, summary['loss'])
         steps_per_eval = eval_freq if step != 0 else 1
         steps_per_sec = steps_per_eval / (time.time() - t_loop_start)
-        train_steps_per_sec = steps_per_eval / t_train.GetDuration()
         t_loop_start = time.time()
 
         if jax.host_id() == 0:
           assert train_summary_writer is not None, ('train_summary_writer was '
                                                     'not initialized on host 0')
           train_summary_writer.scalar('steps per second', steps_per_sec, step)
-          train_summary_writer.scalar('training steps per second',
-                                      train_steps_per_sec, step)
           for key, val in summary.items():
             train_summary_writer.scalar(key, val, step)
 
           summary_utils.write_state_dict_summaries_to_tb(
               state_dict_summary_all, train_summary_writer,
               FLAGS.state_dict_summary_freq, step)
           train_summary_writer.flush()
 
       state_dict_summary_all = []
       metrics_all = []
-      logging.info('train time: %.4f s step %d', t_train.GetDuration(), step)
 
       # TODO(shivaniagrawal): Add bleu score summaries for additional eval
       # datasets?
       # Additional eval metrics
       for eval_dataset_name, eval_ds in datasets.eval_ds_dict.items():
         summary_writer = None
         t_add_eval_start = time.time()
@@ -1306,14 +1356,11 @@
         assert eval_summary_writer is not None, ('eval_summary_writer was not '
                                                  'initialized on host 0')
         eval_summary_writer.scalar('bleu', bleu_score, step)
         eval_summary_writer.scalar('sacrebleu', sacrebleu_score, step)
         eval_summary_writer.text('samples', exemplars, step)
         eval_summary_writer.flush()
 
-      # restart training-only timer
-      t_train.Reset()
-      t_train.Start()
 
 
 if __name__ == '__main__':
   app.run(main)
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/decode.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/decode.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,24 +142,24 @@
 # Beam search state:
 
 
 @flax.struct.dataclass
 class BeamState:
   """Holds beam search state data."""
   # The position of the decoding loop in the length dimension.
-  cur_index: jnp.DeviceArray  # scalar int32: current decoded length index
+  cur_index: jax.Array  # scalar int32: current decoded length index
   # The active sequence log probabilities and finished sequence scores.
-  live_logprobs: jnp.DeviceArray  # float32: [batch_size, beam_size]
-  finished_scores: jnp.DeviceArray  # float32: [batch_size, beam_size]
+  live_logprobs: jax.Array  # float32: [batch_size, beam_size]
+  finished_scores: jax.Array  # float32: [batch_size, beam_size]
   # The current active-beam-searching and finished sequences.
-  live_seqs: jnp.DeviceArray  # int32: [batch_size, beam_size, max_decode_len]
-  finished_seqs: jnp.DeviceArray  # int32: [batch_size, beam_size,
+  live_seqs: jax.Array  # int32: [batch_size, beam_size, max_decode_len]
+  finished_seqs: jax.Array  # int32: [batch_size, beam_size,
   #                                         max_decode_len]
   # Records which of the 'finished_seqs' is occupied and not a filler slot.
-  finished_flags: jnp.DeviceArray  # bool: [batch_size, beam_size]
+  finished_flags: jax.Array  # bool: [batch_size, beam_size]
   # The current state of the autoregressive decoding caches.
   cache: typing.Any  # Any pytree of arrays, e.g. flax attention Cache object
 
 
 def beam_init(batch_size, beam_size, max_decode_len, cache):
   """Initializes the beam search state data structure."""
   cur_index0 = jnp.array(0)
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py` & `aqtp-0.1.0/aqt/jax_legacy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,14 +167,23 @@
     # This tests that the schema of the configdict returned by 'config_schema',
     # once all references are resolved, matches an expected schema. 'Schema'
     # here means the names and structure of fields at each level of the
     # configuration hierarchy. A value of 'None' in the expected schemas defined
     # below indicates a real configuration would have a concrete scalar value
     # there.
 
+    sparsity_schema = {
+        'type': None,
+        'prune_rate': [None, None],  # set to default structured
+        'smallest': None,
+        'order': None,
+        'absolute': None,
+        'structure_decay': None,
+        'sparse_ste': None
+    }
 
     quant_act_schema = {
         'bounds': {
             'initial_bound': None,
             'stddev_coeff': None,
             'absdev_coeff': None,
             'mix_coeff': None,
@@ -192,14 +201,16 @@
 
     dense_schema = {
         'weight_prec': None,
         'weight_quant_granularity': None,
         'quant_type': None,
         'quant_act': quant_act_schema,
         'weight_half_shift': None,
+        'weight_sparsity': sparsity_schema,
+        'act_sparsity': sparsity_schema,
     }
 
     embedding_schema = {
         'weight_prec': None,
         'quant_type': None,
         'quant_act': quant_act_schema,
         'weight_half_shift': None,
@@ -271,14 +282,17 @@
         'quant_type': None,
         'quant_act': quant_act_schema,
         'weight_quant_granularity': None,
         'dense': dense_schema,
         'embedding': embedding_schema,
         'mlp_block': mlp_block_schema,
         'attention': attention_schema,
+        'sparsity': sparsity_schema,
+        'weight_sparsity': sparsity_schema,
+        'act_sparsity': sparsity_schema,
         'model_hparams': {
             'emb_dim': None,
             'num_heads': None,
             'qkv_dim': None,
             'mlp_dim': None,
             'share_embeddings': None,
             'logits_via_embedding': None,
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py`

 * *Files 14% similar despite different names*

```diff
@@ -131,26 +131,44 @@
 flags.DEFINE_bool(
     'compute_train_metrics',
     default=True,
     help='Whether to compute the metrics during training.')
 
 flags.DEFINE_string(
     'output_hlo_filename',
-    default='hlo',
-    help='Output model HLO to filename in FLAGS.model_dir. Both HLO text '
-    '(filename.txt) and protobuf (filename.pb) are emitted. If None, or empty '
-    'string, no HLO files will be written.')
+    default=None,
+    help=(
+        'Output model HLO to filename in FLAGS.model_dir. Both HLO text'
+        ' (filename.txt) and protobuf (filename.pb) are emitted. If None, or'
+        ' empty string, no HLO files will be written.'
+    ),
+)
 
 flags.DEFINE_string(
     'output_beam_hlo_filename',
     default=None,
     help='Output model HLO, including the decoding beam search, to filename in'
     'FLAGS.model_dir. Both HLO text (filename.txt) and protobuf (filename.pb)'
     ' are emitted.')
 
+flags.DEFINE_integer(
+    'sparsity_start_step',
+    default=-1,
+    help=(
+        'First step to compute sparsity mask at, defaults to -1 in which case '
+        'we do not compute sparsity mask.'))
+
+flags.DEFINE_integer(
+    'sparsity_update_freq',
+    default=0,
+    help=(
+        'How often (number of steps )to update sparsity mask, defaults to 0 in '
+        'which case we do not update again.'
+    ),
+)
 
 flags.DEFINE_bool(
     'visualize_acts_bound',
     default=False,
     help=(
         'Whether to visualize activations bounds for auto-clip in Tensorboard.'
         ' The bounds appear as scalar and will be named as "GetBounds_0/bounds"'
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/stats_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/stats_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/flax_attention.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/flax_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,15 +360,15 @@
             key, mask=key_padding_mask_transposed)
 
   if query_padding_mask is not None:
     query_padding_mask_transposed = query_padding_mask.transpose(qk_perm)
     shape_utils.assert_shapes_equal(query_padding_mask_transposed.shape,
                                     (batch_size, 1, query_sequence_length, 1))
 
-  key_get_bounds_params = get_bounds.GetBounds.Params(
+  key_bounds_params = get_bounds.GetBounds.Params(
       update_bounds=dynamic_context.update_bounds,
       update_stats=train,
       paxis_name=paxis_name,
       mask=key_padding_mask_transposed,
       module_name='K')
 
   # v -> (bs, <non-attention dims>, num_heads, channels, <attention dims>)
@@ -383,15 +383,15 @@
                                     (batch_size, 1, 1, key_sequence_length))
 
   if dynamic_context.collect_acts_stats:
     stats_tag.StatsTag(
         channel_axis=None, name='attn_act_v', update_stats=train)(
             value, mask=value_padding_mask_transposed)
 
-  value_get_bounds_params = get_bounds.GetBounds.Params(
+  value_bounds_params = get_bounds.GetBounds.Params(
       update_bounds=dynamic_context.update_bounds,
       update_stats=train,
       paxis_name=paxis_name,
       mask=value_padding_mask_transposed,
       module_name='V')
 
   query = query / jnp.sqrt(depth).astype(dtype)
@@ -400,15 +400,15 @@
       query.shape, (batch_size, num_heads, query_sequence_length, channel_size))
 
   if dynamic_context.collect_acts_stats:
     stats_tag.StatsTag(
         channel_axis=None, name='attn_act_q', update_stats=train)(
             query, mask=query_padding_mask_transposed)
 
-  query_get_bounds_params = get_bounds.GetBounds.Params(
+  query_bounds_params = get_bounds.GetBounds.Params(
       update_bounds=dynamic_context.update_bounds,
       update_stats=train,
       paxis_name=paxis_name,
       mask=query_padding_mask_transposed,
       module_name='Q')
 
   batch_dims_t = tuple(range(len(batch_dims)))
@@ -416,17 +416,17 @@
       lhs_act=query,
       rhs_act=key,
       dot_dimension_numbers=(((n - 1,), (n - 1,)), (batch_dims_t,
                                                     batch_dims_t)),
       dot_precision=precision,
       quant_type=hparams.quant_type,
       lhs_act_hparams=hparams.attn_act_q,
-      lhs_get_bounds_params=query_get_bounds_params,
+      lhs_bounds_params=query_bounds_params,
       rhs_act_hparams=hparams.attn_act_k,
-      rhs_get_bounds_params=key_get_bounds_params,
+      rhs_bounds_params=key_bounds_params,
   )
   # NOTE(shivaniagrawal): we do per-layer quantization here since that's the
   # only way for activation*activation matmuls to be aqt compatible since we use
   # static scaling factors for activations.
 
   shape_utils.assert_shapes_equal(
       attn_weights.shape,
@@ -467,15 +467,15 @@
             attn_weights, mask=attn_mask)
 
   if hparams.attn_act_probs is not None:
     assert hparams.attn_act_probs.bounds == 1.0, (
         'act quantization bounds should '
         'be set to fix value 1.0 to '
         'match Softmax range.')
-  probs_get_bounds_params = get_bounds.GetBounds.Params(
+  probs_bounds_params = get_bounds.GetBounds.Params(
       update_bounds=dynamic_context.update_bounds,
       update_stats=train,
       paxis_name=paxis_name,
       mask=attn_mask,
       module_name='attn_probs')
 
   # compute the new values given the attention weights
@@ -483,17 +483,17 @@
   y = quantized_dynamic_dot_general(
       lhs_act=attn_weights,
       rhs_act=value,
       dot_dimension_numbers=(wv_contracting_dims, (batch_dims_t, batch_dims_t)),
       dot_precision=precision,
       quant_type=hparams.quant_type,
       lhs_act_hparams=hparams.attn_act_probs,
-      lhs_get_bounds_params=probs_get_bounds_params,
+      lhs_bounds_params=probs_bounds_params,
       rhs_act_hparams=hparams.attn_act_v,
-      rhs_get_bounds_params=value_get_bounds_params,
+      rhs_bounds_params=value_bounds_params,
   )
   # NOTE(shivaniagrawal): we do per-layer quantization here since that's the
   # only way for activation*activation matmuls to be aqt compatible since we
   # use static scaling factors for activations.
 
   shape_utils.assert_shapes_equal(
       y.shape, (batch_size, num_heads, query_sequence_length, channel_size))
@@ -832,15 +832,15 @@
     return out
 
 
 class SelfAttentionAqt(MultiHeadDotProductAttentionAqt):
   """Self-attention."""
 
   @nn.compact
-  def __call__(
+  def __call__(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self,
       inputs_q: jnp.ndarray,
       *,
       padding_mask: Optional[jnp.ndarray],
       segmentation: Optional[jnp.ndarray] = None,
   ) -> jnp.ndarray:
     return super().__call__(
```

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/primitives_test.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/primitives_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax_legacy/jax/stats_tag.py` & `aqtp-0.1.0/aqt/jax_legacy/jax/stats_tag.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/tensorflow/aqt_matmul_test.py` & `aqtp-0.1.0/aqt/jax/aqt_tensor.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,507 +7,426 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Accurate Quantized Training ops."""
 
-"""Tests for matmul."""
+from __future__ import annotations
 
-import copy
-from unittest import mock
+from typing import List, Optional, Tuple
 
-from absl.testing import absltest
-from absl.testing import parameterized
+from aqt.common import aqt_common
 from aqt.common import aqt_config
-from aqt.tensorflow import aqt_matmul
-from aqt.tensorflow import aqt_tensor
-from aqt.test import aqt_test_shared_base
-import numpy as np
-import tensorflow.compat.v1 as tf
-
-
-def test_stats_config():
-  """Config base for all the experiments."""
-  return aqt_config.StatsConfig(
-      ema_update_count=1,  # single update overwrites the stats
-      update_count_prior=0,  # easier equations
-      share_stats_axes=[0, 1],  # one stat per whole tensor
-      tpu_cross_replica_sum=False,  # no cross-tpu reduction
-      filter_zeros=False,  # on default zeros are a number like any other
-  )
-
-
-def i64(x):
-  """Convenience tf.i64 wrapper."""
-  return tf.constant(x, dtype=tf.int64)
-
-
-def calibration_config(const_coeff: float) -> aqt_config.CalibrationConfig:
-  return aqt_config.CalibrationConfig(const_bound_coeff=const_coeff)
-
-
-def _schedule_config(bits, const_bound_coeff,
-                     share_stats_axes) -> aqt_config.AqtScheduleConfig:
-  """Creates schedule config with dynamic quantization."""
-  iqc = aqt_config.IntQuantConfig(bits=bits)
-  cc = aqt_config.CalibrationConfig(const_bound_coeff=const_bound_coeff)
-  tc = aqt_config.AqtTensorConfig(
-      quant_config=iqc, calibration_config=cc, freeze_scale_at_begin=True)
-  sc = aqt_config.StatsConfig(
-      ema_update_count=1,
-      share_stats_axes=list(share_stats_axes),
-      update_count_prior=0,
-      tpu_cross_replica_sum=False)
-  return aqt_config.AqtScheduleConfig(sc, [tc])
-
-
-def config_from_schedule(schedule):
-  """Generates a schedule config from [(start, end, bits), ...]."""
-  tensor_configs = []
-  for start, end, bits in schedule:
-    int_quant_config = aqt_config.IntQuantConfig(bits, preserve_zero=False)
-
-    tensor_config = aqt_config.AqtTensorConfig(
-        freeze_scale_at_begin=True,
-        quant_config=int_quant_config,
-        begin_at_event=start,
-        end_at_event=end,
-        calibration_config=calibration_config(1.0))
-
-    tensor_configs.append(tensor_config)
-  return aqt_config.AqtScheduleConfig(test_stats_config(), tensor_configs)
-
-
-def update_event_count(matmul, event_count_int: int):
-  """Update the quantizer's event count without changing stats."""
-  for quantizer in [matmul.lhs_quantizer, matmul.rhs_quantizer]:
-    sample = tf.zeros(quantizer.data_shape)
-    weights = tf.zeros([1] * len(quantizer.data_shape))
-    event_count = tf.constant(event_count_int, tf.int64)
-    quantizer.update(sample, weights, event_count).run()
-
-
-def matmul_config(matmul):
-  """Creates an AqtMatmulConfig corresponding to a Matmul."""
-  return aqt_config.AqtMatmulConfig(matmul.lhs_quantizer.config,
-                                    matmul.rhs_quantizer.config)
-
-
-class IntNarrowedMatMulTest(tf.test.TestCase, parameterized.TestCase):
-
-  def test_chooses_right_matmul(self):
-    # Create a list of settings (left_bits, right_bits, expected_matmul)
-    # and generate a schedule based on those settings.
-    settings = [(8, 16, "default"), (4, 16, "default"), (4, 8, "int8"),
-                (8, 9, "default"), (4, 4, "int8"), (3, 3, "int8"),
-                (9, 7, "default")]
-
-    lhs_schedule = []
-    rhs_schedule = []
-    expected_results = []
-    for i, (l, r, expected) in enumerate(settings):
-      lhs_schedule.append((i, i + 1, l))
-      rhs_schedule.append((i, i + 1, r))
-      expected_results.append(expected)
-
-    lhs_config = config_from_schedule(lhs_schedule)
-    rhs_config = config_from_schedule(rhs_schedule)
-
-    shape = [1, 1]  # Any shape will do, we're mocking.
-    lhs_quant = aqt_tensor.TensorQuantizer(shape, lhs_config, name="lhs")
-    rhs_quant = aqt_tensor.TensorQuantizer(shape, rhs_config, name="rhs")
-
-    module = "aqt.tensorflow.aqt_matmul"
-    with mock.patch(f"{module}.default_matmul") as default_matmul, \
-         mock.patch(f"{module}.int8_matmul") as int8_matmul:
-      default_matmul.return_value = tf.constant("default")
-      int8_matmul.return_value = tf.constant("int8")
-
-      event_ph = tf.placeholder(tf.int64)
-      lhs_quant._last_update = event_ph
-      rhs_quant._last_update = event_ph
-      tf_actual = aqt_matmul._matmul_case(lhs_quant, rhs_quant, None, None,
-                                          True)
-
-      with self.cached_session():
-        tf.global_variables_initializer().run()
-        for i, expected in enumerate(expected_results):
-          actual = tf_actual.eval(feed_dict={event_ph: i})
-          self.assertEqual(
-              actual.decode("utf-8"), expected, msg=f"event_count {i}")
-
-
-class MatmulTest(tf.test.TestCase, parameterized.TestCase):
-
-  def exact_int8_matmul_example(self,
-                                lhs_use_quantized_variable=False,
-                                rhs_use_quantized_variable=False):
-    lhs_config, lhs, rhs_config, rhs = aqt_test_shared_base.exact_int8_example(
-        lhs_shape=(3, 2),
-        rhs_shape=(2, 2),
-        lhs_share_stats_axes=[0, 1],
-        rhs_share_stats_axes=[0, 1],
-        lhs_use_quantized_variable=lhs_use_quantized_variable,
-        rhs_use_quantized_variable=rhs_use_quantized_variable)
-
-    lhs = tf.constant(lhs, tf.float32)
-    rhs = tf.constant(rhs, tf.float32)
-
-    config = aqt_config.AqtMatmulConfig(lhs_config, rhs_config)
-    mm = aqt_matmul.Matmul(config, lhs.shape, rhs.shape)
-
-    return mm, lhs, rhs
-
-  # No quantization and float config give aqt_matmul = tf.matmul
-  def test_matmul_none(self):
-    no_quant_config = aqt_config.AqtScheduleConfig(test_stats_config(), [])
-    float_config_tc = aqt_config.AqtTensorConfig(
-        freeze_scale_at_begin=True,
-        quant_config=aqt_config.FloatConfig(),
-        calibration_config=calibration_config(1))
-    float_config = aqt_config.AqtScheduleConfig(test_stats_config(),
-                                                [float_config_tc])
-
-    lhs = np.random.uniform(-1.0, 1.0, size=(2, 3)).astype(np.float32)
-    lhs = tf.constant(lhs)
-
-    rhs = np.random.uniform(-1.0, 1.0, size=(3, 4)).astype(np.float32)
-    rhs = tf.constant(rhs)
-
-    config = aqt_config.AqtMatmulConfig(no_quant_config, no_quant_config)
-    mm_no_quant = aqt_matmul.Matmul(config, lhs.shape, rhs.shape, "no_quant")
-    config = aqt_config.AqtMatmulConfig(float_config, float_config)
-    mm_float = aqt_matmul.Matmul(config, lhs.shape, rhs.shape, "float")
-
-    no_quant_ret = mm_no_quant.apply(lhs, rhs)
-    float_config_ret = mm_float.apply(lhs, rhs)
-    expected_ret = tf.matmul(lhs, rhs)
-
-    with self.cached_session():
-      tf.global_variables_initializer().run()
-      self.assertAllEqual(no_quant_ret, expected_ret)
-      self.assertAllEqual(float_config_ret, expected_ret)
-
-  def basic_quant_example(self):
-    lhs_config = _schedule_config(3, 7, [0, 1])
-    lhs = tf.constant(
-        np.array(
-            [
-                [-8, 4.01, 4.01],  #
-                [-5.99, 0.01, -4.01],
-            ],
-            dtype=np.float32))
-    qlhs = tf.constant(
-        np.array(
-            [
-                [-6, 4, 4],  #
-                [-6, 0, -4]
-            ],
-            dtype=np.float32))
-
-    # Representable values: -1, 0, 1
-    rhs_config = _schedule_config(2, 1.5, [0, 1])
-    rhs = tf.constant(
-        np.array(
-            [
-                [-3, 0.99],  #
-                [-0.99, 0],
-                [-0.01, 2]
-            ],
-            dtype=np.float32))
-    qrhs = tf.constant(
-        np.array(
-            [
-                [-1, 1],  #
-                [-1, 0],
-                [0, 1]
-            ],
-            dtype=np.float32))
-
-    config = aqt_config.AqtMatmulConfig(lhs_config, rhs_config)
-
-    return config, lhs, qlhs, rhs, qrhs
-
-  def test_basic_matmul(self):
-    config, lhs, qlhs, rhs, qrhs = self.basic_quant_example()
-
-    mm = aqt_matmul.Matmul(config, lhs.shape, rhs.shape)
-
-    event_count = tf.constant(0, tf.int64)
-    updates = [
-        mm.update_lhs(lhs, None, event_count),
-        mm.update_rhs(rhs, None, event_count)
-    ]
-    with tf.control_dependencies(updates):
-      actual = mm.apply(lhs, rhs)
-    expected = tf.matmul(qlhs, qrhs)
-
-    with self.cached_session() as sess, sess.as_default():
-      tf.global_variables_initializer().run()
-      self.assertAllEqual(expected, actual)
-
-  @parameterized.parameters([dict(lhs_float=True), dict(lhs_float=False)])
-  def test_float_config_basic_matmul(self, lhs_float):
-    config, lhs, qlhs, rhs, qrhs = self.basic_quant_example()
-
-    if lhs_float:
-      config.lhs.tensor_configs[0].quant_config = aqt_config.FloatConfig()
+from flax import linen as nn
+from flax import struct
+import jax
+import jax.numpy as jnp
+
+
+def pass_through(x: jnp.ndarray, fn) -> jnp.ndarray:
+  # Create an exactly-zero expression with Sterbenz lemma that has an
+  # exactly-one gradient.
+  return x - jax.lax.stop_gradient(x) + jax.lax.stop_gradient(fn(x))
+
+
+class Stats(nn.Module):
+  """Manages efficient gatherting of running statistics."""
+
+  # This type annotation is what the constructor expects.
+  # However nn.Module silently converts it into immutable Tuple, so
+  # the methods will observe Tuple[Optional[int], ...]
+  data_shape: List[Optional[int]] = struct.field(pytree_node=False)
+  config: aqt_config.StatsConfig = struct.field(pytree_node=False)
+
+  def setup(self):
+    """Constructor to init a Stats instance.
+
+    Returns:
+      A new instance of Stats, with initialized statistics.
+    """
+    self.config.validate(self.data_shape)
+    # TODO(jihwanlee): Move the check below in the config validator.
+    if self.config.lp_order > 30:
+      raise NotImplementedError('For higher norms we should add stabilization.')
+    stats_shape = list(self.data_shape)  # nn.Module converts lists to tuples.
+    for axis in self.config.share_stats_axes:
+      stats_shape[axis] = 1
+    self.stats_shape = stats_shape
+
+    def init_var(init_val: float) -> jnp.ndarray:
+      return jnp.full(self.stats_shape, init_val, dtype=jnp.float32)
+
+    def mk_var(name: str, init_val: float) -> nn.Variable:
+      return self.variable('aqt', name, init_var, init_val)
+
+    self.ema_update_count = self.config.ema_update_count
+    self.sum_of_ones = mk_var('sum_of_ones', self.config.update_count_prior)
+    self.sum_of_vals = mk_var(
+        'sum_of_vals', self.config.mean_prior * self.config.update_count_prior)
+    self.max_of_abs_vals = mk_var('max_of_abs_vals', self.config.max_dev_prior)
+    self.sum_of_l1_vals = mk_var(
+        'sum_of_l1_vals',
+        self.config.l1_dev_prior * self.config.update_count_prior)
+    self.sum_of_lp_vals = mk_var(
+        'sum_of_lp_vals', self.config.lp_dev_prior**self.config.lp_order *
+        self.config.update_count_prior)
+
+  def __call__(self):
+    # Keep __call__() just not to require users to explicitly specify which
+    # method should be called when invoking init().
+    pass
+
+  # TODO(lew): Remvoe override_ema_update_count.
+  #   override_ema_update_count is used only in tests and is a hack.
+  #   However replacing it with  self.ema_update_count does not work,
+  #   because nn.Model will not allow to access it from outside.
+  #   I'm not sure how this should be solved cleanly.
+  def update(self,
+             x: jnp.ndarray,
+             weight: Optional[jnp.ndarray],
+             override_ema_update_count=None):
+    """Returns a new Stats object with updated statistics.
+
+    Since flax.struct.dataclass objects are frozen, thie update method uses
+    the dataclass.replace method to get a new object replacing the existing
+    statistics with new ones and returns it.
+
+    Args:
+      x: input array to update the current statistics with.
+      weight: weight for the input array x.
+      override_ema_update_count: use this value instead of the one in config.
+
+    Returns:
+      Anew object of Stats with updated statistics.
+    """
+    aqt_common.check_shapes_conformal(x.shape, self.data_shape)
+    if weight is not None and len(x.shape) != len(weight.shape):
+      raise ValueError(
+          f'expected rank(x)={len(x.shape)} == rank(weight)={weight.shape}')
+
+    def update_var(var, s, reduce_max=False):
+      assert len(s.shape) == len(self.data_shape), (s.shape, self.data_shape)
+      assert s.size > 0
+      if weight is not None:
+        if reduce_max:
+          # A maximum is a maximum, regardless of its nonzero weight.
+          s = jnp.where(weight > 0, s, 0)
+        else:
+          s = s * weight
+      reduce_fn = jnp.max if reduce_max else jnp.sum
+      s = reduce_fn(s, axis=self.config.share_stats_axes, keepdims=True)
+      if self.config.tpu_cross_replica_sum:
+        raise NotImplementedError(
+            'support for tpu_cross_replica_sum=True is not implemented')
+      override = override_ema_update_count
+      rate = 1.0 / (override if override is not None else self.ema_update_count)
+      var.value = (1.0 - rate) * var.value + rate * s
+
+    # Layers such as ReLU emit zeros often. In such cases, we can model
+    # the non-sparse distribution of weights separately, resulting in
+    # unbiased estimation of non-sparse mean l1 and lp.
+    # This clips away less of the distribution of inputs.
+    if self.config.filter_zeros:
+      ones = jnp.where(x != 0, 1., 0.)
     else:
-      config.rhs.tensor_configs[0].quant_config = aqt_config.FloatConfig()
+      ones = jnp.ones_like(x)
+
+    px = x if self.config.lp_order % 2 == 0 else jnp.abs(x)
+
+    update_var(self.sum_of_ones, ones)
+    update_var(self.sum_of_vals, x)
+    update_var(self.max_of_abs_vals, jnp.abs(x), reduce_max=True)
+    update_var(self.sum_of_l1_vals, jnp.abs(x))
+    update_var(self.sum_of_lp_vals, px**self.config.lp_order)
+
+  def mean(self) -> jnp.ndarray:
+    return self.sum_of_vals.value / self.sum_of_ones.value
 
-    mm = aqt_matmul.Matmul(config, lhs.shape, rhs.shape)
+  def max_dev(self) -> jnp.ndarray:
+    return self.max_of_abs_vals.value
 
-    event_count = tf.constant(0, tf.int64)
-    updates = [
-        mm.update_lhs(lhs, None, event_count),
-        mm.update_rhs(rhs, None, event_count)
+  def l1_dev(self) -> jnp.ndarray:
+    return self.sum_of_l1_vals.value / self.sum_of_ones.value
+
+  def lp_dev(self) -> jnp.ndarray:
+    if self.config.lp_order == 2:
+      # sqrt() is numerically more accurate
+      return jnp.sqrt(self.sum_of_lp_vals.value / self.sum_of_ones.value)
+    else:
+      # TODO(b/205769820): Make sure if the output of pow op below is
+      # numerically valid.
+      return (self.sum_of_lp_vals.value /
+              self.sum_of_ones.value)**(1.0 / self.config.lp_order)
+
+  def bound(  #
+      self, calibration_config: aqt_config.CalibrationConfig) -> jnp.ndarray:
+    """Compute the upper bound on input tensor values, broadcastable to input."""
+    return (calibration_config.l1_dev_coeff * self.l1_dev() +  #
+            calibration_config.lp_dev_coeff * self.lp_dev() +  #
+            calibration_config.max_dev_coeff * self.max_dev() +  #
+            calibration_config.const_bound_coeff)
+
+
+def is_config_active(config: aqt_config.AqtTensorConfig,
+                     event_count: jnp.ndarray) -> bool:
+  """Return whether the configuration is active at event_count."""
+  config.validate()
+  should_q = True
+  if config.begin_at_event is not None:
+    should_q &= config.begin_at_event <= event_count
+  if config.end_at_event is not None:
+    should_q &= event_count < config.end_at_event
+  return should_q
+
+
+class TensorQuantizer(nn.Module):
+  """Maintains state associated with the quantization of an input tensor.
+
+  A TensorQuantizer owns observed statistics for an input tensor, along with
+  variables for the scale and event_count copy, recording the last time of then
+  most recent update to this `TensorQuantizer` class.
+
+  This class provides state-mutating methods for updating statistics for every
+  observation of an input tensor and is used by AQT methods to derive
+  calibration bounds.
+
+  TensorQuantizer assumes the supplied `event_count` strictly monotonically
+  increases across `TensorQuantizer.update` calls and starts out strictly
+  greater than `int32.min`.
+
+  Attributes:
+    data_shape: the shape of input tensor. Some dimensions may be of unknown
+      size, but these must have stats shared in `config.stats_config`. In this
+      case, use of quanitzed variable is disallowed.
+    config: A training quantization schedule.
+    quantized_variable: If provided during initialization, stores the quantized
+      version of the observed tensor from the most recent `update()`.
+  """
+  data_shape: List[Optional[int]]
+  config: Optional[aqt_config.AqtScheduleConfig] = None
+
+  def setup(self):
+    if self.config is not None:
+      self.config.fill_gaps_with_float_config()
+      self.config.validate(self.data_shape)
+      self._stats = Stats(self.data_shape, self.config.stats_config)
+      self._scale = self.variable('TensorQuantizer', 'scale', jnp.zeros,
+                                  self._stats.stats_shape, jnp.float32)
+      self._inv_scale = self.variable('TensorQuantizer', 'inv_scale', jnp.zeros,
+                                      self._stats.stats_shape, jnp.float32)
+      if self.config.use_quantized_variable:
+        self.quantized_variable = self.variable('TensorQuantizer',
+                                                'quantized_variable', jnp.zeros,
+                                                self.data_shape, jnp.int8)
+      else:
+        self.quantized_variable = self.variable('TensorQuantizer',
+                                                'quantized_variable',
+                                                lambda: None)
+      self._last_update = self.variable('TensorQuantizer', 'last_update',
+                                        lambda: jnp.iinfo(jnp.int32).min)
+
+  def __call__(self):
+    # Keep __call__() just not to require users to explicitly specify which
+    # method should be called when invoking init().
+    pass
+
+  def _fresh_scale(
+      self,
+      config: aqt_config.AqtTensorConfig) -> Tuple[jnp.ndarray, jnp.ndarray]:
+    """Returns an updated scale provided by a config or the current one if None."""
+    if isinstance(config.quant_config, aqt_config.FloatConfig):
+      # We shouldn't update the scale if the given config contains FloatConfig;
+      # fill with a poison value if we get into this situation.
+      nan = jnp.full(self._stats.stats_shape, jnp.nan, dtype=jnp.float32)
+      return nan, nan
+
+    x_bound = self._stats.bound(config.calibration_config)
+    clip_bound = aqt_common.get_clip_bound(config.quant_config)
+
+    new_scale = clip_bound / x_bound
+    inv_scale = x_bound / clip_bound
+    return new_scale, inv_scale
+
+  def clip_range(self) -> jnp.ndarray:
+    """Returns the tensor clip range or zeros if no int config is active."""
+    for config in self.config.tensor_configs:
+      if (is_config_active(config, self._last_update.value) and
+          isinstance(config.quant_config, aqt_config.IntQuantConfig)):
+        clip_bound = aqt_common.get_clip_bound(config.quant_config)
+        return self._inv_scale.value * clip_bound
+    return jnp.zeros(self._stats.stats_shape)
+
+  def update(
+      self,  #
+      sample: jnp.ndarray,
+      weight: Optional[jnp.ndarray],
+      event_count: jnp.ndarray):
+    """Updates statistics, scale, and quantized variable."""
+
+    if self.config is None:
+      return
+
+    active_configs = [
+        c for c in self.config.tensor_configs
+        if is_config_active(c, event_count)
     ]
-    with tf.control_dependencies(updates):
-      actual = mm.apply(lhs, rhs)
 
-    if lhs_float:
-      qlhs = lhs  # lhs is not quantized
+    if len(active_configs) == 1:
+      self._update_config(active_configs[0], sample, weight, event_count)
     else:
-      qrhs = rhs  # rhs is not quantized
-    expected = tf.matmul(qlhs, qrhs)
+      raise ValueError('There must be exactly one active config.')
 
-    with self.cached_session() as sess, sess.as_default():
-      tf.global_variables_initializer().run()
-      self.assertAllEqual(expected, actual)
-
-  def with_config(self, mm, config):
-    """Returns new Matmul with the new config but otherwise the same."""
-    with tf.variable_scope(None, default_name="uniqued"):
-      return aqt_matmul.Matmul(config, mm.lhs_quantizer.data_shape,
-                               mm.rhs_quantizer.data_shape, mm.name,
-                               mm.lhs_name, mm.rhs_name)
-
-  def test_validates_contraction(self):
-    mm, _, _ = self.exact_int8_matmul_example()
-
-    config = copy.deepcopy(matmul_config(mm))
-    config.rhs.stats_config.share_stats_axes = [1]
-    with self.assertRaisesRegex(aqt_config.ConfigError,
-                                "expected rhs matmul contraction axis"):
-      self.with_config(mm, config)
-
-    config = copy.deepcopy(matmul_config(mm))
-    config.lhs.stats_config.share_stats_axes = [0]
-    with self.assertRaisesRegex(aqt_config.ConfigError,
-                                "expected lhs matmul contraction axis"):
-      self.with_config(mm, config)
-
-  def test_validates_rank2(self):
-    mm, lhs, rhs = self.exact_int8_matmul_example()
-
-    mm.rhs_quantizer.data_shape.append(1)
-    with self.assertRaisesRegex(aqt_config.ConfigError, "rhs data shape"):
-      mm.apply(lhs, rhs)
-    mm.rhs_quantizer.data_shape = mm.rhs_quantizer.data_shape[:-1]
-
-    mm.lhs_quantizer.data_shape += (1,)
-    with self.assertRaisesRegex(aqt_config.ConfigError, "lhs data shape"):
-      mm.apply(lhs, rhs)
-
-  @parameterized.named_parameters(
-      aqt_test_shared_base.generate_unaligned_schedule_intervals())
-  def test_unaligned_schedule_intervals(self, lhs_intervals, rhs_intervals):
-    bits = 8
-    lhs_intervals = [(start, stop, bits) for start, stop in lhs_intervals]
-    rhs_intervals = [(start, stop, bits) for start, stop in rhs_intervals]
-    lhs_config = config_from_schedule(lhs_intervals)
-    rhs_config = config_from_schedule(rhs_intervals)
-    config = aqt_config.AqtMatmulConfig(lhs_config, rhs_config)
-
-    with self.assertRaisesRegex(aqt_config.ConfigError,
-                                "intervals do not match|config len"):
-      aqt_matmul.Matmul(config, (1, 1), (1, 1))
-
-  def test_vars_dont_kill_grads(self):
-    mm, lhs, rhs = self.exact_int8_matmul_example()
-
-    unsaved_matmul = mm.apply(lhs, rhs)
-
-    with tf.variable_scope("with_var"):
-      mm_q, _, _ = self.exact_int8_matmul_example(True, True)
-
-    saved_matmul = mm_q.apply(lhs, rhs)
-
-    saved_grads = tf.gradients([saved_matmul], [lhs, rhs])
-    unsaved_grads = tf.gradients([unsaved_matmul], [lhs, rhs])
-
-    with self.cached_session():
-      tf.global_variables_initializer().run()
-
-      for matmul in [mm, mm_q]:
-        update_event_count(matmul, 0)
-
-      zipped_grads = zip(saved_grads, unsaved_grads)
-      for actual_grad, expected_grad in zipped_grads:
-        actual = actual_grad.eval()
-        expected = expected_grad.eval()
-
-        self.assertAllEqual(actual, expected)
-
-  @parameterized.parameters([
-      dict(lhs_use_quantized_variable=True),
-      dict(lhs_use_quantized_variable=False)
-  ])
-  def test_vars_over_inputs_at_inference(self, lhs_use_quantized_variable):
-    rhs_use_quantized_variable = not lhs_use_quantized_variable
-    mm, tf_lhs, tf_rhs = self.exact_int8_matmul_example(
-        lhs_use_quantized_variable, rhs_use_quantized_variable)
-    with tf.variable_scope("no_quantize"):
-      mm_train, _, _ = self.exact_int8_matmul_example(
-          lhs_use_quantized_variable=False, rhs_use_quantized_variable=False)
-
-    with self.cached_session():
-      tf.global_variables_initializer().run()
-      update_event_count(mm, 0)
-      actual = mm.apply(tf_lhs, tf_rhs, train=False).eval()
-      expected = np.zeros_like(actual)
-      # Rely on zero initialization for variables as opposed to non-zero inputs.
-      self.assertAllEqual(actual, expected)
-
-      # But if train then use input instead.
-      actual = mm.apply(tf_lhs, tf_rhs, train=True).eval()
-
-      update_event_count(mm_train, 0)
-      expected = mm_train.apply(tf_lhs, tf_rhs)
-      self.assertAllEqual(actual, expected)
-
-  def test_float_config_not_save_quantized_var(self):
-    mm, lhs, rhs = self.exact_int8_matmul_example(
-        lhs_use_quantized_variable=True, rhs_use_quantized_variable=True)
-
-    fc = aqt_config.FloatConfig()
-    mm.lhs_quantizer.config.tensor_configs[0].quant_config = fc
-
-    with self.cached_session():
-      tf.global_variables_initializer().run()
-      event_count = tf.constant(0, tf.int64)
-      mm.update_lhs(lhs, None, event_count).run()
-      mm.update_rhs(rhs, None, event_count).run()
-
-      actual = mm.apply(lhs, rhs, train=False)
-      expected = tf.zeros_like(actual)
-      # Although lhs config sets use_quantized_variable to True, lhs has
-      # a float config, and thus it uses zero-initialized quantized var.
-      self.assertAllEqual(actual, expected)
-
-  def test_exact_grads(self):
-    mm, lhs, rhs = self.exact_int8_matmul_example()
-
-    aqt_mm = mm.apply(lhs, rhs)
-    aqt_mm_grads = tf.gradients([tf.reduce_sum(aqt_mm**2)], [lhs, rhs])
-
-    mm_exact = tf.matmul(lhs, rhs)
-    mm_grads = tf.gradients([tf.reduce_sum(mm_exact**2)], [lhs, rhs])
-
-    with self.cached_session():
-      tf.global_variables_initializer().run()
-      update_event_count(mm, 0)
-
-      for aqt_grad, tf_grad in zip(aqt_mm_grads, mm_grads):
-        actual = aqt_grad.eval()
-        expected = tf_grad.eval()
-
-        self.assertAllEqual(actual, expected)
-
-  def test_grad_linearity(self):
-    """Validates gradients are correct on basic example."""
-    float_config_tc = aqt_config.AqtTensorConfig(
-        freeze_scale_at_begin=True,
-        quant_config=aqt_config.FloatConfig(),
-        calibration_config=calibration_config(1))
-    float_config = aqt_config.AqtScheduleConfig(test_stats_config(),
-                                                [float_config_tc])
-    scale = 10.0
-    int_config = _schedule_config(8, scale, (0, 1))
-
-    lhs_config, rhs_config = int_config, float_config
-    contract_dim = 10
-    lhs_shape = (1, contract_dim)
-    rhs_shape = (contract_dim, 1)
-    target_shape = lhs_shape[:1] + rhs_shape[1:]
-
-    lhs_ph = tf.placeholder(tf.float32, shape=lhs_shape)
-    rhs_ph = tf.placeholder(tf.float32, shape=rhs_shape)
-    target_ph = tf.placeholder(tf.float32, shape=target_shape)
-
-    config = aqt_config.AqtMatmulConfig(lhs_config, rhs_config)
-    mm = aqt_matmul.Matmul(config, lhs_shape, rhs_shape)
-
-    with self.cached_session() as sess, sess.as_default():
-      tf.global_variables_initializer().run()
-
-      event_count = tf.constant(0, tf.int64)
-      updates = [
-          mm.update_lhs(tf.ones(lhs_shape), None, event_count),
-          mm.update_rhs(tf.ones(rhs_shape), None, event_count)
-      ]
-      with tf.control_dependencies(updates):
-        aqt_mm = mm.apply(lhs_ph, rhs_ph)
-
-      aqt_diff = aqt_mm - target_ph
-      aqt_loss = tf.reduce_sum(aqt_diff**2) / 2
-      aqt_mm_grad = tf.gradients([aqt_loss], [rhs_ph])[0]
-
-      rng = np.random.default_rng(1234)
-      for i in range(10):
-        lhs = rng.standard_normal(lhs_shape).astype(np.float32)
-        rhs = rng.standard_normal(rhs_shape).astype(np.float32)
-        target = rng.standard_normal(target_shape).astype(np.float32)
-
-        feed_dict = {lhs_ph: lhs, rhs_ph: rhs, target_ph: target}
-
-        aqtd, aqt_grad = sess.run([aqt_diff, aqt_mm_grad], feed_dict=feed_dict)
-
-        # Notice aqt gradient at position i is quantized(lhs)[i] * aqtd
-        # assuming linearity of gradients.
-        grad_factor = aqtd.ravel()
-        float_grad = lhs.ravel() * grad_factor
-        true_grad = aqt_grad.ravel()
-        diff = np.abs(float_grad - true_grad)
-        bucket_width = scale * 2 / 255
-        for j, err in enumerate(diff):
-          self.assertLessEqual(
-              err,
-              bucket_width * abs(grad_factor),
-              msg=f"trial {i} position {j}")
-
-  def test_diagnostics(self):
-    mm, lhs, rhs = self.exact_int8_matmul_example()
-
-    with self.cached_session():
-      tf.global_variables_initializer().run()
-      update_event_count(mm, 0)
-
-      d = mm.diagnostics(lhs, rhs)
-      quantizers = {"lhs": mm.lhs_quantizer, "rhs": mm.rhs_quantizer}
-      for qname, quantizer in quantizers.items():
-
-        for name, expected in quantizer.calibration_variables().items():
-          actual = d[f"aqt/{qname}/{name}"]
-          self.assertAllEqual(actual, expected)
-
-        actual = d[f"aqt/{qname}/clipped_proportion"]
-        expected = 0.0
-        self.assertAllEqual(actual, expected)
-
-        actual = d[f"aqt/{qname}/clip"]
-        expected = quantizer.clip_range()
-        self.assertAllEqual(actual, expected)
-
-      out_of_range_lhs, out_of_range_rhs = (
-          tf.ones_like(x) * 512.0 for x in (lhs, rhs))
-      d = mm.diagnostics(out_of_range_lhs, out_of_range_rhs)
-      for arg in ["lhs", "rhs"]:
-        actual = d[f"aqt/{arg}/clipped_proportion"]
-        expected = 1.0
-        self.assertAllEqual(actual, expected)
+  def _update_config(
+      self,  #,
+      config: aqt_config.AqtTensorConfig,
+      sample: jnp.ndarray,
+      weight: Optional[jnp.ndarray],
+      event_count: jnp.ndarray):
+    """update(), but with active `config`."""
+
+    should_update_scale = self._should_update_scale(config, event_count)
+    self._last_update.value = event_count
+
+    self._stats.update(sample, weight)
+
+    new_scale, inv_scale = jax.lax.cond(
+        should_update_scale,  #
+        lambda: self._fresh_scale(config),
+        lambda: (self._scale.value, self._inv_scale.value))
+    self._scale.value = new_scale
+    self._inv_scale.value = inv_scale
+
+    if (self.config.use_quantized_variable and
+        isinstance(config.quant_config, aqt_config.IntQuantConfig) and
+        config.quant_config.compatible_with_int8()):
+      scale, _ = self._get_quant_scale(train=True)
+      sample = scale * sample
+      new_var = self._to_quant(
+          sample, train=True).astype(self.quantized_variable.value.dtype)
+      self.quantized_variable.value = new_var
+
+  def _should_update_scale(
+      self,  #
+      config: aqt_config.AqtTensorConfig,
+      event_count: jnp.ndarray) -> bool:
+    """Returns if scale should be updated for the config and event count."""
+    if isinstance(config.quant_config, aqt_config.FloatConfig):
+      return False
+
+    if not config.freeze_scale_at_begin:
+      return True
+
+    # The first time a config is active, even if we freeze scale, we should
+    # update the scale.
+    was_previously_inactive = not is_config_active(config,
+                                                   self._last_update.value)
+
+    # We rely on jnp.int32.min being an illegal event count value, so that
+    # even if is_config_active(config, jnp.int32.min), we still update scale.
+    # This could happen if the very first update happens for a config which
+    # has freeze_scale_at_begin and begin=None.
+    assert event_count > jnp.iinfo(jnp.int32).min, ('event_count cannot be '
+                                                    'int32.min')
+
+    first_event = jnp.array(self._last_update.value == jnp.iinfo(jnp.int32).min)
+
+    return was_previously_inactive | first_event
+
+  def _to_quant(self, x: jnp.ndarray, train: bool) -> jnp.ndarray:
+    """Quantizes x with active quant config, if any, else act as identity."""
+
+    def qparams(
+        config: aqt_config.AqtTensorConfig,
+        check_active: bool = True
+    ) -> Tuple[bool, jnp.array, jnp.array, jnp.array]:
+      """Returns parameters for AQT quantization routine."""
+
+      should_quantize = False
+      clip_bound = jnp.array(0.0)
+      shift_before = jnp.array(0.0)
+      shift_after = jnp.array(0.0)
+
+      config_active = is_config_active(config, self._last_update.value)
+      config_active = not check_active or config_active
+
+      if isinstance(config.quant_config, aqt_config.FloatConfig):
+        clip_bound = jnp.where(config_active, float('inf'), 0.0)
+        return should_quantize, clip_bound, shift_before, shift_after
+      elif isinstance(config.quant_config, aqt_config.IntQuantConfig):
+        should_quantize |= config_active
+        config_active = jnp.float32(config_active)
+
+        clip_bound += config_active * aqt_common.safe_clip_bound(
+            config.quant_config)
+
+        if config.quant_config.preserve_zero:
+          shift_before += config_active * 0.5
+        else:
+          shift_after += config_active * 0.5
+
+        return should_quantize, clip_bound, shift_before, shift_after
+      else:
+        raise NotImplementedError(
+            'Only supporting FloatConfig and IntQuantConfig for now.')
+
+    if self.config is None:
+      clip_bound = jnp.array(float('inf'))
+      shift_before = shift_after = 0.0
+      should_quantize = False
+    elif not train and self.config.inference_config_index is not None:
+      should_quantize, clip_bound, shift_before, shift_after = qparams(
+          self.config.tensor_configs[self.config.inference_config_index],
+          check_active=False)
+    elif self.config.tensor_configs:
+      should_quantize, clip_bound, shift_before, shift_after = zip(
+          *map(qparams, self.config.tensor_configs))
+      should_quantize = any(should_quantize)
+      clip_bound = sum(clip_bound)
+      shift_before = sum(shift_before)
+      shift_after = sum(shift_after)
+    else:
+      clip_bound = shift_before = shift_after = 0.0
+      should_quantize = False
 
+    maybe_floor = (lambda y: jnp.where(should_quantize, jnp.floor(y), y))
+
+    # Note that backprop does not depend directly on the value of _last_update
+    # or any_config_active; only scales and constants need to be maintained
+    # and there's no branching on ops including the input tensor x. This
+    # results in significant memory reduction, see cl/415355150.
+    x = jnp.clip(x, -clip_bound, clip_bound)
+    x += shift_before
+    x = pass_through(x, maybe_floor)
+    # TODO(b/219778053): Add a test that validates the shift of values. Mutants
+    # found that removing the line below doesn't affect any tests.
+    x += shift_after
+
+    return x
+
+  def _get_quant_scale(self, train: bool) -> jnp.ndarray:
+    """Returns scales to quantize/dequantize the active quant config, if any, else ones."""
+    if self.config is None:
+      scale = inv_scale = jnp.array(1.0, dtype=jnp.float32)
+      return scale, inv_scale  # pytype: disable=bad-return-type  # jax-ndarray
+
+    if not train and self.config.inference_config_index is not None:
+      inference_config = self.config.tensor_configs[
+          self.config.inference_config_index]
+      should_quantize = isinstance(inference_config.quant_config,
+                                   aqt_config.IntQuantConfig)
+    else:
+      should_quantize = False
+      for config in self.config.tensor_configs:
+        if isinstance(config.quant_config, aqt_config.FloatConfig):
+          continue
+        config_active = is_config_active(config, self._last_update.value)
+        should_quantize |= config_active
+
+    scale = jnp.where(should_quantize, self._scale.value,
+                      jnp.ones_like(self._scale.value))
+    inv_scale = jnp.where(should_quantize, self._inv_scale.value,
+                          jnp.ones_like(self._inv_scale.value))
 
-if __name__ == "__main__":
-  absltest.main()
+    return scale, inv_scale  # pytype: disable=bad-return-type  # jax-ndarray
```

### Comparing `aqtp-0.0.9/aqt/tensorflow/aqt_tensor.py` & `aqtp-0.1.0/aqt/tensorflow/aqt_tensor.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,23 +15,63 @@
 """Utilities for quantizing single tensor values.
 
 The building block for quantized operations with multiple inputs
 is quantizing individual inputs, possibly with functionally coupled parameters.
 This module provides configurable functions for single-tensor calibration and
 quantization.
 """
-
+import dataclasses
 from typing import Any, Callable, Dict, Iterable, Optional, Tuple
 
 from aqt.common import aqt_common
 from aqt.common import aqt_config
+from aqt.common import emulated_floating_points
+from aqt.common import emulation_utils
 import tensorflow.compat.v1 as tf
 import tensorflow.compat.v1.tpu as tpu_ops
 
 
+def _emulated_fp(
+    t: tf.Tensor,
+    mantissa_bits: tf.Tensor,
+    min_exp: tf.Tensor,
+    max_exp: tf.Tensor,
+) -> tf.Tensor:
+  """Emulates enumerics in bfloat16 or float32 given the FPMetadata.
+
+  This is based on the implementation in:
+  google3/platforms/deepsea/ffds/reduced_precision/emulated_floating_points.py
+  However a separate implementation is needed to incorporate the metadata as
+  tensors in the TF graph.
+
+  Args:
+    t: a tensor whose dtype is either tf.bfloat16 or tf.float32.
+    mantissa_bits: The mantissa bits in the emulated format.
+    min_exp: the allowed minimum exponents in the emulated format.
+    max_exp: the allowed maximum exponents in the emulated format.
+
+  Returns:
+    a same dtype tensor that emulates floating points.
+  """
+  assert t.dtype == tf.float32
+  output_type = t.dtype
+
+  with tf.name_scope('emulated_fp'):
+    v = emulated_floating_points.handle_mantissa(
+        t,
+        mantissa_bits=mantissa_bits,
+        min_exp=min_exp,
+        rounding_mode=emulation_utils.ROUND_TO_NEAREST_EVEN)
+    v = emulated_floating_points.static_handle_exponent(
+        v,
+        min_exp=min_exp - mantissa_bits,
+        max_exp=max_exp,
+        mantissa_bits=mantissa_bits)
+    return tf.cast(v, output_type)
+
 # For compatibility with different frameworks, such as Babelfish, we allow
 # custom variable creation lambdas. Make sure they're not trainable.
 #
 # GetVariable(name, shape, dtype, const_initial_value)
 GetVariable = Callable[[str, Iterable[int], tf.dtypes.DType, Any], tf.Variable]
 
 
@@ -288,15 +328,16 @@
     }
 
   def _fresh_scale(
       self, config: aqt_config.AqtTensorConfig
   ) -> Tuple[tf.Tensor, tf.Tensor]:
     """Returns new scale, inverse scale for a given config and stats, if any."""
     if isinstance(config.quant_config, aqt_config.FloatConfig):
-      # We shouldn't update the scale if the given config contains FloatConfig;
+      # We shouldn't update the scale if the given config contains FloatConfig
+      # and no emulation;
       # fill with a poison value if we get into this situation.
       nan = tf.constant(float('nan'), tf.float32, self._stats.stats_shape)
       return nan, nan
 
     x_bound = self._stats.bound(config.calibration_config)
     clip_bound = aqt_common.get_clip_bound(config.quant_config)
 
@@ -304,15 +345,15 @@
     inv_scale = x_bound / clip_bound
     return new_scale, inv_scale
 
   def clip_range(self) -> tf.Tensor:
     """Returns the tensor clip range or zeros if no int config is active."""
 
     def case_fn(config: aqt_config.AqtTensorConfig) -> tf.Tensor:
-      if not isinstance(config.quant_config, aqt_config.IntQuantConfig):
+      if isinstance(config.quant_config, aqt_config.FloatConfig):
         return tf.zeros(self._stats.stats_shape)
 
       # We return the range derived from the inverse scale, rather than
       # from the stats themselves, to respect freezing settings and
       # report the clipping range that's actually used at all times.
       #
       # The counterfactual clipping range that would have been used
@@ -320,31 +361,36 @@
       # stats values, which are updated regardless of freezing.
       clip_bound = aqt_common.get_clip_bound(config.quant_config)
       return self._inv_scale.read_value() * clip_bound
 
     return self._config_case(case_fn, self._last_update.read_value())
 
   def update(self,  #
-             sample: tf.Tensor,
+             sample: Optional[tf.Tensor],
              weight: Optional[tf.Tensor],
              event_count: tf.Tensor) -> tf.Operation:
     """Op to update statistics, scale, and quantized variable.
 
     Args:
-      sample: an observation of the tensor to quantize.
+      sample: an observation of the tensor to quantize. If None, only update
+        the state variables without updating the stats
       weight: the weight of each observation for updating statistics.
       event_count: the event count this observation corresponds to; this
         determines the scale that's active for any quantized methods referencing
         this `TensorQuantizer`.
 
     Returns:
       A tensorflow operation corresponding to the updates to internal variables
       for capturing this observation of `sample`.
     """
-    with tf.control_dependencies([self._stats.update(sample, weight)]):
+    dependencies = []
+    if sample is not None:
+      # update the stats if a sample is passed, else only update state
+      dependencies.append(self._stats.update(sample, weight))
+    with tf.control_dependencies(dependencies):
 
       def case_fn(config):
         return self._update_state_config(config, sample, event_count)
 
       return self._config_case(case_fn, event_count).op
 
   def _config_case(
@@ -386,129 +432,169 @@
     updates.append(self._scale.assign(updated_scale))
     updates.append(self._inv_scale.assign(updated_inv_scale))
 
     if (self.config.use_quantized_variable and
         isinstance(config.quant_config, aqt_config.IntQuantConfig) and
         config.quant_config.compatible_with_int8()):
       with tf.control_dependencies(updates):
+        scale, _ = self._get_quant_scale(train=True)
+        sample = scale * sample
         updated_quantized_variable = tf.cast(
             self._to_quant(sample, train=True), self.quantized_variable.dtype)
         updates.append(
             self.quantized_variable.assign(updated_quantized_variable))
 
     with tf.control_dependencies(updates):
       return tf.constant(0)
 
   def _quantization_params(self, train):
     """Returns parameters for AQT quantization routine."""
 
-    def qparams(
-        config: aqt_config.AqtTensorConfig,
-        check_active: bool = True
-    ) -> Tuple[tf.Tensor, tf.Tensor, tf.Tensor, tf.Tensor]:
-      """Returns quant parameters for fixed AQT config."""
+    @dataclasses.dataclass
+    class QParams:
+      """Dataclass for quantization parameters."""
+      # Tensors used for quantization
+      should_quantize: tf.Tensor = tf.constant(0.0)
+      clip_bound: tf.Tensor = tf.constant(0.0)
+      shift_before: tf.Tensor = tf.constant(0.0)
+      shift_after: tf.Tensor = tf.constant(0.0)
+
+      # Tensors used for floating point emulation.
+      should_use_small_float: tf.Tensor = tf.constant(0)
+      mantissa_bits: tf.Tensor = tf.constant(0)
+      min_exp: tf.Tensor = tf.constant(0)
+      max_exp: tf.Tensor = tf.constant(0)
+
+      def __iter__(self):
+        return (getattr(self, field.name) for field in dataclasses.fields(self))
 
-      should_quantize = tf.constant(0.0)
-      clip_bound = tf.constant(0.0)
-      shift_before = tf.constant(0.0)
-      shift_after = tf.constant(0.0)
+    def qparams(config: aqt_config.AqtTensorConfig,
+                check_active: bool = True) -> QParams:
+      """Returns quant parameters for fixed AQT config."""
 
+      params = QParams()
       config_active = is_config_active(config, self._last_update.read_value())
       config_active = not check_active or config_active
 
       if isinstance(config.quant_config, aqt_config.FloatConfig):
-        clip_bound = tf.where_v2(config_active, float('inf'), 0.0)
-        return should_quantize, clip_bound, shift_before, shift_after
-
-      config_active = tf.cast(config_active, tf.float32)
-      should_quantize += config_active
-
-      # TODO(vladf): some serving environments, such as adbrain,
-      # automatically rewrite constants from f32 to bf16, which makes the
-      # epsilon used in the function below invalid, so that
-      # safe_clip_bound == clip_bound (incorrectly). We should solve for
-      # that through some configuration.
-      clip_bound += config_active * aqt_common.safe_clip_bound(
-          config.quant_config)
-
-      if config.quant_config.preserve_zero:
-        shift_before += config_active * 0.5
+        params.clip_bound = tf.where_v2(config_active, float('inf'), 0.0)
+      elif isinstance(config.quant_config, aqt_config.IntQuantConfig):
+        config_active = tf.cast(config_active, tf.float32)
+        params.should_quantize += config_active
+
+        # TODO(vladf): some serving environments, such as adbrain,
+        # automatically rewrite constants from f32 to bf16, which makes the
+        # epsilon used in the function below invalid, so that
+        # safe_clip_bound == clip_bound (incorrectly). We should solve for
+        # that through some configuration.
+        params.clip_bound += config_active * aqt_common.safe_clip_bound(
+            config.quant_config)
+        if config.quant_config.preserve_zero:
+          params.shift_before += config_active * 0.5
+        else:
+          params.shift_after += config_active * 0.5
+      elif isinstance(config.quant_config, aqt_config.SmallFloatConfig):
+        # Note: In the case of small floats, we can just use get_clip_bound
+        # as opposed to safe_clip_bound since we are mapping the clip bound
+        # directly to the highest float that can be represented, while in int
+        # world we are mapping biggest value onto 127.4999 to get a slightly
+        # wider and less biased range.
+        config_active = tf.cast(config_active, tf.int32)
+        params.should_use_small_float += config_active
+
+        params.clip_bound += (
+            tf.cast(config_active, tf.float32) *
+            aqt_common.get_clip_bound(config.quant_config))
+
+        params.mantissa_bits += (
+            config_active * config.quant_config.mantissa_bits)
+        params.min_exp += config_active * config.quant_config.min_exp
+        params.max_exp += config_active * config.quant_config.max_exp
       else:
-        shift_after += config_active * 0.5
+        raise ValueError('config.quant_config must have type '
+                         'FloatConfig, IntQuantConfig, or SmallFloatConfig. '
+                         f'But instead got {type(config.quant_config)}.')
 
-      return should_quantize, clip_bound, shift_before, shift_after
+      return params
 
     if not train and self.config.inference_config_index is not None:
-      should_quantize, clip_bound, shift_before, shift_after = qparams(
+      params = qparams(
           self.config.tensor_configs[self.config.inference_config_index],
           check_active=False)
     elif self.config.tensor_configs:
-      should_quantize, clip_bound, shift_before, shift_after = zip(
-          *map(qparams, self.config.tensor_configs))
-      should_quantize = tf.add_n(should_quantize)
-      clip_bound = tf.add_n(clip_bound)
-      shift_before = tf.add_n(shift_before)
-      shift_after = tf.add_n(shift_after)
+      params = QParams(*map(tf.add_n, zip(
+          *map(qparams, self.config.tensor_configs))))
     else:
-      should_quantize = clip_bound = shift_before = shift_after = tf.constant(
-          0.0)
+      return QParams()
 
-    should_quantize = tf.cast(should_quantize, tf.bool)
-    return should_quantize, clip_bound, shift_before, shift_after
+    params.should_quantize = tf.cast(params.should_quantize, tf.bool)
+    params.should_use_small_float = tf.cast(
+        params.should_use_small_float, tf.bool)
+    return params
 
   def _to_quant(self, x: tf.Tensor, train: bool) -> tf.Tensor:
     """Quantizes x with active quant config, if any, else act as identity."""
     with tf.variable_scope('to_quant'):
-      should_quantize, clip_bound, shift_before, shift_after = (
-          self._quantization_params(train))
+      params = self._quantization_params(train)
 
-      scale = tf.where_v2(  #
-          should_quantize, self._scale.read_value(),
-          tf.ones_like(self._scale.read_value()))
-      maybe_floor = (
-          lambda y: tf.where_v2(should_quantize, tf.math.floor(y), y))
+      def maybe_floor_or_small_float(y):
+        # Static check for whether int and small float can coexist in schedule
+        if self.config.allow_int_small_float:
+          return tf.where_v2(params.should_use_small_float,
+                             _emulated_fp(y, params.mantissa_bits,
+                                          params.min_exp,
+                                          params.max_exp),
+                             tf.where_v2(params.should_quantize,
+                                         tf.math.floor(y), y))
+        else:
+          if self.config.quantization_mode() == aqt_config.SmallFloatConfig:
+            return tf.where_v2(
+                params.should_use_small_float,
+                _emulated_fp(y, params.mantissa_bits, params.min_exp,
+                             params.max_exp), y)
+          else:
+            return tf.where_v2(params.should_quantize, tf.math.floor(y), y)
 
       # Note that backprop does not depend directly on the value of _last_update
       # or any_config_active; only scales and constants need to be maintained
       # and there's no branching on ops including the input tensor x. This
       # results in significant memory reduction, see cl/415355150.
-      x = scale * x
-      x = tf.clip_by_value(x, -clip_bound, clip_bound)
-      x += shift_before
-      x = tf.grad_pass_through(maybe_floor)(x)
-      x += shift_after
+      x = tf.clip_by_value(x, -params.clip_bound, params.clip_bound)
+      x += params.shift_before
+      x = tf.grad_pass_through(maybe_floor_or_small_float)(x)
+      x += params.shift_after
 
-      return x
+    return x
 
   def _clip_mask(self, x: tf.Tensor, train: bool) -> tf.Tensor:
     """Returns which entries of x are clipped in _to_quant(x)."""
     # TODO(vladf): we should consider re-using the same clip mask
     # computation in _to_quant to derive this clip mask instead of a separate
     # method.
     with tf.variable_scope('clip_mask'):
-      should_quantize, clip_bound, _, _ = (self._quantization_params(train))
-      scale = tf.where_v2(  #
-          should_quantize, self._scale.read_value(),
-          tf.ones_like(self._scale.read_value()))
-      return tf.abs(scale * x) > clip_bound
+      _, clip_bound, _, _, _, _, _, _ = self._quantization_params(train)
+      return tf.abs(x) > clip_bound
 
-  def _from_quant_scale(self, train: bool) -> tf.Tensor:
-    """Scale to dequantize the active quant config, if any, else ones."""
-    with tf.variable_scope('from_quant'):
-      if not train and self.config.inference_config_index is not None:
-        inference_config = self.config.tensor_configs[
-            self.config.inference_config_index]
-        should_dequantize = tf.constant(
-            isinstance(inference_config.quant_config,
-                       aqt_config.IntQuantConfig))
-      else:
-        should_dequantize = tf.constant(False)
-        for config in self.config.tensor_configs:
-          if isinstance(config.quant_config, aqt_config.FloatConfig):
-            continue
+  def _get_quant_scale(self, train: bool) -> tf.Tensor:
+    """Returns scales to quantize/dequantize the active quant config, if any, else ones."""
+    if not train and self.config.inference_config_index is not None:
+      inference_config = self.config.tensor_configs[
+          self.config.inference_config_index]
+      should_scale = tf.constant(
+          not isinstance(inference_config.quant_config, aqt_config.FloatConfig))
+    else:
+      should_scale = tf.constant(False)
+      for config in self.config.tensor_configs:
+        if isinstance(config.quant_config, aqt_config.FloatConfig):
+          continue
 
-          config_active = is_config_active(config, self._last_update)
-          should_dequantize |= config_active
+        config_active = is_config_active(config, self._last_update)
+        should_scale |= config_active
 
+    # TODO(lew): We can simplify the scopes to just 'compute scales'
+    with tf.variable_scope('to_quant'):
+      scale = tf.where_v2(  #
+          should_scale, self._scale, tf.ones_like(self._scale))
+    with tf.variable_scope('from_quant'):
       inv_scale = tf.where_v2(  #
-          should_dequantize, self._inv_scale, tf.ones_like(self._inv_scale))
-      return inv_scale
+          should_scale, self._inv_scale, tf.ones_like(self._inv_scale))
+    return scale, inv_scale
```

### Comparing `aqtp-0.0.9/aqt/tensorflow/__init__.py` & `aqtp-0.1.0/aqt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/tensorflow/aqt_conv2d_test.py` & `aqtp-0.1.0/aqt/tensorflow/aqt_conv2d_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -127,9 +127,66 @@
           train=False,
           **kwargs)
       expected = aqt_ops.aqt_conv2d(
           input_tq, x, filter_tq, w, train=True, **kwargs)
       self.assertAllEqual(actual_infer, expected)
 
 
+class DepthwiseConv2dTest(Conv2dTest):
+
+  def conv_op_quantized(
+      self,
+      input,  # pylint: disable=redefined-builtin
+      filter,  # pylint: disable=redefined-builtin
+      input_config,
+      filter_config,
+      event_count,
+      event_count_for_filter=None,
+      input_weights=None,
+      train=True,
+      var_scope_name=None,
+      **kwargs):
+    event_count_for_filter = tf.constant(
+        event_count_for_filter if event_count_for_filter else event_count,
+        dtype=tf.int64)
+    event_count = tf.constant(event_count, dtype=tf.int64)
+
+    input = self.constant(input)
+    filter = self.constant(filter)
+
+    with tf.variable_scope(var_scope_name, default_name="default"):
+      input_tq = aqt_tensor.TensorQuantizer(
+          input.shape, input_config, name="input")
+      filter_tq = aqt_tensor.TensorQuantizer(
+          filter.shape, filter_config, name="filter")
+
+    updates = [input_tq.update(input, input_weights, event_count),
+               filter_tq.update(filter, None, event_count_for_filter)]
+
+    # depthwise_conv2d expects a different stride format than conv2d
+    if "strides" in kwargs:
+      stride = kwargs["strides"]
+      kwargs["strides"] = [1, stride, stride, 1]
+
+    with tf.control_dependencies(updates):
+      result = aqt_ops.aqt_depthwise_conv2d(input_tq, input, filter_tq,
+                                            filter, **kwargs)
+
+    with self.cached_session() as sess, sess.as_default():
+      tf.global_variables_initializer().run()
+      return result.eval()
+
+  def conv_op_unquantized(self, input, filter, **kwargs):  # pylint: disable=redefined-builtin
+    input = self.constant(input)
+    filter = self.constant(filter)
+
+    # tf.nn.depthwise_conv2d expects a different stride format than *_conv2d
+    if "strides" in kwargs:
+      stride = kwargs["strides"]
+      kwargs["strides"] = [1, stride, stride, 1]
+
+    with self.cached_session() as sess, sess.as_default():
+      tf.global_variables_initializer().run()
+      return tf.nn.depthwise_conv2d(input, filter, **kwargs).eval()
+
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `aqtp-0.0.9/aqt/tensorflow/aqt_tensor_test.py` & `aqtp-0.1.0/aqt/tensorflow/aqt_tensor_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """Tests for aqt_tensor."""
 
 from typing import Set
 
 from absl.testing import absltest
 from aqt.common import aqt_config
 from aqt.tensorflow import aqt_tensor
@@ -66,14 +65,29 @@
 
   def get_sum_of_lp_vals(self):
     return self._stats.calibration_variables()['sum_of_lp_vals']
 
   def set_ema_update_count(self, ema_update_count):
     self._stats._ema_update_count = ema_update_count
 
+  def mean(self):
+    return self._stats.mean()
+
+  def max_dev(self):
+    return self._stats.max_dev()
+
+  def l1_dev(self):
+    return self._stats.l1_dev()
+
+  def lp_dev(self):
+    return self._stats.lp_dev()
+
+  def bound(self, calibration_config):
+    return self._stats.bound(calibration_config)
+
 
 class AqtTensorQuantizerTest(aqt_tensor_test_base.AqtTensorQuantizerTest):
   """Tests for AqtTensorQuantizer class.
 
   Refer to aqt_tensor_test_base.AqtTensorQuantizerTest for more details.
   """
 
@@ -85,17 +99,18 @@
     with self.cached_session() as sess, sess.as_default():
       quant.update(f32(sample), weight, i64(event_count)).run()
 
   def to_quant(self, quant, x, train=True):
     with self.cached_session() as sess, sess.as_default():
       return quant._to_quant(x, train).eval()
 
-  def from_quant_scale(self, quant, train=True):
+  def get_quant_scale(self, quant, train=True):
     with self.cached_session() as sess, sess.as_default():
-      return quant._from_quant_scale(train).eval()
+      scale, inv_scale = quant._get_quant_scale(train)
+      return scale.eval(), inv_scale.eval()
 
   def init(self):
     with self.cached_session() as sess, sess.as_default():
       tf.global_variables_initializer().run()
 
   def get_scale(self, quant):
     with self.cached_session() as sess, sess.as_default():
@@ -136,16 +151,18 @@
       event_count = tf.constant(0, dtype=tf.int64)
       with self.cached_session():
         tf.global_variables_initializer().run()
         quant.update(f32(x), None, event_count).run()
 
       repeats = []
       for _ in range(10):
+        scale, inv_scale = quant._get_quant_scale(train=True)
+        x = scale * x
         ix = quant._to_quant(x, train=True)
-        qx = quant._from_quant_scale(train=True) * ix
+        qx = inv_scale * ix
         repeats.append(qx)
 
       with self.cached_session():
         for l, r in zip(repeats, repeats[1:]):
           self.assertAllEqual(l, r)
 
     # Extract subgraph attached to `qx`.
@@ -193,20 +210,24 @@
 
         with tf.control_dependencies([var_update]):
           var_update = var_quant.update(f32(y), None, event_count)
         with tf.control_dependencies([alt_update]):
           alt_update = alt_quant.update(f32(y), None, event_count)
 
         with tf.control_dependencies([var_update]):
-          ix = var_quant._to_quant(y, train=True)
-          var_qx = var_quant._from_quant_scale(train=True) * ix
+          scale, inv_scale = var_quant._get_quant_scale(train=True)
+          y_scaled = scale * y
+          ix = var_quant._to_quant(y_scaled, train=True)
+          var_qx = inv_scale * ix
 
         with tf.control_dependencies([alt_update]):
-          ix = alt_quant._to_quant(y, train=True)
-          alt_qx = alt_quant._from_quant_scale(train=True) * ix
+          scale, inv_scale = alt_quant._get_quant_scale(train=True)
+          y_scaled = scale * y
+          ix = alt_quant._to_quant(y_scaled, train=True)
+          alt_qx = inv_scale * ix
 
         with self.cached_session():
           tf.global_variables_initializer().run()
           self.assertAllEqual(var_qx, alt_qx)
 
 
 def extract_referenced_variables(t: tf.Tensor) -> Set[str]:
```

### Comparing `aqtp-0.0.9/aqt/tensorflow/aqt_ops.py` & `aqtp-0.1.0/aqt/tensorflow/aqt_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,10 +79,11 @@
 from aqt.tensorflow import aqt_einsum
 from aqt.tensorflow import aqt_matmul
 
 # TODO(b/193796715): Consider using Union[tf.Tensor, tf.Variable].
 # TODO(vladf): aqt_ops.aqt_matmul is redundant, we should consider
 # renaming to just the short operation name, e.g., aqt_ops.matmul.
 
+aqt_depthwise_conv2d = aqt_conv2d.depthwise_conv2d
 aqt_conv2d = aqt_conv2d.conv2d
 aqt_einsum = aqt_einsum.einsum
 aqt_matmul = aqt_matmul.matmul
```

### Comparing `aqtp-0.0.9/aqt/tensorflow/aqt_einsum.py` & `aqtp-0.1.0/aqt/tensorflow/aqt_einsum.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """Quantized einsum.
 
 Quantized einsum for the analogous :py:func:`tf.einsum`.
 
 Note that only 2-argument einsum is supported. For details, see go/aqtp-einsum.
 In a two argument einsum, we have an equation `lhs,rhs->out` where `lhs`, `rhs`,
 and `out` are strings containing single-character axes labels. Note that a
@@ -34,14 +33,15 @@
 label are contracting.
 """
 
 import string
 from typing import Tuple
 
 from aqt.common import aqt_config
+from aqt.common import aqt_config_utils
 from aqt.tensorflow import aqt_tensor
 import tensorflow.compat.v1 as tf
 
 # We repeatedly use protected methods from classes defined in other modules to
 # avoid exporting them as part of the public API.
 # pylint: disable=protected-access
 
@@ -139,21 +139,30 @@
   lhs_labels, rhs_labels, out_labels = _parse_equation(eq)
   _validate_shared_axes(
       lhs_quantizer.config.stats_config,  #
       rhs_quantizer.config.stats_config,
       lhs_labels,
       rhs_labels,
       out_labels)
-  aqt_config._validate_alignment(
+  aqt_config_utils._validate_alignment(
       'lhs_quantizer.config.tensor_configs',  #
       lhs_quantizer.config.tensor_configs,
       'rhs_quantizer.config.tensor_configs',
       rhs_quantizer.config.tensor_configs)
 
   with tf.name_scope('AqtEinsum'):
+    with tf.name_scope('get_quant_scale'):
+      with tf.name_scope('lhs'):
+        lhs_scale, lhs_inv_scale = lhs_quantizer._get_quant_scale(train)
+      with tf.name_scope('rhs'):
+        rhs_scale, rhs_inv_scale = rhs_quantizer._get_quant_scale(train)
+
+    lhs = lhs_scale * lhs
+    rhs = rhs_scale * rhs
+
     with tf.name_scope('to_quant'):
       with tf.name_scope('lhs'):
         lhs = lhs_quantizer._to_quant(lhs, train)
       with tf.name_scope('rhs'):
         rhs = rhs_quantizer._to_quant(rhs, train)
 
     # TODO(vladf): until tf.einsum supports int8 arguments, we need to cast
@@ -162,19 +171,13 @@
       lhs = tf.cast(lhs_quantizer.quantized_variable.read_value(), tf.float32)
     if rhs_quantizer.config.use_quantized_variable and not train:
       rhs = tf.cast(rhs_quantizer.quantized_variable.read_value(), tf.float32)
 
     with tf.name_scope('einsum'):
       out = tf.einsum(eq, lhs, rhs, **tf_einsum_kwargs)
 
-    with tf.name_scope('from_quant'):
-      with tf.name_scope('lhs'):
-        lhs_inv_scale = lhs_quantizer._from_quant_scale(train)
-      with tf.name_scope('rhs'):
-        rhs_inv_scale = rhs_quantizer._from_quant_scale(train)
-
     with tf.name_scope('inv_scale'):
       assert len(lhs_inv_scale.shape) == len(lhs.shape)
       assert len(rhs_inv_scale.shape) == len(rhs.shape)
       inv_scale = tf.einsum(eq, lhs_inv_scale, rhs_inv_scale,
                             **tf_einsum_kwargs)
       return out * inv_scale
```

### Comparing `aqtp-0.0.9/aqt/tensorflow/aqt_einsum_test.py` & `aqtp-0.1.0/aqt/tensorflow/aqt_einsum_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,14 +47,38 @@
   cc = aqt_config.CalibrationConfig(const_bound_coeff=const_bound_coeff)
   tc = aqt_config.AqtTensorConfig(
       quant_config=iqc, calibration_config=cc, freeze_scale_at_begin=True)
   sc = _stats_config(share_stats_axes)
   return aqt_config.AqtScheduleConfig(sc, [tc])
 
 
+def _schedule_config_emulation(
+    share_stats_axes) -> aqt_config.AqtScheduleConfig:
+  """Creates schedule config for emulated precision."""
+  iqc = aqt_config.SmallFloatConfig(
+      exponent_bits=5,
+      mantissa_bits=2,
+      min_exp=-14,
+      max_exp=15,
+      support_inf=False,
+      rounding_mode=aqt_config.RoundingMode.ROUND_TO_NEAREST_EVEN)
+  # Using the max number essentially disables scaling.
+  cc = aqt_config.CalibrationConfig(
+      const_bound_coeff=aqt_common._get_max_number_float(
+          mantissa_bits=2, max_exp=15))
+  tc = aqt_config.AqtTensorConfig(
+      quant_config=iqc, calibration_config=cc, freeze_scale_at_begin=True)
+  sc = aqt_config.StatsConfig(
+      ema_update_count=1,
+      share_stats_axes=list(share_stats_axes),
+      update_count_prior=0,
+      tpu_cross_replica_sum=False)
+  return aqt_config.AqtScheduleConfig(sc, [tc])
+
+
 def _empty_config(
     share_stats_axes: Sequence[int]) -> aqt_config.AqtScheduleConfig:
   return aqt_config.AqtScheduleConfig(_stats_config(share_stats_axes), [])
 
 
 def _einsum_op(
     eq: str,  #
@@ -242,17 +266,60 @@
                 [-1, 0],
                 [0, 1]
             ],
             dtype=np.float32))
 
     return eq, lhs_config, lhs, qlhs, rhs_config, rhs, qrhs
 
+  def basic_emulation_example(self):
+    eq = "ij,jk->ik"
+    lhs_config = _schedule_config_emulation([0, 1])
+    lhs = tf.constant(
+        np.array(
+            [
+                [-8.5, 4.3, 4.1],  #
+                [-0.05, 0.01, -4.7],
+            ],
+            dtype=np.float32))
+    qlhs = tf.constant(
+        np.array(
+            [
+                [-8.0, 4.0, 4.0],  #
+                [-0.046875, 0.00976562, -5.0]
+            ],
+            dtype=np.float32))
+
+    rhs_config = _schedule_config_emulation([0, 1])
+    rhs = tf.constant(
+        np.array(
+            [
+                [-0.2, 0.02],  #
+                [-1.1, 0],
+                [-0.04, 2.3]
+            ],
+            dtype=np.float32))
+    qrhs = tf.constant(
+        np.array(
+            [
+                [-0.1875, 0.01953125],  #
+                [-1.0, 0.0],
+                [-0.0390625, 2.5]
+            ],
+            dtype=np.float32))
+
+    return eq, lhs_config, lhs, qlhs, rhs_config, rhs, qrhs
+
   def test_basic_einsum(self):
-    eq, lhs_config, lhs, qlhs, rhs_config, rhs, qrhs = self.basic_quant_example(
-    )
+    with self.subTest("quant_example"):
+      eq, lhs_config, lhs, qlhs, rhs_config, rhs, qrhs = (
+          self.basic_quant_example())
+
+    with self.subTest("emulation_example"):
+      eq, lhs_config, lhs, qlhs, rhs_config, rhs, qrhs = (
+          self.basic_emulation_example())
 
     actual = _einsum_op(eq, lhs, rhs, lhs_config, rhs_config)
     expected = tf.einsum(eq, qlhs, qrhs)
 
     with self.cached_session() as sess, sess.as_default():
       tf.global_variables_initializer().run()
       self.assertAllEqual(expected, actual)
```

### Comparing `aqtp-0.0.9/aqt/tensorflow/aqt_matmul.py` & `aqtp-0.1.0/aqt/tensorflow/aqt_matmul.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,44 +7,42 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """Quantized matrix multiplication.
 
 The matmul operation is a form of tensor product applied to two arguments
 `(a, b)` which contracts the penultimate axis of `a` with the ultimate axis
 of `b`.
 
 For details on quantized operations and common configuration arguments, see
 `aqt_ops`.
 """
 
 from typing import Callable, Dict, Iterable, Optional
 
 from aqt.common import aqt_config
+from aqt.common import aqt_config_utils
 from aqt.tensorflow import aqt_tensor
 import tensorflow.compat.v1 as tf
 
-
 # TODO(b/220181240): Remove the pylint disable below and avoid using protected
 # methods.
 # We repeatedly use protected methods from classes defined in other modules to
 # avoid exporting them as part of the public API.
 # pylint: disable=protected-access
 
-
 MatmulFn = Callable[[tf.Tensor, tf.Tensor], tf.Tensor]
 
 
 def _possibly_use_quantized_variable(
-    quantizer: aqt_tensor.TensorQuantizer,
+    quantizer: aqt_tensor.TensorQuantizer,  #
     x: tf.Tensor,
     train: bool) -> tf.Tensor:
   """Returns quantized variable if not training and TQ.use_quantized_variable, casted to x.dtype.
 
   Given an input tensor and its tensor quantizer, here we enforce to use the
   quantized variable stored in the tensor quantizer as long as
   TQ.use_quantized_variable is true and it is in inference, no matter if
@@ -72,28 +70,34 @@
 
 
 def default_matmul(
     lhs_quantizer: aqt_tensor.TensorQuantizer,  #
     rhs_quantizer: aqt_tensor.TensorQuantizer,
     lhs: tf.Tensor,
     rhs: tf.Tensor,
-    train: bool) -> tf.Tensor:
+    train: bool,
+    transpose_a: bool = False,
+    transpose_b: bool = False,
+) -> tf.Tensor:
   """Perform tf.matmul with input tensors of float32 type."""
   lhs = _possibly_use_quantized_variable(lhs_quantizer, lhs, train)
   rhs = _possibly_use_quantized_variable(rhs_quantizer, rhs, train)
 
-  return tf.matmul(lhs, rhs)
+  return tf.matmul(lhs, rhs, transpose_a=transpose_a, transpose_b=transpose_b)
 
 
 def int8_matmul(
     lhs_quantizer: aqt_tensor.TensorQuantizer,  #
     rhs_quantizer: aqt_tensor.TensorQuantizer,
     lhs: tf.Tensor,
     rhs: tf.Tensor,
-    train: bool) -> tf.Tensor:
+    train: bool,
+    transpose_a: bool = False,
+    transpose_b: bool = False,
+    ) -> tf.Tensor:
   """Perform integral matmul after i8 cast while preserving gradients.
 
   1. If {lhs,rhs}_quantizer indicates the currently-active configuration
      should use saved quantized variables, then uses them. Otherwise,
      casts lhs/rhs to tf.int8.
   2. Performs native int8 matmul.
   3. Casts int32 result to f32.
@@ -104,14 +108,16 @@
     lhs_quantizer: TensorQuantizer for lhs.
     rhs_quantizer: TensorQuantizer for rhs.
     lhs: left hand side of the matmul, as a float.
     rhs: right hand side of the matmul, as a float.
     train: If false and `TQ.use_quantized_variable` is True, then use the
       quantized variable, instead of input tensors, for the respective input
       tensor.
+    transpose_a: Whether to transpose the LHS.
+    transpose_b: Whether to transpose the RHS.
 
   Returns:
     The result of the integer matmul.
   """
 
   def grad_fn(dy, variables=None):
     # We could manually write the backward pass of matmul with respect to the
@@ -129,48 +135,70 @@
         grad_ys=[dy])
 
     # The variables used by fwd() are quantized, so they have no gradients.
     if variables:
       return grads, [None] * len(variables)
     return grads
 
-  @tf.custom_gradient
-  def fwd(arg_lhs, arg_rhs):
+  def fwd_no_grad(arg_lhs, arg_rhs):
     # Wrap a custom-gradient op around the cast to propagate gradients,
     # since casting stops the gradient.
     int_lhs = tf.cast(arg_lhs, tf.int8)
     int_rhs = tf.cast(arg_rhs, tf.int8)
 
     int_lhs = _possibly_use_quantized_variable(lhs_quantizer, int_lhs, train)
     int_rhs = _possibly_use_quantized_variable(rhs_quantizer, int_rhs, train)
 
-    imm = tf.matmul(int_lhs, int_rhs, output_type=tf.int32)
+    imm = tf.matmul(
+        int_lhs,
+        int_rhs,
+        output_type=tf.int32,
+        transpose_a=transpose_a,
+        transpose_b=transpose_b)
     mm = tf.cast(imm, tf.float32)
-    return mm, grad_fn
+    return mm
 
-  return fwd(lhs, rhs)
+  fwd = tf.custom_gradient(lambda l, r: (fwd_no_grad(l, r), grad_fn))
+
+  # If not training, do not install the custom gradient since it would cause
+  # both sets of weights (float + int8) to be pulled into the graph, making it
+  # difficult to prune away the unused set of weights for serving.
+  if train:
+    return fwd(lhs, rhs)
+  else:
+    return fwd_no_grad(lhs, rhs)
 
 
-def _matmul_case(lhs_quantizer, rhs_quantizer, lhs, rhs, train):
+def _matmul_case(
+    lhs_quantizer,
+    rhs_quantizer,
+    lhs,
+    rhs,
+    train,
+    transpose_a: bool = False,
+    transpose_b: bool = False,
+):
   """Switch over matmuls based on event count and configs.
 
   The `TensorQuantizer`s for each argument are provided to supply the
   configurations for each input tensor. Also, if indicated by constituent
   configs, this uses the quantized variables in each tensor quantizer rather
   than the inputs themselves. Regardless, gradients are preserved as if this was
   a matmul over the original `(lhs, rhs)` inputs.
 
   Args:
     lhs_quantizer: TensorQuantizer for lhs.
     rhs_quantizer: TensorQuantizer for rhs.
     lhs: float input for lhs.
     rhs: float input for rhs.
     train: If false and `TQ.use_quantized_variable` is True, then use the
-    quantized variable, instead of input tensors, for the respective input
-    tensor.
+      quantized variable, instead of input tensors, for the respective input
+      tensor.
+    transpose_a: Whether to transpose the LHS.
+    transpose_b: Whether to transpose the RHS.
 
   Returns:
     The `tf.Tensor` from the resulting quantized matmul.
   """
 
   lhs_configs = lhs_quantizer.config.tensor_configs
   rhs_configs = rhs_quantizer.config.tensor_configs
@@ -180,98 +208,137 @@
             isinstance(rhs_config.quant_config, aqt_config.IntQuantConfig) and
             lhs_config.quant_config.bits <= 8 and
             rhs_config.quant_config.bits <= 8)
 
   lhs_index = lhs_quantizer.config.inference_config_index
   rhs_index = rhs_quantizer.config.inference_config_index
 
+  def cond_int8_matmul():
+    return int8_matmul(lhs_quantizer, rhs_quantizer, lhs, rhs, train,
+                       transpose_a, transpose_b)
+
+  def cond_default_matmul():
+    return default_matmul(lhs_quantizer, rhs_quantizer, lhs, rhs, train,
+                          transpose_a, transpose_b)
+
   if train or lhs_index is None or rhs_index is None:
     should_int8_quantize = tf.constant(False)
     for lhs_config in lhs_configs:
       for rhs_config in rhs_configs:
         # If any of lhs and rhs is FloatConfig, use the default matmul.
         if is_int8_compatible(lhs_config, rhs_config):
           should_int8_quantize |= (
               aqt_tensor.is_config_active(lhs_config,
                                           lhs_quantizer._last_update)
               & aqt_tensor.is_config_active(rhs_config,
                                             rhs_quantizer._last_update))
+    # Use go/tf-control-flow-v2, which we've noticed fuses better on TPU XLA.
+    v2_was_enabled = tf.control_flow_v2_enabled()
+    if not v2_was_enabled:
+      tf.enable_control_flow_v2()
+    cond = tf.cond(should_int8_quantize, cond_int8_matmul, cond_default_matmul)
+    if not v2_was_enabled:
+      tf.disable_control_flow_v2()
   else:
-    should_int8_quantize = tf.constant(
-        is_int8_compatible(lhs_configs[lhs_index], rhs_configs[rhs_index]))
-
-  # Use go/tf-control-flow-v2, which we've noticed fuses better on TPU XLA.
-  v2_was_enabled = tf.control_flow_v2_enabled()
-  if not v2_was_enabled:
-    tf.enable_control_flow_v2()
-  cond = tf.cond(
-      should_int8_quantize,
-      lambda: int8_matmul(lhs_quantizer, rhs_quantizer, lhs, rhs, train),
-      lambda: default_matmul(lhs_quantizer, rhs_quantizer, lhs, rhs, train))
-  if not v2_was_enabled:
-    tf.disable_control_flow_v2()
+    # In the inference setting, if inference config indices are specified,
+    # then manualy const-prop the tf.cond to avoid overheads such as loading
+    # bf16 weights
+    should_int8_quantize = is_int8_compatible(
+        lhs_configs[lhs_index], rhs_configs[rhs_index]
+    )
+    if should_int8_quantize:
+      cond = cond_int8_matmul()
+    else:
+      cond = cond_default_matmul()
   return cond
 
 
 def _validate_inputs(
     lhs_quantizer: aqt_tensor.TensorQuantizer,  #
     rhs_quantizer: aqt_tensor.TensorQuantizer,
+    grad_quantizer: Optional[aqt_tensor.TensorQuantizer],
 ):
   """Validates configs and inputs for matmul."""
 
   if len(lhs_quantizer.data_shape) != 2:
     raise aqt_config.ConfigError(
         f'lhs data shape ({lhs_quantizer.data_shape}) not rank 2')
 
   if len(rhs_quantizer.data_shape) != 2:
     raise aqt_config.ConfigError(
         f'rhs data shape ({rhs_quantizer.data_shape}) not rank 2')
 
   lhs_config = lhs_quantizer.config
   rhs_config = rhs_quantizer.config
 
-  aqt_config._validate_alignment(
+  aqt_config_utils._validate_alignment(
       'lhs_config',  #
       lhs_config.tensor_configs,
       'rhs_config',
       rhs_config.tensor_configs)
 
   if 1 not in lhs_config.stats_config.share_stats_axes:
     raise aqt_config.ConfigError(
         f'expected lhs matmul contraction axis (1) to be in '
         f'share_stats_axes={lhs_config.stats_config.share_stats_axes}')
   if 0 not in rhs_config.stats_config.share_stats_axes:
     raise aqt_config.ConfigError(
         f'expected rhs matmul contraction axis (0) to be in '
         f'share_stats_axes={rhs_config.stats_config.share_stats_axes}')
 
+  if grad_quantizer:
+    # Other quantizations are possible -- for now the only quantization we allow
+    # for the gradient is based on scalar scaling.
+    # For now we also restrict the possible values to dynamic quantization.
+    grad_config = grad_quantizer.config
+    if (0 not in grad_config.stats_config.share_stats_axes or
+        1 not in grad_config.stats_config.share_stats_axes):
+      raise aqt_config.ConfigError(
+          f'expected grad matmul axes (0, 1) to both be in '
+          f'share_stats_axes={rhs_config.stats_config.share_stats_axes}')
+    if grad_config.stats_config.ema_update_count != 1:
+      raise aqt_config.ConfigError(
+          'Currently only supporting dynamic quantization for the gradient ' +
+          'with ema_update_count=1, but instead found ' +
+          f'{grad_config.stats_config.ema_update_count}.')
+    for tensor_config in grad_config.tensor_configs:
+      if tensor_config.freeze_scale_at_begin:
+        raise aqt_config.ConfigError(
+            'Currently only supporting dynamic quantization for the gradient ' +
+            'with freeze_scale_at_begin=False, but got True.')
+
 
 def matmul(
     lhs_quantizer: aqt_tensor.TensorQuantizer,  #
     lhs: tf.Tensor,
     rhs_quantizer: aqt_tensor.TensorQuantizer,
     rhs: tf.Tensor,
-    train: bool = True
+    grad_quantizer: Optional[aqt_tensor.TensorQuantizer] = None,
+    train: bool = True,
 ) -> tf.Tensor:
   """Quantized tf.matmul.
 
   Gradients are propagated using the straight-through estimator [1] to
   `lhs` and `rhs` arguments. Note that this is a pure function, with
   quantization determined by the argument quantizers, which must be
   updated separately.
 
   If not `lhs_quantizer.train` (which should be equal to that of RHS)
   and the quantizers have cached quantized variables, then those are
   used instead, if the quantization config indicates as much.
 
+  When grad quantization is enabled, we use the approach described here:
+  https://g3doc.corp.google.com/third_party/py/aqt/google/g3doc/aqt_math_and_algorithms.md?cl=474412951#one-pragmatic-approach
+
   Args:
-    lhs_quantizer: the tensor quantizer for lhs
-    lhs: left-hand side of the matmul
-    rhs_quantizer: the tensor quantizer for rhs
-    rhs: right-hand side of the matmul
+    lhs_quantizer: the tensor quantizer for lhs.
+    lhs: left-hand side of the matmul, with shape [B, C].
+    rhs_quantizer: the tensor quantizer for rhs.
+    rhs: right-hand side of the matmul, with shape [C, F].
+    grad_quantizer: Optional quantizer for the gradient, with shape [B, F].
     train: If false and `use_quantized_variable` in lhs_quantizer or
       rhs_quantizer, then this indicates `aqt_matmul` should use the quantized
       variable with the latest quantized, memorized from the most recent
       `TensorQuantizer.update()` in quantized operations rather than the float
       tensor input `lhs` or `rhs` provided to those operations at inference
       time.
 
@@ -281,37 +348,43 @@
   Raises:
     aqt_config.ConfigError: if the configurations for the two quantizers
       are incompatible or unaligned (endpoints for start/stop event counts
       must be the same).
 
   [1]: https://arxiv.org/abs/1308.3432
   """
-  _validate_inputs(lhs_quantizer, rhs_quantizer)
+  _validate_inputs(lhs_quantizer, rhs_quantizer, grad_quantizer)
 
   def fwd(lhs, rhs):
     with tf.name_scope('AqtMatMul'):
-      with tf.name_scope('to_quant'):
+      with tf.name_scope('get_quant_scale'):
         with tf.name_scope('lhs'):
-          lhs = lhs_quantizer._to_quant(lhs, train)
+          lhs_scale, lhs_inv_scale = lhs_quantizer._get_quant_scale(
+              train)  # [B, 1]
         with tf.name_scope('rhs'):
-          rhs = rhs_quantizer._to_quant(rhs, train)
+          rhs_scale, rhs_inv_scale = rhs_quantizer._get_quant_scale(
+              train)  # [1, F]
 
-      with tf.name_scope('matmul'):
-        mm = _matmul_case(lhs_quantizer, rhs_quantizer, lhs, rhs, train)
+      lhs = lhs_scale * lhs  # [B, 1] * [B, C]
+      rhs = rhs_scale * rhs  # [1, F] * [C, F]
 
-      with tf.name_scope('from_quant'):
+      with tf.name_scope('to_quant'):
         with tf.name_scope('lhs'):
-          lhs_inv_scale = lhs_quantizer._from_quant_scale(train)
+          lhs = lhs_quantizer._to_quant(lhs, train)  # [B, C]
         with tf.name_scope('rhs'):
-          rhs_inv_scale = rhs_quantizer._from_quant_scale(train)
+          rhs = rhs_quantizer._to_quant(rhs, train)  # [C, F]
+
+      with tf.name_scope('matmul'):
+        mm = _matmul_case(lhs_quantizer, rhs_quantizer, lhs, rhs,
+                          train)  # [B, F]
 
       with tf.name_scope('inv_scale'):
         # TODO(b/236024344): consider alternative multiply associations here.
-        inv_scale = (lhs_inv_scale * rhs_inv_scale)
-        out = mm * inv_scale
+        inv_scale = (lhs_inv_scale * rhs_inv_scale)  # [B, 1] * [1, F]
+        out = mm * inv_scale  # [B, F] * [B, F]
 
     return out
 
   @tf.custom_gradient
   def qmatmul(lhs, rhs):
 
     out = fwd(lhs, rhs)
@@ -331,75 +404,146 @@
         #     fprop and bprop, this is manual rematerialization.
         # (2) Each bprop matmul can avoid a multiplication
         #     by an scale and inverse scale of an fprop argument
         #     due to cancellation.
 
         with tf.name_scope('BwdAqtMatMul'):
 
-          with tf.name_scope('from_quant'):
+          with tf.name_scope('get_quant'):
             with tf.name_scope('lhs'):
-              lhs_inv_scale = lhs_quantizer._from_quant_scale(train)
+              lhs_scale, lhs_inv_scale = lhs_quantizer._get_quant_scale(train)
             with tf.name_scope('rhs'):
-              rhs_inv_scale = rhs_quantizer._from_quant_scale(train)
+              rhs_scale, rhs_inv_scale = rhs_quantizer._get_quant_scale(train)
+
+          lhs_scaled = lhs_scale * lhs
+          rhs_scaled = rhs_scale * rhs
+
+          if grad_quantizer:
+            with tf.name_scope('grad_quant'):
+              # [B, F] * [B, 1] * [1, F]
+              grad = grad * lhs_inv_scale * rhs_inv_scale
+              # For now we simplify the gradient update by disabling the ability
+              # to pass the `weight` argument to update.
+
+              # We can also reuse the _last_update from the lhs_quantizer to
+              # pass the `event_count` which is expected to be consistent for
+              # the LHS, RHS, and gradient.
+              op = grad_quantizer.update(
+                  grad, weight=None, event_count=lhs_quantizer._last_update)
+              with tf.control_dependencies([op]):
+                # For now we assume that the gradient quantization is used only
+                # at the scalar level, i.e., grad_scale and grad_inv_scale have
+                # shape [1, 1]. This is enforced by the validation step.
+                # However, in principle the code below does not depend on this
+                # assumption. More generally the gradient may have other per
+                # channel quantization, in which case the shapes could be
+                # [B, 1], [1, F] or [B, F].
+                grad_scale, grad_inv_scale = grad_quantizer._get_quant_scale(
+                    train)
+
+                grad = grad * grad_scale
+                grad = grad_quantizer._to_quant(grad, train)
 
           with tf.name_scope('lhs'):
-            qrhs = rhs_quantizer._to_quant(rhs, train)
-            lhs_bwd = tf.matmul(grad * rhs_inv_scale, tf.transpose(qrhs))
+            qrhs = rhs_quantizer._to_quant(rhs_scaled, train)
+            if grad_quantizer:
+              lhs_bwd = grad_inv_scale * lhs_scale * _matmul_case(
+                  lhs_quantizer=grad_quantizer,
+                  rhs_quantizer=rhs_quantizer,
+                  lhs=grad,
+                  rhs=qrhs,
+                  train=train,
+                  transpose_a=False,
+                  transpose_b=True)
+            else:
+              lhs_bwd = tf.matmul(grad * rhs_inv_scale, tf.transpose(qrhs))
             lhs_bwd = tf.where_v2(
-                lhs_quantizer._clip_mask(lhs, train), 0.0, lhs_bwd)
+                lhs_quantizer._clip_mask(lhs_scaled, train), 0.0, lhs_bwd)
 
           with tf.name_scope('rhs'):
-            qlhs = lhs_quantizer._to_quant(lhs, train)
-            rhs_bwd = tf.matmul(tf.transpose(qlhs), grad * lhs_inv_scale)
+            qlhs = lhs_quantizer._to_quant(lhs_scaled, train)
+            if grad_quantizer:
+              rhs_bwd = grad_inv_scale * rhs_scale * _matmul_case(
+                  lhs_quantizer=lhs_quantizer,
+                  rhs_quantizer=grad_quantizer,
+                  lhs=qlhs,
+                  rhs=grad,
+                  train=train,
+                  transpose_a=True,
+                  transpose_b=False)
+            else:
+              rhs_bwd = tf.matmul(tf.transpose(qlhs), grad * lhs_inv_scale)
             rhs_bwd = tf.where_v2(
-                rhs_quantizer._clip_mask(rhs, train), 0.0, rhs_bwd)
+                rhs_quantizer._clip_mask(rhs_scaled, train), 0.0, rhs_bwd)
 
         return [lhs_bwd, rhs_bwd]
 
     return out, bwd
 
-  return qmatmul(lhs, rhs)
+  # If not training, do not install the custom gradient since it would cause
+  # both sets of weights (float + int8) to be pulled into the graph, making it
+  # difficult to prune away the unused set of weights for serving.
+  if train:
+    return qmatmul(lhs, rhs)
+  else:
+    return fwd(lhs, rhs)
 
 
 class Matmul:
   """Encapsulates a quantized matmul op and calibration state."""
 
-  def __init__(self,
-               config: aqt_config.AqtMatmulConfig,
-               lhs_shape: Iterable[Optional[int]],
-               rhs_shape: Iterable[Optional[int]],
-               name: str = 'aqt',
-               lhs_name: str = 'lhs',
-               rhs_name: str = 'rhs'):
+  def __init__(
+      self,
+      config: aqt_config.AqtMatmulConfig,
+      lhs_shape: Iterable[Optional[int]],
+      rhs_shape: Iterable[Optional[int]],
+      name: str = 'aqt',
+      lhs_name: str = 'lhs',
+      rhs_name: str = 'rhs',
+      grad_name: str = 'grad',
+  ):
     """Creates a Matmul instance.
 
     This encapsulates the state necessary for quantizing both
     of the matmul arguments.
 
     Args:
       config: an AqtMatmulConfig
       lhs_shape: shape of the lhs tensor to multiply
       rhs_shape: shape of the rhs tensor to multiply
       name: variable scope for all variables to be created.
       lhs_name: scope for left hand side variables only.
       rhs_name: scope for right hand side variables only.
+      grad_name: scope for the grad variables only (if quantizing).
     """
     self.name = name
     self.lhs_name = lhs_name
     self.rhs_name = rhs_name
+    self.grad_name = grad_name
     with tf.variable_scope(name):
       self.lhs_quantizer = aqt_tensor.TensorQuantizer(
           lhs_shape, config.lhs, name=lhs_name)
       self.rhs_quantizer = aqt_tensor.TensorQuantizer(
           rhs_shape, config.rhs, name=rhs_name)
-
-    _validate_inputs(self.lhs_quantizer, self.rhs_quantizer)
-
-  def update_lhs(self, x: tf.Tensor, weights: tf.Tensor,
-                 event_count: tf.Tensor) -> tf.Operation:
+      if config.grad:  # The gradient shape is inferred from the rhs and lhs.
+        grad_shape = [list(lhs_shape)[0], list(rhs_shape)[1]]
+        self.grad_quantizer = aqt_tensor.TensorQuantizer(
+            grad_shape, config.grad, name=grad_name)
+      else:
+        self.grad_quantizer = None
+
+    _validate_inputs(self.lhs_quantizer, self.rhs_quantizer,
+                     self.grad_quantizer)
+
+  def update_lhs(
+      self,
+      x: tf.Tensor,
+      weights: tf.Tensor,
+      event_count: tf.Tensor,
+  ) -> tf.Operation:
     """Updates variables for an observation of the lhs.
 
     Updating variables for an argument updates the statistics
     for a new input to account for incremental observations of
     a tensor's entries' magnitudes.
 
     This also updates the scales, if they were set according to
@@ -415,23 +559,29 @@
       event_count: the event of the observation
 
     Returns:
       The tf.Operation corresponding to the update
     """
     return self.lhs_quantizer.update(x, weights, event_count)
 
-  def update_rhs(self, x: tf.Tensor, weights: tf.Tensor,
-                 event_count: tf.Tensor) -> tf.Operation:
+  def update_rhs(
+      self,
+      x: tf.Tensor,
+      weights: tf.Tensor,
+      event_count: tf.Tensor,
+  ) -> tf.Operation:
     """Computes analogue of update_lhs, but for rhs."""
     return self.rhs_quantizer.update(x, weights, event_count)
 
-  def apply(self,
-            lhs: tf.Tensor,
-            rhs: tf.Tensor,
-            train: bool = True) -> tf.Tensor:
+  def apply(
+      self,
+      lhs: tf.Tensor,
+      rhs: tf.Tensor,
+      train: bool = True,
+  ) -> tf.Tensor:
     """Generates a pure quantized matmul op.
 
     Make sure that `apply` is called within the context of any updates
     to statistics used for calibration you'd like to happen before the
     op.
 
     Args:
@@ -440,35 +590,53 @@
       train: whether to generate the training or serving graph
 
     Returns:
       A tf.Tensor generated from possibly quantizing lhs and rhs
       with clip bounds derived from the current quantizer statistics.
     """
 
-    return matmul(self.lhs_quantizer, lhs, self.rhs_quantizer, rhs, train=train)
-
-  def diagnostics(self, lhs: tf.Tensor, rhs: tf.Tensor) -> Dict[str, tf.Tensor]:
+    return matmul(
+        self.lhs_quantizer,
+        lhs,
+        self.rhs_quantizer,
+        rhs,
+        self.grad_quantizer,
+        train=train)
+
+  def diagnostics(
+      self,
+      lhs: tf.Tensor,
+      rhs: tf.Tensor,
+      grad: Optional[tf.Tensor] = None,
+  ) -> Dict[str, tf.Tensor]:
     """Returns a dictionary from keys to diagnostic tensors.
 
     Args:
-      lhs: lhs argument to self.Apply, used for derving diangostics relative to
+      lhs: lhs argument to self.Apply, used for deriving diangostics relative to
         a given input.
       rhs: as above, but for rhs
+      grad: If specified, the gradient for deriving diagnostics.
 
     Returns:
       A dictionary with various quantization-related diagnostics,
       whose string keys are prefixed by self.name/self.{lhs,rhs}_name.
     """
     d = {}
-    for prefix, quantizer, argument in [
+    quantizers = [
         (self.lhs_name, self.lhs_quantizer, lhs),
-        (self.rhs_name, self.rhs_quantizer, rhs)
-    ]:
-      clipped_proportion = tf.cast(argument > quantizer.clip_range(),
+        (self.rhs_name, self.rhs_quantizer, rhs),
+    ]
+    if grad is not None:
+      assert self.grad_quantizer is not None, (
+          'If grad is given, then grad_quantizer must be defined.')
+      quantizers.append((self.grad_name, self.grad_quantizer, grad))
+    for prefix, quantizer, argument in quantizers:
+      clipped_proportion = tf.cast(tf.abs(argument) > quantizer.clip_range(),
                                    tf.float32)
       prefix = f'{self.name}/{prefix}'
       d[f'{prefix}/clipped_proportion'] = tf.math.reduce_mean(
           clipped_proportion)
       d[f'{prefix}/clip'] = quantizer.clip_range()
+      d[f'{prefix}/event_count'] = quantizer._last_update
       for name, var in quantizer.calibration_variables().items():
         d[f'{prefix}/{name}'] = var
     return d
```

### Comparing `aqtp-0.0.9/aqt/jax/aqt_dot_general_test.py` & `aqtp-0.1.0/aqt/jax/aqt_dot_general_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for dot_general."""
 import copy
-from typing import Any, Dict, Iterable, Sequence
+from typing import Any, Dict, Iterable, Optional, Sequence
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from aqt.common import aqt_config
 from aqt.jax import aqt_ops
 from aqt.jax import aqt_tensor
 from aqt.test import aqt_test_shared_base
@@ -60,16 +60,16 @@
         calibration_config=calibration_config(1.0))
     tensor_configs.append(tensor_config)
   return aqt_config.AqtScheduleConfig(
       test_stats_config(share_stats_axes), tensor_configs)
 
 
 class DotModule(nn.Module):
-  lhs_config: aqt_config.AqtScheduleConfig
-  rhs_config: aqt_config.AqtScheduleConfig
+  lhs_config: Optional[aqt_config.AqtScheduleConfig]
+  rhs_config: Optional[aqt_config.AqtScheduleConfig]
   lhs_shape: Iterable[int]
   rhs_shape: Iterable[int]
 
   @nn.compact
   def __call__(self):
     lhs_quantizer = aqt_tensor.TensorQuantizer(list(self.lhs_shape),
                                                self.lhs_config)
@@ -79,28 +79,28 @@
         lhs,
         rhs,
         lhs_quantizer,
         rhs_quantizer)
 
 
 class DotGeneralModule(nn.Module):
-  lhs_config: aqt_config.AqtScheduleConfig
-  rhs_config: aqt_config.AqtScheduleConfig
+  lhs_config: Optional[aqt_config.AqtScheduleConfig]
+  rhs_config: Optional[aqt_config.AqtScheduleConfig]
   lhs_shape: Iterable[int]
   rhs_shape: Iterable[int]
 
   @nn.compact
   def __call__(self, lhs, rhs, train=True):
     lhs_quantizer = aqt_tensor.TensorQuantizer(list(self.lhs_shape),
                                                self.lhs_config)
     rhs_quantizer = aqt_tensor.TensorQuantizer(list(self.rhs_shape),
                                                self.rhs_config)
 
-    lhs_quantizer.update(lhs, None, 0)
-    rhs_quantizer.update(rhs, None, 0)
+    lhs_quantizer.update(lhs, None, 0)  # pytype: disable=wrong-arg-types  # jax-ndarray
+    rhs_quantizer.update(rhs, None, 0)  # pytype: disable=wrong-arg-types  # jax-ndarray
 
     return lambda lhs, rhs, dimension_numbers: aqt_ops.aqt_dot_general(
         lhs,
         rhs,
         lhs_quantizer,
         rhs_quantizer,
         dimension_numbers=dimension_numbers,
@@ -183,21 +183,28 @@
 
   @parameterized.named_parameters(_generate_dimension_numbers())
   def test_dot_general_none(self, dimension_numbers):
     no_quant_config = aqt_config.AqtScheduleConfig(
         test_stats_config([0, 1, 2]), [])
     lhs = np.random.uniform(-1.0, 1.0, size=(2, 2, 2)).astype(np.float32)
     rhs = np.random.uniform(-1.0, 1.0, size=(2, 2, 2)).astype(np.float32)
+
+    # Creates a dot_general module with empty tensor configs.
     dot_general, _ = self.get_dot_general_module(no_quant_config,
                                                  no_quant_config, lhs, rhs)
     actual_ret = dot_general(lhs, rhs, dimension_numbers=dimension_numbers)
     expected_ret = lax.dot_general(
         lhs, rhs, dimension_numbers=dimension_numbers)
     np.testing.assert_array_equal(actual_ret, expected_ret)
 
+    # Creates a dot_general module with None schedule configs.
+    dot_general, _ = self.get_dot_general_module(None, None, lhs, rhs)
+    actual_ret = dot_general(lhs, rhs, dimension_numbers=dimension_numbers)
+    np.testing.assert_array_equal(actual_ret, expected_ret)
+
   @parameterized.named_parameters(_generate_dimension_numbers())
   def test_validates_contraction(self, dimension_numbers):
     lhs_config, lhs, rhs_config, rhs = self.exact_int8_dot_general_example()
     bad_rhs_config = copy.deepcopy(rhs_config)
     bad_rhs_config.stats_config.share_stats_axes = [0]
     dot_general, _ = self.get_dot_general_module(lhs_config, bad_rhs_config,
                                                  lhs, rhs)
@@ -296,10 +303,29 @@
         lhs, rhs, dimension_numbers=dimension_numbers)**2)
     dg_grads = self.vgrad(dg, lhs, rhs)
     for aqt_grad, jax_grad in zip(aqt_dg_grads, dg_grads):
       actual = aqt_grad
       expected = jax_grad
       np.testing.assert_array_equal(actual, expected)
 
+  def test_weight_only_quantization(self):
+    lhs = np.random.uniform(-1.0, 1.0, size=(2, 2, 2)).astype(np.float32)
+    rhs = np.random.uniform(-1.0, 1.0, size=(2, 2, 2)).astype(np.float32)
+    lhs_config = config_from_schedule([(None, None, 8)], [0, 1, 2])
+    rhs_config = config_from_schedule([(None, None, 8)], [0, 1, 2])
+    lhs_config.tensor_configs[0].quant_config = aqt_config.FloatConfig()
+    # dimension numbers for batch matmul
+    dimension_numbers = (((2,), (1,)), ((0,), (0,)))
+
+    dot_general, _ = self.get_dot_general_module(lhs_config, rhs_config, lhs,
+                                                 rhs)
+    result_with_float_config = dot_general(
+        lhs, rhs, dimension_numbers=dimension_numbers)
+    dot_general, _ = self.get_dot_general_module(None, rhs_config, lhs, rhs)
+    result_with_none_config = dot_general(
+        lhs, rhs, dimension_numbers=dimension_numbers)
+    np.testing.assert_array_equal(result_with_float_config,
+                                  result_with_none_config)
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `aqtp-0.0.9/aqt/jax/aqt_dot_general.py` & `aqtp-0.1.0/aqt/jax/aqt_dot_general.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,26 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """Quantized dot_general."""
 
-
 import functools
 
 from aqt.common import aqt_config
+from aqt.common import aqt_config_utils
 from aqt.jax import aqt_tensor
 from aqt.jax import aqt_utils
 import jax
 from jax import lax
 import jax.numpy as jnp
 
-
 # TODO(b/220181240): Remove accesses to protected methods. e.g., TQ._to_quant()
 # -> TQ.to_quant().
 # We repeatedly use protected methods from classes defined in other modules to
 # avoid exporting them as part of the public API.
 # pylint: disable=protected-access
 
 
@@ -51,35 +49,32 @@
   See docstring of lax.dot_general.
 
   Args:
     lhs: Left-hand side of the dot_general.
     rhs: Right-hand side of the dot_general.
     lhs_quantizer: The tensor quantizer for lhs.
     rhs_quantizer: The tensor quantizer for rhs.
-    dimension_numbers: a tuple of tuples of the form
-      `((lhs_contracting_dims, rhs_contracting_dims),
-      (lhs_batch_dims, rhs_batch_dims))`
-    should_int8_quantize: If true, inputs to lax.dot_general will be
-      cast to int8 and results accumulated to int32, then converted back to
-      the original input type.
+    dimension_numbers: a tuple of tuples of the form `((lhs_contracting_dims,
+      rhs_contracting_dims), (lhs_batch_dims, rhs_batch_dims))`
+    should_int8_quantize: If true, inputs to lax.dot_general will be cast to
+      int8 and results accumulated to int32, then converted back to the original
+      input type.
     train: If false and `TensorQuantizer.use_quantized_variable` is True, then
       use the quantized variable, instead of input tensors, for the respective
       input tensor.
 
   Returns:
     Same as lax.dot_general, but its quantized version.
   """
+
   def dot_general_float(ops):
     lhs_, rhs_ = ops
     lhs_ = aqt_utils.possibly_use_quantized_variable(lhs_quantizer, lhs_, train)
     rhs_ = aqt_utils.possibly_use_quantized_variable(rhs_quantizer, rhs_, train)
-    return lax.dot_general(
-        lhs_,
-        rhs_,
-        dimension_numbers=dimension_numbers)
+    return lax.dot_general(lhs_, rhs_, dimension_numbers=dimension_numbers)
 
   def dot_general_int(ops):
     lhs_, rhs_ = ops
     lhs_int = lhs_.astype(jnp.int8)
     rhs_int = rhs_.astype(jnp.int8)
 
     lhs_int = aqt_utils.possibly_use_quantized_variable(lhs_quantizer, lhs_int,
@@ -115,60 +110,58 @@
       lhs_quantizer,
       rhs_quantizer,
       dimension_numbers=dimension_numbers,
       should_int8_quantize=should_int8_quantize,
       train=train)
 
   def differentiable_dot_general(lhs_, rhs_):
-    return lax.dot_general(
-        lhs_,
-        rhs_,
-        dimension_numbers=dimension_numbers)
-
-  _, y_tangent = jax.jvp(differentiable_dot_general,  #
-                         (lhs, rhs),
-                         (lhs_dot, rhs_dot))
+    return lax.dot_general(lhs_, rhs_, dimension_numbers=dimension_numbers)
+
+  _, y_tangent = jax.jvp(
+      differentiable_dot_general,  #
+      (lhs, rhs),
+      (lhs_dot, rhs_dot))
   return y, y_tangent
 
 
 def _validate_inputs(
     lhs_quantizer: aqt_tensor.TensorQuantizer,  #
     rhs_quantizer: aqt_tensor.TensorQuantizer,
-    dimension_numbers: lax.DotDimensionNumbers
-):
+    dimension_numbers: lax.DotDimensionNumbers):
   """Validates configs and inputs for dot_general."""
 
   lhs_config = lhs_quantizer.config
   rhs_config = rhs_quantizer.config
 
-  aqt_config._validate_alignment(
-      'lhs_config',  #
-      lhs_config.tensor_configs,
-      'rhs_config',
-      rhs_config.tensor_configs)
+  if lhs_config is not None and rhs_config is not None:
+    aqt_config_utils._validate_alignment(
+        'lhs_config',  #
+        lhs_config.tensor_configs,
+        'rhs_config',
+        rhs_config.tensor_configs)
 
   lhs_contracting_dims, rhs_contracting_dims = dimension_numbers[0]
 
-  if not any(a in lhs_config.stats_config.share_stats_axes
-             for a in lhs_contracting_dims):
+  if not (lhs_config is None or
+          any(a in lhs_config.stats_config.share_stats_axes
+              for a in lhs_contracting_dims)):
     raise aqt_config.ConfigError(
         f'expected lhs dot_general contraction axis to be in '
         f'share_stats_axes={lhs_config.stats_config.share_stats_axes}')
-  if not any(a in rhs_config.stats_config.share_stats_axes
-             for a in rhs_contracting_dims):
+  if not (rhs_config is None or
+          any(a in rhs_config.stats_config.share_stats_axes
+              for a in rhs_contracting_dims)):
     raise aqt_config.ConfigError(
         f'expected rhs dot_general contraction axis to be in '
         f'share_stats_axes={rhs_config.stats_config.share_stats_axes}')
 
 
-def dot(
-    lhs: jnp.ndarray,
-    rhs: jnp.ndarray,
-    lhs_quantizer: aqt_tensor.TensorQuantizer,
-    rhs_quantizer: aqt_tensor.TensorQuantizer) -> jnp.ndarray:
+def dot(lhs: jnp.ndarray, rhs: jnp.ndarray,
+        lhs_quantizer: aqt_tensor.TensorQuantizer,
+        rhs_quantizer: aqt_tensor.TensorQuantizer) -> jnp.ndarray:
   """Quantized lax.dot.
 
   This dot operator is based on lax.dot,
   https://jax.readthedocs.io/en/latest/_modules/jax/_src/lax/lax.html#dot.
   For more general contraction, see the `dot_general` operator.
 
   Args:
@@ -177,50 +170,58 @@
     lhs_quantizer: The tensor quantizer for lhs.
     rhs_quantizer: The tensor quantizer for rhs.
 
   Returns:
     An array containing the result with the same dtype as 'lhs' and 'rhs'.
   """
   if 1 <= lhs.ndim <= 2 and 1 <= rhs.ndim <= 2 and lhs.shape[-1] == rhs.shape[0]:
-    return dot_general(lhs, rhs, lhs_quantizer, rhs_quantizer,
-                       dimension_numbers=(((lhs.ndim - 1,), (0,)), ((), ())))
+    return dot_general(
+        lhs,
+        rhs,
+        lhs_quantizer,
+        rhs_quantizer,
+        dimension_numbers=(((lhs.ndim - 1,), (0,)), ((), ())))
   else:
     raise TypeError('Incompatible shapes for dot: got {} and {}.'.format(
         lhs.shape, rhs.shape))
 
 
-def dot_general(
-    lhs: jnp.ndarray,
-    rhs: jnp.ndarray,
-    lhs_quantizer: aqt_tensor.TensorQuantizer,
-    rhs_quantizer: aqt_tensor.TensorQuantizer,
-    dimension_numbers: lax.DotDimensionNumbers,
-    train: bool = True) -> jnp.ndarray:
+def dot_general(lhs: jnp.ndarray,
+                rhs: jnp.ndarray,
+                lhs_quantizer: aqt_tensor.TensorQuantizer,
+                rhs_quantizer: aqt_tensor.TensorQuantizer,
+                dimension_numbers: lax.DotDimensionNumbers,
+                train: bool = True) -> jnp.ndarray:
   """Quantized jax.lax.dot_general.
 
   Args:
     lhs: Left-hand side of the dot_general.
     rhs: Left-hand side of the dot_general.
     lhs_quantizer: The tensor quantizer for lhs.
     rhs_quantizer: The tensor quantizer for rhs.
-    dimension_numbers: a tuple of tuples of the form
-      `((lhs_contracting_dims, rhs_contracting_dims),
-      (lhs_batch_dims, rhs_batch_dims))`
+    dimension_numbers: a tuple of tuples of the form `((lhs_contracting_dims,
+      rhs_contracting_dims), (lhs_batch_dims, rhs_batch_dims))`
     train: If false and `use_quantized_variable` in lhs_quantizer or
       rhs_quantizer, then this indicates `aqt_dot_general` should use the
       quantized variable with the latest quantized, memorized from the most
       recent `TensorQuantizer.update()` in quantized operations rather than the
       float tensor input `lhs` or `rhs` provided to those operations at
       inference time.
 
   Returns:
     An array containing the result with the same dtype as 'lhs' and 'rhs'.
   """
   _validate_inputs(lhs_quantizer, rhs_quantizer, dimension_numbers)
 
+  lhs_scale, lhs_inv_scale = lhs_quantizer._get_quant_scale(train)
+  rhs_scale, rhs_inv_scale = rhs_quantizer._get_quant_scale(train)
+
+  lhs = lhs_scale * lhs
+  rhs = rhs_scale * rhs
+
   lhs = lhs_quantizer._to_quant(lhs, train)
   rhs = rhs_quantizer._to_quant(rhs, train)
 
   should_int8_quantize = aqt_utils.should_int8_quantize(lhs_quantizer,
                                                         rhs_quantizer)
 
   out = _dot_general_aqt(
@@ -228,15 +229,25 @@
       rhs,
       lhs_quantizer,
       rhs_quantizer,
       dimension_numbers=dimension_numbers,
       should_int8_quantize=should_int8_quantize,
       train=train)
 
-  lhs_inv_scale = lhs_quantizer._from_quant_scale(train)
-  rhs_inv_scale = rhs_quantizer._from_quant_scale(train)
-
-  inv_scale = lax.dot_general(lhs_inv_scale,
-                              rhs_inv_scale,
-                              dimension_numbers=dimension_numbers)
+  if lhs_quantizer.config is not None and rhs_quantizer.config is not None:
+    inv_scale = lax.dot_general(
+        lhs_inv_scale, rhs_inv_scale, dimension_numbers=dimension_numbers)
+  else:
+    inv_scale = lhs_inv_scale * rhs_inv_scale
 
   return out * inv_scale
+
+
+def injectable_dot_general(lhs_quantizer, rhs_quantizer, train):
+  """Wrapper of aqt_dot_general, supposed to be used in injection API."""
+  return lambda a, b, dimension_numbers, precision: dot_general(  # pylint: disable=g-long-lambda
+      lhs=a,
+      rhs=b,
+      lhs_quantizer=lhs_quantizer,
+      rhs_quantizer=rhs_quantizer,
+      dimension_numbers=dimension_numbers,
+      train=train)
```

### Comparing `aqtp-0.0.9/aqt/jax/aqt_conv_general.py` & `aqtp-0.1.0/aqt/jax/aqt_conv_general.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """Quantized conv_general."""
 
 import functools
 from typing import Optional, Sequence, Tuple, Union
 
 from aqt.common import aqt_config
+from aqt.common import aqt_config_utils
 from aqt.jax import aqt_tensor
 from aqt.jax import aqt_utils
 import jax
 from jax import lax
 import jax.numpy as jnp
 
 # pylint: disable=protected-access
+# pytype: disable=attribute-error
 
 
 @functools.partial(
     jax.custom_jvp, nondiff_argnums=(2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12))
 def _conv_general_aqt(
     lhs: jnp.ndarray,  #
     rhs: jnp.ndarray,
@@ -40,14 +41,15 @@
     padding: Union[str, Sequence[Tuple[int, int]]],
     lhs_dilation: Optional[Sequence[int]],
     rhs_dilation: Optional[Sequence[int]],
     dimension_numbers: lax.ConvGeneralDilatedDimensionNumbers,
     feature_group_count: int,
     batch_group_count: int) -> jnp.ndarray:
   """Wrapper around lax.conv_general_dilated, but with option to use integer conv."""
+
   def conv_general_float(ops):
     lhs_, rhs_ = ops
     lhs_ = aqt_utils.possibly_use_quantized_variable(lhs_quantizer, lhs_, train)
     rhs_ = aqt_utils.possibly_use_quantized_variable(rhs_quantizer, rhs_, train)
     return lax.conv_general_dilated(
         lhs_,
         rhs_,
@@ -128,24 +130,26 @@
         padding=padding,
         lhs_dilation=lhs_dilation,
         rhs_dilation=rhs_dilation,
         dimension_numbers=dimension_numbers,
         feature_group_count=feature_group_count,
         batch_group_count=batch_group_count)
 
-  _, y_tangent = jax.jvp(differentiable_conv_general,  #
-                         (lhs, rhs),
-                         (lhs_dot, rhs_dot))
-  return y, y_tangent
+  _, y_tangent = jax.jvp(
+      differentiable_conv_general,  #
+      (lhs, rhs),
+      (lhs_dot, rhs_dot))
+  return y, y_tangent  # pytype: disable=bad-return-type  # jax-ndarray
 
 
-def _validate_dilation_argument(lhs_quantizer,  #
-                                rhs_quantizer,
-                                lhs_dilation,
-                                rhs_dilation):
+def _validate_dilation_argument(
+    lhs_quantizer,  #
+    rhs_quantizer,
+    lhs_dilation,
+    rhs_dilation):
   """Validates preserve_zero=True of AqtIntQuantConfig when the dilation is used."""
   lhs_configs = lhs_quantizer.config.tensor_configs
   rhs_configs = rhs_quantizer.config.tensor_configs
   event_count = lhs_quantizer._last_update.value
 
   for lhs_config, rhs_config in zip(lhs_configs, rhs_configs):
     if (isinstance(lhs_config.quant_config, aqt_config.IntQuantConfig) and
@@ -178,35 +182,39 @@
   Raises:
     aqt_config.ConfigError: The input or filter quantizer configurations
       do not share statistics along contraction axes as described by
       `_validate_contraction`, or their quantization schedules are not aligned
       per `aqt_config._validate_alignment`.
   """
 
-  aqt_config._validate_alignment('input_quantizer.config.tensor_configs',
-                                 input_quantizer.config.tensor_configs,
-                                 'filter_quantizer.config.tensor_configs',
-                                 filter_quantizer.config.tensor_configs)
+  if input_quantizer.config is not None and filter_quantizer.config is not None:
+    aqt_config_utils._validate_alignment(
+        'input_quantizer.config.tensor_configs',
+        input_quantizer.config.tensor_configs,
+        'filter_quantizer.config.tensor_configs',
+        filter_quantizer.config.tensor_configs)
 
   input_spec, filter_spec, _ = dimension_numbers  # pytype: disable=attribute-error
   _, *input_contracted_dims = input_spec
   _, *filter_contracted_dims = filter_spec
 
-  for axis in input_contracted_dims:
-    if axis not in input_quantizer.config.stats_config.share_stats_axes:
-      raise aqt_config.ConfigError(
-          f'expected contraction axis ({axis}) to be in '
-          f'input_quantizer.config.stats_config.share_stats_axes={input_quantizer.config.stats_config.share_stats_axes}'
-      )
-  for axis in filter_contracted_dims:
-    if axis not in filter_quantizer.config.stats_config.share_stats_axes:
-      raise aqt_config.ConfigError(
-          f'expected contraction axis ({axis}) to be in '
-          f'filter_quantizer.config.stats_config.share_stats_axes={filter_quantizer.config.stats_config.share_stats_axes}'
-      )
+  if input_quantizer.config is not None:
+    for axis in input_contracted_dims:
+      if axis not in input_quantizer.config.stats_config.share_stats_axes:
+        raise aqt_config.ConfigError(
+            f'expected contraction axis ({axis}) to be in '
+            f'input_quantizer.config.stats_config.share_stats_axes={input_quantizer.config.stats_config.share_stats_axes}'
+        )
+  if filter_quantizer.config is not None:
+    for axis in filter_contracted_dims:
+      if axis not in filter_quantizer.config.stats_config.share_stats_axes:
+        raise aqt_config.ConfigError(
+            f'expected contraction axis ({axis}) to be in '
+            f'filter_quantizer.config.stats_config.share_stats_axes={filter_quantizer.config.stats_config.share_stats_axes}'
+        )
 
 
 def _transpose_inv_scale(x, dimension_numbers_before, dimension_numbers_after):
   """Changes the order of axes in x from dimension_numbers_before to dimension_numbers_after."""
   assert (len(dimension_numbers_before) == len(dimension_numbers_after)), (
       f'len(dimension_numbers_before) ({len(dimension_numbers_before)}) must ',
       f'be equal to len(dimension_numbers_after) ({len(dimension_numbers_after)})'
@@ -215,48 +223,48 @@
   axes = [0] * len(dimension_numbers_before)
   for i, axis in enumerate(dimension_numbers_after):
     axes[axis] = dimension_numbers_before[i]
 
   return jnp.transpose(x, axes)
 
 
-def conv_general_dilated(
-    lhs: jnp.ndarray,
-    rhs: jnp.ndarray,
-    lhs_quantizer: aqt_tensor.TensorQuantizer,
-    rhs_quantizer: aqt_tensor.TensorQuantizer,
-    window_strides: Sequence[int],
-    padding: Union[str, Sequence[Tuple[int, int]]],
-    lhs_dilation: Optional[Sequence[int]] = None,
-    rhs_dilation: Optional[Sequence[int]] = None,
-    dimension_numbers: Optional[lax.ConvGeneralDilatedDimensionNumbers] = None,
-    feature_group_count: int = 1,
-    batch_group_count: int = 1,
-    train: bool = True) -> jnp.ndarray:
+def conv_general_dilated(lhs: jnp.ndarray,
+                         rhs: jnp.ndarray,
+                         lhs_quantizer: aqt_tensor.TensorQuantizer,
+                         rhs_quantizer: aqt_tensor.TensorQuantizer,
+                         window_strides: Sequence[int],
+                         padding: Union[str, Sequence[Tuple[int, int]]],
+                         lhs_dilation: Optional[Sequence[int]] = None,
+                         rhs_dilation: Optional[Sequence[int]] = None,
+                         dimension_numbers: Optional[
+                             lax.ConvGeneralDilatedDimensionNumbers] = None,
+                         feature_group_count: int = 1,
+                         batch_group_count: int = 1,
+                         train: bool = True) -> jnp.ndarray:
   """Quantized jax.lax.conv_general_dilated.
 
   Args:
     lhs: Left-hand side of the conv_general_dilated (input).
     rhs: Right-hand side of the conv_general_dilated (filter).
     lhs_quantizer: The tensor quantizer for lhs.
     rhs_quantizer: The tensor quantizer for rhs.
     window_strides: a sequence of `n` integers, representing the inter-window
       strides.
     padding: either the string `'SAME'`, the string `'VALID'`, or a sequence of
       `n` `(low, high)` integer pairs that give the padding to apply before and
       after each spatial dimension.
-    lhs_dilation: `None`, or a sequence of `n` integers, giving the
-      dilation factor to apply in each spatial dimension of `lhs`. LHS dilation
-      is also known as transposed convolution.
-    rhs_dilation: `None`, or a sequence of `n` integers, giving the
-      dilation factor to apply in each spatial dimension of `rhs`. RHS dilation
-      is also known as atrous convolution.
-    dimension_numbers: either `None`, a ``ConvDimensionNumbers`` object, or
-      a 3-tuple ``(lhs_spec, rhs_spec, out_spec)``, where each element is a
-      string of length `n+2`.
+    lhs_dilation: `None`, or a sequence of `n` integers, giving the dilation
+      factor to apply in each spatial dimension of `lhs`. LHS dilation is also
+      known as transposed convolution.
+    rhs_dilation: `None`, or a sequence of `n` integers, giving the dilation
+      factor to apply in each spatial dimension of `rhs`. RHS dilation is also
+      known as atrous convolution.
+    dimension_numbers: either `None`, a ``ConvDimensionNumbers`` object, or a
+      3-tuple ``(lhs_spec, rhs_spec, out_spec)``, where each element is a string
+      of length `n+2`.
     feature_group_count: integer, default 1. See XLA HLO docs.
     batch_group_count: integer, default 1. See XLA HLO docs.
     train: If false and `use_quantized_variable` in lhs_quantizer or
       rhs_quantizer, then this indicates `aqt_conv_general` should use the
       quantized variable with the latest quantized, memorized from the most
       recent `TensorQuantizer.update()` in quantized operations rather than the
       float tensor input `lhs` or `rhs` provided to those operations at
@@ -271,14 +279,20 @@
                               'only 2-D convolution.')
 
   dimension_numbers = lax.conv_dimension_numbers(lhs.shape, rhs.shape,
                                                  dimension_numbers)
 
   _validate_inputs(lhs_quantizer, rhs_quantizer, dimension_numbers)
 
+  lhs_scale, lhs_inv_scale = lhs_quantizer._get_quant_scale(train)
+  rhs_scale, rhs_inv_scale = rhs_quantizer._get_quant_scale(train)
+
+  lhs = lhs_scale * lhs
+  rhs = rhs_scale * rhs
+
   lhs = lhs_quantizer._to_quant(lhs, train)
   rhs = rhs_quantizer._to_quant(rhs, train)
 
   should_int8_quantize = aqt_utils.should_int8_quantize(lhs_quantizer,
                                                         rhs_quantizer)
 
   if should_int8_quantize:
@@ -286,29 +300,27 @@
                                 rhs_dilation)
 
   conv = _conv_general_aqt(lhs, rhs, lhs_quantizer, rhs_quantizer,
                            should_int8_quantize, train, window_strides, padding,
                            lhs_dilation, rhs_dilation, dimension_numbers,
                            feature_group_count, batch_group_count)
 
-  lhs_inv_scale = lhs_quantizer._from_quant_scale(train)
-  rhs_inv_scale = rhs_quantizer._from_quant_scale(train)
-
   # Transpose both lhs_inv_scale and rhs_inv_scale such that they have `NHWC`
   # and `HWIO` shapes, respectively, which allows them to be broadcastable no
   # matter how they were shaped originally by `dimension_numbers`.
   dim_numbers = {
       'NHWC': (0, 3, 1, 2),
       'HWIO': (3, 2, 0, 1),
   }
-  lhs_inv_scale = _transpose_inv_scale(lhs_inv_scale, dimension_numbers[0],
-                                       dim_numbers['NHWC'])
-  rhs_inv_scale = _transpose_inv_scale(rhs_inv_scale, dimension_numbers[1],
-                                       dim_numbers['HWIO'])
-  assert len(lhs_inv_scale.shape) == len(rhs_inv_scale.shape)
+  if lhs_quantizer.config is not None and rhs_quantizer.config is not None:
+    lhs_inv_scale = _transpose_inv_scale(lhs_inv_scale, dimension_numbers[0],
+                                         dim_numbers['NHWC'])
+    rhs_inv_scale = _transpose_inv_scale(rhs_inv_scale, dimension_numbers[1],
+                                         dim_numbers['HWIO'])
+    assert len(lhs_inv_scale.shape) == len(rhs_inv_scale.shape)
 
   inv_scale = lhs_inv_scale * rhs_inv_scale
   # Reverse the shape of inv_scale back to one specified by out_spec in
   # `dimension_numbers`
   inv_scale = _transpose_inv_scale(inv_scale, dim_numbers['NHWC'],
                                    dimension_numbers[2])
   return conv * inv_scale
```

### Comparing `aqtp-0.0.9/aqt/jax/aqt_utils.py` & `aqtp-0.1.0/aqt/jax/aqt_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """Common utilities for Jax AQTp."""
 
 from aqt.common import aqt_config
 from aqt.jax import aqt_tensor
 import jax.numpy as jnp
 
 # pylint: disable=protected-access
+# pytype: disable=attribute-error
 
 
 def possibly_use_quantized_variable(
     quantizer: aqt_tensor.TensorQuantizer,
     x: jnp.ndarray,
     train: bool) -> jnp.ndarray:
   """Returns quantized variable if not training and TQ.use_quantized_variable, casted to x.dtype.
@@ -37,28 +38,28 @@
     quantizer: TensorQuantizer for the input tensor x.
     x: lhs or rhs of conv_general.
     train: Indicates if in training or not.
 
   Returns:
     The input tensor x or its quantized one.
   """
-  if quantizer.config.use_quantized_variable and not train:
+  if quantizer.config is not None and quantizer.config.use_quantized_variable and not train:
     qx = quantizer.quantized_variable.value
     qx = qx.astype(x.dtype)
     return qx
   return x
 
 
 def should_int8_quantize(
     lhs_quantizer: aqt_tensor.TensorQuantizer,
     rhs_quantizer: aqt_tensor.TensorQuantizer) -> bool:
   """Determines whether or not to quantize."""
 
-  assert lhs_quantizer._last_update.value == rhs_quantizer._last_update.value, (
-      'lhs_quantizer._last_update != rhs_quantizer._last_update')
+  if lhs_quantizer.config is None or rhs_quantizer.config is None:
+    return jnp.bool_(False)
 
   lhs_configs = lhs_quantizer.config.tensor_configs
   rhs_configs = rhs_quantizer.config.tensor_configs
 
   should_quantize = False
   for lhs_config in lhs_configs:
     for rhs_config in rhs_configs:
```

### Comparing `aqtp-0.0.9/aqt/jax/aqt_conv_general_test.py` & `aqtp-0.1.0/aqt/jax/aqt_conv_general_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for conv_general."""
 
 import itertools
-from typing import Iterable
+from typing import Iterable, Optional
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from aqt.common import aqt_config
 from aqt.jax import aqt_conv_general
 from aqt.jax import aqt_ops
 from aqt.jax import aqt_tensor
@@ -53,16 +53,16 @@
             window_strides=strides,
             padding=padding))
 
   return case_dicts
 
 
 class ConvGeneralModule(nn.Module):
-  lhs_config: aqt_config.AqtScheduleConfig
-  rhs_config: aqt_config.AqtScheduleConfig
+  lhs_config: Optional[aqt_config.AqtScheduleConfig]
+  rhs_config: Optional[aqt_config.AqtScheduleConfig]
   lhs_shape: Iterable[int]
   rhs_shape: Iterable[int]
 
   @nn.compact
   def __call__(self,
                lhs,
                rhs,
@@ -301,10 +301,26 @@
                                            jnp.newaxis, :]
     feature_inv_scale = aqt_conv_general._transpose_inv_scale(
         feature_inv_scale, dim_numbers["NHWC"], dimension_numbers[2])
     expected *= (batch_inv_scale * feature_inv_scale)
 
     self.assertAllEqual(actual, expected)
 
+  def test_weight_only_quantization(self):
+    x, w = self.create_random_input_and_filter()
+    input_config = aqt_conv_test_base.schedule_config(
+        "input", bits=8, const_coeff=1.0)
+    filter_config = aqt_conv_test_base.schedule_config(
+        "filter", bits=8, const_coeff=1.0)
+    input_config.tensor_configs[0].quant_config = aqt_config.FloatConfig()
+
+    kwargs = self.get_conv_kwargs(strides=1, padding="VALID")
+    result_with_float_config = self.conv_op_quantized(
+        x, w, input_config, filter_config, event_count=0, **kwargs)
+    result_with_none_config = self.conv_op_quantized(
+        x, w, None, filter_config, event_count=0, **kwargs)
+
+    self.assertAllEqual(result_with_float_config, result_with_none_config)
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `aqtp-0.0.9/aqt/jax/__init__.py` & `aqtp-0.1.0/aqt/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.0.9/aqt/jax/aqt_tensor_test.py` & `aqtp-0.1.0/aqt/jax/aqt_tensor_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """Tests for aqt_tensor."""
 
 from absl.testing import absltest
 from aqt.jax import aqt_tensor
 from aqt.test import aqt_stats_test_base
 from aqt.test import aqt_tensor_test_base
 import jax
@@ -31,71 +30,94 @@
 class StatsTest(aqt_stats_test_base.StatsTest):
   """Tests for Stats class.
 
   Refer to aqt_stats_test_base.StatsTest for more details.
   """
 
   def set_stats(self, data_shape, config):
-    self._stats = aqt_tensor.Stats.init_stats(
-        data_shape=data_shape, config=config)
+    self._stats = aqt_tensor.Stats(data_shape=data_shape, config=config)
+    self._stats_state = self._stats.init(jax.random.PRNGKey(0))
+    self.override_ema_update_count = None
 
   def update(self, sample, weight):
-    self._stats = self._stats.with_update(f32(sample), f32(weight))
+    _, self._stats_state = self._stats.apply(
+        self._stats_state,
+        f32(sample),
+        f32(weight),
+        override_ema_update_count=self.override_ema_update_count,
+        method=self._stats.update,
+        mutable=["aqt"])
 
   def get_sum_of_ones(self):
-    return self._stats.sum_of_ones
+    return self._stats_state["aqt"]["sum_of_ones"]
 
   def get_sum_of_vals(self):
-    return self._stats.sum_of_vals
+    return self._stats_state["aqt"]["sum_of_vals"]
 
   def get_max_of_abs_vals(self):
-    return self._stats.max_dev()
+    return self._stats_state["aqt"]["max_of_abs_vals"]
 
   def get_sum_of_l1_vals(self):
-    return self._stats.sum_of_l1_vals
+    return self._stats_state["aqt"]["sum_of_l1_vals"]
 
   def get_sum_of_lp_vals(self):
-    return self._stats.sum_of_lp_vals
+    return self._stats_state["aqt"]["sum_of_lp_vals"]
 
   def set_ema_update_count(self, ema_update_count):
-    self._stats = self._stats.replace(ema_update_count=ema_update_count)
+    self.override_ema_update_count = ema_update_count
+
+  def mean(self):
+    return self._stats.apply(self._stats_state, method=self._stats.mean)
+
+  def max_dev(self):
+    return self._stats.apply(self._stats_state, method=self._stats.max_dev)
+
+  def l1_dev(self):
+    return self._stats.apply(self._stats_state, method=self._stats.l1_dev)
+
+  def lp_dev(self):
+    return self._stats.apply(self._stats_state, method=self._stats.lp_dev)
+
+  def bound(self, calibration_config):
+    return self._stats.apply(
+        self._stats_state, calibration_config, method=self._stats.bound)
 
 
 class AqtTensorQuantizerTest(aqt_tensor_test_base.AqtTensorQuantizerTest):
   """Tests for AqtTensorQuantizer class.
 
   Refer to aqt_test_shared_base.AqtTensorQuantizerTest for more details.
   """
 
   _quant_state = {}
 
   def make_tensor_quantizer(self, data_shape, config, name="tq"):
-    quant = aqt_tensor.TensorQuantizer(data_shape=data_shape, config=config,
-                                       name=name)
+    quant = aqt_tensor.TensorQuantizer(
+        data_shape=data_shape, config=config, name=name)
     self._quant_state[name] = quant.init(jax.random.PRNGKey(0))
     return quant
 
   def update_quantizer(self, quant, sample, weight, event_count):
     _, self._quant_state[quant.name] = quant.apply(
         self._quant_state[quant.name],
         sample,
         weight,
         int(event_count),
         method=quant.update,
-        mutable="TensorQuantizer")
+        mutable=["TensorQuantizer", "aqt"])
 
   def to_quant(self, quant, x, train=True):
     return quant.apply(
         self._quant_state[quant.name], x, train, method=quant._to_quant)
 
-  def from_quant_scale(self, quant, train=True):
+  def get_quant_scale(self, quant, train=True):
     return quant.apply(
         self._quant_state[quant.name],  #
         train,
-        method=quant._from_quant_scale)
+        method=quant._get_quant_scale)
 
   def init(self):
     pass
 
   def get_scale(self, quant):
     return self._quant_state[quant.name]["TensorQuantizer"]["scale"]
 
@@ -120,12 +142,14 @@
     expected = fn(inp)
 
     # Pass-through function should return the same output as fn(x).
     np.testing.assert_equal(actual, expected)
 
     # The gradient of fn() should be 1.0 since STE makes it pretend to be an
     # identity function during the backward pass.
-    np.testing.assert_equal(jnp.array(1.0),
-                            jax.grad(aqt_tensor.pass_through)(inp, fn))
+    np.testing.assert_equal(
+        jnp.array(1.0),
+        jax.grad(aqt_tensor.pass_through)(inp, fn))
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `aqtp-0.0.9/aqt/jax/aqt_ops.py` & `aqtp-0.1.0/aqt/jax/aqt_ops.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,12 +18,14 @@
 the quantization algorithm in AQTp.
 """
 # TODO(jihwanlee): Create a shared doc, referred to by both TF and Jax.
 
 
 from aqt.jax import aqt_conv_general
 from aqt.jax import aqt_dot_general
+from aqt.jax import aqt_matmul
 
 
 aqt_conv_general_dilated = aqt_conv_general.conv_general_dilated
 aqt_dot = aqt_dot_general.dot
 aqt_dot_general = aqt_dot_general.dot_general
+aqt_matmul = aqt_matmul.matmul
```

### Comparing `aqtp-0.0.9/setup.py` & `aqtp-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "tensorflow-datasets>=4.5.2",
     "dacite>=1.6.0",
     "ml_collections>=0.1.1",
 ]
 
 setup(
     name="aqtp",
-    version="0.0.9",
+    version="0.1.0",
     description="AQT: Accurate Quantized Training",
     long_description="\n\n".join([README]),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
```

### Comparing `aqtp-0.0.9/aqtp.egg-info/SOURCES.txt` & `aqtp-0.1.0/aqtp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 LICENSE
+README.md
 setup.py
 aqt/__init__.py
+aqt/common/__init__.py
+aqt/common/aqt_common.py
+aqt/common/aqt_config.py
+aqt/common/aqt_config_schedule_test.py
+aqt/common/aqt_config_utils.py
+aqt/common/emulated_floating_points.py
+aqt/common/emulation_utils.py
 aqt/jax/__init__.py
 aqt/jax/aqt_conv_general.py
 aqt/jax/aqt_conv_general_test.py
 aqt/jax/aqt_dot_general.py
 aqt/jax/aqt_dot_general_test.py
+aqt/jax/aqt_matmul.py
+aqt/jax/aqt_matmul_test.py
 aqt/jax/aqt_ops.py
 aqt/jax/aqt_tensor.py
 aqt/jax/aqt_tensor_test.py
 aqt/jax/aqt_utils.py
 aqt/jax_legacy/__init__.py
 aqt/jax_legacy/jax/__init__.py
 aqt/jax_legacy/jax/compute_cost_utils.py
@@ -26,14 +36,16 @@
 aqt/jax_legacy/jax/hlo_utils_test.py
 aqt/jax_legacy/jax/primitives.py
 aqt/jax_legacy/jax/primitives_test.py
 aqt/jax_legacy/jax/quant_config.py
 aqt/jax_legacy/jax/quantization.py
 aqt/jax_legacy/jax/quantization_test.py
 aqt/jax_legacy/jax/shape_utils.py
+aqt/jax_legacy/jax/sparsity.py
+aqt/jax_legacy/jax/sparsity_test.py
 aqt/jax_legacy/jax/stats.py
 aqt/jax_legacy/jax/stats_tag.py
 aqt/jax_legacy/jax/stats_tag_test.py
 aqt/jax_legacy/jax/stats_test.py
 aqt/jax_legacy/jax/test_utils.py
 aqt/jax_legacy/jax/train_utils.py
 aqt/jax_legacy/jax/train_utils_test.py
@@ -47,14 +59,15 @@
 aqt/jax_legacy/jax/imagenet/input_pipeline.py
 aqt/jax_legacy/jax/imagenet/models.py
 aqt/jax_legacy/jax/imagenet/models_test.py
 aqt/jax_legacy/jax/imagenet/pokebnn.py
 aqt/jax_legacy/jax/imagenet/pokebnn_test.py
 aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
 aqt/jax_legacy/jax/imagenet/train.py
+aqt/jax_legacy/jax/imagenet/train_benchmark.py
 aqt/jax_legacy/jax/imagenet/train_test.py
 aqt/jax_legacy/jax/imagenet/train_utils.py
 aqt/jax_legacy/jax/imagenet/configs/__init__.py
 aqt/jax_legacy/jax/imagenet/configs/base_config.py
 aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
 aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
 aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
```

