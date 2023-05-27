# Comparing `tmp/GANDLF-0.0.17.dev20230526.tar.gz` & `tmp/GANDLF-0.0.17.dev20230527.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.17.dev20230526.tar", last modified: Fri May 26 03:13:37 2023, max compression
+gzip compressed data, was "GANDLF-0.0.17.dev20230527.tar", last modified: Sat May 27 03:12:46 2023, max compression
```

## Comparing `GANDLF-0.0.17.dev20230526.tar` & `GANDLF-0.0.17.dev20230527.tar`

### file list

```diff
@@ -1,170 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.778779 GANDLF-0.0.17.dev20230526/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/Dockerfile-CPU
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/Dockerfile-CUDA11.6
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/Dockerfile-ROCm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.670778 GANDLF-0.0.17.dev20230526/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.674778 GANDLF-0.0.17.dev20230526/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.682778 GANDLF-0.0.17.dev20230526/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.686778 GANDLF-0.0.17.dev20230526/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.690778 GANDLF-0.0.17.dev20230526/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.694778 GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.694778 GANDLF-0.0.17.dev20230526/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.698778 GANDLF-0.0.17.dev20230526/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.702778 GANDLF-0.0.17.dev20230526/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.706778 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.710778 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.714778 GANDLF-0.0.17.dev20230526/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.718778 GANDLF-0.0.17.dev20230526/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.722778 GANDLF-0.0.17.dev20230526/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/metrics/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.746778 GANDLF-0.0.17.dev20230526/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.766779 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.770779 GANDLF-0.0.17.dev20230526/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.770779 GANDLF-0.0.17.dev20230526/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.778779 GANDLF-0.0.17.dev20230526/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 03:13:29.000000 GANDLF-0.0.17.dev20230526/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:13:37.670778 GANDLF-0.0.17.dev20230526/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-26 03:13:37.000000 GANDLF-0.0.17.dev20230526/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-26 03:13:37.000000 GANDLF-0.0.17.dev20230526/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 03:13:37.000000 GANDLF-0.0.17.dev20230526/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 03:10:34.000000 GANDLF-0.0.17.dev20230526/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-26 03:13:37.000000 GANDLF-0.0.17.dev20230526/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 03:13:37.000000 GANDLF-0.0.17.dev20230526/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-26 03:13:37.778779 GANDLF-0.0.17.dev20230526/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 03:13:37.778779 GANDLF-0.0.17.dev20230526/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-26 03:10:14.000000 GANDLF-0.0.17.dev20230526/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.982974 GANDLF-0.0.17.dev20230527/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/Dockerfile-CPU
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/Dockerfile-CUDA11.6
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/Dockerfile-ROCm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.942974 GANDLF-0.0.17.dev20230527/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.942974 GANDLF-0.0.17.dev20230527/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.946974 GANDLF-0.0.17.dev20230527/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/cli/generate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.950974 GANDLF-0.0.17.dev20230527/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.950974 GANDLF-0.0.17.dev20230527/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.954974 GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.954974 GANDLF-0.0.17.dev20230527/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.954974 GANDLF-0.0.17.dev20230527/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21747 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.954974 GANDLF-0.0.17.dev20230527/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.958974 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.958974 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.958974 GANDLF-0.0.17.dev20230527/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.962974 GANDLF-0.0.17.dev20230527/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.962974 GANDLF-0.0.17.dev20230527/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/metrics/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.970974 GANDLF-0.0.17.dev20230527/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.978974 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.978974 GANDLF-0.0.17.dev20230527/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29587 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.978974 GANDLF-0.0.17.dev20230527/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.982974 GANDLF-0.0.17.dev20230527/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-27 03:12:40.000000 GANDLF-0.0.17.dev20230527/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 03:12:46.942974 GANDLF-0.0.17.dev20230527/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-27 03:12:46.000000 GANDLF-0.0.17.dev20230527/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-27 03:12:46.000000 GANDLF-0.0.17.dev20230527/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 03:12:46.000000 GANDLF-0.0.17.dev20230527/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 03:10:32.000000 GANDLF-0.0.17.dev20230527/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-27 03:12:46.000000 GANDLF-0.0.17.dev20230527/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 03:12:46.000000 GANDLF-0.0.17.dev20230527/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-27 03:12:46.982974 GANDLF-0.0.17.dev20230527/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_generateMetrics
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 03:12:46.982974 GANDLF-0.0.17.dev20230527/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-27 03:10:11.000000 GANDLF-0.0.17.dev20230527/setup.py
```

### Comparing `GANDLF-0.0.17.dev20230526/CODE_OF_CONDUCT.md` & `GANDLF-0.0.17.dev20230527/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/CONTRIBUTING.md` & `GANDLF-0.0.17.dev20230527/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/Dockerfile-CPU` & `GANDLF-0.0.17.dev20230527/Dockerfile-CPU`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/Dockerfile-CUDA11.6` & `GANDLF-0.0.17.dev20230527/Dockerfile-CUDA11.6`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/Dockerfile-ROCm` & `GANDLF-0.0.17.dev20230527/Dockerfile-ROCm`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.17.dev20230527/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.17.dev20230527/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/cli/__init__.py` & `GANDLF-0.0.17.dev20230527/GANDLF/cli/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .patch_extraction import patch_extraction
 from .main_run import main_run
 from .preprocess_and_save import preprocess_and_save
 from .config_generator import config_generator
 from .deploy import deploy_targets, run_deployment
 from .recover_config import recover_config
 from .post_training_model_optimization import post_training_model_optimization
+from .generate_metrics import generate_metrics_dict
 
 from datetime import date
 
 copyrightMessage = (
     "Contact: gandlf@mlcommons.org\n\n"
     + "This program is NOT FDA/CE approved and NOT intended for clinical use.\nCopyright (c) "
     + str(date.today().year)
```

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/cli/config_generator.py` & `GANDLF-0.0.17.dev20230527/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/cli/deploy.py` & `GANDLF-0.0.17.dev20230527/GANDLF/cli/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,22 +154,37 @@
         f.write(yaml.dump(mlcube_config, sort_keys=False, default_flow_style=False))
 
     # This tag will be modified later by our deployment mechanism
     docker_image = mlcube_config["docker"]["image"]
 
     # Run the mlcube_docker configuration process, forcing build from local repo
     gandlf_root = os.path.realpath(os.path.dirname(__file__) + "/../../")
-    site_packages_dir = sysconfig.get_path('purelib')
+    site_packages_dir = sysconfig.get_path("purelib")
     symlink_location = ""
-    if gandlf_root == site_packages_dir: # Installed via pip, not as editable source install, extra work is needed
-        setup_files = ['setup.py', '.dockerignore', 'pyproject.toml', 'MANIFEST.in']
-        dockerfiles = [item for item in os.listdir(gandlf_root) if os.path.isfile(os.path.join(gandlf_root, item)) and item.startswith("Dockerfile-")]
-        entrypoints = [item for item in os.listdir(gandlf_root) if os.path.isfile(os.path.join(gandlf_root, item)) and item.startswith("gandlf_")]
+    if (
+        gandlf_root == site_packages_dir
+    ):  # Installed via pip, not as editable source install, extra work is needed
+        setup_files = ["setup.py", ".dockerignore", "pyproject.toml", "MANIFEST.in"]
+        dockerfiles = [
+            item
+            for item in os.listdir(gandlf_root)
+            if os.path.isfile(os.path.join(gandlf_root, item))
+            and item.startswith("Dockerfile-")
+        ]
+        entrypoints = [
+            item
+            for item in os.listdir(gandlf_root)
+            if os.path.isfile(os.path.join(gandlf_root, item))
+            and item.startswith("gandlf_")
+        ]
         for file in setup_files + dockerfiles + entrypoints:
-            shutil.copy(os.path.join(gandlf_root, file), os.path.join(gandlf_root, "GANDLF", file))
+            shutil.copy(
+                os.path.join(gandlf_root, file),
+                os.path.join(gandlf_root, "GANDLF", file),
+            )
         if not os.path.exists(os.path.join(gandlf_root, "GANDLF", "GANDLF")):
             # point to same package directory, acts as a recursive location for the GaNDLF package
             symlink_location = os.path.join(gandlf_root, "GANDLF", "GANDLF")
             os.symlink("./", os.path.join(gandlf_root, "GANDLF", "GANDLF"))
         gandlf_root = os.path.join(gandlf_root, "GANDLF")
 
     print(os.listdir(gandlf_root))
```

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/cli/main_run.py` & `GANDLF-0.0.17.dev20230527/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.17.dev20230527/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.17.dev20230527/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.17.dev20230527/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/cli/recover_config.py` & `GANDLF-0.0.17.dev20230527/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.17.dev20230527/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/compute/generic.py` & `GANDLF-0.0.17.dev20230527/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.17.dev20230527/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.17.dev20230527/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/compute/step.py` & `GANDLF-0.0.17.dev20230527/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/compute/training_loop.py` & `GANDLF-0.0.17.dev20230527/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/__init__.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.17.dev20230527/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.17.dev20230527/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.17.dev20230527/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.17.dev20230527/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/inference_manager.py` & `GANDLF-0.0.17.dev20230527/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/logger.py` & `GANDLF-0.0.17.dev20230527/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/losses/__init__.py` & `GANDLF-0.0.17.dev20230527/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/losses/hybrid.py` & `GANDLF-0.0.17.dev20230527/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/losses/regression.py` & `GANDLF-0.0.17.dev20230527/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/losses/segmentation.py` & `GANDLF-0.0.17.dev20230527/GANDLF/losses/segmentation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import torch
 
 
 # Dice scores and dice losses
 def dice(predicted, target):
     """
     This function computes a dice score between two tensors
@@ -15,51 +16,42 @@
 
     Returns
     -------
     Tensor
         Computed Dice Score
 
     """
-    smooth = 1e-7
-
-    predicted_flat = predicted.contiguous().view(-1)
-    label_flat = target.contiguous().view(-1)
+    predicted_flat = predicted.flatten()
+    label_flat = target.flatten()
     intersection = (predicted_flat * label_flat).sum()
 
-    dice_score = (2.0 * intersection + smooth) / (
-        predicted_flat.sum() + label_flat.sum() + smooth
+    dice_score = (2.0 * intersection + sys.float_info.min) / (
+        predicted_flat.sum() + label_flat.sum() + sys.float_info.min
     )
 
     return dice_score
 
 
 def MCD(predicted, target, num_class, weights=None, ignore_class=None, loss_type=0):
     """
-    Parameters
-    ----------
-    predicted : torch.Tensor
-        Prediction tensor generated by the model
-    tarrget : torch.Tensor
-        Ground truth tensor
-    num_class : int
-        Number of classes (including the background class)
-    weights : list, optional
-        Dice weights for each class (excluding the background class), defaults to None
-    ignore_class : int, optional
-        Class to ignore, defaults to None
-    loss_type : int, optional
-        Type of loss to compute, defaults to 0
-        0: no loss, normal dice calculation
-        1: dice loss, (1-dice)
-        2: log dice, -log(dice)
+    This function computes the mean class dice score between two tensors
 
-    Returns
-    -------
-    Tensor
-        Mean Class Dice score
+    Args:
+        predicted (torch.Tensor): predicted generally by the network
+        target (torch.Tensor): Required target label to match the predicted with
+        num_class (int): Number of classes (including the background class)
+        weights (list, optional): Dice weights for each class (excluding the background class), defaults to None
+        ignore_class (int, optional): Class to ignore, defaults to None
+        loss_type (int, optional): Type of loss to compute, defaults to 0
+            0: no loss, normal dice calculation
+            1: dice loss, (1-dice)
+            2: log dice, -log(dice)
+
+    Returns:
+        torch.Tensor: Mean Class Dice score
     """
 
     acc_dice = 0
 
     for i in range(num_class):  # 0 is background
         currentDice = dice(predicted[:, i, ...], target[:, i, ...])
 
@@ -104,36 +96,26 @@
         len(params["model"]["class_list"]),
         params["weights"],
         None,
         2,
     )
 
 
-def tversky_loss(predicted, target, alpha=0.5, beta=0.5, smooth=1e-7):
+def tversky_loss(predicted, target, alpha=0.5, beta=0.5):
     """
     This function calculates the Tversky loss between two tensors.
 
-    Parameters
-    ----------
-    predicted : torch.Tensor
-        predicted predicted generally by the network
-    target : torch.Tensor
-        Required target label to match the predicted with
-    alpha : float, optional
-        Weight of false positives
-    beta : float, optional
-        Weight of false negatives
-    smooth : float, optional
-        Smoothing factor to avoid division by zero
-
-    Returns
-    -------
-    torch.Tensor
-        Computed Tversky Loss
+    Args:
+        predicted (torch.Tensor): predicted generally by the network
+        target (torch.Tensor): Required target label to match the predicted with
+        alpha (float, optional): Weight of false positives. Defaults to 0.5.
+        beta (float, optional): Weight of false negatives. Defaults to 0.5.
 
+    Returns:
+        torch.Tensor: Computed Tversky Loss
     """
     # Move this part later to parameter parsing, no need to check every time
     assert 0 <= alpha <= 1, f"Invalid alpha value: {alpha}"
     assert 0 <= beta <= 1, f"Invalid beta value: {beta}"
     assert 0 <= alpha + beta <= 1, f"Invalid alpha and beta values: {alpha}, {beta}"
 
     predicted_flat = predicted.contiguous().view(-1)
@@ -141,38 +123,31 @@
 
     true_positives = (predicted_flat * target_flat).sum()
     false_positives = ((1 - target_flat) * predicted_flat).sum()
     false_negatives = (target_flat * (1 - predicted_flat)).sum()
 
     numerator = true_positives
     denominator = true_positives + alpha * false_positives + beta * false_negatives
-    score = (numerator + smooth) / (denominator + smooth)
+    score = (numerator + sys.float_info.min) / (denominator + sys.float_info.min)
 
     loss = 1 - score
     return loss
 
 
 def MCT_loss(predicted, target, params=None):
     """
     This function calculates the Multi-Class Tversky loss between two tensors.
 
-    Parameters
-    ----------
-    predicted : torch.Tensor
-        predicted predicted generally by the network
-    target : torch.Tensor
-        Required target label to match the predicted with
-    params : dict, optional
-        Additional parameters for computing loss function, including weights for each class
-
-    Returns
-    -------
-    torch.Tensor
-        Computed Multi-Class Tversky Loss
+    Args:
+        predicted (torch.Tensor): predicted generally by the network
+        target (torch.Tensor): Required target label to match the predicted with
+        params (dict, optional): Additional parameters for computing loss function, including weights for each class
 
+    Returns:
+        torch.Tensor: Computed Multi-Class Tversky Loss
     """
 
     acc_tv_loss = 0
     num_classes = predicted.shape[1]
 
     for i in range(num_classes):
         curr_loss = tversky_loss(predicted[:, i, ...], target[:, i, ...])
@@ -186,24 +161,17 @@
     return acc_tv_loss
 
 
 def KullbackLeiblerDivergence(mu, logvar, params=None):
     """
     Calculates the Kullback-Leibler divergence between two Gaussian distributions.
 
-    Parameters
-    ----------
-    mu : torch.Tensor
-        The mean of the first Gaussian distribution
-    logvar : torch.Tensor
-        The logarithm of the variance of the first Gaussian distribution
-    params : dict, optional
-        A dictionary of optional parameters
-
-    Returns
-    -------
-    torch.Tensor
-        The computed Kullback-Leibler divergence
+    Args:
+        mu (torch.Tensor): The mean of the first Gaussian distribution
+        logvar (torch.Tensor): The logarithm of the variance of the first Gaussian distribution
+        params (dict, optional): A dictionary of optional parameters
 
+    Returns:
+        torch.Tensor: The computed Kullback-Leibler divergence
     """
     loss = -0.5 * torch.sum(1 + logvar - mu.pow(2) - logvar.exp(), dim=-1)
     return loss.mean()
```

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/metrics/__init__.py` & `GANDLF-0.0.17.dev20230527/GANDLF/metrics/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,30 @@
     multi_class_dice_per_label,
     hd100,
     hd100_per_label,
     hd95,
     hd95_per_label,
     nsd,
     nsd_per_label,
+    sensitivity,
+    sensitivity_per_label,
+    specificity_segmentation,
+    specificity_segmentation_per_label,
+    jaccard,
+    jaccard_per_label,
 )
 from .regression import classification_accuracy, balanced_acc_score, per_label_accuracy
-from .generic import recall_score, precision_score, iou_score, f1_score, accuracy, specificity_score
+from .generic import (
+    recall_score,
+    precision_score,
+    iou_score,
+    f1_score,
+    accuracy,
+    specificity_score,
+)
 import GANDLF.metrics.classification as classification
 import GANDLF.metrics.regression as regression
 
 
 # global defines for the metrics
 global_metrics_dict = {
     "dice": multi_class_dice,
@@ -44,14 +57,20 @@
     "classification_accuracy": classification_accuracy,
     "precision": precision_score,
     "recall": recall_score,
     "specificity": specificity_score,
     "iou": iou_score,
     "balanced_accuracy": balanced_acc_score,
     "per_label_one_hot_accuracy": per_label_accuracy,
+    "sensitivity": sensitivity,
+    "sensitivity_per_label": sensitivity_per_label,
+    "specificity_segmentation": specificity_segmentation,
+    "specificity_segmentation_per_label": specificity_segmentation_per_label,
+    "jaccard": jaccard,
+    "jaccard_per_label": jaccard_per_label,
 }
 
 
 # global define for the metrics that use surface distances, and hence require "connectivity" to be defined
 surface_distance_ids = [
     "hd95",
     "hd95_per_label",
```

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/metrics/classification.py` & `GANDLF-0.0.17.dev20230527/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/metrics/generic.py` & `GANDLF-0.0.17.dev20230527/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/metrics/regression.py` & `GANDLF-0.0.17.dev20230527/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/MSDNet.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/__init__.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/brain_age.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/deep_unet.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/densenet.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/efficientnet.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/fcn.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/light_unet.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/modelBase.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/resnet.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/sdnet.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/transunet.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/uinc.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/unet.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/unetr.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/models/vgg.py` & `GANDLF-0.0.17.dev20230527/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.17.dev20230527/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.17.dev20230527/GANDLF/optimizers/wrap_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Adam,
     AdamW,
     # SparseAdam,
     Adamax,
     Adadelta,
     Adagrad,
     RMSprop,
-    RAdam
+    RAdam,
 )
 
 
 def sgd(parameters):
     """
     Creates a Stochastic Gradient Descent optimizer from the PyTorch `torch.optim` module using the input parameters.
 
@@ -99,14 +99,15 @@
 
     Returns:
         optimizer (torch.optim.AdamW): An AdamW optimizer.
 
     """
     return adam(parameters, opt_type="AdamW")
 
+
 def adamax(parameters):
     """
     Creates an Adamax optimizer from the PyTorch `torch.optim` module using the input parameters.
 
     Args:
         parameters (dict): A dictionary containing the input parameters for the optimizer.
 
@@ -220,27 +221,27 @@
         alpha=parameters["optimizer"].get("alpha", 0.99),
         eps=parameters["optimizer"].get("eps", 1e-8),
         centered=parameters["optimizer"].get("centered", False),
         momentum=parameters["optimizer"].get("momentum", 0),
         weight_decay=parameters["optimizer"].get("weight_decay", 0),
     )
 
+
 def radam(parameters):
     """
-    Creates a RAdam optimizer from the PyTorch `torch.optim` module using the input parameters. 
-    
-    Args: 
+    Creates a RAdam optimizer from the PyTorch `torch.optim` module using the input parameters.
+
+    Args:
         parameters (dict): A dictionary containing the input parameters for the optimizer.
-        
-    Returns: 
+
+    Returns:
         optimizer (torch.optim.RAdam): A RAdam optimizer.
     """
     # Create the optimizer using the input parameters
     return RAdam(
         parameters["model_parameters"],
         lr=parameters.get("learning_rate"),
         betas=parameters["optimizer"].get("betas", (0.9, 0.999)),
         eps=parameters["optimizer"].get("eps", 1e-8),
         weight_decay=parameters["optimizer"].get("weight_decay", 0),
         foreach=parameters["optimizer"].get("foreach", None),
     )
-
```

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/parseConfig.py` & `GANDLF-0.0.17.dev20230527/GANDLF/parseConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,25 +196,35 @@
         # initialize metrics dict
         for metric in params["metrics"]:
             # assigning a new variable because some metrics can be dicts, and we want to get the first key
             comparison_string = metric
             if isinstance(metric, dict):
                 comparison_string = list(metric.keys())[0]
             # these metrics always need to be dicts
-            if comparison_string in ["accuracy", "f1", "precision", "recall", "specificity", "iou"]:
+            if comparison_string in [
+                "accuracy",
+                "f1",
+                "precision",
+                "recall",
+                "specificity",
+                "iou",
+            ]:
                 if not isinstance(metric, dict):
                     temp_dict[metric] = {}
                 else:
                     temp_dict[comparison_string] = metric
             elif not isinstance(metric, dict):
                 temp_dict[metric] = None
 
             # special case for accuracy, precision, recall, and specificity; which could be dicts
             ## need to find a better way to do this
-            if any(_ in comparison_string for _ in ["precision", "recall", "specificity", "accuracy", "f1"]):
+            if any(
+                _ in comparison_string
+                for _ in ["precision", "recall", "specificity", "accuracy", "f1"]
+            ):
                 if comparison_string != "classification_accuracy":
                     temp_dict[comparison_string] = initialize_key(
                         temp_dict[comparison_string], "average", "weighted"
                     )
                     temp_dict[comparison_string] = initialize_key(
                         temp_dict[comparison_string], "multi_class", True
                     )
```

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.17.dev20230527/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.17.dev20230527/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/training_manager.py` & `GANDLF-0.0.17.dev20230527/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/utils/__init__.py` & `GANDLF-0.0.17.dev20230527/GANDLF/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     get_dataframe,
     convert_relative_paths_in_dataframe,
 )
 
 from .parameter_processing import (
     populate_header_in_parameters,
     find_problem_type,
+    find_problem_type_from_parameters,
     populate_channel_keys_in_params,
 )
 
 from .generic import (
     get_date_time,
     get_unique_timestamp,
     get_filename_extension_sanitized,
```

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/utils/generic.py` & `GANDLF-0.0.17.dev20230527/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.17.dev20230527/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/utils/imaging.py` & `GANDLF-0.0.17.dev20230527/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/utils/modelbase.py` & `GANDLF-0.0.17.dev20230527/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/utils/modelio.py` & `GANDLF-0.0.17.dev20230527/GANDLF/utils/modelio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/utils/tensor.py` & `GANDLF-0.0.17.dev20230527/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF/utils/write_parse.py` & `GANDLF-0.0.17.dev20230527/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.17.dev20230527/GANDLF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230526
+Version: 0.0.17.dev20230527
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230526 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230527 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230526/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.17.dev20230527/GANDLF.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 README.md
 SECURITY.md
 gandlf_anonymizer
 gandlf_collectStats
 gandlf_configGenerator
 gandlf_constructCSV
 gandlf_deploy
+gandlf_generateMetrics
 gandlf_optimizeModel
 gandlf_patchMiner
 gandlf_preprocess
 gandlf_recoverConfig
 gandlf_run
 gandlf_verifyInstall
 setup.py
@@ -39,27 +40,29 @@
 GANDLF/../Dockerfile-ROCm
 GANDLF/../MANIFEST.in
 GANDLF/../gandlf_anonymizer
 GANDLF/../gandlf_collectStats
 GANDLF/../gandlf_configGenerator
 GANDLF/../gandlf_constructCSV
 GANDLF/../gandlf_deploy
+GANDLF/../gandlf_generateMetrics
 GANDLF/../gandlf_optimizeModel
 GANDLF/../gandlf_patchMiner
 GANDLF/../gandlf_preprocess
 GANDLF/../gandlf_recoverConfig
 GANDLF/../gandlf_run
 GANDLF/../gandlf_verifyInstall
 GANDLF/../pyproject.toml
 GANDLF/../setup.py
 GANDLF/anonymize/__init__.py
 GANDLF/anonymize/convert_to_nifti.py
 GANDLF/cli/__init__.py
 GANDLF/cli/config_generator.py
 GANDLF/cli/deploy.py
+GANDLF/cli/generate_metrics.py
 GANDLF/cli/main_run.py
 GANDLF/cli/patch_extraction.py
 GANDLF/cli/post_training_model_optimization.py
 GANDLF/cli/preprocess_and_save.py
 GANDLF/cli/recover_config.py
 GANDLF/compute/__init__.py
 GANDLF/compute/forward_pass.py
```

### Comparing `GANDLF-0.0.17.dev20230526/HISTORY.md` & `GANDLF-0.0.17.dev20230527/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ## 0.0.17
-
+- Added a CLI for metrics computation
 
 ## 0.0.16
 - Added a script "gandlf_deploy", allowing deployment of models into MLCubes (currently requires Docker)
 - ImageNet pre-trained models for UNet with variable encoders is now available
 - ACS/Soft conversion is available for ImageNet-pretrained UNet
 - Updated links, copyright and email to MLCommons
 - Allowing provision for user to generate multiple configurations for experimentation
```

### Comparing `GANDLF-0.0.17.dev20230526/LICENSE` & `GANDLF-0.0.17.dev20230527/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/PKG-INFO` & `GANDLF-0.0.17.dev20230527/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230526
+Version: 0.0.17.dev20230527
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230526 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230527 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230526/README.md` & `GANDLF-0.0.17.dev20230527/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/SECURITY.md` & `GANDLF-0.0.17.dev20230527/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/gandlf_anonymizer` & `GANDLF-0.0.17.dev20230527/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/gandlf_collectStats` & `GANDLF-0.0.17.dev20230527/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/gandlf_configGenerator` & `GANDLF-0.0.17.dev20230527/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/gandlf_constructCSV` & `GANDLF-0.0.17.dev20230527/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/gandlf_deploy` & `GANDLF-0.0.17.dev20230527/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/gandlf_optimizeModel` & `GANDLF-0.0.17.dev20230527/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/gandlf_patchMiner` & `GANDLF-0.0.17.dev20230527/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/gandlf_preprocess` & `GANDLF-0.0.17.dev20230527/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/gandlf_recoverConfig` & `GANDLF-0.0.17.dev20230527/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/gandlf_run` & `GANDLF-0.0.17.dev20230527/gandlf_run`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from __future__ import print_function, division
 import os
 import argparse
 import ast
 import sys
 import traceback
 
 from GANDLF import version
```

### Comparing `GANDLF-0.0.17.dev20230526/gandlf_verifyInstall` & `GANDLF-0.0.17.dev20230527/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230526/setup.py` & `GANDLF-0.0.17.dev20230527/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,23 +38,44 @@
     (__version__,) = re.findall('__version__ = "(.*)"', version_file.read())
 
 except Exception as error:
     __version__ = "0.0.1"
     sys.stderr.write("Warning: Could not open '%s' due %s\n" % (filepath, error))
 
 # Handle cases where specific files need to be bundled into the final package as installed via PyPI
-dockerfiles = [item for item in os.listdir(os.path.dirname(os.path.abspath(__file__))) if (os.path.isfile(item) and item.startswith("Dockerfile-"))]
-entrypoint_files = [item for item in os.listdir(os.path.dirname(os.path.abspath(__file__))) if (os.path.isfile(item) and item.startswith("gandlf_"))]
-setup_files = ['setup.py', '.dockerignore', 'pyproject.toml', 'MANIFEST.in']
+dockerfiles = [
+    item
+    for item in os.listdir(os.path.dirname(os.path.abspath(__file__)))
+    if (os.path.isfile(item) and item.startswith("Dockerfile-"))
+]
+entrypoint_files = [
+    item
+    for item in os.listdir(os.path.dirname(os.path.abspath(__file__)))
+    if (os.path.isfile(item) and item.startswith("gandlf_"))
+]
+setup_files = ["setup.py", ".dockerignore", "pyproject.toml", "MANIFEST.in"]
 all_extra_files = dockerfiles + entrypoint_files + setup_files
 all_extra_files_pathcorrected = [os.path.join("../", item) for item in all_extra_files]
 # find_packages should only ever find these as subpackages of gandlf, not as top-level packages
 # generate this dynamically?
 # GANDLF.GANDLF is needed to prevent recursion madness in deployments
-toplevel_package_excludes = ['GANDLF.GANDLF', 'anonymize', 'cli', 'compute', 'data', 'grad_clipping', 'losses', 'metrics', 'models', 'optimizers', 'schedulers', 'utils']
+toplevel_package_excludes = [
+    "GANDLF.GANDLF",
+    "anonymize",
+    "cli",
+    "compute",
+    "data",
+    "grad_clipping",
+    "losses",
+    "metrics",
+    "models",
+    "optimizers",
+    "schedulers",
+    "utils",
+]
 
 
 requirements = [
     "torch==1.13.1",
     "black",
     "numpy==1.22.0",
     "scipy",
@@ -96,15 +117,18 @@
 if __name__ == "__main__":
     setup(
         name="GANDLF",
         version=__version__,
         author="MLCommons",
         author_email="gandlf@mlcommons.org",
         python_requires=">=3.8",
-        packages=find_packages(where=os.path.dirname(os.path.abspath(__file__)), exclude=toplevel_package_excludes),
+        packages=find_packages(
+            where=os.path.dirname(os.path.abspath(__file__)),
+            exclude=toplevel_package_excludes,
+        ),
         cmdclass={
             "install": CustomInstallCommand,
             "develop": CustomDevelopCommand,
             "egg_info": CustomEggInfoCommand,
         },
         scripts=[
             "gandlf_run",
@@ -114,14 +138,15 @@
             "gandlf_preprocess",
             "gandlf_anonymizer",
             "gandlf_verifyInstall",
             "gandlf_configGenerator",
             "gandlf_recoverConfig",
             "gandlf_deploy",
             "gandlf_optimizeModel",
+            "gandlf_generateMetrics",
         ],
         classifiers=[
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: Apache Software License",
             "Natural Language :: English",
             "Operating System :: OS Independent",
@@ -134,11 +159,11 @@
             "PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging."
         ),
         install_requires=requirements,
         license="Apache-2.0",
         long_description=readme,
         long_description_content_type="text/markdown",
         include_package_data=True,
-        package_data={'GANDLF': all_extra_files_pathcorrected},
+        package_data={"GANDLF": all_extra_files_pathcorrected},
         keywords="semantic, segmentation, regression, classification, data-augmentation, medical-imaging, clinical-workflows, deep-learning, pytorch",
         zip_safe=False,
     )
```

