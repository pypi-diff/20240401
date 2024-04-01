# Comparing `tmp/deep_utils-1.3.8.tar.gz` & `tmp/deep_utils-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_utils-1.3.8.tar", last modified: Wed Dec  6 06:19:50 2023, max compression
+gzip compressed data, was "deep_utils-1.3.9.tar", last modified: Fri Dec 22 21:25:56 2023, max compression
```

## Comparing `deep_utils-1.3.8.tar` & `deep_utils-1.3.9.tar`

### file list

```diff
@@ -1,659 +1,662 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.685301 deep_utils-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-06 06:19:41.000000 deep_utils-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26630 2023-12-06 06:19:50.685301 deep_utils-1.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.617301 deep_utils-1.3.8/deep_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/asr/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/asr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/asr/wav2vec2/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/asr/wav2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/asr/wav2vec2/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/asr/wav2vec2/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/asr/wav2vec2/torch/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/audio_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/audio_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/audio_utils/librosa_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/audio_utils/torchaudio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/audio_utils/vox_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/classification/wav2vec2/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/classification/wav2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/classification/wav2vec2/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/classification/wav2vec2/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/diarization/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/diarization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/diarization/pyannote/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/diarization/pyannote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/vad/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/vad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/audio/vad/pyannote/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/vad/pyannote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/augmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/augmentation/cutmix/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/augmentation/cutmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/augmentation/cutmix/cutmix_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/augmentation/cutmix/cutmix_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/augmentation/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/augmentation/torch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8071 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/augmentation/torch/augmentation_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/blocks/tf/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/blocks/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/blocks/tf/blocks_tf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/blocks/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/blocks/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/blocks/torch/blocks_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/callbacks/tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/callbacks/tf_keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/callbacks/tf_keras/lr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/callbacks/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/callbacks/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/callbacks/torch/torch_csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/callbacks/torch/torch_model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/callbacks/torch/torch_tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/design_patterns/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/design_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/design_patterns/chain_of_responsibility/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/design_patterns/chain_of_responsibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/dummy_objects/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/dummy_objects/audio/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/dummy_objects/audio/asr/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/audio/asr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/dummy_objects/audio/asr/wave2vec2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/audio/asr/wave2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/dummy_objects/audio/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/audio/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/dummy_objects/audio/classification/wav2vec2/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/audio/classification/wav2vec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.625301 deep_utils-1.3.8/deep_utils/dummy_objects/audio/diarization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/audio/diarization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/audio/diarization/pyannote/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/audio/diarization/pyannote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/audio/utils_/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/audio/utils_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/audio/vad/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/audio/vad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/audio/vad/pyannote/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/audio/vad/pyannote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/augmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/augmentation/cutmix/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/augmentation/cutmix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/blocks/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/blocks/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/callbacks/tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/callbacks/tf_keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/dummies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/dummy_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/elasticsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/utils/git_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/utils/git_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/utils/memory_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/utils/memory_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/utils/sqlalchemy_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/utils/sqlalchemy_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/utils/torch_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/utils/torch_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/vision/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/vision/face_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/vision/face_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/vision/face_recognition/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/vision/face_recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/vision/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/vision/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/vision/object_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/vision/object_tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/vision/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/vision/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/vision/ocr/crnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/vision/ocr/crnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/vision/ocr/crnn/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/vision/ocr/crnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/vision/torch_vision/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/vision/torch_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/vision/vision_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/vision/vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/dummy_objects/vision/vision_utils/torch_vision_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/dummy_objects/vision/vision_utils/torch_vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.629301 deep_utils-1.3.8/deep_utils/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/elasticsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/elasticsearch/search_engine/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/elasticsearch/search_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23209 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/gis/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/gis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/gis/projection/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/gis/projection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/gis/projection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/main_abs/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/main_abs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/main_abs/cv2/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/main_abs/cv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/main_abs/cv2/cv2_caffe.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/main_abs/cv2/cv2_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/main_abs/cv2/cv2_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/main_abs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/main_abs/main_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/medical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/medical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/medical/nib_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/medical/nib_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/medical/nib_utils/nib_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/medical/sitk_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/medical/sitk_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/medical/sitk_utils/sitk_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/multi_modals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/multi_modals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/multi_modals/_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/multi_modals/_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10566 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/models/blip.py
--rw-r--r--   0 runner    (1001) docker     (127)    41523 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/models/med.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/models/med_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.633301 deep_utils-1.3.8/deep_utils/nlp/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/nlp/ner/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10689 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/ner/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/ner/base_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/ner/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/ner/taggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/ner/utils_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/nlp/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/nlp/utils/multi_lang_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/utils/multi_lang_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/utils/multi_lang_utils/multi_lang_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/nlp/utils/persian/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/utils/persian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/nlp/utils/persian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/preprocessing/monai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/preprocessing/monai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/preprocessing/monai/monai_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/utils/algorithm_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/algorithm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/algorithm_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/utils/box_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/box_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/box_utils/box_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)    36114 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/box_utils/boxes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/utils/coco_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/coco_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9287 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/coco_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/utils/color_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/color_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/color_utils/color_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/utils/compress_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/compress_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/compress_utils/zip_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.637301 deep_utils-1.3.8/deep_utils/utils/ctc_decoder/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/ctc_decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7673 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/ctc_decoder/ctc_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.641301 deep_utils-1.3.8/deep_utils/utils/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/decorators/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.641301 deep_utils-1.3.8/deep_utils/utils/dict_named_tuple_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/dict_named_tuple_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.641301 deep_utils-1.3.8/deep_utils/utils/dict_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/dict_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/dict_utils/dict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.641301 deep_utils-1.3.8/deep_utils/utils/dir_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/dir_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21118 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/dir_utils/dir_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.641301 deep_utils-1.3.8/deep_utils/utils/download_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/download_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/download_utils/download_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.641301 deep_utils-1.3.8/deep_utils/utils/encodes/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/encodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/encodes/b64.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/encodes/web_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.641301 deep_utils-1.3.8/deep_utils/utils/gif_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/gif_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/gif_utils/gif_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.641301 deep_utils-1.3.8/deep_utils/utils/hash_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/hash_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/hash_utils/hash_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.641301 deep_utils-1.3.8/deep_utils/utils/image_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/image_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/image_utils/image_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.641301 deep_utils-1.3.8/deep_utils/utils/json_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/json_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/json_utils/json_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.641301 deep_utils-1.3.8/deep_utils/utils/kafka_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/kafka_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/kafka_utils/kafka_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/lib_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/lib_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/lib_utils/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/lib_utils/integeration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/lib_utils/lib_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/lib_utils/main_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/list_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/list_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/list_utils/list_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/logging_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/logging_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7135 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/logging_utils/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/lr_scheduler_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/lr_scheduler_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/lr_scheduler_utils/warmup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/matplotlib_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/matplotlib_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/matplotlib_utils/bar_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/matplotlib_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/memory_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/memory_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/memory_utils/torch_memory_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/minio_lib/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/minio_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/minio_lib/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/multi_label_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/multi_label_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/multi_label_utils/stratify/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/multi_label_utils/stratify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/np_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/np_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/np_utils/main_np.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/object_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/object_utils/object_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/opencv_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/opencv_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/opencv_utils/opencv_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/optimizers/tf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.645301 deep_utils-1.3.8/deep_utils/utils/os_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/os_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/os_utils/os_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/pickle_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/pickle_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/pickle_utils/pickle_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/postgresql_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/postgresql_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/postgresql_utils/postgresql_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/py_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/py_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/py_utils/py_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/qdrant_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/qdrant_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/qdrant_utils/qdrant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/random_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/random_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/random_utils/random_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/re_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/re_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/re_utils/re_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/requests_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/requests_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/requests_utils/requests_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/resize_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/resize_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/resize_utils/main_resize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/shutil_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/shutil_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/shutil_utils/shutil_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/sqlalchemy/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/sqlalchemy/insert.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/tensorboard_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/tensorboard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/tf_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/tf_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/tf_utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/tf_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.649301 deep_utils-1.3.8/deep_utils/utils/torch_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/torch_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/torch_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/utils/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/utils/hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/utils/shuffle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/utils/yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/utils/variable_naming_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/variable_naming_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/utils/variable_naming_utils/variable_naming_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/vision/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/vision/color_recognition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/color_recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/vision/color_recognition/cnn_color/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/color_recognition/cnn_color/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/vision/color_recognition/cnn_color/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/color_recognition/cnn_color/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch_pred.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/vision/face_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/vision/face_detection/haarcascade/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/haarcascade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/vision/face_detection/haarcascade/cv2_/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/haarcascade/cv2_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/haarcascade/cv2_/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/vision/face_detection/main/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/main/main_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.653301 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/net.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13383 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.657301 deep_utils-1.3.8/deep_utils/vision/face_detection/ssd/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ssd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.661301 deep_utils-1.3.8/deep_utils/vision/face_detection/ssd/cv2/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ssd/cv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.661301 deep_utils-1.3.8/deep_utils/vision/face_detection/ssd/cv2/caffe/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ssd/cv2/caffe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.661301 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.661301 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.661301 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/utils/op.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.661301 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9270 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py
--rw-r--r--   0 runner    (1001) docker     (127)    18077 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/face_recognition/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_recognition/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/face_recognition/main/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_recognition/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_recognition/main/main_face_recognition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/torch/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/torch/src/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/torch/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5859 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/image_caption/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/image_caption/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/image_caption/blip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/image_caption/blip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/image_caption/blip/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/image_caption/blip/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/image_caption/blip/torch/blip_torch_image_caption.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/image_caption/image_caption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/image_editing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/image_editing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/image_editing/glide/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/image_editing/glide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13150 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/image_editing/glide/glide_image_editing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/object_detection/main/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/main/main_object_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.665301 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.669301 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/models/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    42372 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4435 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    27031 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18183 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.669301 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    17021 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    55706 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    48196 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)    46792 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    14576 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    24456 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.673301 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)    13798 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    19648 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.673301 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.673301 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.673301 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/models/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84416 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10905 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    40059 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.677301 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (127)    56265 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    36907 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    75043 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    10167 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20998 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    15474 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19151 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/yolo_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.677301 deep_utils-1.3.8/deep_utils/vision/object_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.677301 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.677301 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.677301 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/deep/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.677301 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     8059 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5449 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.677301 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12138 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.677301 deep_utils-1.3.8/deep_utils/vision/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.677301 deep_utils-1.3.8/deep_utils/vision/ocr/crnn/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/ocr/crnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.677301 deep_utils-1.3.8/deep_utils/vision/ocr/crnn/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/ocr/crnn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/ocr/crnn/torch/crnn_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/ocr/crnn/torch/crnn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/deep_utils/vision/text2box_visual_grounding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/text2box_visual_grounding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/deep_utils/vision/text2box_visual_grounding/dino/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/text2box_visual_grounding/dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/text2box_visual_grounding/dino/visual_grounding_dino_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/deep_utils/vision/torch_vision/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/torch_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/deep_utils/vision/torch_vision/torch_vision_inference/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/torch_vision/torch_vision_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/deep_utils/vision/torch_vision/torch_vision_models/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/torch_vision/torch_vision_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/deep_utils/vision/vision_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/deep_utils/vision/vision_utils/torch_vision_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/vision_utils/torch_vision_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-12-06 06:19:41.000000 deep_utils-1.3.8/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.621301 deep_utils-1.3.8/deep_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26630 2023-12-06 06:19:50.000000 deep_utils-1.3.8/deep_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23630 2023-12-06 06:19:50.000000 deep_utils-1.3.8/deep_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 06:19:50.000000 deep_utils-1.3.8/deep_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-12-06 06:19:50.000000 deep_utils-1.3.8/deep_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-06 06:19:50.000000 deep_utils-1.3.8/deep_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-06 06:19:50.685301 deep_utils-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-12-06 06:19:41.000000 deep_utils-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/utils/encoding_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/utils/encoding_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/utils/encoding_utils/encoding_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/utils/np_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/utils/np_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/utils/np_utils/np_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/utils/resize_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/utils/resize_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/utils/resize_utils/resize_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/utils/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/vision/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/vision/face_detection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/face_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/vision/face_detection/mtcnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/face_detection/mtcnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/vision/face_detection/mtcnn/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/face_detection/mtcnn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/vision/face_detection/ultralight/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/face_detection/ultralight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.681301 deep_utils-1.3.8/tests/vision/face_detection/ultralight/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/face_detection/ultralight/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.685301 deep_utils-1.3.8/tests/vision/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/object_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.685301 deep_utils-1.3.8/tests/vision/object_detection/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/object_detection/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.685301 deep_utils-1.3.8/tests/vision/object_detection/yolo/v5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/object_detection/yolo/v5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.685301 deep_utils-1.3.8/tests/vision/object_detection/yolo/v5/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/object_detection/yolo/v5/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.685301 deep_utils-1.3.8/tests/vision/vision_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/vision_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:50.685301 deep_utils-1.3.8/tests/vision/vision_utils/torch_vision_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/vision_utils/torch_vision_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-12-06 06:19:41.000000 deep_utils-1.3.8/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-22 21:25:42.000000 deep_utils-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26630 2023-12-22 21:25:56.242109 deep_utils-1.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.170109 deep_utils-1.3.9/deep_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.170109 deep_utils-1.3.9/deep_utils/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.170109 deep_utils-1.3.9/deep_utils/audio/asr/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/asr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.170109 deep_utils-1.3.9/deep_utils/audio/asr/wav2vec2/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/asr/wav2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.170109 deep_utils-1.3.9/deep_utils/audio/asr/wav2vec2/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/asr/wav2vec2/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/asr/wav2vec2/torch/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/audio/audio_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/audio_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/audio_utils/librosa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/audio_utils/torchaudio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/audio_utils/vox_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/audio/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/audio/classification/wav2vec2/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/classification/wav2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/audio/classification/wav2vec2/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/classification/wav2vec2/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/audio/diarization/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/diarization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/audio/diarization/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/diarization/pyannote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/audio/vad/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/vad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/audio/vad/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/vad/pyannote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/augmentation/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/augmentation/cutmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/augmentation/cutmix/cutmix_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/augmentation/cutmix/cutmix_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/augmentation/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/augmentation/torch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8071 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/augmentation/torch/augmentation_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/blocks/tf/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/blocks/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/blocks/tf/blocks_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/blocks/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/blocks/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/blocks/torch/blocks_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.174109 deep_utils-1.3.9/deep_utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/callbacks/tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/callbacks/tf_keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/callbacks/tf_keras/lr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/callbacks/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/callbacks/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/callbacks/torch/torch_csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/callbacks/torch/torch_model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/callbacks/torch/torch_tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/design_patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/design_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/design_patterns/chain_of_responsibility/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/design_patterns/chain_of_responsibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/audio/asr/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/audio/asr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/audio/asr/wave2vec2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/audio/asr/wave2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/audio/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/audio/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/audio/classification/wav2vec2/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/audio/classification/wav2vec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/audio/diarization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/audio/diarization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/audio/diarization/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/audio/diarization/pyannote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/audio/utils_/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/audio/utils_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/audio/vad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/audio/vad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/audio/vad/pyannote/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/audio/vad/pyannote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/augmentation/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/augmentation/cutmix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/blocks/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/blocks/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.178109 deep_utils-1.3.9/deep_utils/dummy_objects/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/callbacks/tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/callbacks/tf_keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/dummies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/dummy_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/elasticsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/utils/git_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/utils/git_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/utils/memory_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/utils/memory_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/utils/sqlalchemy_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/utils/sqlalchemy_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/utils/torch_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/utils/torch_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/vision/face_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/vision/face_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/vision/face_recognition/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/vision/face_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/vision/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/vision/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/vision/object_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/vision/object_tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/vision/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/vision/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/vision/ocr/crnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/vision/ocr/crnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/vision/ocr/crnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/vision/ocr/crnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/vision/torch_vision/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/vision/torch_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/vision/vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/vision/vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/dummy_objects/vision/vision_utils/torch_vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/dummy_objects/vision/vision_utils/torch_vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/elasticsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/elasticsearch/search_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/elasticsearch/search_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23864 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/gis/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/gis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/gis/projection/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/gis/projection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/gis/projection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.182109 deep_utils-1.3.9/deep_utils/main_abs/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/main_abs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/main_abs/cv2/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/main_abs/cv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/main_abs/cv2/cv2_caffe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/main_abs/cv2/cv2_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/main_abs/cv2/cv2_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/main_abs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/main_abs/main_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/medical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/medical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/medical/nib_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/medical/nib_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/medical/nib_utils/nib_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/medical/sitk_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/medical/sitk_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/medical/sitk_utils/sitk_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/multi_modals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/multi_modals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/multi_modals/_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/multi_modals/_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10566 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/models/blip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41523 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/models/med.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/models/med_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/nlp/ner/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/ner/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/ner/base_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/ner/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/ner/taggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/ner/utils_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.186109 deep_utils-1.3.9/deep_utils/nlp/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/nlp/utils/multi_lang_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/utils/multi_lang_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/utils/multi_lang_utils/multi_lang_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/nlp/utils/persian/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/utils/persian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/nlp/utils/persian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/preprocessing/monai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/preprocessing/monai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/preprocessing/monai/monai_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/utils/algorithm_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/algorithm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/algorithm_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/utils/box_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/box_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/box_utils/box_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36114 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/box_utils/boxes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/utils/coco_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/coco_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9287 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/coco_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/utils/color_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/color_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/color_utils/color_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/utils/compress_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/compress_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/compress_utils/zip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/utils/ctc_decoder/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/ctc_decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7673 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/ctc_decoder/ctc_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.190109 deep_utils-1.3.9/deep_utils/utils/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/decorators/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/dict_named_tuple_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/dict_named_tuple_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/dict_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/dict_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/dict_utils/dict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/dir_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/dir_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21228 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/dir_utils/dir_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/download_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/download_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/download_utils/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/encodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/encodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/encodes/b64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/encodes/web_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/fa_nlp_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/fa_nlp_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/fa_nlp_utils/fa_nlp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/gif_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/gif_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/gif_utils/gif_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/hash_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/hash_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/hash_utils/hash_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/image_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/image_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/image_utils/image_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/json_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/json_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/json_utils/json_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/kafka_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/kafka_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/kafka_utils/kafka_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.194109 deep_utils-1.3.9/deep_utils/utils/lib_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/lib_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/lib_utils/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/lib_utils/integeration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/lib_utils/lib_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/lib_utils/main_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/list_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/list_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/list_utils/list_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/logging_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/logging_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7135 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/logging_utils/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/lr_scheduler_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/lr_scheduler_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/lr_scheduler_utils/warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/matplotlib_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/matplotlib_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/matplotlib_utils/bar_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/matplotlib_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/memory_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/memory_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/memory_utils/torch_memory_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/minio_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/minio_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/minio_lib/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/multi_label_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/multi_label_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/multi_label_utils/stratify/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/multi_label_utils/stratify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/np_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/np_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/np_utils/main_np.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/object_utils/object_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/opencv_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/opencv_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/opencv_utils/opencv_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/optimizers/tf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.198109 deep_utils-1.3.9/deep_utils/utils/os_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/os_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/os_utils/os_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.202109 deep_utils-1.3.9/deep_utils/utils/pickle_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/pickle_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/pickle_utils/pickle_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.202109 deep_utils-1.3.9/deep_utils/utils/postgresql_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/postgresql_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/postgresql_utils/postgresql_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.202109 deep_utils-1.3.9/deep_utils/utils/py_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/py_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/py_utils/py_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.202109 deep_utils-1.3.9/deep_utils/utils/qdrant_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/qdrant_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/qdrant_utils/qdrant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.202109 deep_utils-1.3.9/deep_utils/utils/random_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/random_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/random_utils/random_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.202109 deep_utils-1.3.9/deep_utils/utils/re_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/re_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/re_utils/re_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.202109 deep_utils-1.3.9/deep_utils/utils/requests_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/requests_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/requests_utils/requests_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.202109 deep_utils-1.3.9/deep_utils/utils/resize_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/resize_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/resize_utils/main_resize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.202109 deep_utils-1.3.9/deep_utils/utils/shutil_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/shutil_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/shutil_utils/shutil_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.202109 deep_utils-1.3.9/deep_utils/utils/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/sqlalchemy/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/sqlalchemy/insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.202109 deep_utils-1.3.9/deep_utils/utils/tensorboard_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/tensorboard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/utils/tf_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/tf_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/tf_utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/tf_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/utils/torch_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/torch_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/torch_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/utils/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/utils/hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/utils/shuffle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/utils/yaml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/utils/variable_naming_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/variable_naming_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/utils/variable_naming_utils/variable_naming_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/vision/color_recognition/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/color_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/vision/color_recognition/cnn_color/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/color_recognition/cnn_color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/vision/color_recognition/cnn_color/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/color_recognition/cnn_color/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch_pred.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/vision/face_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/vision/face_detection/haarcascade/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/haarcascade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/vision/face_detection/haarcascade/cv2_/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/haarcascade/cv2_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/haarcascade/cv2_/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/vision/face_detection/main/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/main/main_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.206109 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.210109 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.210109 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.210109 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.210109 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.210109 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.210109 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.210109 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.210109 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.210109 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.210109 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.214109 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13383 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.214109 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.214109 deep_utils-1.3.9/deep_utils/vision/face_detection/ssd/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ssd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.214109 deep_utils-1.3.9/deep_utils/vision/face_detection/ssd/cv2/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ssd/cv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.214109 deep_utils-1.3.9/deep_utils/vision/face_detection/ssd/cv2/caffe/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ssd/cv2/caffe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.214109 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.214109 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.214109 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/utils/op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.214109 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.218109 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9270 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18077 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.218109 deep_utils-1.3.9/deep_utils/vision/face_recognition/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_recognition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.218109 deep_utils-1.3.9/deep_utils/vision/face_recognition/main/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_recognition/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_recognition/main/main_face_recognition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.218109 deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.218109 deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/torch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.218109 deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/torch/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/torch/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5859 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.218109 deep_utils-1.3.9/deep_utils/vision/image_caption/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/image_caption/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.218109 deep_utils-1.3.9/deep_utils/vision/image_caption/blip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/image_caption/blip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.218109 deep_utils-1.3.9/deep_utils/vision/image_caption/blip/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/image_caption/blip/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/image_caption/blip/torch/blip_torch_image_caption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/image_caption/image_caption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.218109 deep_utils-1.3.9/deep_utils/vision/image_editing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/image_editing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.218109 deep_utils-1.3.9/deep_utils/vision/image_editing/glide/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/image_editing/glide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13150 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/image_editing/glide/glide_image_editing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.222109 deep_utils-1.3.9/deep_utils/vision/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.222109 deep_utils-1.3.9/deep_utils/vision/object_detection/main/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/main/main_object_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.222109 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.222109 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.222109 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.222109 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42372 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4435 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27031 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18183 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.226109 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17021 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55706 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48196 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46792 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14576 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24456 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.226109 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19648 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.226109 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.226109 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.226109 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84416 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10905 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40059 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.230109 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56265 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36907 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75043 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10167 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20998 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15474 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19151 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/yolo_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.230109 deep_utils-1.3.9/deep_utils/vision/object_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.230109 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.230109 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.230109 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/deep/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5449 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12138 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/ocr/crnn/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/ocr/crnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/ocr/crnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/ocr/crnn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/ocr/crnn/torch/crnn_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/ocr/crnn/torch/crnn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/text2box_visual_grounding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/text2box_visual_grounding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/text2box_visual_grounding/dino/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/text2box_visual_grounding/dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/text2box_visual_grounding/dino/visual_grounding_dino_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/torch_vision/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/torch_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/torch_vision/torch_vision_inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/torch_vision/torch_vision_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/torch_vision/torch_vision_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/torch_vision/torch_vision_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.234109 deep_utils-1.3.9/deep_utils/vision/vision_utils/torch_vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/vision_utils/torch_vision_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2023-12-22 21:25:42.000000 deep_utils-1.3.9/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.170109 deep_utils-1.3.9/deep_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26630 2023-12-22 21:25:55.000000 deep_utils-1.3.9/deep_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23718 2023-12-22 21:25:56.000000 deep_utils-1.3.9/deep_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 21:25:55.000000 deep_utils-1.3.9/deep_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2023-12-22 21:25:55.000000 deep_utils-1.3.9/deep_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-22 21:25:55.000000 deep_utils-1.3.9/deep_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-22 21:25:56.242109 deep_utils-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-12-22 21:25:42.000000 deep_utils-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/utils/encoding_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/utils/encoding_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/utils/encoding_utils/encoding_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/utils/np_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/utils/np_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/utils/np_utils/np_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/utils/resize_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/utils/resize_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/utils/resize_utils/resize_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/utils/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/face_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/face_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/face_detection/mtcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/face_detection/mtcnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/face_detection/mtcnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/face_detection/mtcnn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/face_detection/ultralight/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/face_detection/ultralight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/face_detection/ultralight/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/face_detection/ultralight/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/object_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/object_detection/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/object_detection/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/object_detection/yolo/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/object_detection/yolo/v5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/object_detection/yolo/v5/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/object_detection/yolo/v5/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/vision_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:56.238109 deep_utils-1.3.9/tests/vision/vision_utils/torch_vision_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/vision_utils/torch_vision_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-12-22 21:25:42.000000 deep_utils-1.3.9/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py
```

### Comparing `deep_utils-1.3.8/LICENSE` & `deep_utils-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/PKG-INFO` & `deep_utils-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deep_utils
-Version: 1.3.8
+Version: 1.3.9
 Summary: Deep Utils
 Home-page: https://github.com/pooya-mohammadi/deep_utils
 Author: Pooya Mohammadi Kazaj
 Author-email: pooyamohammadikazaj@gmial.com
 License: UNKNOWN
-Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.3.8.tar.gz
+Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.3.9.tar.gz
 Description: [![Downloads](https://static.pepy.tech/badge/deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
         
         <div id="top"></div>
         <!-- PROJECT LOGO -->
         <br />
         <div align="center">
           <a href="https://github.com/pooya-mohammadi/deep_utils">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: deep_utils Version: 1.3.8 Summary: Deep Utils Home-
+Metadata-Version: 2.1 Name: deep_utils Version: 1.3.9 Summary: Deep Utils Home-
 page: https://github.com/pooya-mohammadi/deep_utils Author: Pooya Mohammadi
 Kazaj Author-email: pooyamohammadikazaj@gmial.com License: UNKNOWN Download-
 URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/
-1.3.8.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
+1.3.9.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
 deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://
 img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
 
                                     _[_L_o_g_o_]
                              ******** DDeeeepp UUttiillss ********
                   A toolkit for deep-learning practitioners!
 This repository contains the most frequently used deep learning models and
```

### Comparing `deep_utils-1.3.8/deep_utils/__init__.py` & `deep_utils-1.3.9/deep_utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TYPE_CHECKING
 
 from deep_utils.dummy_objects.dummy_framework import LazyModule
 from .utils.lib_utils.integeration_utils import import_lazy_module
 
 # Deep Utils version number
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 
 from .utils.constants import DUMMY_PATH, Backends
 
 # no third-party python libraries are required for the following classes
 _import_structure = {
     "utils.box_utils.boxes": ["Box", "Point"],
     "utils.box_utils.box_dataclasses": ["BoxDataClass", "PointDataClass"],
@@ -27,14 +27,15 @@
                                   "combine_directory_of_directories",
                                   "DirUtils"],
     "utils.logging_utils.logging_utils": ["get_logger"],
     "utils.lr_scheduler_utils.warmup": ["cosine_reduce", "warmup_cosine"],
     "utils.py_utils.py_utils": ["PyUtils"],
     "utils.json_utils.json_utils": ["JsonUtils"],
     "utils.pickle_utils.pickle_utils": ["PickleUtils"],
+    "utils.fa_nlp_utils.fa_nlp_utils": ['FaNLPUtils'],
     DUMMY_PATH: [],
 }
 
 import_lazy_module("SITKUtils", "medical/sitk_utils/sitk_utils")
 import_lazy_module("TFUtils", "utils.tf_utils.main")
 import_lazy_module('QdrantUtils', 'utils.qdrant_utils.qdrant_utils')
 import_lazy_module('DownloadUtils', 'utils.download_utils.download_utils')
@@ -54,14 +55,15 @@
 import_lazy_module('YOLOV5TorchObjectDetector', 'vision.object_detection.yolo.v5.torch.yolo_v5_torch_object_detection')
 import_lazy_module('YOLOV7TorchObjectDetector', 'vision.object_detection.yolo.v7.torch.yolo_v7_torch_object_detection')
 import_lazy_module('ColorRecognitionCNNTorchPrediction',
                    'vision.color_recognition.cnn_color.torch.color_cnn_torch_pred')
 import_lazy_module("CRNNInferenceTorch", "vision.ocr.crnn.torch.crnn_inference")
 import_lazy_module("CRNNModelTorch", "vision.ocr.crnn.torch.crnn_model")
 import_lazy_module("MTCNNTFFaceDetector", "vision.face_detection.mtcnn.tf.mtcnn_tf_face_detection")
+import_lazy_module("ElasticsearchEngin", "elasticsearch.search_engine.elasticsearch_search_engine")
 
 if TYPE_CHECKING:
     from .utils.box_utils.boxes import Box, Point
     from .vision.face_detection.haarcascade.cv2_.haarcascade_cv2_face_detection import HaarcascadeCV2FaceDetector
     from .vision.face_detection.mtcnn.tf.mtcnn_tf_face_detection import MTCNNTFFaceDetector
     from .vision.face_detection.mtcnn.torch.mtcnn_torch_face_detection import MTCNNTorchFaceDetector
     from .vision.face_detection.haarcascade.cv2_.haarcascade_cv2_face_detection import HaarcascadeCV2FaceDetector
@@ -91,14 +93,16 @@
     from .utils.download_utils.download_utils import DownloadUtils
     from .utils.lr_scheduler_utils.warmup import cosine_reduce, warmup_cosine
     from .utils.py_utils.py_utils import PyUtils
     from .utils.json_utils.json_utils import JsonUtils
     from .utils.qdrant_utils.qdrant_utils import QdrantUtils
     from .utils.pickle_utils.pickle_utils import PickleUtils
     from .medical.sitk_utils.sitk_utils import SITKUtils
+    from .utils.fa_nlp_utils.fa_nlp_utils import FaNLPUtils
+    from .elasticsearch.search_engine.elasticsearch_search_engine import ElasticsearchEngin
 else:
     import sys
 
     sys.modules[__name__] = LazyModule(
         __name__,
         globals()["__file__"],
         _import_structure,
```

### Comparing `deep_utils-1.3.8/deep_utils/audio/asr/wav2vec2/torch/main.py` & `deep_utils-1.3.9/deep_utils/audio/asr/wav2vec2/torch/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/audio/audio_utils/librosa_utils.py` & `deep_utils-1.3.9/deep_utils/audio/audio_utils/librosa_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/audio/audio_utils/torchaudio_utils.py` & `deep_utils-1.3.9/deep_utils/audio/audio_utils/torchaudio_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/audio/audio_utils/vox_utils.py` & `deep_utils-1.3.9/deep_utils/audio/audio_utils/vox_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py` & `deep_utils-1.3.9/deep_utils/audio/classification/wav2vec2/torch/audio_classification_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py` & `deep_utils-1.3.9/deep_utils/audio/diarization/pyannote/pyannote_audio_diarization.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py` & `deep_utils-1.3.9/deep_utils/audio/vad/pyannote/pyannote_audio_vad.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/augmentation/cutmix/cutmix_tf.py` & `deep_utils-1.3.9/deep_utils/augmentation/cutmix/cutmix_tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/augmentation/cutmix/cutmix_torch.py` & `deep_utils-1.3.9/deep_utils/augmentation/cutmix/cutmix_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/augmentation/torch/augmentation_torch.py` & `deep_utils-1.3.9/deep_utils/augmentation/torch/augmentation_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/blocks/tf/blocks_tf.py` & `deep_utils-1.3.9/deep_utils/blocks/tf/blocks_tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/blocks/torch/blocks_torch.py` & `deep_utils-1.3.9/deep_utils/blocks/torch/blocks_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/callbacks/tf_keras/lr.py` & `deep_utils-1.3.9/deep_utils/callbacks/tf_keras/lr.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/callbacks/torch/torch_csv_logger.py` & `deep_utils-1.3.9/deep_utils/callbacks/torch/torch_csv_logger.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/callbacks/torch/torch_model_checkpoint.py` & `deep_utils-1.3.9/deep_utils/callbacks/torch/torch_model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/callbacks/torch/torch_tensorboard.py` & `deep_utils-1.3.9/deep_utils/callbacks/torch/torch_tensorboard.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py` & `deep_utils-1.3.9/deep_utils/design_patterns/chain_of_responsibility/chain_of_responsibilities_handlers.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/dummy_objects/dummies.py` & `deep_utils-1.3.9/deep_utils/dummy_objects/dummies.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,7 +89,11 @@
 class BlipTorchImageCaption(metaclass=DummyObject):
     _backend = [Backends.TORCH,
                 Backends.TORCHVISION,
                 Backends.TIMM,
                 Backends.TRANSFORMERS,
                 Backends.FAIRSCALE
                 ]
+
+
+class ElasticsearchEngin(metaclass=DummyObject):
+    _backend = [Backends.ELASTICSEARCH]
```

### Comparing `deep_utils-1.3.8/deep_utils/dummy_objects/dummy_framework.py` & `deep_utils-1.3.9/deep_utils/dummy_objects/dummy_framework.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/dummy_objects/utils/sqlalchemy_utils/__init__.py` & `deep_utils-1.3.9/deep_utils/dummy_objects/utils/sqlalchemy_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/dummy_objects/vision/face_detection/__init__.py` & `deep_utils-1.3.9/deep_utils/dummy_objects/vision/face_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/dummy_objects/vision/object_detection/__init__.py` & `deep_utils-1.3.9/deep_utils/dummy_objects/vision/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/dummy_objects/vision/object_tracker/__init__.py` & `deep_utils-1.3.9/deep_utils/dummy_objects/vision/object_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py` & `deep_utils-1.3.9/deep_utils/elasticsearch/search_engine/elasticsearch_search_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
-import random
 from typing import Dict, Union, List
+
 from elasticsearch import Elasticsearch, NotFoundError
+
+from deep_utils.utils.json_utils.json_utils import JsonUtils
 from deep_utils.utils.logging_utils.logging_utils import value_error_log
-from deep_utils.utils.json_utils.json_utils import dump_json
 
 
 class ElasticsearchEngin:
     def __init__(self, elastic_url="http://localhost:9200", es=None, timeout=10, logger=None, verbose=1):
         if es is None:
             self.es = Elasticsearch(elastic_url, timeout=timeout)
         elif isinstance(es, Elasticsearch):
@@ -108,15 +109,15 @@
                 return None, None
             return None
         if len(hits) > 1:
             value = hits[0]["_source"]
             province = value['province_name']
             city_name = value['name']
             os.makedirs("equals", exist_ok=True)
-            dump_json(f"equals/{province}_{city_name}.json", hits, ensure_ascii=False)
+            JsonUtils.dump_json(f"equals/{province}_{city_name}.json", hits, ensure_ascii=False)
             print(f"There are two objects with the same characteristics with the same name, {hits}")
             hits = [hits[0]]
 
         if len(hits) == 1:
             value = hits[0]["_source"]
             _id = value['id']
             if area_type:
@@ -382,23 +383,26 @@
         """
         query = self.get_query_multi_match_fuzzy(query_value=query_value, field_names=field_names, fuzziness=fuzziness)
         results = self.es.search(index=index_name, query=query, size=size)
         hits = ElasticsearchEngin.get_hits(results)
         return hits
 
     @staticmethod
-    def get_hits(results):
+    def get_hits(results, return_source: bool = False):
         """
         This is a simple method to extract hits or return none when the output of the search has no hits
         :param results:
+        :param return_source: If set to true the _source keyword will be returned!
         :return:
         """
         hits = results['hits']['hits']
         if len(hits) == 0:
             hits = None
+        elif return_source:
+            hits = [hit["_source"] for hit in hits]
         return hits
 
     def search_bool_must_fuzzy_query_geo_sort(self,
                                               field_term_dict: dict,
                                               index_name: str,
                                               lat: float,
                                               lon: float,
@@ -530,18 +534,37 @@
             query = {
                 keyword: {}
             }
         else:
             raise ValueError(f"keyword: {keyword} is not valid!")
         return query
 
-    def search_match_query(self, index_name, field_name="", field_value="", keyword="match", size=None):
+    def search_match_query(self, index_name, field_name="", field_value="", keyword="match", size=None,
+                           return_source: bool = False):
+        """
+        A simple match search
+        {
+        "query": {
+            "keyword": {
+                "field_name": "field_value"
+                     }
+                 }
+         }
+        :param index_name:
+        :param field_name:
+        :param field_value:
+        :param keyword:
+        :param size:
+        :param return_source:
+        :return:
+
+        """
         query = self.get_match_query(field_name=field_name, field_value=field_value, keyword=keyword)
         results = self.es.search(index=index_name, query=query, size=size).body
-        hits = ElasticsearchEngin.get_hits(results)
+        hits = ElasticsearchEngin.get_hits(results, return_source=return_source)
         return hits
 
     def search_by_id(self, index_name, id_value, id_field_name="_id") -> Union[dict, None]:
         hits = self.search_match_query(index_name, field_name=id_field_name, field_value=id_value, keyword="match",
                                        size=1)
         if len(hits) == 1:
             return hits[0]["_source"]
```

### Comparing `deep_utils-1.3.8/deep_utils/gis/projection/main.py` & `deep_utils-1.3.9/deep_utils/gis/projection/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/main_abs/cv2/cv2_caffe.py` & `deep_utils-1.3.9/deep_utils/main_abs/cv2/cv2_caffe.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/main_abs/cv2/cv2_main.py` & `deep_utils-1.3.9/deep_utils/main_abs/cv2/cv2_main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/main_abs/main.py` & `deep_utils-1.3.9/deep_utils/main_abs/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/main_abs/main_config.py` & `deep_utils-1.3.9/deep_utils/main_abs/main_config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/medical/sitk_utils/sitk_utils.py` & `deep_utils-1.3.9/deep_utils/medical/sitk_utils/sitk_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/models/blip.py` & `deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/models/blip.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/models/med.py` & `deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/models/med.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/models/med_configs.py` & `deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/models/med_configs.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/multi_modals/_models/blip/torch/models/vit.py` & `deep_utils-1.3.9/deep_utils/multi_modals/_models/blip/torch/models/vit.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/nlp/ner/augmentation.py` & `deep_utils-1.3.9/deep_utils/nlp/ner/augmentation.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/nlp/ner/base_operations.py` & `deep_utils-1.3.9/deep_utils/nlp/ner/base_operations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/nlp/ner/preprocessing.py` & `deep_utils-1.3.9/deep_utils/nlp/ner/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/nlp/ner/utils_.py` & `deep_utils-1.3.9/deep_utils/nlp/ner/utils_.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/nlp/utils/persian/utils.py` & `deep_utils-1.3.9/deep_utils/nlp/utils/persian/utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/preprocessing/monai/monai_segmentation.py` & `deep_utils-1.3.9/deep_utils/preprocessing/monai/monai_segmentation.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/algorithm_utils/main.py` & `deep_utils-1.3.9/deep_utils/utils/algorithm_utils/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/box_utils/boxes.py` & `deep_utils-1.3.9/deep_utils/utils/box_utils/boxes.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/coco_utils/main.py` & `deep_utils-1.3.9/deep_utils/utils/coco_utils/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/color_utils/color_utils.py` & `deep_utils-1.3.9/deep_utils/utils/color_utils/color_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/compress_utils/zip_utils.py` & `deep_utils-1.3.9/deep_utils/utils/compress_utils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/constants.py` & `deep_utils-1.3.9/deep_utils/utils/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -31,10 +31,11 @@
     CV2 = "cv2"
     GLIDE_TEXT2IM = "glide_text2im"
     GROUNDINGDINO = "groundingdino"
     MONAI = "monai"
     TORCHVISION = "torchvision"
     TIMM = "timm"
     FAIRSCALE = "fairscale"
+    ELASTICSEARCH = "elasticsearch"
 
     def __str__(self):
         return str(self.value)
```

### Comparing `deep_utils-1.3.8/deep_utils/utils/ctc_decoder/ctc_decoder.py` & `deep_utils-1.3.9/deep_utils/utils/ctc_decoder/ctc_decoder.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/decorators/main.py` & `deep_utils-1.3.9/deep_utils/utils/decorators/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py` & `deep_utils-1.3.9/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_37.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py` & `deep_utils-1.3.9/deep_utils/utils/dict_named_tuple_utils/dictnamedtuple_38.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/dict_utils/dict_utils.py` & `deep_utils-1.3.9/deep_utils/utils/dict_utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/dir_utils/dir_utils.py` & `deep_utils-1.3.9/deep_utils/utils/dir_utils/dir_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,14 +595,15 @@
         :param filter_directories: If set to True, return on objects and not directories. This won't work,
         if only_directories is set to True,
         :param interest_extensions: If provided, files that have this extension will be chosen!
         :param only_directories: If set to True, only directories are extracted and filter_directories is ignored.
         :return:
         """
         interest_extensions = [interest_extensions] if isinstance(interest_extensions, str) else interest_extensions
+        interest_extensions = [f".{ext}" if not ext.startswith(".") else ext  for ext in interest_extensions]
         output = []
         for filename in os.listdir(directory):
             file_path = join(directory, filename)
             if not only_directories:
                 if filter_directories and os.path.isdir(file_path):
                     continue
                 if interest_extensions and DirUtils.split_extension(file_path)[1] not in interest_extensions:
```

### Comparing `deep_utils-1.3.8/deep_utils/utils/download_utils/download_utils.py` & `deep_utils-1.3.9/deep_utils/utils/download_utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/encodes/b64.py` & `deep_utils-1.3.9/deep_utils/utils/encodes/b64.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/gif_utils/gif_utils.py` & `deep_utils-1.3.9/deep_utils/utils/gif_utils/gif_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/hash_utils/hash_utils.py` & `deep_utils-1.3.9/deep_utils/utils/hash_utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/image_utils/image_utils.py` & `deep_utils-1.3.9/deep_utils/utils/image_utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/json_utils/json_utils.py` & `deep_utils-1.3.9/deep_utils/utils/json_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/kafka_utils/kafka_utils.py` & `deep_utils-1.3.9/deep_utils/utils/kafka_utils/kafka_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/lib_utils/download_utils.py` & `deep_utils-1.3.9/deep_utils/utils/lib_utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/lib_utils/integeration_utils.py` & `deep_utils-1.3.9/deep_utils/utils/lib_utils/integeration_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/lib_utils/lib_decorators.py` & `deep_utils-1.3.9/deep_utils/utils/lib_utils/lib_decorators.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/lib_utils/main_utils.py` & `deep_utils-1.3.9/deep_utils/utils/lib_utils/main_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/logging_utils/logging_utils.py` & `deep_utils-1.3.9/deep_utils/utils/logging_utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/lr_scheduler_utils/warmup.py` & `deep_utils-1.3.9/deep_utils/utils/lr_scheduler_utils/warmup.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/matplotlib_utils/bar_plots.py` & `deep_utils-1.3.9/deep_utils/utils/matplotlib_utils/bar_plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/matplotlib_utils/main.py` & `deep_utils-1.3.9/deep_utils/utils/matplotlib_utils/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/memory_utils/torch_memory_utils.py` & `deep_utils-1.3.9/deep_utils/utils/memory_utils/torch_memory_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/minio_lib/main.py` & `deep_utils-1.3.9/deep_utils/utils/minio_lib/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py` & `deep_utils-1.3.9/deep_utils/utils/multi_label_utils/stratify/stratify_train_test_split.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/np_utils/main_np.py` & `deep_utils-1.3.9/deep_utils/utils/np_utils/main_np.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/object_utils/object_utils.py` & `deep_utils-1.3.9/deep_utils/utils/object_utils/object_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/opencv_utils/opencv_utils.py` & `deep_utils-1.3.9/deep_utils/utils/opencv_utils/opencv_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/optimizers/tf.py` & `deep_utils-1.3.9/deep_utils/utils/optimizers/tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/os_utils/os_path.py` & `deep_utils-1.3.9/deep_utils/utils/os_utils/os_path.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/postgresql_utils/postgresql_utils.py` & `deep_utils-1.3.9/deep_utils/utils/postgresql_utils/postgresql_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/py_utils/py_utils.py` & `deep_utils-1.3.9/deep_utils/utils/py_utils/py_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,16 @@
             "bright_magenta": "\033[95m",
             "bright_cyan": "\033[96m",
             "bright_white": "\033[97m",
             "end": "\033[0m",  # misc
             "bold": "\033[1m",
             "underline": "\033[4m",
         }
-        return (colors[color.lower()] if color is not None else "") + ("".join(colors[m.lower()] for m in mode) if mode is not None else "") + text + \
+        return (colors[color.lower()] if color is not None else "") + (
+            "".join(colors[m.lower()] for m in mode) if mode is not None else "") + text + \
             colors["end"]
 
     @staticmethod
     def print(*args, sep=' ', end='\n', file=None, color: Optional[str] = None, mode: Union[str, list] = None):
         """
         colorful print!
         :param args:
```

### Comparing `deep_utils-1.3.8/deep_utils/utils/qdrant_utils/qdrant_utils.py` & `deep_utils-1.3.9/deep_utils/utils/qdrant_utils/qdrant_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/re_utils/re_utils.py` & `deep_utils-1.3.9/deep_utils/utils/re_utils/re_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/requests_utils/requests_utils.py` & `deep_utils-1.3.9/deep_utils/utils/requests_utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/resize_utils/main_resize.py` & `deep_utils-1.3.9/deep_utils/utils/resize_utils/main_resize.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/shutil_utils/shutil_utils.py` & `deep_utils-1.3.9/deep_utils/utils/shutil_utils/shutil_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/sqlalchemy/__init__.py` & `deep_utils-1.3.9/deep_utils/utils/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/sqlalchemy/checks.py` & `deep_utils-1.3.9/deep_utils/utils/sqlalchemy/checks.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py` & `deep_utils-1.3.9/deep_utils/utils/sqlalchemy/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py` & `deep_utils-1.3.9/deep_utils/utils/tensorboard_utils/tesnsorboard_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/tf_utils/logging.py` & `deep_utils-1.3.9/deep_utils/utils/tf_utils/logging.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/tf_utils/main.py` & `deep_utils-1.3.9/deep_utils/utils/tf_utils/main.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/torch_utils/torch_utils.py` & `deep_utils-1.3.9/deep_utils/utils/torch_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/utils/hyper_parameters.py` & `deep_utils-1.3.9/deep_utils/utils/utils/hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/utils/shuffle_utils.py` & `deep_utils-1.3.9/deep_utils/utils/utils/shuffle_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/utils/utils/yaml_utils.py` & `deep_utils-1.3.9/deep_utils/utils/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch.py` & `deep_utils-1.3.9/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch_pred.py` & `deep_utils-1.3.9/deep_utils/vision/color_recognition/cnn_color/torch/color_cnn_torch_pred.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/__init__.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/haarcascade/cv2_/config.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/haarcascade/cv2_/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/haarcascade/cv2_/haarcascade_cv2_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/main/main_face_detection.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/main/main_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/config.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/mtcnn_tf_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/src/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/src/first_stage.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/tf/src/get_nets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/config.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/mtcnn_torch_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/src/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/src/first_stage.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/mtcnn/torch/src/get_nets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/config.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/retinaface_torch_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/layers/functions/prior_box.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/layers/modules/multibox_loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/load_model.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/net.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/net.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/retinaface.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/utils/nms/py_cpu_nms.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/retinaface/torch/src/utils/timer.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ssd/cv2/caffe/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ssd/cv2/caffe/ssd_cv2_caffe_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/ultralight_tf_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/utils/op.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/utils/op.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/utils/rfb_320.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/utils/slim_320.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/tf/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/config.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/ultralight_torch_face_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/box_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/fd_config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_RFB_fd.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/mb_tiny_fd.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/misc.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/predictor.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/ssd.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py` & `deep_utils-1.3.9/deep_utils/vision/face_detection/ultralight/torch/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_recognition/main/main_face_recognition.py` & `deep_utils-1.3.9/deep_utils/vision/face_recognition/main/main_face_recognition.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/torch/config.py` & `deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py` & `deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/torch/src/senet_model.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py` & `deep_utils-1.3.9/deep_utils/vision/face_recognition/vggface2/torch/vggface2_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/image_caption/blip/torch/blip_torch_image_caption.py` & `deep_utils-1.3.9/deep_utils/vision/image_caption/blip/torch/blip_torch_image_caption.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/image_caption/image_caption.py` & `deep_utils-1.3.9/deep_utils/vision/image_caption/image_caption.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/image_editing/glide/glide_image_editing.py` & `deep_utils-1.3.9/deep_utils/vision/image_editing/glide/glide_image_editing.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/__init__.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/main/main_object_detection.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/main/main_object_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/config.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/models/common.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/models/experimental.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/models/tf.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/models/yolo.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolo_v5_torch_object_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/activations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/downloads.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/general.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/augmentations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/dataloaders.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/general.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/segment/plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v5/torch/yolov5_utils/triton.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/config.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/config.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/models/common.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/models/experimental.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/models/yolo.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolo_v7_torch_object_detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/activations.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/general.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/loss.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/plots.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/v7/torch/yolov7_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_detection/yolo/yolo_detector.py` & `deep_utils-1.3.9/deep_utils/vision/object_detection/yolo/yolo_detector.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/__init__.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/__init__.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/deep_sort.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/detection.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/iou_matching.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/nn_matching.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/track.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/sort/tracker.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/draw.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/io.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/json_logger.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/parser.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py` & `deep_utils-1.3.9/deep_utils/vision/object_tracker/deep_sort/torch/utils/tools.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/ocr/crnn/torch/crnn_inference.py` & `deep_utils-1.3.9/deep_utils/vision/ocr/crnn/torch/crnn_inference.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/ocr/crnn/torch/crnn_model.py` & `deep_utils-1.3.9/deep_utils/vision/ocr/crnn/torch/crnn_model.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/text2box_visual_grounding/dino/visual_grounding_dino_torch.py` & `deep_utils-1.3.9/deep_utils/vision/text2box_visual_grounding/dino/visual_grounding_dino_torch.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py` & `deep_utils-1.3.9/deep_utils/vision/torch_vision/torch_vision_inference/torch_vision_inference.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py` & `deep_utils-1.3.9/deep_utils/vision/torch_vision/torch_vision_models/torch_vision_models.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py` & `deep_utils-1.3.9/deep_utils/vision/vision_utils/torch_vision_utils/torch_vision_utils.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/deep_utils.egg-info/PKG-INFO` & `deep_utils-1.3.9/deep_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deep-utils
-Version: 1.3.8
+Version: 1.3.9
 Summary: Deep Utils
 Home-page: https://github.com/pooya-mohammadi/deep_utils
 Author: Pooya Mohammadi Kazaj
 Author-email: pooyamohammadikazaj@gmial.com
 License: UNKNOWN
-Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.3.8.tar.gz
+Download-URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/1.3.9.tar.gz
 Description: [![Downloads](https://static.pepy.tech/badge/deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
         
         <div id="top"></div>
         <!-- PROJECT LOGO -->
         <br />
         <div align="center">
           <a href="https://github.com/pooya-mohammadi/deep_utils">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: deep-utils Version: 1.3.8 Summary: Deep Utils Home-
+Metadata-Version: 2.1 Name: deep-utils Version: 1.3.9 Summary: Deep Utils Home-
 page: https://github.com/pooya-mohammadi/deep_utils Author: Pooya Mohammadi
 Kazaj Author-email: pooyamohammadikazaj@gmial.com License: UNKNOWN Download-
 URL: https://github.com/pooya-mohammadi/deep_utils/archive/refs/tags/
-1.3.8.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
+1.3.9.tar.gz Description: [![Downloads](https://static.pepy.tech/badge/
 deep_utils)](https://pepy.tech/project/deep_utils) [![PyPI](https://
 img.shields.io/pypi/v/deep_utils.svg)](https://pypi.python.org/pypi/deep_utils)
 
                                     _[_L_o_g_o_]
                              ******** DDeeeepp UUttiillss ********
                   A toolkit for deep-learning practitioners!
 This repository contains the most frequently used deep learning models and
```

### Comparing `deep_utils-1.3.8/deep_utils.egg-info/SOURCES.txt` & `deep_utils-1.3.9/deep_utils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,16 @@
 deep_utils/utils/dir_utils/__init__.py
 deep_utils/utils/dir_utils/dir_utils.py
 deep_utils/utils/download_utils/__init__.py
 deep_utils/utils/download_utils/download_utils.py
 deep_utils/utils/encodes/__init__.py
 deep_utils/utils/encodes/b64.py
 deep_utils/utils/encodes/web_inputs.py
+deep_utils/utils/fa_nlp_utils/__init__.py
+deep_utils/utils/fa_nlp_utils/fa_nlp_utils.py
 deep_utils/utils/gif_utils/__init__.py
 deep_utils/utils/gif_utils/gif_utils.py
 deep_utils/utils/hash_utils/__init__.py
 deep_utils/utils/hash_utils/hash_utils.py
 deep_utils/utils/image_utils/__init__.py
 deep_utils/utils/image_utils/image_utils.py
 deep_utils/utils/json_utils/__init__.py
```

### Comparing `deep_utils-1.3.8/setup.py` & `deep_utils-1.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "1.3.8"
+VERSION = "1.3.9"
 
 long_description = open("Readme.md", mode="r", encoding="utf-8").read()
 
 # Module dependencies
 dependency_links = []
 
 requirements = [
```

### Comparing `deep_utils-1.3.8/tests/utils/encoding_utils/encoding_utils_test.py` & `deep_utils-1.3.9/tests/utils/encoding_utils/encoding_utils_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/tests/utils/np_utils/np_utils_test.py` & `deep_utils-1.3.9/tests/utils/np_utils/np_utils_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/tests/utils/resize_utils/resize_utils_test.py` & `deep_utils-1.3.9/tests/utils/resize_utils/resize_utils_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py` & `deep_utils-1.3.9/tests/vision/face_detection/mtcnn/torch/mtcnn_torch_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py` & `deep_utils-1.3.9/tests/vision/face_detection/ultralight/torch/ultralight_torch_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py` & `deep_utils-1.3.9/tests/vision/object_detection/yolo/v5/torch/yolov5_detection_test.py`

 * *Files identical despite different names*

### Comparing `deep_utils-1.3.8/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py` & `deep_utils-1.3.9/tests/vision/vision_utils/torch_vision_utils/torch_vision_utils_test.py`

 * *Files identical despite different names*

