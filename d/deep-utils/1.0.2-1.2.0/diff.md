# Comparing `tmp/deep_utils-1.0.2.tar.gz` & `tmp/deep_utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_utils-1.0.2.tar", last modified: Sat Apr  1 20:37:05 2023, max compression
+gzip compressed data, was "deep_utils-1.2.0.tar", last modified: Sat May 27 18:10:16 2023, max compression
```

## Comparing `deep_utils-1.0.2.tar` & `deep_utils-1.2.0.tar`

### file list

```diff
@@ -1,610 +1,655 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-01 20:36:54.000000 deep_utils-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23756 2023-04-01 20:37:05.547108 deep_utils-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.475107 deep_utils-1.0.2/deep_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/asr/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/asr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/asr/wav2vec2/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/asr/wav2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/asr/wav2vec2/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/asr/wav2vec2/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/asr/wav2vec2/torch/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/audio_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/audio_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/audio_utils/librosa_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/audio_utils/torchaudio_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/audio_utils/vox_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/classification/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/classification/wav2vec2/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/classification/wav2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/classification/wav2vec2/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/classification/wav2vec2/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/diarization/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/diarization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/diarization/pyannote/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/diarization/pyannote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/vad/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/vad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/audio/vad/pyannote/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/vad/pyannote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.479107 deep_utils-1.0.2/deep_utils/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/augmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.483107 deep_utils-1.0.2/deep_utils/augmentation/cutmix/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/augmentation/cutmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/augmentation/cutmix/cutmix_tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/augmentation/cutmix/cutmix_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.483107 deep_utils-1.0.2/deep_utils/augmentation/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/augmentation/torch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8071 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/augmentation/torch/augmentation_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.483107 deep_utils-1.0.2/deep_utils/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.483107 deep_utils-1.0.2/deep_utils/blocks/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/blocks/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/blocks/tf/blocks_tf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.483107 deep_utils-1.0.2/deep_utils/blocks/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/blocks/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/blocks/torch/blocks_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.483107 deep_utils-1.0.2/deep_utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.483107 deep_utils-1.0.2/deep_utils/callbacks/tf_keras/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/callbacks/tf_keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/callbacks/tf_keras/lr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.483107 deep_utils-1.0.2/deep_utils/callbacks/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/callbacks/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/callbacks/torch/torch_csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/callbacks/torch/torch_model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/callbacks/torch/torch_tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.483107 deep_utils-1.0.2/deep_utils/design_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/design_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.483107 deep_utils-1.0.2/deep_utils/design_patterns/chain_of_responsibility/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/design_patterns/chain_of_responsibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/audio/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/audio/asr/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/audio/asr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/audio/asr/wave2vec2/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/audio/asr/wave2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/audio/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/audio/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/audio/classification/wav2vec2/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/audio/classification/wav2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/audio/diarization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/audio/diarization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/audio/diarization/pyannote/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/audio/diarization/pyannote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/audio/utils_/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/audio/utils_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/audio/vad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/audio/vad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/audio/vad/pyannote/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/audio/vad/pyannote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/augmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/augmentation/cutmix/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/augmentation/cutmix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/blocks/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/blocks/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/callbacks/tf_keras/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/callbacks/tf_keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/cv2_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/dummy_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/dummy_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/dummy_framework/dummy_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/tf_cv2_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/torch_cv2_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/torch_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/torch_monai_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.487107 deep_utils-1.0.2/deep_utils/dummy_objects/utils/git_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/utils/git_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/utils/memory_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/utils/memory_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/utils/sqlalchemy_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/utils/sqlalchemy_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/utils/torch_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/utils/torch_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/vision/face_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/vision/face_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/vision/face_recognition/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/vision/face_recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/vision/object_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/vision/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/vision/object_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/vision/object_tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/vision/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/vision/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/vision/ocr/crnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/vision/ocr/crnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/vision/ocr/crnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/vision/ocr/crnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/vision/torch_vision/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/vision/torch_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/vision/vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/vision/vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/dummy_objects/vision/vision_utils/torch_vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/dummy_objects/vision/vision_utils/torch_vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.491107 deep_utils-1.0.2/deep_utils/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/elasticsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.495107 deep_utils-1.0.2/deep_utils/elasticsearch/search_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/elasticsearch/search_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.495107 deep_utils-1.0.2/deep_utils/gis/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/gis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.495107 deep_utils-1.0.2/deep_utils/gis/projection/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/gis/projection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/gis/projection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.495107 deep_utils-1.0.2/deep_utils/main_abs/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/main_abs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.495107 deep_utils-1.0.2/deep_utils/main_abs/cv2/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/main_abs/cv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/main_abs/cv2/cv2_caffe.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/main_abs/cv2/cv2_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/main_abs/cv2/cv2_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/main_abs/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/main_abs/main_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.495107 deep_utils-1.0.2/deep_utils/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.495107 deep_utils-1.0.2/deep_utils/nlp/ner/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/ner/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/ner/base_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/ner/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/ner/taggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/ner/utils_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.495107 deep_utils-1.0.2/deep_utils/nlp/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.495107 deep_utils-1.0.2/deep_utils/nlp/utils/multi_lang_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/utils/multi_lang_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/utils/multi_lang_utils/multi_lang_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.495107 deep_utils-1.0.2/deep_utils/nlp/utils/persian/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/utils/persian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/nlp/utils/persian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.495107 deep_utils-1.0.2/deep_utils/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.499107 deep_utils-1.0.2/deep_utils/preprocessing/monai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/preprocessing/monai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/preprocessing/monai/monai_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.499107 deep_utils-1.0.2/deep_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.499107 deep_utils-1.0.2/deep_utils/utils/algorithm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/algorithm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/algorithm_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.499107 deep_utils-1.0.2/deep_utils/utils/box_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/box_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34030 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/box_utils/boxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.499107 deep_utils-1.0.2/deep_utils/utils/coco_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/coco_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/coco_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.499107 deep_utils-1.0.2/deep_utils/utils/color_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/color_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/color_utils/color_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.499107 deep_utils-1.0.2/deep_utils/utils/compress_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/compress_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/compress_utils/zip_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.499107 deep_utils-1.0.2/deep_utils/utils/ctc_decoder/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/ctc_decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/ctc_decoder/ctc_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.499107 deep_utils-1.0.2/deep_utils/utils/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/decorators/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.499107 deep_utils-1.0.2/deep_utils/utils/dict_named_tuple_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/dict_named_tuple_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.499107 deep_utils-1.0.2/deep_utils/utils/dict_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/dict_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/dict_utils/dict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.503107 deep_utils-1.0.2/deep_utils/utils/dir_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/dir_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/dir_utils/dir_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.503107 deep_utils-1.0.2/deep_utils/utils/download_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/download_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/download_utils/download_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.503107 deep_utils-1.0.2/deep_utils/utils/encodes/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/encodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/encodes/b64.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/encodes/web_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.503107 deep_utils-1.0.2/deep_utils/utils/gif_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/gif_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/gif_utils/gif_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.503107 deep_utils-1.0.2/deep_utils/utils/hash_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/hash_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/hash_utils/hash_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.503107 deep_utils-1.0.2/deep_utils/utils/image_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/image_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/image_utils/image_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.503107 deep_utils-1.0.2/deep_utils/utils/json_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/json_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/json_utils/json_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.503107 deep_utils-1.0.2/deep_utils/utils/kafka_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/kafka_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/kafka_utils/kafka_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.503107 deep_utils-1.0.2/deep_utils/utils/lib_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/lib_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/lib_utils/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/lib_utils/lib_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/lib_utils/main_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.503107 deep_utils-1.0.2/deep_utils/utils/list_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/list_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/list_utils/list_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.503107 deep_utils-1.0.2/deep_utils/utils/logging_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/logging_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/logging_utils/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.507108 deep_utils-1.0.2/deep_utils/utils/lr_scheduler_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/lr_scheduler_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/lr_scheduler_utils/warmup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.507108 deep_utils-1.0.2/deep_utils/utils/matplotlib_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/matplotlib_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/matplotlib_utils/bar_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/matplotlib_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.507108 deep_utils-1.0.2/deep_utils/utils/memory_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/memory_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/memory_utils/torch_memory_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.507108 deep_utils-1.0.2/deep_utils/utils/minio_lib/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/minio_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/minio_lib/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.507108 deep_utils-1.0.2/deep_utils/utils/multi_label_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/multi_label_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.507108 deep_utils-1.0.2/deep_utils/utils/multi_label_utils/stratify/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/multi_label_utils/stratify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.507108 deep_utils-1.0.2/deep_utils/utils/np_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/np_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/np_utils/main_np.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.507108 deep_utils-1.0.2/deep_utils/utils/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/object_utils/object_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.507108 deep_utils-1.0.2/deep_utils/utils/opencv_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/opencv_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/opencv_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.507108 deep_utils-1.0.2/deep_utils/utils/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/optimizers/tf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.511108 deep_utils-1.0.2/deep_utils/utils/os_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/os_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/os_utils/os_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.511108 deep_utils-1.0.2/deep_utils/utils/pickle_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/pickle_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/pickle_utils/pickles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.511108 deep_utils-1.0.2/deep_utils/utils/postgresql_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/postgresql_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/postgresql_utils/postgresql_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.511108 deep_utils-1.0.2/deep_utils/utils/random_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/random_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/random_utils/random_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.511108 deep_utils-1.0.2/deep_utils/utils/re_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/re_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/re_utils/re_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.511108 deep_utils-1.0.2/deep_utils/utils/requests_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/requests_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/requests_utils/requests_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.511108 deep_utils-1.0.2/deep_utils/utils/resize_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/resize_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/resize_utils/main_resize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.511108 deep_utils-1.0.2/deep_utils/utils/shutil_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/shutil_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/shutil_utils/shutil_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.511108 deep_utils-1.0.2/deep_utils/utils/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/sqlalchemy/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/sqlalchemy/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.511108 deep_utils-1.0.2/deep_utils/utils/tensorboard_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/tensorboard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.515107 deep_utils-1.0.2/deep_utils/utils/tf_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/tf_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/tf_utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/tf_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.515107 deep_utils-1.0.2/deep_utils/utils/torch_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/torch_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/torch_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.515107 deep_utils-1.0.2/deep_utils/utils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/utils/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/utils/hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/utils/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/utils/shuffle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/utils/str_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/utils/yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.515107 deep_utils-1.0.2/deep_utils/utils/variable_naming_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/variable_naming_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/utils/variable_naming_utils/variable_naming_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.515107 deep_utils-1.0.2/deep_utils/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.515107 deep_utils-1.0.2/deep_utils/vision/face_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.515107 deep_utils-1.0.2/deep_utils/vision/face_detection/haarcascade/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/haarcascade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.515107 deep_utils-1.0.2/deep_utils/vision/face_detection/haarcascade/cv2_/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/haarcascade/cv2_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/haarcascade/cv2_/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.515107 deep_utils-1.0.2/deep_utils/vision/face_detection/main/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/main/main_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.515107 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.519108 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.519108 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.519108 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.519108 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.519108 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.519108 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.519108 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.519108 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.519108 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.523108 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.523108 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13383 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.523108 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.523108 deep_utils-1.0.2/deep_utils/vision/face_detection/ssd/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ssd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.523108 deep_utils-1.0.2/deep_utils/vision/face_detection/ssd/cv2/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ssd/cv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.523108 deep_utils-1.0.2/deep_utils/vision/face_detection/ssd/cv2/caffe/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ssd/cv2/caffe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.523108 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.523108 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.523108 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/utils/op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.523108 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.527108 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.527108 deep_utils-1.0.2/deep_utils/vision/face_recognition/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.527108 deep_utils-1.0.2/deep_utils/vision/face_recognition/main/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_recognition/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_recognition/main/main_face_recognition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.527108 deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.527108 deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/torch/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.527108 deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/torch/src/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/torch/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5859 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.531108 deep_utils-1.0.2/deep_utils/vision/object_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.531108 deep_utils-1.0.2/deep_utils/vision/object_detection/main/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/main/main_object_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.531108 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.531108 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.531108 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.531108 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42372 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4435 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    27031 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18183 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.535108 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    55706 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    48196 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    46792 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    24456 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.535108 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.535108 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.535108 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.535108 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/models/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84416 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    40059 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.539108 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)    56265 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    36907 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    75043 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    20998 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18114 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/yolo_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.539108 deep_utils-1.0.2/deep_utils/vision/object_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.539108 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.539108 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.539108 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/deep/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.539108 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/deep_utils/vision/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/deep_utils/vision/ocr/crnn/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/ocr/crnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/deep_utils/vision/ocr/crnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/ocr/crnn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/ocr/crnn/torch/crnn_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/ocr/crnn/torch/crnn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/deep_utils/vision/torch_vision/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/torch_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/deep_utils/vision/torch_vision/torch_vision_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/torch_vision/torch_vision_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/deep_utils/vision/torch_vision/torch_vision_models/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/torch_vision/torch_vision_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/deep_utils/vision/vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/deep_utils/vision/vision_utils/torch_vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/vision_utils/torch_vision_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-01 20:36:54.000000 deep_utils-1.0.2/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.475107 deep_utils-1.0.2/deep_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23756 2023-04-01 20:37:05.000000 deep_utils-1.0.2/deep_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22018 2023-04-01 20:37:05.000000 deep_utils-1.0.2/deep_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 20:37:05.000000 deep_utils-1.0.2/deep_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-01 20:37:05.000000 deep_utils-1.0.2/deep_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-01 20:37:05.000000 deep_utils-1.0.2/deep_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-01 20:37:05.551108 deep_utils-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-01 20:36:54.000000 deep_utils-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.543108 deep_utils-1.0.2/tests/utils/encoding_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/utils/encoding_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/utils/encoding_utils/encoding_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/utils/np_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/utils/np_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/utils/np_utils/np_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/utils/resize_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/utils/resize_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/utils/resize_utils/resize_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/utils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/utils/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/face_detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/face_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/face_detection/mtcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/face_detection/mtcnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/face_detection/mtcnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/face_detection/mtcnn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/face_detection/ultralight/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/face_detection/ultralight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/face_detection/ultralight/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/face_detection/ultralight/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/object_detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/object_detection/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/object_detection/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/object_detection/yolo/v5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/object_detection/yolo/v5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/object_detection/yolo/v5/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/object_detection/yolo/v5/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 20:37:05.547108 deep_utils-1.0.2/tests/vision/vision_utils/torch_vision_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/vision_utils/torch_vision_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-01 20:36:54.000000 deep_utils-1.0.2/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.716773 deep_utils-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-27 18:10:04.000000 deep_utils-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-05-27 18:10:16.716773 deep_utils-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.652773 deep_utils-1.2.0/deep_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/asr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/asr/wave2vec2/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/asr/wave2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/classification/wav2vec2/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/classification/wav2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/diarization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/diarization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/diarization/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/diarization/pyannote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/utils_/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/utils_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/vad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/vad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/vad/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/audio/vad/pyannote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/augmentation/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/augmentation/cutmix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/blocks/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/blocks/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/callbacks/tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/callbacks/tf_keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/cv2_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/dummy_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/dummy_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/dummy_framework/dummy_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/glide_text2im_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/groundingdino_torch_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/requests_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/tf_cv2_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/tf_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/torch_cv2_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/torch_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/torch_monai_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/torchvision_torch_timm_transformers_fairscale_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/utils/git_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/utils/git_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/utils/memory_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/utils/memory_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/utils/sqlalchemy_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/utils/sqlalchemy_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/utils/torch_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/utils/torch_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.656773 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/face_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/face_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/face_recognition/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/face_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/object_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/object_tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/ocr/crnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/ocr/crnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/ocr/crnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/ocr/crnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/torch_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/torch_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/vision_utils/torch_vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/_dummy_objects/vision/vision_utils/torch_vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/asr/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/asr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/asr/wav2vec2/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/asr/wav2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/asr/wav2vec2/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/asr/wav2vec2/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/asr/wav2vec2/torch/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/audio_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/audio_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/audio_utils/librosa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/audio_utils/torchaudio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/audio_utils/vox_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/classification/wav2vec2/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/classification/wav2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/classification/wav2vec2/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/classification/wav2vec2/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/diarization/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/diarization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/diarization/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/diarization/pyannote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/vad/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/vad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.660773 deep_utils-1.2.0/deep_utils/audio/vad/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/vad/pyannote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/augmentation/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/augmentation/cutmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/augmentation/cutmix/cutmix_tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/augmentation/cutmix/cutmix_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/augmentation/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/augmentation/torch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8071 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/augmentation/torch/augmentation_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/blocks/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/blocks/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/blocks/tf/blocks_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/blocks/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/blocks/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/blocks/torch/blocks_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/callbacks/tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/callbacks/tf_keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/callbacks/tf_keras/lr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/callbacks/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/callbacks/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/callbacks/torch/torch_csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/callbacks/torch/torch_model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/callbacks/torch/torch_tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/design_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/design_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/design_patterns/chain_of_responsibility/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/design_patterns/chain_of_responsibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/elasticsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/elasticsearch/search_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/elasticsearch/search_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/gis/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/gis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.664773 deep_utils-1.2.0/deep_utils/gis/projection/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/gis/projection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/gis/projection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/main_abs/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/main_abs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/main_abs/cv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/main_abs/cv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/main_abs/cv2/cv2_caffe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/main_abs/cv2/cv2_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/main_abs/cv2/cv2_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/main_abs/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/main_abs/main_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/multi_modals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/multi_modals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/multi_modals/_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/multi_modals/_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/multi_modals/_models/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/multi_modals/_models/blip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/multi_modals/_models/blip/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/multi_modals/_models/blip/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/multi_modals/_models/blip/torch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/multi_modals/_models/blip/torch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/multi_modals/_models/blip/torch/models/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41523 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/multi_modals/_models/blip/torch/models/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/multi_modals/_models/blip/torch/models/med_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/multi_modals/_models/blip/torch/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/nlp/ner/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/ner/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/ner/base_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/ner/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/ner/taggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/ner/utils_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/nlp/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/nlp/utils/multi_lang_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/utils/multi_lang_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/utils/multi_lang_utils/multi_lang_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/nlp/utils/persian/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/utils/persian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/nlp/utils/persian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.668773 deep_utils-1.2.0/deep_utils/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/preprocessing/monai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/preprocessing/monai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/preprocessing/monai/monai_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/algorithm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/algorithm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/algorithm_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/box_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/box_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/box_utils/box_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36114 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/box_utils/boxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/coco_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/coco_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/coco_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/color_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/color_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/color_utils/color_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/compress_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/compress_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/compress_utils/zip_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/ctc_decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/ctc_decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/ctc_decoder/ctc_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/decorators/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/dict_named_tuple_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/dict_named_tuple_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/dict_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/dict_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/dict_utils/dict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/dir_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/dir_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/dir_utils/dir_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.672773 deep_utils-1.2.0/deep_utils/utils/download_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/download_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/download_utils/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/encodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/encodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/encodes/b64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/encodes/web_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/gif_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/gif_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/gif_utils/gif_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/hash_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/hash_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/hash_utils/hash_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/image_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/image_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/image_utils/image_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/json_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/json_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/json_utils/json_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/kafka_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/kafka_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/kafka_utils/kafka_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/lib_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/lib_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/lib_utils/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/lib_utils/lib_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/lib_utils/main_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/list_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/list_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/list_utils/list_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/logging_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/logging_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/logging_utils/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/lr_scheduler_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/lr_scheduler_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/lr_scheduler_utils/warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/matplotlib_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/matplotlib_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/matplotlib_utils/bar_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/matplotlib_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/memory_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/memory_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/memory_utils/torch_memory_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.676773 deep_utils-1.2.0/deep_utils/utils/minio_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/minio_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/minio_lib/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/multi_label_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/multi_label_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/multi_label_utils/stratify/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/multi_label_utils/stratify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/np_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/np_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/np_utils/main_np.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/object_utils/object_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/opencv_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/opencv_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/opencv_utils/opencv_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/optimizers/tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/os_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/os_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/os_utils/os_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/pickle_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/pickle_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/pickle_utils/pickle_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/postgresql_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/postgresql_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/postgresql_utils/postgresql_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/random_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/random_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/random_utils/random_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/re_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/re_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/re_utils/re_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/requests_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/requests_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/requests_utils/requests_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/resize_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/resize_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/resize_utils/main_resize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.680773 deep_utils-1.2.0/deep_utils/utils/shutil_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/shutil_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/shutil_utils/shutil_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/utils/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/sqlalchemy/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/sqlalchemy/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/utils/tensorboard_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/tensorboard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/utils/tf_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/tf_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/tf_utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/tf_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/utils/torch_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/torch_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/torch_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/utils/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/utils/hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/utils/shuffle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/utils/str_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/utils/yaml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/utils/variable_naming_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/variable_naming_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/utils/variable_naming_utils/variable_naming_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/vision/color_recognition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/color_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/vision/color_recognition/cnn_color/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/color_recognition/cnn_color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/vision/color_recognition/cnn_color/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/color_recognition/cnn_color/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch_pred.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/vision/face_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/vision/face_detection/haarcascade/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/haarcascade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.684773 deep_utils-1.2.0/deep_utils/vision/face_detection/haarcascade/cv2_/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/haarcascade/cv2_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/haarcascade/cv2_/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.688773 deep_utils-1.2.0/deep_utils/vision/face_detection/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/main/main_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.688773 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.688773 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.688773 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.688773 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.688773 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.688773 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.688773 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.688773 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.688773 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.688773 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.692773 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.692773 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13383 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.692773 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.692773 deep_utils-1.2.0/deep_utils/vision/face_detection/ssd/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ssd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.692773 deep_utils-1.2.0/deep_utils/vision/face_detection/ssd/cv2/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ssd/cv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.692773 deep_utils-1.2.0/deep_utils/vision/face_detection/ssd/cv2/caffe/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ssd/cv2/caffe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.692773 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.692773 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.692773 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/utils/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.692773 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/face_recognition/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/face_recognition/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_recognition/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_recognition/main/main_face_recognition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/torch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/torch/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/torch/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5859 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/image_caption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/image_caption/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/image_caption/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/image_caption/blip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/image_caption/blip/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/image_caption/blip/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/image_caption/blip/torch/blip_torch_image_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/image_caption/image_caption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/image_editing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/image_editing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/image_editing/glide/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/image_editing/glide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/image_editing/glide/glide_image_editing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.696773 deep_utils-1.2.0/deep_utils/vision/object_detection/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/main/main_object_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.700773 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.700773 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.700773 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.700773 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42372 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4435 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27031 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18183 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.704773 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55706 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48196 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46792 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24456 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.704773 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.704773 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.704773 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.704773 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84416 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40059 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.708773 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56265 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36907 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75043 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20998 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/yolo_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.708773 deep_utils-1.2.0/deep_utils/vision/object_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.708773 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.708773 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.708773 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.708773 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.708773 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/deep_utils/vision/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/deep_utils/vision/ocr/crnn/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/ocr/crnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/deep_utils/vision/ocr/crnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/ocr/crnn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/ocr/crnn/torch/crnn_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/ocr/crnn/torch/crnn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/deep_utils/vision/text2box_visual_grounding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/text2box_visual_grounding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/deep_utils/vision/text2box_visual_grounding/dino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/text2box_visual_grounding/dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/text2box_visual_grounding/dino/visual_grounding_dino_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/deep_utils/vision/torch_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/torch_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/deep_utils/vision/torch_vision/torch_vision_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/torch_vision/torch_vision_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/deep_utils/vision/torch_vision/torch_vision_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/torch_vision/torch_vision_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/deep_utils/vision/vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/deep_utils/vision/vision_utils/torch_vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/vision_utils/torch_vision_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-27 18:10:04.000000 deep_utils-1.2.0/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.652773 deep_utils-1.2.0/deep_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-05-27 18:10:16.000000 deep_utils-1.2.0/deep_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-05-27 18:10:16.000000 deep_utils-1.2.0/deep_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 18:10:16.000000 deep_utils-1.2.0/deep_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-27 18:10:16.000000 deep_utils-1.2.0/deep_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-27 18:10:16.000000 deep_utils-1.2.0/deep_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 18:10:16.716773 deep_utils-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-27 18:10:04.000000 deep_utils-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/tests/utils/encoding_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/utils/encoding_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/utils/encoding_utils/encoding_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/tests/utils/np_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/utils/np_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/utils/np_utils/np_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/tests/utils/resize_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/utils/resize_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/utils/resize_utils/resize_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/tests/utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/utils/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/tests/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/tests/vision/face_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/face_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/tests/vision/face_detection/mtcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/face_detection/mtcnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.712773 deep_utils-1.2.0/tests/vision/face_detection/mtcnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/face_detection/mtcnn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.716773 deep_utils-1.2.0/tests/vision/face_detection/ultralight/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/face_detection/ultralight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.716773 deep_utils-1.2.0/tests/vision/face_detection/ultralight/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/face_detection/ultralight/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.716773 deep_utils-1.2.0/tests/vision/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.716773 deep_utils-1.2.0/tests/vision/object_detection/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/object_detection/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.716773 deep_utils-1.2.0/tests/vision/object_detection/yolo/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/object_detection/yolo/v5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.716773 deep_utils-1.2.0/tests/vision/object_detection/yolo/v5/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/object_detection/yolo/v5/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.716773 deep_utils-1.2.0/tests/vision/vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:16.716773 deep_utils-1.2.0/tests/vision/vision_utils/torch_vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/vision_utils/torch_vision_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-27 18:10:04.000000 deep_utils-1.2.0/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py
```

### Comparing `deep_utils-1.0.2/LICENSE` & `deep_utils-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/PKG-INFO` & `deep_utils-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: deep_utils
-Version: 1.0.2
+Version: 1.2.0
 Summary: Deep Utils
 Home-page: https://github.com/pooya-mohammadi/deep_utils
 Author: Pooya Mohammadi Kazaj
 Author-email: pooyamohammadikazaj@gmial.com
 License: UNKNOWN
-Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.0.2.tar.gz
-Description: [![Downloads](https://static.pepy.tech/badge/deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils) [![build](https://github.com/pooya-mohammadi/deep_utils/actions/workflows/ci-tests.yml/badge.svg)](https://github.com/pooya-mohammadi/deep_utils/actions/workflows/ci-tests.yml)
+Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.2.0.tar.gz
+Description: [![Downloads](https://static.pepy.tech/badge/deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
         
         <div id="top"></div>
         <!-- PROJECT LOGO -->
         <br />
         <div align="center">
           <a href="https://github.com/pooya-mohammadi/deep_utils">
             <img src="https://raw.githubusercontent.com/pooya-mohammadi/deep_utils/master/images/logo/deep_utils.png" alt="Logo">
@@ -33,14 +33,18 @@
         * [About The Project](#about-the-project)
         * [Installation](#installation)
         * [Vision](#vision)
             * [Face Detection](#face-detection)
                 * [MTCNN](#mtcnn)
             * [Object Detection](#object-detection)
                 * [yolov5](#yolov5)
+            * [Visual Grounding](#visual-grounding)
+                * [Grounding DINO](#grounding-dino)
+            * [Image Editing](#image-editing)
+                * [GLIDE](#glide)
         * [NLP](#NLP)
             * [NER](#NER)
                 * [Replacement Augmentation](replacement-augmentation)
                 * [Remove Augmentation](remove-augmentation)
         * [Augmentation](#augmentation)
             * [CutMix](#cutmix)
         * [Utils](#utils)
@@ -232,40 +236,109 @@
         # visualize using oepncv
         # show_destroy_cv2(img)
         ```
         
         <img src="https://raw.githubusercontent.com/pooya-mohammadi/deep-utils-notebooks/main/vision/images/dog_yolov5.jpg" alt="Logo" >
         <p align="right">(<a href="#top">back to top</a>)</p>
         
+        ## Visual Grounding
+        
+        ### Grounding DINO
+        
+        DINO is a self-supervised learning method for visual grounding. It is a simple and efficient method that can be used for
+        visual grounding. Let's see how we can use it in `deep_utils`:
+        
+        #### Download a sample image
+        
+        ```commandline
+        wget -q https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/golsa_in_garden.jpg
+        ```
+        
+        ```python
+        from PIL import Image
+        from deep_utils import Text2BoxVisualGroundingDino
+        import numpy as np
+        import matplotlib.pyplot as plt
+        
+        model = Text2BoxVisualGroundingDino()
+        
+        img_path = "golsa_in_garden.jpg"
+        img = np.asarray(Image.open(img_path))
+        
+        output = model.text_to_box(text="Hen", img=img)
+        print(output.boxes, output.scores, output.labels)
+        annotated_img = model.annotate(img, output)
+        plt.axis("off")
+        plt.imshow(annotated_img)
+        ```
+        
+        Output Image:<br/>
+        <img src="https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/golsa_in_garden_dino.png" width="400">
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
+        ## Image Editing
+        
+        ### GLIDE
+        
+        GLIDE is a simple and efficient method for image editing/inpainting. It is developed by OpenAI.
+        
+        #### Download a sample image
+        
+        ```commandline
+        wget -q https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/golsa_in_garden.jpg
+        ```
+        
+        **Input Image**:<br/>
+        <img src="https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/golsa_in_garden.jpg" width="400">
+        
+        ```python
+        import matplotlib.pyplot as plt
+        from deep_utils import ImageEditingGLIDE
+        from PIL import Image
+        
+        pil_img = Image.open("golsa_in_garden.jpg")
+        # position of the editing box. Here the hen in the image. The  
+        box = [340.6672668457031, 403.7683410644531, 372.0812072753906, 439.3288879394531]
+        glide_model = ImageEditingGLIDE()
+        text = "dead leaves"
+        edited_image = glide_model.edit_box(pil_img, text=text, box=box)
+        plt.imshow(edited_image)
+        ```
+        
+        **Output Image**: The `hen` is removed and replaced with `dead leaves` as the background<br/>
+        <img src="https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/glide_output.jpg" width="400">
+        
+        **Note:** The best way to get the box is to use the `Text2BoxVisualGroundingDino` model. See the example in the previous
+        section.
+        
         ## NLP
         
         In this section, models and utilities for nlp projects are provided
         
         ### NER
         
         Name Entity Recognition
         
         #### multi-label-stratify
         
         ## Augmentation
         
         ### CutMix
         
-        <a href="https://colab.research.google.com/github/pooya-mohammadi/deep-utils-notebooks/blob/main/augmentation/cutmix/cutmix_tf.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+        <a href="https://colab.research.google.com/github/pooya-mohammadi/deep-utils-notebooks/blob/main/augmentation/cutmix/cutmix_tf.ipynb" target="_parent"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" /> </a> 
         
         CutMix is one of the best augmentation methods that's proven to be very effective in different vision-based project.
-        Therefore, CutMix is now available on `deep_utils` to be used both for segmentation and classification tasks. Let some
-        examples:
+        Therefore, CutMix is now
+        available on `deep_utils` to be used both for segmentation and classification tasks.Let some examples:
         
         #### Segmentation
         
         ```python
         import cv2
         import numpy as np
-        from PIL import Image
         from deep_utils import CutMixTF, group_show, repeat_dimension
         
         # creating random images, the code for this section can be found in the colab notebook
         image_a = np.zeros((300, 300, 3), np.uint8) * 255
         mask_a = np.zeros_like(image_a)
         pt1 = (150, 100)
         pt2 = (100, 200)
@@ -356,17 +429,19 @@
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ### Multi-Label-Stratify
         
         While splitting a dataset for NER or Object detection tasks, you might have noticed that there is no way to split the
         dataset using
-        stratify functionality of `train_test_split` of the `scikit-learn` library because not only does each sample in these two tasks may
+        stratify functionality of `train_test_split` of the `scikit-learn` library because not only does each sample in these
+        two tasks may
         have
-        more than one tag/object, but also each tag/object of each class may appear more than once. For example, an image/sample may
+        more than one tag/object, but also each tag/object of each class may appear more than once. For example, an image/sample
+        may
         contain two dogs and three cats, which means the label/y of that sample would be like [2, 3] in which the index zero
         corresponds
         to the dog class, and the index one corresponds to the cat class.
         To split these types of datasets, the following function is
         developed in the `deep_utils` library which is very easy to use. To use this function, two arrays are needed. The first
         is an array
         or list containing the input samples. The type of these samples could be anything; they could be a list of sentences, a
@@ -446,14 +521,15 @@
         
         
         <!-- LICENSE -->
         
         ## 🌟 Spread the word!
         
         If you want to say thank you and/or support active development of the repo:
+        
         - Add a GitHub Star to the project!
         - Join our discord servers [Deep Utils](https://discord.gg/pWe3yChw) .
         - Follow my profile [pooya-mohammadi](https://github.com/pooya-mohammadi)
         
         Thanks so much for your interest in growing the reach of the repo!
         <p align="right">(<a href="#top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,33 +1,32 @@
-Metadata-Version: 2.1 Name: deep_utils Version: 1.0.2 Summary: Deep Utils Home-
+Metadata-Version: 2.1 Name: deep_utils Version: 1.2.0 Summary: Deep Utils Home-
 page: https://github.com/pooya-mohammadi/deep_utils Author: Pooya Mohammadi
 Kazaj Author-email: pooyamohammadikazaj@gmial.com License: UNKNOWN Download-
 URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/
-1.0.2.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
+1.2.0.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
 deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://
 img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
-[![build](https://github.com/pooya-mohammadi/deep_utils/actions/workflows/ci-
-tests.yml/badge.svg)](https://github.com/pooya-mohammadi/deep_utils/actions/
-workflows/ci-tests.yml)
 
                                     [Logo]
                              **** Deep Utils ****
                   A toolkit for deep-learning practitioners!
 This repository contains the most frequently used deep learning models and
 functions. **Deep_Utils** is still under heavy development, so take into
 consideration that many features may change in the future and make sure to
 install the latest version using pypi. ## Table of contents * [About The
 Project](#about-the-project) * [Installation](#installation) * [Vision]
 (#vision) * [Face Detection](#face-detection) * [MTCNN](#mtcnn) * [Object
-Detection](#object-detection) * [yolov5](#yolov5) * [NLP](#NLP) * [NER](#NER) *
-[Replacement Augmentation](replacement-augmentation) * [Remove Augmentation]
-(remove-augmentation) * [Augmentation](#augmentation) * [CutMix](#cutmix) *
-[Utils](#utils) * [DictNamedTuple](#dictnametuple) * [multi-label-stratify]
-(#multi-label-stratify) * [Tests](#tests) * [Contributing](#Contributing) *
-[Licence](#Licence) * [Collaborators](#Collaborators) * [Contact](#Contact) *
+Detection](#object-detection) * [yolov5](#yolov5) * [Visual Grounding](#visual-
+grounding) * [Grounding DINO](#grounding-dino) * [Image Editing](#image-
+editing) * [GLIDE](#glide) * [NLP](#NLP) * [NER](#NER) * [Replacement
+Augmentation](replacement-augmentation) * [Remove Augmentation](remove-
+augmentation) * [Augmentation](#augmentation) * [CutMix](#cutmix) * [Utils]
+(#utils) * [DictNamedTuple](#dictnametuple) * [multi-label-stratify](#multi-
+label-stratify) * [Tests](#tests) * [Contributing](#Contributing) * [Licence]
+(#Licence) * [Collaborators](#Collaborators) * [Contact](#Contact) *
 [References](#references) * [Citation](#citation)
                                                                   (back_to_top)
 ## About the Project Many deep learning toolkits are available on GitHub;
 however, we couldn't find one that would suit our needs. So, we created this
 improved one. This toolkit minimizes the deep learning teams' coding efforts to
 utilize the functionalities of famous deep learning models such as MTCNN in
 face detection, yolov5 in object detection, and many other repositories and
@@ -95,33 +94,62 @@
 `False` result = yolov5.detect_objects(base_image, is_rgb=False,
 confidence=0.5) # Draw detected boxes on the image. img = Box.put_box_text
 (base_image, box=result.boxes, label=[f"{c_n} {c}" for c_n, c in zip
 (result.class_names, result.confidences)]) # pil.Image is used for
 visualization Image.fromarray(img[..., ::-1]) # convert to rgb # visualize
 using oepncv # show_destroy_cv2(img) ``` [Logo]
                                                                   (back_to_top)
+## Visual Grounding ### Grounding DINO DINO is a self-supervised learning
+method for visual grounding. It is a simple and efficient method that can be
+used for visual grounding. Let's see how we can use it in `deep_utils`: ####
+Download a sample image ```commandline wget -q https://github.com/pooya-
+mohammadi/deep_utils/releases/download/1.0.2/golsa_in_garden.jpg ``` ```python
+from PIL import Image from deep_utils import Text2BoxVisualGroundingDino import
+numpy as np import matplotlib.pyplot as plt model = Text2BoxVisualGroundingDino
+() img_path = "golsa_in_garden.jpg" img = np.asarray(Image.open(img_path))
+output = model.text_to_box(text="Hen", img=img) print(output.boxes,
+output.scores, output.labels) annotated_img = model.annotate(img, output)
+plt.axis("off") plt.imshow(annotated_img) ``` Output Image:
+[https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/
+golsa_in_garden_dino.png]
+                                                                  (back_to_top)
+## Image Editing ### GLIDE GLIDE is a simple and efficient method for image
+editing/inpainting. It is developed by OpenAI. #### Download a sample image
+```commandline wget -q https://github.com/pooya-mohammadi/deep_utils/releases/
+download/1.0.2/golsa_in_garden.jpg ``` **Input Image**:
+[https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/
+golsa_in_garden.jpg] ```python import matplotlib.pyplot as plt from deep_utils
+import ImageEditingGLIDE from PIL import Image pil_img = Image.open
+("golsa_in_garden.jpg") # position of the editing box. Here the hen in the
+image. The box = [340.6672668457031, 403.7683410644531, 372.0812072753906,
+439.3288879394531] glide_model = ImageEditingGLIDE() text = "dead leaves"
+edited_image = glide_model.edit_box(pil_img, text=text, box=box) plt.imshow
+(edited_image) ``` **Output Image**: The `hen` is removed and replaced with
+`dead leaves` as the background
+[https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/
+glide_output.jpg] **Note:** The best way to get the box is to use the
+`Text2BoxVisualGroundingDino` model. See the example in the previous section.
 ## NLP In this section, models and utilities for nlp projects are provided ###
 NER Name Entity Recognition #### multi-label-stratify ## Augmentation ###
 CutMix [Open_In_Colab] CutMix is one of the best augmentation methods that's
 proven to be very effective in different vision-based project. Therefore,
 CutMix is now available on `deep_utils` to be used both for segmentation and
-classification tasks. Let some examples: #### Segmentation ```python import cv2
-import numpy as np from PIL import Image from deep_utils import CutMixTF,
-group_show, repeat_dimension # creating random images, the code for this
-section can be found in the colab notebook image_a = np.zeros((300, 300, 3),
-np.uint8) * 255 mask_a = np.zeros_like(image_a) pt1 = (150, 100) pt2 = (100,
-200) pt3 = (200, 200) triangle_cnt = np.array([pt1, pt2, pt3]) image_a =
-cv2.drawContours(image_a, [triangle_cnt], 0, (0, 255, 0), -1) mask_a =
-cv2.drawContours(mask_a, [triangle_cnt], 0, (255, 255, 255), -1) image_b =
-np.zeros((300, 300, 3), np.uint8) * 255 mask_b = np.zeros_like(image_b) pt1 =
-(150, 150) image_b = cv2.circle(image_b, pt1, 50, (0, 255, 0), -1) mask_b =
-cv2.circle(mask_b, pt1, 50, (255, 255, 255), -1) # CutMix for two individual
-images: cutmix_img, cutmix_mask = CutMixTF.seg_cutmix(image_a, mask_a[..., 0],
-image_b, mask_b[..., 0], beta=1) ``` The input and output are as follows:
-**Input:** [Logo]
+classification tasks.Let some examples: #### Segmentation ```python import cv2
+import numpy as np from deep_utils import CutMixTF, group_show,
+repeat_dimension # creating random images, the code for this section can be
+found in the colab notebook image_a = np.zeros((300, 300, 3), np.uint8) * 255
+mask_a = np.zeros_like(image_a) pt1 = (150, 100) pt2 = (100, 200) pt3 = (200,
+200) triangle_cnt = np.array([pt1, pt2, pt3]) image_a = cv2.drawContours
+(image_a, [triangle_cnt], 0, (0, 255, 0), -1) mask_a = cv2.drawContours(mask_a,
+[triangle_cnt], 0, (255, 255, 255), -1) image_b = np.zeros((300, 300, 3),
+np.uint8) * 255 mask_b = np.zeros_like(image_b) pt1 = (150, 150) image_b =
+cv2.circle(image_b, pt1, 50, (0, 255, 0), -1) mask_b = cv2.circle(mask_b, pt1,
+50, (255, 255, 255), -1) # CutMix for two individual images: cutmix_img,
+cutmix_mask = CutMixTF.seg_cutmix(image_a, mask_a[..., 0], image_b, mask_b[...,
+0], beta=1) ``` The input and output are as follows: **Input:** [Logo]
 **Output:** [Logo] As it illustrated in the above image a section of the
 triangle and the circle are combined together. By changing `seg_cutmix` to
 `seg_cutmix_batch` one can use CutMix augmentation for batch of images.
 ```python cutmix_img, cutmix_mask = CutMixTF.seg_cutmix_batch
 (a_images=batch_img, a_masks=batch_mask[..., 0], beta=1) ``` **Input:**
 [cutmix]
 **Output:** [cutmix]
```

### Comparing `deep_utils-1.0.2/deep_utils/audio/asr/wav2vec2/torch/main.py` & `deep_utils-1.2.0/deep_utils/audio/asr/wav2vec2/torch/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/audio/audio_utils/librosa_utils.py` & `deep_utils-1.2.0/deep_utils/audio/audio_utils/librosa_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/audio/audio_utils/torchaudio_utils.py` & `deep_utils-1.2.0/deep_utils/audio/audio_utils/torchaudio_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/audio/audio_utils/vox_utils.py` & `deep_utils-1.2.0/deep_utils/audio/audio_utils/vox_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py` & `deep_utils-1.2.0/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from transformers import AutoFeatureExtractor, AutoModelForAudioClassification
 from typing import Union
 from pathlib import Path
 import torch
 import torchaudio
 import librosa
 import numpy as np
-from deep_utils.utils.pickle_utils.pickles import load_pickle
+from deep_utils.utils.pickle_utils.pickle_utils import load_pickle
 from deep_utils.utils.logging_utils.logging_utils import log_print
 from deep_utils.audio.audio_utils.torchaudio_utils import TorchAudioUtils
 
 
 class AudioClassificationWav2vec2Torch:
     def __init__(self, model_path, num_labels, device="cpu", sr=16_000, label2id="label2id.pkl",
                  feature_extractor="facebook/wav2vec2-base", logger=None, verbose=1):
```

### Comparing `deep_utils-1.0.2/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py` & `deep_utils-1.2.0/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py` & `deep_utils-1.2.0/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/augmentation/cutmix/cutmix_tf.py` & `deep_utils-1.2.0/deep_utils/augmentation/cutmix/cutmix_tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/augmentation/cutmix/cutmix_torch.py` & `deep_utils-1.2.0/deep_utils/augmentation/cutmix/cutmix_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/augmentation/torch/augmentation_torch.py` & `deep_utils-1.2.0/deep_utils/augmentation/torch/augmentation_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/blocks/tf/blocks_tf.py` & `deep_utils-1.2.0/deep_utils/blocks/tf/blocks_tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/blocks/torch/blocks_torch.py` & `deep_utils-1.2.0/deep_utils/blocks/torch/blocks_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/callbacks/tf_keras/lr.py` & `deep_utils-1.2.0/deep_utils/callbacks/tf_keras/lr.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/callbacks/torch/torch_csv_logger.py` & `deep_utils-1.2.0/deep_utils/callbacks/torch/torch_csv_logger.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/callbacks/torch/torch_model_checkpoint.py` & `deep_utils-1.2.0/deep_utils/callbacks/torch/torch_model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/callbacks/torch/torch_tensorboard.py` & `deep_utils-1.2.0/deep_utils/callbacks/torch/torch_tensorboard.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py` & `deep_utils-1.2.0/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/dummy_objects/dummy_framework/dummy_framework.py` & `deep_utils-1.2.0/deep_utils/_dummy_objects/dummy_framework/dummy_framework.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,39 @@
 _is_torch_available = importlib.util.find_spec("torch") is not None
 _is_cv2_available = importlib.util.find_spec("cv2") is not None
 _is_torchvision_available = importlib.util.find_spec("torchvision") is not None
 _is_torchaudio_available = importlib.util.find_spec("torchaudio") is not None
 _is_pyannote_audio_available = importlib.util.find_spec("pyannote") is not None
 _is_transformers_available = importlib.util.find_spec("transformers") is not None
 _is_monai_available = importlib.util.find_spec("monai") is not None
+_is_timm_available = importlib.util.find_spec("timm") is not None
+_is_glide_text2im_available = importlib.util.find_spec("glide_text2im") is not None
+_is_groundingdino_available = importlib.util.find_spec("groundingdino") is not None
+_is_pillow_available = importlib.util.find_spec("PIL") is not None
+_is_requests_available = importlib.util.find_spec("requests") is not None
+
+
+def is_requests_available():
+    return _is_requests_available
+
+
+def is_pillow_available():
+    return _is_pillow_available
+
+
+def is_groundingdino_available():
+    return _is_groundingdino_available
+
+
+def is_glide_text2im_available():
+    return _is_glide_text2im_available
+
+
+def is_timm_available():
+    return _is_timm_available
 
 
 def is_monai_available():
     return _is_monai_available
 
 
 def is_transformers_available():
@@ -155,44 +180,56 @@
 ```
 In a notebook or a colab, you can install it by executing a cell with
 ```
 !pip install pyannote.audio
 ```
 """
 
-BACKENDS_MAPPING = OrderedDict(
+
+class BackendMapping(OrderedDict):
+    def __getitem__(self, item):
+        try:
+            return super().__getitem__(item)
+        except KeyError:
+            raise KeyError(f"Library {item} is not available in BACKENDS_MAPPING. Contact the Library Maintainers.")
+
+
+BACKENDS_MAPPING = BackendMapping(
     [
         ("cv2", (is_cv2_available, CV2_IMPORT_ERROR)),
         ("tf", (is_tf_available, TENSORFLOW_IMPORT_ERROR)),
         ("torch", (is_torch_available, PYTORCH_IMPORT_ERROR)),
         ("torchvision", (is_torchvision_available, TORCHVISION_IMPORT_ERROR)),
         ("torchaudio", (is_torchaudio_available, TORCHAUDIO_IMPORT_ERROR)),
         is_available("seaborn"),
         is_available("numpy"),
         is_available("albumentations"),
         is_available("sklearn"),
-        is_available("PIL"),
+        is_available("PIL", "Pillow"),
         is_available("pyannote"),
         is_available("librosa"),
         is_available("transformers"),
         is_available("soundfile"),
         is_available("psutil"),
         is_available("yaml", "pyyaml"),
         is_available("ipython", "IPython"),
-        is_available("monai")
+        is_available("monai"),
+        is_available("glide_text2im"),
+        is_available("groundingdino"),
+        is_available("requests"),
     ]
 )
 
 
 def requires_backends(obj, backends, module_name: str = None, cls_name: str = None):
     if not isinstance(backends, (list, tuple)):
         backends = [backends]
 
     name = obj.__name__ if hasattr(obj, "__name__") else obj.__class__.__name__
-    checks = (BACKENDS_MAPPING[backend] for backend in backends)
+    checks = (BACKENDS_MAPPING[backend[0] if isinstance(backend, tuple) else backend] for backend in backends)
     failed = [msg.format(name) for available, msg in checks if not available()]
     if failed:
         color_str("".join(failed), color="red", mode=["bold", "underline"])
         print("".join(failed))
     else:
         assert isinstance(module_name, str), f"module_name is not defined for obj: {name}"
         error = import_module(module_name, cls_name)
```

### Comparing `deep_utils-1.0.2/deep_utils/dummy_objects/torch_dummy.py` & `deep_utils-1.2.0/deep_utils/_dummy_objects/vision/object_detection/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from deep_utils.dummy_objects.dummy_framework import DummyObject, requires_backends
+from deep_utils._dummy_objects.dummy_framework import DummyObject, requires_backends
 
 
-class TensorboardTorch(metaclass=DummyObject):
-    _backend = ["torch"]
-    _module = "deep_utils.callbacks.torch.torch_tensorboard"
+class YOLOV5TorchObjectDetector(metaclass=DummyObject):
+    _backend = ["torch", "cv2", "seaborn", "psutil", "yaml", "ipython"]
+    _module = "deep_utils.vision.object_detection.yolo.v5.torch.yolo_v5_torch_object_detection"
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, self._backend, module_name=self._module, cls_name=self.__class__.__name__)
 
 
-class TorchUtils(metaclass=DummyObject):
-    _backend = ["torch"]
-    _module = "deep_utils.utils.torch_utils.torch_utils"
+class YOLOV7TorchObjectDetector(metaclass=DummyObject):
+    _backend = ["torch", "cv2", "seaborn", "yaml"]
+    _module = "deep_utils.vision.object_detection.yolo.v7.torch.yolo_v7_torch_object_detection"
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, self._backend, module_name=self._module, cls_name=self.__class__.__name__)
```

### Comparing `deep_utils-1.0.2/deep_utils/dummy_objects/utils/sqlalchemy_utils/__init__.py` & `deep_utils-1.2.0/deep_utils/_dummy_objects/utils/sqlalchemy_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from deep_utils.dummy_objects.dummy_framework import DummyObject, requires_backends
+from deep_utils._dummy_objects.dummy_framework import DummyObject, requires_backends
 
 
 class SQLAlchemyChecks(metaclass=DummyObject):
     _backend = ["sqlalchemy"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, self._backend)
```

### Comparing `deep_utils-1.0.2/deep_utils/dummy_objects/vision/face_detection/__init__.py` & `deep_utils-1.2.0/deep_utils/_dummy_objects/vision/face_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/dummy_objects/vision/object_detection/__init__.py` & `deep_utils-1.2.0/deep_utils/_dummy_objects/cv2_dummy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from deep_utils.dummy_objects.dummy_framework import DummyObject, requires_backends
+from deep_utils._dummy_objects.dummy_framework import DummyObject, requires_backends
 
 
-class YOLOV5TorchObjectDetector(metaclass=DummyObject):
-    _backend = ["torch", "cv2", "seaborn", "psutil", "yaml", "ipython"]
-    _module = "deep_utils.vision.object_detection.yolo.v5.torch.yolo_v5_torch_object_detection"
+class HaarcascadeCV2FaceDetector(metaclass=DummyObject):
+    _backend = ["cv2"]
+    _module = "deep_utils.vision.face_detection.haarcascade.cv2_.haarcascade_cv2_face_detection"
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, self._backend, module_name=self._module, cls_name=self.__class__.__name__)
 
 
-class YOLOV7TorchObjectDetector(metaclass=DummyObject):
-    _backend = ["torch", "cv2", "seaborn", "yaml"]
-    _module = "deep_utils.vision.object_detection.yolo.v7.torch.yolo_v7_torch_object_detection"
+class CVUtils(metaclass=DummyObject):
+    _backend = ["cv2"]
+    _module = "deep_utils.utils.opencv_utils.opencv_utils"
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, self._backend, module_name=self._module, cls_name=self.__class__.__name__)
```

### Comparing `deep_utils-1.0.2/deep_utils/dummy_objects/vision/object_tracker/__init__.py` & `deep_utils-1.2.0/deep_utils/_dummy_objects/vision/object_tracker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from deep_utils.dummy_objects.dummy_framework import DummyObject, requires_backends
+from deep_utils._dummy_objects.dummy_framework import DummyObject, requires_backends
 
 
 class DeepSortTorch(metaclass=DummyObject):
     _backend = ["torch", "cv2"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, self._backend)
```

### Comparing `deep_utils-1.0.2/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py` & `deep_utils-1.2.0/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/gis/projection/main.py` & `deep_utils-1.2.0/deep_utils/gis/projection/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/main_abs/cv2/cv2_caffe.py` & `deep_utils-1.2.0/deep_utils/main_abs/cv2/cv2_caffe.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/main_abs/cv2/cv2_main.py` & `deep_utils-1.2.0/deep_utils/main_abs/cv2/cv2_main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/main_abs/main.py` & `deep_utils-1.2.0/deep_utils/main_abs/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 import os
 from abc import ABC
 from typing import Any, Dict, Union
 
 from deep_utils.utils.lib_utils.main_utils import import_module
-from deep_utils.utils.os_utils import split_all
+from deep_utils.utils.os_utils.os_path import split_all
 
 
 class MainClass(ABC):
     def __init__(self, name, file_path, **kwargs):
         self.config = None
         self.model = None
         self.name = name
```

### Comparing `deep_utils-1.0.2/deep_utils/main_abs/main_config.py` & `deep_utils-1.2.0/deep_utils/main_abs/main_config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/nlp/ner/augmentation.py` & `deep_utils-1.2.0/deep_utils/nlp/ner/augmentation.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/nlp/ner/base_operations.py` & `deep_utils-1.2.0/deep_utils/nlp/ner/base_operations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/nlp/ner/preprocessing.py` & `deep_utils-1.2.0/deep_utils/nlp/ner/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/nlp/ner/utils_.py` & `deep_utils-1.2.0/deep_utils/nlp/ner/utils_.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/nlp/utils/persian/utils.py` & `deep_utils-1.2.0/deep_utils/nlp/utils/persian/utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/preprocessing/monai/monai_segmentation.py` & `deep_utils-1.2.0/deep_utils/preprocessing/monai/monai_segmentation.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/__init__.py` & `deep_utils-1.2.0/deep_utils/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/algorithm_utils/main.py` & `deep_utils-1.2.0/deep_utils/utils/algorithm_utils/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/box_utils/boxes.py` & `deep_utils-1.2.0/deep_utils/utils/box_utils/boxes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from enum import Enum
-from typing import Sequence, Union
+from typing import Sequence, Union, Tuple, List
+
 import numpy as np
-from deep_utils.utils.logging_utils.logging_utils import log_print, value_error_log
+
+from deep_utils.utils.logging_utils.logging_utils import value_error_log
 
 
 class Point:
     class PointSource(Enum):
         Torch = "Torch"
         TF = "TF"
         CV = "CV"
@@ -223,14 +225,70 @@
         Numpy = "Numpy"
 
     class OutType(Enum):
         Numpy = np.array
         List = list
         Tuple = tuple
 
+    PointSource = Point.PointSource
+
+    @staticmethod
+    def check_overlap(box_a: Union[Tuple[int, int, int, int], List[int]],
+                      box_b: Union[Tuple[int, int, int, int], List[int]]):
+        """
+        Check if two boxes overlap
+        :param box_a:
+        :param box_b:
+        :return:
+        """
+        p1_x1, p1_y1, p1_x2, p1_y2 = box_a
+        p2_x1, p2_y1, p2_x2, p2_y2 = box_b
+
+        if p1_x1 > p2_x2 or p1_x2 < p2_x1:
+            return False
+        if p1_y1 > p2_y2 or p1_y2 < p2_y1:
+            return False
+        return True
+
+    @staticmethod
+    def resize_box(box: List[int],
+                   img_input_shape: Union[list, tuple] = None,
+                   img_resized_shape: Union[list, tuple] = None,
+                   return_int: bool = True):
+        """
+        Resize a box from one source to another when the image is resized. Box and shapes must be in Numpy source.
+        Box must be in XYXY format.
+        :param box:
+        :param img_input_shape:
+        :param img_resized_shape:
+        :param return_int: if True, return the box as int, else return as float
+        :return:
+        """
+        if box is None or len(box) == 0:
+            raise ValueError("box is None or empty")
+        if len(box) != 4:
+            raise ValueError(f"box must have 4 elements, got {len(box)}")
+        # get the ratio
+        if img_input_shape is None or img_resized_shape is None:
+            raise ValueError("img_input_shape and img_resized_shape must be provided")
+        if len(img_input_shape) != 2 or len(img_resized_shape) != 2:
+            raise ValueError("img_input_shape and img_resized_shape must be 2D")
+        ratio_w = img_resized_shape[0] / img_input_shape[0]
+        ratio_h = img_resized_shape[1] / img_input_shape[1]
+        # resize the box
+        resized_box = [
+            box[0] * ratio_w,
+            box[1] * ratio_h,
+            box[2] * ratio_w,
+            box[3] * ratio_h,
+        ]
+        if return_int:
+            resized_box = [round(b) for b in resized_box]
+        return resized_box
+
     @staticmethod
     def box2box(
             box,
             in_format=None,
             to_format=None,
             in_source: Union[str, BoxSource] = BoxSource.Numpy,
             to_source: Union[str, BoxSource] = BoxSource.Numpy,
```

### Comparing `deep_utils-1.0.2/deep_utils/utils/coco_utils/main.py` & `deep_utils-1.2.0/deep_utils/utils/coco_utils/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/color_utils/color_utils.py` & `deep_utils-1.2.0/deep_utils/utils/color_utils/color_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/compress_utils/zip_utils.py` & `deep_utils-1.2.0/deep_utils/utils/compress_utils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/ctc_decoder/ctc_decoder.py` & `deep_utils-1.2.0/deep_utils/utils/ctc_decoder/ctc_decoder.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/decorators/main.py` & `deep_utils-1.2.0/deep_utils/utils/decorators/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py` & `deep_utils-1.2.0/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py` & `deep_utils-1.2.0/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/dict_utils/dict_utils.py` & `deep_utils-1.2.0/deep_utils/utils/dict_utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/dir_utils/dir_utils.py` & `deep_utils-1.2.0/deep_utils/utils/dir_utils/dir_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/encodes/b64.py` & `deep_utils-1.2.0/deep_utils/utils/encodes/b64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Union
 
 import numpy as np
 
-from deep_utils.utils.logging_utils import log_print, value_error_log
+from deep_utils.utils.logging_utils.logging_utils import log_print, value_error_log
 
 
 def img_to_b64(image: np.ndarray, extension: str = ".jpg") -> str:
     """
     returns a base64 encoded string from an image
     :param image: The input image
     :param extension: the extension to encode
```

### Comparing `deep_utils-1.0.2/deep_utils/utils/gif_utils/gif_utils.py` & `deep_utils-1.2.0/deep_utils/utils/gif_utils/gif_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/hash_utils/hash_utils.py` & `deep_utils-1.2.0/deep_utils/utils/hash_utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/image_utils/image_utils.py` & `deep_utils-1.2.0/deep_utils/utils/image_utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/json_utils/json_utils.py` & `deep_utils-1.2.0/deep_utils/utils/json_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/kafka_utils/kafka_utils.py` & `deep_utils-1.2.0/deep_utils/utils/kafka_utils/kafka_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/lib_utils/download_utils.py` & `deep_utils-1.2.0/deep_utils/utils/lib_utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/lib_utils/lib_decorators.py` & `deep_utils-1.2.0/deep_utils/utils/lib_utils/lib_decorators.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/lib_utils/main_utils.py` & `deep_utils-1.2.0/deep_utils/utils/lib_utils/main_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/logging_utils/logging_utils.py` & `deep_utils-1.2.0/deep_utils/utils/logging_utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/lr_scheduler_utils/warmup.py` & `deep_utils-1.2.0/deep_utils/utils/lr_scheduler_utils/warmup.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/matplotlib_utils/bar_plots.py` & `deep_utils-1.2.0/deep_utils/utils/matplotlib_utils/bar_plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/matplotlib_utils/main.py` & `deep_utils-1.2.0/deep_utils/utils/matplotlib_utils/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/memory_utils/torch_memory_utils.py` & `deep_utils-1.2.0/deep_utils/utils/memory_utils/torch_memory_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/minio_lib/main.py` & `deep_utils-1.2.0/deep_utils/utils/minio_lib/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py` & `deep_utils-1.2.0/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/np_utils/main_np.py` & `deep_utils-1.2.0/deep_utils/utils/np_utils/main_np.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/object_utils/object_utils.py` & `deep_utils-1.2.0/deep_utils/utils/object_utils/object_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/opencv_utils/main.py` & `deep_utils-1.2.0/deep_utils/utils/opencv_utils/opencv_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import cv2
 import numpy as np
+
 from deep_utils.utils.box_utils.boxes import Point
 from deep_utils.utils.resize_utils.main_resize import resize
 
 
 class VideoWriterCV:
     def __init__(
             self,
@@ -11,74 +13,74 @@
             height,
             fourcc="XVID",
             fps=30,
             colorful=True,
             in_source="Numpy",
     ):
         self.width, self.height = width, height
-        import cv2
 
         point = Point.point2point(
             (width, height), in_source=in_source, to_source=Point.PointSource.CV
         )
         fourcc = cv2.VideoWriter_fourcc(
             *fourcc) if isinstance(fourcc, str) else fourcc
         self.vw = cv2.VideoWriter(save_path, fourcc, fps, point, colorful)
 
     def write(self, frame):
         if frame.shape[:2] != (self.width, self.height):
             frame = resize(frame, (self.width, self.height))
         self.vw.write(frame)
 
 
-def rotate(
-        img,
-        rotation_degree,
-        center_point=None,
-        scale=1.0,
-        dsize=None,
-        bound=False,
-        clockwise=True,
-):
-    import cv2
-
-    h, w = img.shape[:2]
-    (w, h) = dsize = (w, h) if dsize is None else dsize
-    center_point = (w // 2, h // 2) if center_point is None else center_point
-    # negative angle >> clockwise rotation | positive angle >> counter clockwise rotation
-    rotation_degree = -rotation_degree if clockwise else rotation_degree
-    m = cv2.getRotationMatrix2D(center_point, rotation_degree, scale)
-    if bound:
+class CVUtils:
+    @staticmethod
+    def rotate(
+            img,
+            rotation_degree,
+            center_point=None,
+            scale=1.0,
+            dsize=None,
+            bound=False,
+            clockwise=True,
+    ):
+
         h, w = img.shape[:2]
-        cos = abs(m[0, 0])
-        sin = abs(m[0, 1])
-        w_ = int((cos * w) + (sin * h))
-        h_ = int((cos * h) + (sin * w))
-        m[0, 2] += w_ // 2 - w // 2
-        m[1, 2] += h_ // 2 - h // 2
-        dsize = (w_, h_)
-    rotated = cv2.warpAffine(img, m, dsize)
-
-    return rotated
-
-
-def translate(img, tx, ty, dsize=None):
-    import cv2
-
-    h, w = img.shape[:2][::-1]
-    dsize = (w, h) if dsize is None else dsize
-    translation_matrix = np.array([[1, 0, tx], [0, 1, ty]], dtype=np.float32)
-    translated_image = cv2.warpAffine(
-        src=img, M=translation_matrix, dsize=dsize)
-    return translated_image
-
-
-def show_destroy_cv2(img, win_name="", show=True):
-    import cv2
-    if show:
-        try:
-            cv2.imshow(win_name, img)
-            cv2.waitKey(0)
-            cv2.destroyWindow(win_name)
-        except Exception as e:
-            cv2.destroyWindow(win_name)
-            raise e
+        (w, h) = dsize = (w, h) if dsize is None else dsize
+        center_point = (w // 2, h // 2) if center_point is None else center_point
+        # negative angle >> clockwise rotation | positive angle >> counter clockwise rotation
+        rotation_degree = -rotation_degree if clockwise else rotation_degree
+        m = cv2.getRotationMatrix2D(center_point, rotation_degree, scale)
+        if bound:
+            h, w = img.shape[:2]
+            cos = abs(m[0, 0])
+            sin = abs(m[0, 1])
+            w_ = int((cos * w) + (sin * h))
+            h_ = int((cos * h) + (sin * w))
+            m[0, 2] += w_ // 2 - w // 2
+            m[1, 2] += h_ // 2 - h // 2
+            dsize = (w_, h_)
+        rotated = cv2.warpAffine(img, m, dsize)
+
+        return rotated
+
+    @staticmethod
+    def translate(img, tx, ty, dsize=None):
+        h, w = img.shape[:2][::-1]
+        dsize = (w, h) if dsize is None else dsize
+        translation_matrix = np.array([[1, 0, tx], [0, 1, ty]], dtype=np.float32)
+        translated_image = cv2.warpAffine(
+            src=img, M=translation_matrix, dsize=dsize)
+        return translated_image
+
+    @staticmethod
+    def show_destroy_cv2(img, win_name="", show=True):
+        if show:
+            try:
+                cv2.imshow(win_name, img)
+                cv2.waitKey(0)
+                cv2.destroyWindow(win_name)
+            except Exception as e:
+                cv2.destroyWindow(win_name)
+                raise e
+
+
+show_destroy_cv2 = CVUtils.show_destroy_cv2
```

### Comparing `deep_utils-1.0.2/deep_utils/utils/optimizers/tf.py` & `deep_utils-1.2.0/deep_utils/utils/optimizers/tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/os_utils/os_path.py` & `deep_utils-1.2.0/deep_utils/utils/os_utils/os_path.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/postgresql_utils/postgresql_utils.py` & `deep_utils-1.2.0/deep_utils/utils/postgresql_utils/postgresql_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/re_utils/re_utils.py` & `deep_utils-1.2.0/deep_utils/utils/re_utils/re_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/requests_utils/requests_utils.py` & `deep_utils-1.2.0/deep_utils/utils/requests_utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/resize_utils/main_resize.py` & `deep_utils-1.2.0/deep_utils/utils/resize_utils/main_resize.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/shutil_utils/shutil_utils.py` & `deep_utils-1.2.0/deep_utils/utils/shutil_utils/shutil_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/sqlalchemy/__init__.py` & `deep_utils-1.2.0/deep_utils/utils/sqlalchemy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # try:
-#     from deep_utils.dummy_objects.utils.sqlalchemy_utils import SQLAlchemyChecks
+#     from deep_utils._dummy_objects.utils.sqlalchemy_utils import SQLAlchemyChecks
 #     from .checks import SQLAlchemyChecks
 # except ModuleNotFoundError:
 #     pass
 #
 # try:
-#     from deep_utils.dummy_objects.utils.sqlalchemy_utils import SQLAlchemyInserts
+#     from deep_utils._dummy_objects.utils.sqlalchemy_utils import SQLAlchemyInserts
 #     from .insert import SQLAlchemyInserts
 # except ModuleNotFoundError:
 #     pass
 #
 # try:
-#     from deep_utils.dummy_objects.utils.sqlalchemy_utils import SQLAlchemyUtils
+#     from deep_utils._dummy_objects.utils.sqlalchemy_utils import SQLAlchemyUtils
 #     from .sqlalchemy_utils import SQLAlchemyUtils
 # except ModuleNotFoundError:
 #     pass
```

### Comparing `deep_utils-1.0.2/deep_utils/utils/sqlalchemy/checks.py` & `deep_utils-1.2.0/deep_utils/utils/sqlalchemy/checks.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py` & `deep_utils-1.2.0/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py` & `deep_utils-1.2.0/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/tf_utils/logging.py` & `deep_utils-1.2.0/deep_utils/utils/tf_utils/logging.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/utils/hyper_parameters.py` & `deep_utils-1.2.0/deep_utils/utils/utils/hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/utils/shuffle_utils.py` & `deep_utils-1.2.0/deep_utils/utils/utils/shuffle_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/utils/str_utils.py` & `deep_utils-1.2.0/deep_utils/utils/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/utils/utils/yaml_utils.py` & `deep_utils-1.2.0/deep_utils/utils/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/__init__.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/haarcascade/cv2_/config.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/haarcascade/cv2_/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/main/main_face_detection.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/main/main_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/config.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/config.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/config.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/net.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/net.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/utils/op.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/utils/op.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/config.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py` & `deep_utils-1.2.0/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_recognition/main/main_face_recognition.py` & `deep_utils-1.2.0/deep_utils/vision/face_recognition/main/main_face_recognition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import numpy as np
 from abc import abstractmethod
-from deep_utils.utils.pickle_utils.pickles import dump_pickle
+from deep_utils.utils.pickle_utils.pickle_utils import dump_pickle
 from deep_utils.main_abs.main import MainClass
 from deep_utils.utils.dict_named_tuple_utils import dictnamedtuple
 from deep_utils.utils.dir_utils.dir_utils import remove_create
 from deep_utils.utils.os_utils.os_path import split_extension
 from deep_utils.utils.logging_utils.logging_utils import log_print
 
 OUTPUT_CLASS = dictnamedtuple(
```

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/torch/config.py` & `deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py` & `deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py` & `deep_utils-1.2.0/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from deep_utils.utils.lib_utils.download_utils import download_decorator
 from deep_utils.utils.lib_utils.lib_decorators import (
     expand_input,
     get_elapsed_time,
     get_from_config,
     lib_rgb2bgr
 )
-from deep_utils.utils.pickle_utils.pickles import load_pickle
+from deep_utils.utils.pickle_utils.pickle_utils import load_pickle
 from deep_utils.vision.face_recognition.main.main_face_recognition import FaceRecognition, OUTPUT_CLASS
 from .config import Config
 from .src import load_model
 
 
 class VggFace2TorchFaceRecognition(FaceRecognition):
     def __init__(self, **kwargs):
```

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/main/main_object_detection.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/main/main_object_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/config.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/config.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_detection/yolo/yolo_detector.py` & `deep_utils-1.2.0/deep_utils/vision/object_detection/yolo/yolo_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 import shutil
 from abc import ABC
 from os.path import join, split
 from typing import Dict, List, Union, Type
 
 from tqdm import tqdm
-
-from deep_utils.main_abs import MainClass
+import cv2
+from deep_utils.main_abs.main import MainClass
 from deep_utils.utils.box_utils.boxes import Box
 from deep_utils.utils.dict_named_tuple_utils import dictnamedtuple
 from deep_utils.utils.dir_utils.dir_utils import (
     dir_train_test_split,
     remove_create,
     transfer_directory_items,
     file_incremental
 )
-from deep_utils.utils.logging_utils import log_print
-from deep_utils.utils.opencv_utils.main import show_destroy_cv2
+from deep_utils.utils.logging_utils.logging_utils import log_print
+from deep_utils.utils.opencv_utils.opencv_utils import CVUtils
 from deep_utils.utils.os_utils.os_path import split_extension
 from deep_utils.utils.shutil_utils.shutil_utils import mv_or_copy
 from deep_utils.utils.os_utils.os_path import validate_file_extension
 from deep_utils.utils.shutil_utils.shutil_utils import mv_or_copy_list
 
 OUTPUT_CLASS = dictnamedtuple(
     "Object", ["class_indices", "boxes", "confidences", "class_names", "elapsed_time"]
@@ -38,20 +38,24 @@
 class YOLOObjectDetector(MainClass, ABC):
     """
     This class contains handy functions for yolo versions!
     """
 
     @staticmethod
     def test_label_dir(dataset_dir, rename_dict: Union[Dict[int, str], None] = None, images_name="images",
-                       labels_name="labels"):
+                       labels_name="labels", show=True):
         images_path = join(dataset_dir, images_name)
         for name in sorted(os.listdir(images_path)):
             img_address = join(images_path, name)
             text_address = join(dataset_dir, labels_name, split_extension(name, '.txt'))
-            YOLOObjectDetector.test_label(img_address, text_address, rename_dict=rename_dict)
+            if show:
+                YOLOObjectDetector.test_label(img_address, text_address, rename_dict=rename_dict, show=show)
+            else:
+                img = YOLOObjectDetector.test_label(img_address, text_address, rename_dict=rename_dict, show=show)
+                yield img
 
     @staticmethod
     def test_label(img_path, label_path, rename_dict: Union[Dict[int, str], None] = None, show=True):
         import cv2
 
         img = cv2.imread(img_path)
         boxes, texts, orgs = [], [], []
@@ -71,15 +75,15 @@
                             in_relative=True,
                             to_relative=False,
                             shape_source="Numpy",
                             shape=img.shape[:2],
                             )
         img = Box.put_box_text(img, boxes, texts)
         if show:
-            show_destroy_cv2(img)
+            CVUtils.show_destroy_cv2(img)
         return img
 
     @staticmethod
     def split_dataset(
             base_dir,
             out_dir,
             mode="cp",
@@ -339,14 +343,32 @@
                        img_size=None,
                        agnostic=None,
                        get_time=False,
                        logger=None,
                        verbose=1) -> Union[Type[OutputType], Dict[str, list]]:
         raise NotImplementedError("object_detects is not implemented!")
 
+    def detect_img_file(self,
+                        img_file,
+                        class_indices=None,
+                        confidence=None,
+                        iou_thresh=None,
+                        img_size=None,
+                        agnostic=None,
+                        get_time=False,
+                        logger=None,
+                        verbose=1) -> Union[Type[OutputType], Dict[str, list]]:
+        img = cv2.imread(img_file)
+        if img is None:
+            log_print(logger, f"Image {img_file} is not valid", verbose=verbose)
+        else:
+            return self.detect_objects(img, False, class_indices, confidence,
+                                       iou_thresh, img_size, agnostic, get_time,
+                                       logger, verbose)
+
     def detect_dir(self,
                    dir_,
                    confidence=None,
                    iou_thresh=None,
                    classes=None,
                    extensions=(".png", ".jpg", ".jpeg"),
                    save_labels_dir=None,
```

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/__init__.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 try:
-    from deep_utils.dummy_objects.vision.object_tracker import DeepSortTorch
+    from deep_utils._dummy_objects.vision.object_tracker import DeepSortTorch
     from deep_utils.vision.object_tracker.deep_sort import DeepSortTorch
 except:
     pass
 
 
 try:
-    from deep_utils.dummy_objects.vision.object_tracker import DeepSortTorchFeatureExtractor
+    from deep_utils._dummy_objects.vision.object_tracker import DeepSortTorchFeatureExtractor
     from deep_utils.vision.object_tracker.deep_sort import DeepSortTorchFeatureExtractor
 except:
     pass
 
 try:
-    from deep_utils.dummy_objects.vision.object_tracker import DeepSortTorchTracker
+    from deep_utils._dummy_objects.vision.object_tracker import DeepSortTorchTracker
     from deep_utils.vision.object_tracker.deep_sort import DeepSortTorchTracker
 except:
     pass
```

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/__init__.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py` & `deep_utils-1.2.0/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/ocr/crnn/torch/crnn_inference.py` & `deep_utils-1.2.0/deep_utils/vision/ocr/crnn/torch/crnn_inference.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/ocr/crnn/torch/crnn_model.py` & `deep_utils-1.2.0/deep_utils/vision/ocr/crnn/torch/crnn_model.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py` & `deep_utils-1.2.0/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py` & `deep_utils-1.2.0/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py` & `deep_utils-1.2.0/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/deep_utils.egg-info/PKG-INFO` & `deep_utils-1.2.0/deep_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: deep-utils
-Version: 1.0.2
+Version: 1.2.0
 Summary: Deep Utils
 Home-page: https://github.com/pooya-mohammadi/deep_utils
 Author: Pooya Mohammadi Kazaj
 Author-email: pooyamohammadikazaj@gmial.com
 License: UNKNOWN
-Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.0.2.tar.gz
-Description: [![Downloads](https://static.pepy.tech/badge/deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils) [![build](https://github.com/pooya-mohammadi/deep_utils/actions/workflows/ci-tests.yml/badge.svg)](https://github.com/pooya-mohammadi/deep_utils/actions/workflows/ci-tests.yml)
+Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.2.0.tar.gz
+Description: [![Downloads](https://static.pepy.tech/badge/deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
         
         <div id="top"></div>
         <!-- PROJECT LOGO -->
         <br />
         <div align="center">
           <a href="https://github.com/pooya-mohammadi/deep_utils">
             <img src="https://raw.githubusercontent.com/pooya-mohammadi/deep_utils/master/images/logo/deep_utils.png" alt="Logo">
@@ -33,14 +33,18 @@
         * [About The Project](#about-the-project)
         * [Installation](#installation)
         * [Vision](#vision)
             * [Face Detection](#face-detection)
                 * [MTCNN](#mtcnn)
             * [Object Detection](#object-detection)
                 * [yolov5](#yolov5)
+            * [Visual Grounding](#visual-grounding)
+                * [Grounding DINO](#grounding-dino)
+            * [Image Editing](#image-editing)
+                * [GLIDE](#glide)
         * [NLP](#NLP)
             * [NER](#NER)
                 * [Replacement Augmentation](replacement-augmentation)
                 * [Remove Augmentation](remove-augmentation)
         * [Augmentation](#augmentation)
             * [CutMix](#cutmix)
         * [Utils](#utils)
@@ -232,40 +236,109 @@
         # visualize using oepncv
         # show_destroy_cv2(img)
         ```
         
         <img src="https://raw.githubusercontent.com/pooya-mohammadi/deep-utils-notebooks/main/vision/images/dog_yolov5.jpg" alt="Logo" >
         <p align="right">(<a href="#top">back to top</a>)</p>
         
+        ## Visual Grounding
+        
+        ### Grounding DINO
+        
+        DINO is a self-supervised learning method for visual grounding. It is a simple and efficient method that can be used for
+        visual grounding. Let's see how we can use it in `deep_utils`:
+        
+        #### Download a sample image
+        
+        ```commandline
+        wget -q https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/golsa_in_garden.jpg
+        ```
+        
+        ```python
+        from PIL import Image
+        from deep_utils import Text2BoxVisualGroundingDino
+        import numpy as np
+        import matplotlib.pyplot as plt
+        
+        model = Text2BoxVisualGroundingDino()
+        
+        img_path = "golsa_in_garden.jpg"
+        img = np.asarray(Image.open(img_path))
+        
+        output = model.text_to_box(text="Hen", img=img)
+        print(output.boxes, output.scores, output.labels)
+        annotated_img = model.annotate(img, output)
+        plt.axis("off")
+        plt.imshow(annotated_img)
+        ```
+        
+        Output Image:<br/>
+        <img src="https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/golsa_in_garden_dino.png" width="400">
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
+        ## Image Editing
+        
+        ### GLIDE
+        
+        GLIDE is a simple and efficient method for image editing/inpainting. It is developed by OpenAI.
+        
+        #### Download a sample image
+        
+        ```commandline
+        wget -q https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/golsa_in_garden.jpg
+        ```
+        
+        **Input Image**:<br/>
+        <img src="https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/golsa_in_garden.jpg" width="400">
+        
+        ```python
+        import matplotlib.pyplot as plt
+        from deep_utils import ImageEditingGLIDE
+        from PIL import Image
+        
+        pil_img = Image.open("golsa_in_garden.jpg")
+        # position of the editing box. Here the hen in the image. The  
+        box = [340.6672668457031, 403.7683410644531, 372.0812072753906, 439.3288879394531]
+        glide_model = ImageEditingGLIDE()
+        text = "dead leaves"
+        edited_image = glide_model.edit_box(pil_img, text=text, box=box)
+        plt.imshow(edited_image)
+        ```
+        
+        **Output Image**: The `hen` is removed and replaced with `dead leaves` as the background<br/>
+        <img src="https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/glide_output.jpg" width="400">
+        
+        **Note:** The best way to get the box is to use the `Text2BoxVisualGroundingDino` model. See the example in the previous
+        section.
+        
         ## NLP
         
         In this section, models and utilities for nlp projects are provided
         
         ### NER
         
         Name Entity Recognition
         
         #### multi-label-stratify
         
         ## Augmentation
         
         ### CutMix
         
-        <a href="https://colab.research.google.com/github/pooya-mohammadi/deep-utils-notebooks/blob/main/augmentation/cutmix/cutmix_tf.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+        <a href="https://colab.research.google.com/github/pooya-mohammadi/deep-utils-notebooks/blob/main/augmentation/cutmix/cutmix_tf.ipynb" target="_parent"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" /> </a> 
         
         CutMix is one of the best augmentation methods that's proven to be very effective in different vision-based project.
-        Therefore, CutMix is now available on `deep_utils` to be used both for segmentation and classification tasks. Let some
-        examples:
+        Therefore, CutMix is now
+        available on `deep_utils` to be used both for segmentation and classification tasks.Let some examples:
         
         #### Segmentation
         
         ```python
         import cv2
         import numpy as np
-        from PIL import Image
         from deep_utils import CutMixTF, group_show, repeat_dimension
         
         # creating random images, the code for this section can be found in the colab notebook
         image_a = np.zeros((300, 300, 3), np.uint8) * 255
         mask_a = np.zeros_like(image_a)
         pt1 = (150, 100)
         pt2 = (100, 200)
@@ -356,17 +429,19 @@
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ### Multi-Label-Stratify
         
         While splitting a dataset for NER or Object detection tasks, you might have noticed that there is no way to split the
         dataset using
-        stratify functionality of `train_test_split` of the `scikit-learn` library because not only does each sample in these two tasks may
+        stratify functionality of `train_test_split` of the `scikit-learn` library because not only does each sample in these
+        two tasks may
         have
-        more than one tag/object, but also each tag/object of each class may appear more than once. For example, an image/sample may
+        more than one tag/object, but also each tag/object of each class may appear more than once. For example, an image/sample
+        may
         contain two dogs and three cats, which means the label/y of that sample would be like [2, 3] in which the index zero
         corresponds
         to the dog class, and the index one corresponds to the cat class.
         To split these types of datasets, the following function is
         developed in the `deep_utils` library which is very easy to use. To use this function, two arrays are needed. The first
         is an array
         or list containing the input samples. The type of these samples could be anything; they could be a list of sentences, a
@@ -446,14 +521,15 @@
         
         
         <!-- LICENSE -->
         
         ## 🌟 Spread the word!
         
         If you want to say thank you and/or support active development of the repo:
+        
         - Add a GitHub Star to the project!
         - Join our discord servers [Deep Utils](https://discord.gg/pWe3yChw) .
         - Follow my profile [pooya-mohammadi](https://github.com/pooya-mohammadi)
         
         Thanks so much for your interest in growing the reach of the repo!
         <p align="right">(<a href="#top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,33 +1,32 @@
-Metadata-Version: 2.1 Name: deep-utils Version: 1.0.2 Summary: Deep Utils Home-
+Metadata-Version: 2.1 Name: deep-utils Version: 1.2.0 Summary: Deep Utils Home-
 page: https://github.com/pooya-mohammadi/deep_utils Author: Pooya Mohammadi
 Kazaj Author-email: pooyamohammadikazaj@gmial.com License: UNKNOWN Download-
 URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/
-1.0.2.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
+1.2.0.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
 deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://
 img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
-[![build](https://github.com/pooya-mohammadi/deep_utils/actions/workflows/ci-
-tests.yml/badge.svg)](https://github.com/pooya-mohammadi/deep_utils/actions/
-workflows/ci-tests.yml)
 
                                     [Logo]
                              **** Deep Utils ****
                   A toolkit for deep-learning practitioners!
 This repository contains the most frequently used deep learning models and
 functions. **Deep_Utils** is still under heavy development, so take into
 consideration that many features may change in the future and make sure to
 install the latest version using pypi. ## Table of contents * [About The
 Project](#about-the-project) * [Installation](#installation) * [Vision]
 (#vision) * [Face Detection](#face-detection) * [MTCNN](#mtcnn) * [Object
-Detection](#object-detection) * [yolov5](#yolov5) * [NLP](#NLP) * [NER](#NER) *
-[Replacement Augmentation](replacement-augmentation) * [Remove Augmentation]
-(remove-augmentation) * [Augmentation](#augmentation) * [CutMix](#cutmix) *
-[Utils](#utils) * [DictNamedTuple](#dictnametuple) * [multi-label-stratify]
-(#multi-label-stratify) * [Tests](#tests) * [Contributing](#Contributing) *
-[Licence](#Licence) * [Collaborators](#Collaborators) * [Contact](#Contact) *
+Detection](#object-detection) * [yolov5](#yolov5) * [Visual Grounding](#visual-
+grounding) * [Grounding DINO](#grounding-dino) * [Image Editing](#image-
+editing) * [GLIDE](#glide) * [NLP](#NLP) * [NER](#NER) * [Replacement
+Augmentation](replacement-augmentation) * [Remove Augmentation](remove-
+augmentation) * [Augmentation](#augmentation) * [CutMix](#cutmix) * [Utils]
+(#utils) * [DictNamedTuple](#dictnametuple) * [multi-label-stratify](#multi-
+label-stratify) * [Tests](#tests) * [Contributing](#Contributing) * [Licence]
+(#Licence) * [Collaborators](#Collaborators) * [Contact](#Contact) *
 [References](#references) * [Citation](#citation)
                                                                   (back_to_top)
 ## About the Project Many deep learning toolkits are available on GitHub;
 however, we couldn't find one that would suit our needs. So, we created this
 improved one. This toolkit minimizes the deep learning teams' coding efforts to
 utilize the functionalities of famous deep learning models such as MTCNN in
 face detection, yolov5 in object detection, and many other repositories and
@@ -95,33 +94,62 @@
 `False` result = yolov5.detect_objects(base_image, is_rgb=False,
 confidence=0.5) # Draw detected boxes on the image. img = Box.put_box_text
 (base_image, box=result.boxes, label=[f"{c_n} {c}" for c_n, c in zip
 (result.class_names, result.confidences)]) # pil.Image is used for
 visualization Image.fromarray(img[..., ::-1]) # convert to rgb # visualize
 using oepncv # show_destroy_cv2(img) ``` [Logo]
                                                                   (back_to_top)
+## Visual Grounding ### Grounding DINO DINO is a self-supervised learning
+method for visual grounding. It is a simple and efficient method that can be
+used for visual grounding. Let's see how we can use it in `deep_utils`: ####
+Download a sample image ```commandline wget -q https://github.com/pooya-
+mohammadi/deep_utils/releases/download/1.0.2/golsa_in_garden.jpg ``` ```python
+from PIL import Image from deep_utils import Text2BoxVisualGroundingDino import
+numpy as np import matplotlib.pyplot as plt model = Text2BoxVisualGroundingDino
+() img_path = "golsa_in_garden.jpg" img = np.asarray(Image.open(img_path))
+output = model.text_to_box(text="Hen", img=img) print(output.boxes,
+output.scores, output.labels) annotated_img = model.annotate(img, output)
+plt.axis("off") plt.imshow(annotated_img) ``` Output Image:
+[https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/
+golsa_in_garden_dino.png]
+                                                                  (back_to_top)
+## Image Editing ### GLIDE GLIDE is a simple and efficient method for image
+editing/inpainting. It is developed by OpenAI. #### Download a sample image
+```commandline wget -q https://github.com/pooya-mohammadi/deep_utils/releases/
+download/1.0.2/golsa_in_garden.jpg ``` **Input Image**:
+[https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/
+golsa_in_garden.jpg] ```python import matplotlib.pyplot as plt from deep_utils
+import ImageEditingGLIDE from PIL import Image pil_img = Image.open
+("golsa_in_garden.jpg") # position of the editing box. Here the hen in the
+image. The box = [340.6672668457031, 403.7683410644531, 372.0812072753906,
+439.3288879394531] glide_model = ImageEditingGLIDE() text = "dead leaves"
+edited_image = glide_model.edit_box(pil_img, text=text, box=box) plt.imshow
+(edited_image) ``` **Output Image**: The `hen` is removed and replaced with
+`dead leaves` as the background
+[https://github.com/pooya-mohammadi/deep_utils/releases/download/1.0.2/
+glide_output.jpg] **Note:** The best way to get the box is to use the
+`Text2BoxVisualGroundingDino` model. See the example in the previous section.
 ## NLP In this section, models and utilities for nlp projects are provided ###
 NER Name Entity Recognition #### multi-label-stratify ## Augmentation ###
 CutMix [Open_In_Colab] CutMix is one of the best augmentation methods that's
 proven to be very effective in different vision-based project. Therefore,
 CutMix is now available on `deep_utils` to be used both for segmentation and
-classification tasks. Let some examples: #### Segmentation ```python import cv2
-import numpy as np from PIL import Image from deep_utils import CutMixTF,
-group_show, repeat_dimension # creating random images, the code for this
-section can be found in the colab notebook image_a = np.zeros((300, 300, 3),
-np.uint8) * 255 mask_a = np.zeros_like(image_a) pt1 = (150, 100) pt2 = (100,
-200) pt3 = (200, 200) triangle_cnt = np.array([pt1, pt2, pt3]) image_a =
-cv2.drawContours(image_a, [triangle_cnt], 0, (0, 255, 0), -1) mask_a =
-cv2.drawContours(mask_a, [triangle_cnt], 0, (255, 255, 255), -1) image_b =
-np.zeros((300, 300, 3), np.uint8) * 255 mask_b = np.zeros_like(image_b) pt1 =
-(150, 150) image_b = cv2.circle(image_b, pt1, 50, (0, 255, 0), -1) mask_b =
-cv2.circle(mask_b, pt1, 50, (255, 255, 255), -1) # CutMix for two individual
-images: cutmix_img, cutmix_mask = CutMixTF.seg_cutmix(image_a, mask_a[..., 0],
-image_b, mask_b[..., 0], beta=1) ``` The input and output are as follows:
-**Input:** [Logo]
+classification tasks.Let some examples: #### Segmentation ```python import cv2
+import numpy as np from deep_utils import CutMixTF, group_show,
+repeat_dimension # creating random images, the code for this section can be
+found in the colab notebook image_a = np.zeros((300, 300, 3), np.uint8) * 255
+mask_a = np.zeros_like(image_a) pt1 = (150, 100) pt2 = (100, 200) pt3 = (200,
+200) triangle_cnt = np.array([pt1, pt2, pt3]) image_a = cv2.drawContours
+(image_a, [triangle_cnt], 0, (0, 255, 0), -1) mask_a = cv2.drawContours(mask_a,
+[triangle_cnt], 0, (255, 255, 255), -1) image_b = np.zeros((300, 300, 3),
+np.uint8) * 255 mask_b = np.zeros_like(image_b) pt1 = (150, 150) image_b =
+cv2.circle(image_b, pt1, 50, (0, 255, 0), -1) mask_b = cv2.circle(mask_b, pt1,
+50, (255, 255, 255), -1) # CutMix for two individual images: cutmix_img,
+cutmix_mask = CutMixTF.seg_cutmix(image_a, mask_a[..., 0], image_b, mask_b[...,
+0], beta=1) ``` The input and output are as follows: **Input:** [Logo]
 **Output:** [Logo] As it illustrated in the above image a section of the
 triangle and the circle are combined together. By changing `seg_cutmix` to
 `seg_cutmix_batch` one can use CutMix augmentation for batch of images.
 ```python cutmix_img, cutmix_mask = CutMixTF.seg_cutmix_batch
 (a_images=batch_img, a_masks=batch_mask[..., 0], beta=1) ``` **Input:**
 [cutmix]
 **Output:** [cutmix]
```

### Comparing `deep_utils-1.0.2/deep_utils.egg-info/SOURCES.txt` & `deep_utils-1.2.0/deep_utils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,60 @@
 setup.py
 deep_utils/__init__.py
 deep_utils.egg-info/PKG-INFO
 deep_utils.egg-info/SOURCES.txt
 deep_utils.egg-info/dependency_links.txt
 deep_utils.egg-info/requires.txt
 deep_utils.egg-info/top_level.txt
+deep_utils/_dummy_objects/__init__.py
+deep_utils/_dummy_objects/cv2_dummy.py
+deep_utils/_dummy_objects/glide_text2im_dummy.py
+deep_utils/_dummy_objects/groundingdino_torch_dummy.py
+deep_utils/_dummy_objects/requests_dummy.py
+deep_utils/_dummy_objects/tf_cv2_dummy.py
+deep_utils/_dummy_objects/tf_dummy.py
+deep_utils/_dummy_objects/torch_cv2_dummy.py
+deep_utils/_dummy_objects/torch_dummy.py
+deep_utils/_dummy_objects/torch_monai_dummy.py
+deep_utils/_dummy_objects/torchvision_torch_timm_transformers_fairscale_dummy.py
+deep_utils/_dummy_objects/audio/__init__.py
+deep_utils/_dummy_objects/audio/asr/__init__.py
+deep_utils/_dummy_objects/audio/asr/wave2vec2/__init__.py
+deep_utils/_dummy_objects/audio/classification/__init__.py
+deep_utils/_dummy_objects/audio/classification/wav2vec2/__init__.py
+deep_utils/_dummy_objects/audio/diarization/__init__.py
+deep_utils/_dummy_objects/audio/diarization/pyannote/__init__.py
+deep_utils/_dummy_objects/audio/utils_/__init__.py
+deep_utils/_dummy_objects/audio/vad/__init__.py
+deep_utils/_dummy_objects/audio/vad/pyannote/__init__.py
+deep_utils/_dummy_objects/augmentation/__init__.py
+deep_utils/_dummy_objects/augmentation/cutmix/__init__.py
+deep_utils/_dummy_objects/blocks/__init__.py
+deep_utils/_dummy_objects/blocks/torch/__init__.py
+deep_utils/_dummy_objects/callbacks/__init__.py
+deep_utils/_dummy_objects/callbacks/tf_keras/__init__.py
+deep_utils/_dummy_objects/dummy_framework/__init__.py
+deep_utils/_dummy_objects/dummy_framework/dummy_framework.py
+deep_utils/_dummy_objects/elasticsearch/__init__.py
+deep_utils/_dummy_objects/utils/__init__.py
+deep_utils/_dummy_objects/utils/git_utils/__init__.py
+deep_utils/_dummy_objects/utils/memory_utils/__init__.py
+deep_utils/_dummy_objects/utils/sqlalchemy_utils/__init__.py
+deep_utils/_dummy_objects/utils/torch_utils/__init__.py
+deep_utils/_dummy_objects/vision/__init__.py
+deep_utils/_dummy_objects/vision/face_detection/__init__.py
+deep_utils/_dummy_objects/vision/face_recognition/__init__.py
+deep_utils/_dummy_objects/vision/object_detection/__init__.py
+deep_utils/_dummy_objects/vision/object_tracker/__init__.py
+deep_utils/_dummy_objects/vision/ocr/__init__.py
+deep_utils/_dummy_objects/vision/ocr/crnn/__init__.py
+deep_utils/_dummy_objects/vision/ocr/crnn/torch/__init__.py
+deep_utils/_dummy_objects/vision/torch_vision/__init__.py
+deep_utils/_dummy_objects/vision/vision_utils/__init__.py
+deep_utils/_dummy_objects/vision/vision_utils/torch_vision_utils/__init__.py
 deep_utils/audio/__init__.py
 deep_utils/audio/asr/__init__.py
 deep_utils/audio/asr/wav2vec2/__init__.py
 deep_utils/audio/asr/wav2vec2/torch/__init__.py
 deep_utils/audio/asr/wav2vec2/torch/main.py
 deep_utils/audio/audio_utils/__init__.py
 deep_utils/audio/audio_utils/librosa_utils.py
@@ -43,68 +89,36 @@
 deep_utils/callbacks/torch/__init__.py
 deep_utils/callbacks/torch/torch_csv_logger.py
 deep_utils/callbacks/torch/torch_model_checkpoint.py
 deep_utils/callbacks/torch/torch_tensorboard.py
 deep_utils/design_patterns/__init__.py
 deep_utils/design_patterns/chain_of_responsibility/__init__.py
 deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py
-deep_utils/dummy_objects/__init__.py
-deep_utils/dummy_objects/cv2_dummy.py
-deep_utils/dummy_objects/tf_cv2_dummy.py
-deep_utils/dummy_objects/torch_cv2_dummy.py
-deep_utils/dummy_objects/torch_dummy.py
-deep_utils/dummy_objects/torch_monai_dummy.py
-deep_utils/dummy_objects/audio/__init__.py
-deep_utils/dummy_objects/audio/asr/__init__.py
-deep_utils/dummy_objects/audio/asr/wave2vec2/__init__.py
-deep_utils/dummy_objects/audio/classification/__init__.py
-deep_utils/dummy_objects/audio/classification/wav2vec2/__init__.py
-deep_utils/dummy_objects/audio/diarization/__init__.py
-deep_utils/dummy_objects/audio/diarization/pyannote/__init__.py
-deep_utils/dummy_objects/audio/utils_/__init__.py
-deep_utils/dummy_objects/audio/vad/__init__.py
-deep_utils/dummy_objects/audio/vad/pyannote/__init__.py
-deep_utils/dummy_objects/augmentation/__init__.py
-deep_utils/dummy_objects/augmentation/cutmix/__init__.py
-deep_utils/dummy_objects/blocks/__init__.py
-deep_utils/dummy_objects/blocks/torch/__init__.py
-deep_utils/dummy_objects/callbacks/__init__.py
-deep_utils/dummy_objects/callbacks/tf_keras/__init__.py
-deep_utils/dummy_objects/dummy_framework/__init__.py
-deep_utils/dummy_objects/dummy_framework/dummy_framework.py
-deep_utils/dummy_objects/elasticsearch/__init__.py
-deep_utils/dummy_objects/utils/__init__.py
-deep_utils/dummy_objects/utils/git_utils/__init__.py
-deep_utils/dummy_objects/utils/memory_utils/__init__.py
-deep_utils/dummy_objects/utils/sqlalchemy_utils/__init__.py
-deep_utils/dummy_objects/utils/torch_utils/__init__.py
-deep_utils/dummy_objects/vision/__init__.py
-deep_utils/dummy_objects/vision/face_detection/__init__.py
-deep_utils/dummy_objects/vision/face_recognition/__init__.py
-deep_utils/dummy_objects/vision/object_detection/__init__.py
-deep_utils/dummy_objects/vision/object_tracker/__init__.py
-deep_utils/dummy_objects/vision/ocr/__init__.py
-deep_utils/dummy_objects/vision/ocr/crnn/__init__.py
-deep_utils/dummy_objects/vision/ocr/crnn/torch/__init__.py
-deep_utils/dummy_objects/vision/torch_vision/__init__.py
-deep_utils/dummy_objects/vision/vision_utils/__init__.py
-deep_utils/dummy_objects/vision/vision_utils/torch_vision_utils/__init__.py
 deep_utils/elasticsearch/__init__.py
 deep_utils/elasticsearch/search_engine/__init__.py
 deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py
 deep_utils/gis/__init__.py
 deep_utils/gis/projection/__init__.py
 deep_utils/gis/projection/main.py
 deep_utils/main_abs/__init__.py
 deep_utils/main_abs/main.py
 deep_utils/main_abs/main_config.py
 deep_utils/main_abs/cv2/__init__.py
 deep_utils/main_abs/cv2/cv2_caffe.py
 deep_utils/main_abs/cv2/cv2_config.py
 deep_utils/main_abs/cv2/cv2_main.py
+deep_utils/multi_modals/__init__.py
+deep_utils/multi_modals/_models/__init__.py
+deep_utils/multi_modals/_models/blip/__init__.py
+deep_utils/multi_modals/_models/blip/torch/__init__.py
+deep_utils/multi_modals/_models/blip/torch/models/__init__.py
+deep_utils/multi_modals/_models/blip/torch/models/blip.py
+deep_utils/multi_modals/_models/blip/torch/models/med.py
+deep_utils/multi_modals/_models/blip/torch/models/med_configs.py
+deep_utils/multi_modals/_models/blip/torch/models/vit.py
 deep_utils/nlp/__init__.py
 deep_utils/nlp/ner/__init__.py
 deep_utils/nlp/ner/augmentation.py
 deep_utils/nlp/ner/base_operations.py
 deep_utils/nlp/ner/preprocessing.py
 deep_utils/nlp/ner/taggers.py
 deep_utils/nlp/ner/utils_.py
@@ -116,14 +130,15 @@
 deep_utils/preprocessing/__init__.py
 deep_utils/preprocessing/monai/__init__.py
 deep_utils/preprocessing/monai/monai_segmentation.py
 deep_utils/utils/__init__.py
 deep_utils/utils/algorithm_utils/__init__.py
 deep_utils/utils/algorithm_utils/main.py
 deep_utils/utils/box_utils/__init__.py
+deep_utils/utils/box_utils/box_dataclasses.py
 deep_utils/utils/box_utils/boxes.py
 deep_utils/utils/coco_utils/__init__.py
 deep_utils/utils/coco_utils/main.py
 deep_utils/utils/color_utils/__init__.py
 deep_utils/utils/color_utils/color_utils.py
 deep_utils/utils/compress_utils/__init__.py
 deep_utils/utils/compress_utils/zip_utils.py
@@ -174,21 +189,21 @@
 deep_utils/utils/multi_label_utils/stratify/__init__.py
 deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py
 deep_utils/utils/np_utils/__init__.py
 deep_utils/utils/np_utils/main_np.py
 deep_utils/utils/object_utils/__init__.py
 deep_utils/utils/object_utils/object_utils.py
 deep_utils/utils/opencv_utils/__init__.py
-deep_utils/utils/opencv_utils/main.py
+deep_utils/utils/opencv_utils/opencv_utils.py
 deep_utils/utils/optimizers/__init__.py
 deep_utils/utils/optimizers/tf.py
 deep_utils/utils/os_utils/__init__.py
 deep_utils/utils/os_utils/os_path.py
 deep_utils/utils/pickle_utils/__init__.py
-deep_utils/utils/pickle_utils/pickles.py
+deep_utils/utils/pickle_utils/pickle_utils.py
 deep_utils/utils/postgresql_utils/__init__.py
 deep_utils/utils/postgresql_utils/postgresql_utils.py
 deep_utils/utils/random_utils/__init__.py
 deep_utils/utils/random_utils/random_utils.py
 deep_utils/utils/re_utils/__init__.py
 deep_utils/utils/re_utils/re_utils.py
 deep_utils/utils/requests_utils/__init__.py
@@ -207,21 +222,25 @@
 deep_utils/utils/tf_utils/logging.py
 deep_utils/utils/tf_utils/main.py
 deep_utils/utils/torch_utils/__init__.py
 deep_utils/utils/torch_utils/torch_utils.py
 deep_utils/utils/utils/__init__.py
 deep_utils/utils/utils/arg_parser.py
 deep_utils/utils/utils/hyper_parameters.py
-deep_utils/utils/utils/seeds.py
 deep_utils/utils/utils/shuffle_utils.py
 deep_utils/utils/utils/str_utils.py
 deep_utils/utils/utils/yaml_utils.py
 deep_utils/utils/variable_naming_utils/__init__.py
 deep_utils/utils/variable_naming_utils/variable_naming_utils.py
 deep_utils/vision/__init__.py
+deep_utils/vision/color_recognition/__init__.py
+deep_utils/vision/color_recognition/cnn_color/__init__.py
+deep_utils/vision/color_recognition/cnn_color/torch/__init__.py
+deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch.py
+deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch_pred.py
 deep_utils/vision/face_detection/__init__.py
 deep_utils/vision/face_detection/haarcascade/__init__.py
 deep_utils/vision/face_detection/haarcascade/cv2_/__init__.py
 deep_utils/vision/face_detection/haarcascade/cv2_/config.py
 deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py
 deep_utils/vision/face_detection/main/__init__.py
 deep_utils/vision/face_detection/main/main_face_detection.py
@@ -292,14 +311,22 @@
 deep_utils/vision/face_recognition/main/main_face_recognition.py
 deep_utils/vision/face_recognition/vggface2/__init__.py
 deep_utils/vision/face_recognition/vggface2/torch/__init__.py
 deep_utils/vision/face_recognition/vggface2/torch/config.py
 deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py
 deep_utils/vision/face_recognition/vggface2/torch/src/__init__.py
 deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py
+deep_utils/vision/image_caption/__init__.py
+deep_utils/vision/image_caption/image_caption.py
+deep_utils/vision/image_caption/blip/__init__.py
+deep_utils/vision/image_caption/blip/torch/__init__.py
+deep_utils/vision/image_caption/blip/torch/blip_torch_image_caption.py
+deep_utils/vision/image_editing/__init__.py
+deep_utils/vision/image_editing/glide/__init__.py
+deep_utils/vision/image_editing/glide/glide_image_editing.py
 deep_utils/vision/object_detection/__init__.py
 deep_utils/vision/object_detection/main/__init__.py
 deep_utils/vision/object_detection/main/main_object_detection.py
 deep_utils/vision/object_detection/yolo/__init__.py
 deep_utils/vision/object_detection/yolo/yolo_detector.py
 deep_utils/vision/object_detection/yolo/v5/__init__.py
 deep_utils/vision/object_detection/yolo/v5/torch/__init__.py
@@ -376,14 +403,17 @@
 deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py
 deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py
 deep_utils/vision/ocr/__init__.py
 deep_utils/vision/ocr/crnn/__init__.py
 deep_utils/vision/ocr/crnn/torch/__init__.py
 deep_utils/vision/ocr/crnn/torch/crnn_inference.py
 deep_utils/vision/ocr/crnn/torch/crnn_model.py
+deep_utils/vision/text2box_visual_grounding/__init__.py
+deep_utils/vision/text2box_visual_grounding/dino/__init__.py
+deep_utils/vision/text2box_visual_grounding/dino/visual_grounding_dino_torch.py
 deep_utils/vision/torch_vision/__init__.py
 deep_utils/vision/torch_vision/torch_vision_inference/__init__.py
 deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py
 deep_utils/vision/torch_vision/torch_vision_models/__init__.py
 deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py
 deep_utils/vision/vision_utils/__init__.py
 deep_utils/vision/vision_utils/torch_vision_utils/__init__.py
```

### Comparing `deep_utils-1.0.2/setup.py` & `deep_utils-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "1.0.2"
+VERSION = "1.2.0"
 
 try:
     import pypandoc
 
     long_description = pypandoc.convert("Readme.md", "rst")
 except (IOError, ImportError):
     long_description = open("Readme.md", mode="r", encoding="utf-8").read()
```

### Comparing `deep_utils-1.0.2/tests/utils/encoding_utils/encoding_utils_test.py` & `deep_utils-1.2.0/tests/utils/encoding_utils/encoding_utils_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/tests/utils/np_utils/np_utils_test.py` & `deep_utils-1.2.0/tests/utils/np_utils/np_utils_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/tests/utils/resize_utils/resize_utils_test.py` & `deep_utils-1.2.0/tests/utils/resize_utils/resize_utils_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py` & `deep_utils-1.2.0/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py` & `deep_utils-1.2.0/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py` & `deep_utils-1.2.0/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.0.2/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py` & `deep_utils-1.2.0/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py`

 * *Files identical despite different names*

